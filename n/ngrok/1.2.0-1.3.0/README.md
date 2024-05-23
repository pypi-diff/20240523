# Comparing `tmp/ngrok-1.2.0-cp37-abi3-win_amd64.whl.zip` & `tmp/ngrok-1.3.0-cp37-abi3-musllinux_1_2_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,16 @@
-Zip file size: 3034048 bytes, number of entries: 13
--rw-r--r--  4.6 unx    19032 b- defN 24-Mar-12 16:20 ngrok-1.2.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 24-Mar-12 16:20 ngrok-1.2.0.dist-info/WHEEL
--rw-r--r--  4.6 unx       53 b- defN 24-Mar-12 16:20 ngrok-1.2.0.dist-info/entry_points.txt
--rw-r--r--  4.6 unx    11558 b- defN 24-Mar-12 16:20 ngrok-1.2.0.dist-info/license_files/LICENSE-APACHE
--rw-r--r--  4.6 unx     1056 b- defN 24-Mar-12 16:20 ngrok-1.2.0.dist-info/license_files/LICENSE-MIT
--rw-r--r--  4.6 unx       34 b- defN 24-Mar-12 16:20 ngrok/mypy.ini
--rw-r--r--  4.6 unx     7330 b- defN 24-Mar-12 16:20 ngrok/ngrok.pyi
--rw-r--r--  4.6 unx     5149 b- defN 24-Mar-12 16:20 ngrok/ngrok_parser.py
--rw-r--r--  4.6 unx        0 b- defN 24-Mar-12 16:20 ngrok/py.typed
--rw-r--r--  4.6 unx      109 b- defN 24-Mar-12 16:20 ngrok/__init__.py
--rw-r--r--  4.6 unx     6547 b- defN 24-Mar-12 16:20 ngrok/__main__.py
--rwxr-xr-x  4.6 unx  8264192 b- defN 24-Mar-12 16:20 ngrok/ngrok.pyd
--rw-r--r--  4.6 unx     1015 b- defN 24-Mar-12 16:20 ngrok-1.2.0.dist-info/RECORD
-13 files, 8316171 bytes uncompressed, 3032372 bytes compressed:  63.5%
+Zip file size: 2916317 bytes, number of entries: 14
+-rw-r--r--  4.6 unx    18864 b- defN 24-May-23 21:07 ngrok-1.3.0.dist-info/METADATA
+-rw-r--r--  4.6 unx      106 b- defN 24-May-23 21:07 ngrok-1.3.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx       53 b- defN 24-May-23 21:07 ngrok-1.3.0.dist-info/entry_points.txt
+-rw-r--r--  4.6 unx    11357 b- defN 24-May-23 21:07 ngrok-1.3.0.dist-info/license_files/LICENSE-APACHE
+-rw-r--r--  4.6 unx     1050 b- defN 24-May-23 21:07 ngrok-1.3.0.dist-info/license_files/LICENSE-MIT
+-rwxr-xr-x  4.6 unx   724137 b- defN 24-May-23 21:07 ngrok.libs/libgcc_s-60abea67.so.1
+-rw-r--r--  4.6 unx     6323 b- defN 24-May-23 21:07 ngrok/__main__.py
+-rw-r--r--  4.6 unx      104 b- defN 24-May-23 21:07 ngrok/__init__.py
+-rw-r--r--  4.6 unx        0 b- defN 24-May-23 21:07 ngrok/py.typed
+-rw-r--r--  4.6 unx     7613 b- defN 24-May-23 21:07 ngrok/ngrok.pyi
+-rw-r--r--  4.6 unx       32 b- defN 24-May-23 21:07 ngrok/mypy.ini
+-rw-r--r--  4.6 unx     5011 b- defN 24-May-23 21:07 ngrok/ngrok_parser.py
+-rwxr-xr-x  4.6 unx  6491521 b- defN 24-May-23 21:07 ngrok/ngrok.abi3.so
+-rw-r--r--  4.6 unx     1112 b- defN 24-May-23 21:07 ngrok-1.3.0.dist-info/RECORD
+14 files, 7267283 bytes uncompressed, 2914491 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -1,40 +1,43 @@
-Filename: ngrok-1.2.0.dist-info/METADATA
+Filename: ngrok-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: ngrok-1.2.0.dist-info/WHEEL
+Filename: ngrok-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: ngrok-1.2.0.dist-info/entry_points.txt
+Filename: ngrok-1.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: ngrok-1.2.0.dist-info/license_files/LICENSE-APACHE
+Filename: ngrok-1.3.0.dist-info/license_files/LICENSE-APACHE
 Comment: 
 
-Filename: ngrok-1.2.0.dist-info/license_files/LICENSE-MIT
+Filename: ngrok-1.3.0.dist-info/license_files/LICENSE-MIT
 Comment: 
 
-Filename: ngrok/mypy.ini
+Filename: ngrok.libs/libgcc_s-60abea67.so.1
 Comment: 
 
-Filename: ngrok/ngrok.pyi
+Filename: ngrok/__main__.py
 Comment: 
 
-Filename: ngrok/ngrok_parser.py
+Filename: ngrok/__init__.py
 Comment: 
 
 Filename: ngrok/py.typed
 Comment: 
 
-Filename: ngrok/__init__.py
+Filename: ngrok/ngrok.pyi
 Comment: 
 
-Filename: ngrok/__main__.py
+Filename: ngrok/mypy.ini
+Comment: 
+
+Filename: ngrok/ngrok_parser.py
 Comment: 
 
-Filename: ngrok/ngrok.pyd
+Filename: ngrok/ngrok.abi3.so
 Comment: 
 
-Filename: ngrok-1.2.0.dist-info/RECORD
+Filename: ngrok-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ngrok/mypy.ini

 * *Ordering differences only*

```diff
@@ -1,2 +1,2 @@
-[mypy]
-implicit_optional = True
+[mypy]
+implicit_optional = True
```

## ngrok/ngrok.pyi

```diff
@@ -1,149 +1,156 @@
-from typing import Union, Optional, Any, Awaitable, List, Mapping, Callable
-
-# See API documentation for full information on the available functions:
-# https://ngrok.github.io/ngrok-python/
-
-def connect(
-    addr: Union[None, str, int] = None,
-    listener: Optional[Listener] = None,
-    **options: object,
-) -> Listener: ...
-def default(session: Optional[Session] = None) -> Listener: ...
-def disconnect(url: Optional[str] = None) -> None: ...
-def fd(session: Optional[Session] = None) -> int: ...
-def forward(
-    addr: Union[None, str, int] = None,
-    listener: Optional[Listener] = None,
-    **options: object,
-) -> Listener: ...
-def getsockname(session: Optional[Session] = None) -> str: ...
-def kill() -> None: ...
-def listen(
-    server: Optional[Any] = None, listener: Optional[Listener] = None
-) -> Listener: ...
-def log_level(level: str = "INFO") -> None: ...
-def pipe_name() -> str: ...
-def werkzeug_develop(
-    listener: Optional[Listener] = None,
-) -> Union[Awaitable[Listener], Listener]: ...
-
-class Listener:
-    def close(self) -> Awaitable[None]: ...
-    def forward(self, addr: str) -> Awaitable[None]: ...
-    def forwards_to(self) -> str: ...
-    def id(self) -> str: ...
-    def labels(self) -> Mapping[str, str]: ...
-    def metadata(self) -> str: ...
-    def proto(self) -> str: ...
-    def url(self) -> str: ...
-
-class Session:
-    def close(self) -> Awaitable[None]: ...
-    def close_listener(self, id: str) -> Awaitable[None]: ...
-    def get_listeners(self) -> List[Listener]: ...
-    def http_endpoint(self) -> HttpListenerBuilder: ...
-    def labeled_listener(self) -> LabeledListenerBuilder: ...
-    def tcp_endpoint(self) -> TcpListenerBuilder: ...
-    def tls_endpoint(self) -> TlsListenerBuilder: ...
-
-class SessionBuilder:
-    def authtoken(self, authtoken: str) -> SessionBuilder: ...
-    def authtoken_from_env(self) -> SessionBuilder: ...
-    def ca_cert(self, cert_bytes: bytearray) -> SessionBuilder: ...
-    def client_info(
-        self, client_type: str, version: str, comments: Optional[str] = None
-    ) -> SessionBuilder: ...
-    def connect(self) -> Awaitable[Session]: ...
-    def handle_disconnection(self, handler: Callable[[str, str]]) -> SessionBuilder: ...
-    def handle_heartbeat(self, handler: Callable[[int]]) -> SessionBuilder: ...
-    def handle_restart_command(self, handler: Callable[[]]) -> SessionBuilder: ...
-    def handle_stop_command(self, handler: Callable[[]]) -> SessionBuilder: ...
-    def handle_update_command(
-        self, handler: Callable[[str, str]]
-    ) -> SessionBuilder: ...
-    def heartbeat_interval(self, heartbeat_interval: int) -> SessionBuilder: ...
-    def heartbeat_tolerance(self, heartbeat_tolerance: int) -> SessionBuilder: ...
-    def metadata(self, metadata: str) -> SessionBuilder: ...
-    def server_addr(self, server_addr: str) -> SessionBuilder: ...
-
-class HttpListenerBuilder:
-    def allow_cidr(self, cidr: str) -> HttpListenerBuilder: ...
-    def allow_user_agent(self, regex: str) -> HttpListenerBuilder: ...
-    def app_protocol(self, app_protocol: str) -> HttpListenerBuilder: ...
-    def basic_auth(self, username: str, password: str) -> HttpListenerBuilder: ...
-    def circuit_breaker(self, circuit_breaker: float) -> HttpListenerBuilder: ...
-    def compression(self) -> HttpListenerBuilder: ...
-    def deny_cidr(self, cidr: str) -> HttpListenerBuilder: ...
-    def deny_user_agent(self, regex: str) -> HttpListenerBuilder: ...
-    def domain(self, domain: str) -> HttpListenerBuilder: ...
-    def forwards_to(self, forwards_to: str) -> HttpListenerBuilder: ...
-    def listen(self) -> Awaitable[Listener]: ...
-    def listen_and_forward(self, url: str) -> Awaitable[Listener]: ...
-    def listen_and_serve(self, server: Any) -> Awaitable[Listener]: ...
-    def metadata(self, metadata: str) -> HttpListenerBuilder: ...
-    def mutual_tlsca(self, mutual_tlsca: bytearray) -> HttpListenerBuilder: ...
-    def oauth(
-        self,
-        provider: str,
-        allow_emails: Optional[list[str]] = None,
-        allow_domains: Optional[list[str]] = None,
-        scopes: Optional[list[str]] = None,
-        client_id: Optional[str] = None,
-        client_secret: Optional[str] = None,
-    ) -> HttpListenerBuilder: ...
-    def oidc(
-        self,
-        issuer_url: str,
-        client_id: str,
-        client_secret: str,
-        allow_emails: Optional[list[str]] = None,
-        allow_domains: Optional[list[str]] = None,
-        scopes: Optional[list[str]] = None,
-    ) -> HttpListenerBuilder: ...
-    def policy(self, policy: str) -> HttpListenerBuilder: ...
-    def proxy_proto(self, proxy_proto: str) -> HttpListenerBuilder: ...
-    def remove_request_header(self, name: str) -> HttpListenerBuilder: ...
-    def remove_response_header(self, name: str) -> HttpListenerBuilder: ...
-    def request_header(self, name: str, value: str) -> HttpListenerBuilder: ...
-    def response_header(self, name: str, value: str) -> HttpListenerBuilder: ...
-    def scheme(self, scheme: str) -> HttpListenerBuilder: ...
-    def webhook_verification(
-        self, provider: str, secret: str
-    ) -> HttpListenerBuilder: ...
-    def websocket_tcp_conversion(self) -> HttpListenerBuilder: ...
-
-class LabeledListenerBuilder:
-    def app_protocol(self, app_protocol: str) -> LabeledListenerBuilder: ...
-    def label(self, label: str, value: str) -> LabeledListenerBuilder: ...
-    def listen(self) -> Awaitable[Listener]: ...
-    def listen_and_forward(self, url: str) -> Awaitable[Listener]: ...
-    def listen_and_serve(self, server: Any) -> Awaitable[Listener]: ...
-    def metadata(self, metadata: str) -> LabeledListenerBuilder: ...
-
-class TcpListenerBuilder:
-    def allow_cidr(self, cidr: str) -> TcpListenerBuilder: ...
-    def deny_cidr(self, cidr: str) -> TcpListenerBuilder: ...
-    def forwards_to(self, forwards_to: str) -> TcpListenerBuilder: ...
-    def listen(self) -> Awaitable[Listener]: ...
-    def listen_and_forward(self, url: str) -> Awaitable[Listener]: ...
-    def listen_and_serve(self, server: Any) -> Awaitable[Listener]: ...
-    def metadata(self, metadata: str) -> TcpListenerBuilder: ...
-    def policy(self, policy: str) -> TcpListenerBuilder: ...
-    def proxy_proto(self, proxy_proto: str) -> TcpListenerBuilder: ...
-    def remote_addr(self, remote_addr: str) -> TcpListenerBuilder: ...
-
-class TlsListenerBuilder:
-    def allow_cidr(self, cidr: str) -> TlsListenerBuilder: ...
-    def deny_cidr(self, cidr: str) -> TlsListenerBuilder: ...
-    def domain(self, domain: str) -> TlsListenerBuilder: ...
-    def forwards_to(self, forwards_to: str) -> TlsListenerBuilder: ...
-    def listen(self) -> Awaitable[Listener]: ...
-    def listen_and_forward(self, url: str) -> Awaitable[Listener]: ...
-    def listen_and_serve(self, server: Any) -> Awaitable[Listener]: ...
-    def metadata(self, metadata: str) -> TlsListenerBuilder: ...
-    def mutual_tlsca(self, mutual_tlsca: bytearray) -> TlsListenerBuilder: ...
-    def policy(self, policy: str) -> TlsListenerBuilder: ...
-    def proxy_proto(self, proxy_proto: str) -> TlsListenerBuilder: ...
-    def termination(
-        self, cert_pem: bytearray, key_pem: bytearray
-    ) -> TlsListenerBuilder: ...
+from typing import Union, Optional, Any, Awaitable, List, Mapping, Callable
+
+# See API documentation for full information on the available functions:
+# https://ngrok.github.io/ngrok-python/
+
+def connect(
+    addr: Union[None, str, int] = None,
+    listener: Optional[Listener] = None,
+    **options: object,
+) -> Listener: ...
+def default(session: Optional[Session] = None) -> Listener: ...
+def disconnect(url: Optional[str] = None) -> None: ...
+def fd(session: Optional[Session] = None) -> int: ...
+def forward(
+    addr: Union[None, str, int] = None,
+    listener: Optional[Listener] = None,
+    **options: object,
+) -> Listener: ...
+def getsockname(session: Optional[Session] = None) -> str: ...
+def kill() -> None: ...
+def listen(
+    server: Optional[Any] = None, listener: Optional[Listener] = None
+) -> Listener: ...
+def log_level(level: str = "INFO") -> None: ...
+def pipe_name() -> str: ...
+def werkzeug_develop(
+    listener: Optional[Listener] = None,
+) -> Union[Awaitable[Listener], Listener]: ...
+
+class Listener:
+    def close(self) -> Awaitable[None]: ...
+    def forward(self, addr: str) -> Awaitable[None]: ...
+    def forwards_to(self) -> str: ...
+    def id(self) -> str: ...
+    def labels(self) -> Mapping[str, str]: ...
+    def metadata(self) -> str: ...
+    def proto(self) -> str: ...
+    def url(self) -> str: ...
+
+class Session:
+    def close(self) -> Awaitable[None]: ...
+    def close_listener(self, id: str) -> Awaitable[None]: ...
+    def get_listeners(self) -> List[Listener]: ...
+    def http_endpoint(self) -> HttpListenerBuilder: ...
+    def labeled_listener(self) -> LabeledListenerBuilder: ...
+    def tcp_endpoint(self) -> TcpListenerBuilder: ...
+    def tls_endpoint(self) -> TlsListenerBuilder: ...
+
+class SessionBuilder:
+    def authtoken(self, authtoken: str) -> SessionBuilder: ...
+    def authtoken_from_env(self) -> SessionBuilder: ...
+    def ca_cert(self, cert_bytes: bytearray) -> SessionBuilder: ...
+    def client_info(
+        self, client_type: str, version: str, comments: Optional[str] = None
+    ) -> SessionBuilder: ...
+    def connect(self) -> Awaitable[Session]: ...
+    def handle_disconnection(self, handler: Callable[[str, str]]) -> SessionBuilder: ...
+    def handle_heartbeat(self, handler: Callable[[int]]) -> SessionBuilder: ...
+    def handle_restart_command(self, handler: Callable[[]]) -> SessionBuilder: ...
+    def handle_stop_command(self, handler: Callable[[]]) -> SessionBuilder: ...
+    def handle_update_command(
+        self, handler: Callable[[str, str]]
+    ) -> SessionBuilder: ...
+    def heartbeat_interval(self, heartbeat_interval: int) -> SessionBuilder: ...
+    def heartbeat_tolerance(self, heartbeat_tolerance: int) -> SessionBuilder: ...
+    def metadata(self, metadata: str) -> SessionBuilder: ...
+    def root_cas(self, root_cas: str) -> SessionBuilder: ...
+    def server_addr(self, server_addr: str) -> SessionBuilder: ...
+
+class HttpListenerBuilder:
+    def allow_cidr(self, cidr: str) -> HttpListenerBuilder: ...
+    def allow_user_agent(self, regex: str) -> HttpListenerBuilder: ...
+    def app_protocol(self, app_protocol: str) -> HttpListenerBuilder: ...
+    def basic_auth(self, username: str, password: str) -> HttpListenerBuilder: ...
+    def circuit_breaker(self, circuit_breaker: float) -> HttpListenerBuilder: ...
+    def compression(self) -> HttpListenerBuilder: ...
+    def deny_cidr(self, cidr: str) -> HttpListenerBuilder: ...
+    def deny_user_agent(self, regex: str) -> HttpListenerBuilder: ...
+    def domain(self, domain: str) -> HttpListenerBuilder: ...
+    def forwards_to(self, forwards_to: str) -> HttpListenerBuilder: ...
+    def listen(self) -> Awaitable[Listener]: ...
+    def listen_and_forward(self, url: str) -> Awaitable[Listener]: ...
+    def listen_and_serve(self, server: Any) -> Awaitable[Listener]: ...
+    def metadata(self, metadata: str) -> HttpListenerBuilder: ...
+    def mutual_tlsca(self, mutual_tlsca: bytearray) -> HttpListenerBuilder: ...
+    def oauth(
+        self,
+        provider: str,
+        allow_emails: Optional[list[str]] = None,
+        allow_domains: Optional[list[str]] = None,
+        scopes: Optional[list[str]] = None,
+        client_id: Optional[str] = None,
+        client_secret: Optional[str] = None,
+    ) -> HttpListenerBuilder: ...
+    def oidc(
+        self,
+        issuer_url: str,
+        client_id: str,
+        client_secret: str,
+        allow_emails: Optional[list[str]] = None,
+        allow_domains: Optional[list[str]] = None,
+        scopes: Optional[list[str]] = None,
+    ) -> HttpListenerBuilder: ...
+    def policy(self, policy: str) -> HttpListenerBuilder: ...
+    def proxy_proto(self, proxy_proto: str) -> HttpListenerBuilder: ...
+    def remove_request_header(self, name: str) -> HttpListenerBuilder: ...
+    def remove_response_header(self, name: str) -> HttpListenerBuilder: ...
+    def request_header(self, name: str, value: str) -> HttpListenerBuilder: ...
+    def response_header(self, name: str, value: str) -> HttpListenerBuilder: ...
+    def scheme(self, scheme: str) -> HttpListenerBuilder: ...
+    def verify_upstream_tls(self, verify_upstream_tls: bool) -> HttpListenerBuilder: ...
+    def webhook_verification(
+        self, provider: str, secret: str
+    ) -> HttpListenerBuilder: ...
+    def websocket_tcp_conversion(self) -> HttpListenerBuilder: ...
+
+class LabeledListenerBuilder:
+    def app_protocol(self, app_protocol: str) -> LabeledListenerBuilder: ...
+    def label(self, label: str, value: str) -> LabeledListenerBuilder: ...
+    def listen(self) -> Awaitable[Listener]: ...
+    def listen_and_forward(self, url: str) -> Awaitable[Listener]: ...
+    def listen_and_serve(self, server: Any) -> Awaitable[Listener]: ...
+    def metadata(self, metadata: str) -> LabeledListenerBuilder: ...
+    def verify_upstream_tls(
+        self, verify_upstream_tls: bool
+    ) -> LabeledListenerBuilder: ...
+
+class TcpListenerBuilder:
+    def allow_cidr(self, cidr: str) -> TcpListenerBuilder: ...
+    def deny_cidr(self, cidr: str) -> TcpListenerBuilder: ...
+    def forwards_to(self, forwards_to: str) -> TcpListenerBuilder: ...
+    def listen(self) -> Awaitable[Listener]: ...
+    def listen_and_forward(self, url: str) -> Awaitable[Listener]: ...
+    def listen_and_serve(self, server: Any) -> Awaitable[Listener]: ...
+    def metadata(self, metadata: str) -> TcpListenerBuilder: ...
+    def policy(self, policy: str) -> TcpListenerBuilder: ...
+    def proxy_proto(self, proxy_proto: str) -> TcpListenerBuilder: ...
+    def remote_addr(self, remote_addr: str) -> TcpListenerBuilder: ...
+    def verify_upstream_tls(self, verify_upstream_tls: bool) -> TcpListenerBuilder: ...
+
+class TlsListenerBuilder:
+    def allow_cidr(self, cidr: str) -> TlsListenerBuilder: ...
+    def deny_cidr(self, cidr: str) -> TlsListenerBuilder: ...
+    def domain(self, domain: str) -> TlsListenerBuilder: ...
+    def forwards_to(self, forwards_to: str) -> TlsListenerBuilder: ...
+    def listen(self) -> Awaitable[Listener]: ...
+    def listen_and_forward(self, url: str) -> Awaitable[Listener]: ...
+    def listen_and_serve(self, server: Any) -> Awaitable[Listener]: ...
+    def metadata(self, metadata: str) -> TlsListenerBuilder: ...
+    def mutual_tlsca(self, mutual_tlsca: bytearray) -> TlsListenerBuilder: ...
+    def policy(self, policy: str) -> TlsListenerBuilder: ...
+    def proxy_proto(self, proxy_proto: str) -> TlsListenerBuilder: ...
+    def termination(
+        self, cert_pem: bytearray, key_pem: bytearray
+    ) -> TlsListenerBuilder: ...
+    def verify_upstream_tls(self, verify_upstream_tls: bool) -> TlsListenerBuilder: ...
```

## ngrok/ngrok_parser.py

 * *Ordering differences only*

```diff
@@ -1,138 +1,138 @@
-import argparse
-
-
-def get_pass_through_args():
-    return {"host", "port", "uds", "fd", "config", "bind"}
-
-
-def get_parser():
-    # argument parsing
-    parser = argparse.ArgumentParser(
-        prog="ngrok-asgi",
-        description="ASGI wrapper for ngrok",
-        epilog="Online in One Line",
-    )
-    parser.add_argument(
-        "command", choices=["gunicorn", "uvicorn"], help="gunicorn or uvicorn"
-    )
-    # ngrok session options
-    parser.add_argument(
-        "--authtoken",
-        help="Ngrok authtoken, otherwise uses NGROK_AUTH_TOKEN environment variable",
-    )
-    parser.add_argument(
-        "--session-metadata",
-        help="Configures the opaque, machine-readable metadata string for this session.",
-    )
-
-    # ngrok listener options
-    parser.add_argument(
-        "--allow-cidr",
-        action="append",
-        help="Restriction placed on the origin of incoming connections to the edge to only allow these CIDR ranges. Call multiple times to add additional CIDR ranges.",
-    )
-    parser.add_argument(
-        "--basic-auth",
-        nargs=2,
-        metavar=("username", "password"),
-        help="Credentials for basic authentication.",
-    )
-    parser.add_argument(
-        "--circuit-breaker",
-        help="Reject requests when 5XX responses exceed this ratio. Disabled when 0.",
-    )
-    parser.add_argument(
-        "--compression",
-        action="store_true",
-        help="Enable gzip compression for HTTP responses.",
-    )
-    parser.add_argument(
-        "--deny-cidr",
-        action="append",
-        help="Restriction placed on the origin of incoming connections to the edge to deny these CIDR ranges. Call multiple times to add additional CIDR ranges.",
-    )
-    parser.add_argument("--domain", help="The domain to request for this edge.")
-    parser.add_argument(
-        "--forwards-to",
-        help="Listener backend metadata. Viewable via the dashboard and API, but has no bearing on listener behavior.",
-    )
-    parser.add_argument(
-        "--metadata", help="Listener-specific opaque metadata. Viewable via the API."
-    )
-    parser.add_argument(
-        "--mutual-tlsca",
-        help="Filename of certificates to use for client authentication at the ngrok edge.",
-    )
-    parser.add_argument("--oauth-provider", help="OAuth provider configuration.")
-    parser.add_argument(
-        "--oidc",
-        nargs=3,
-        metavar=("issuer-url", "client-id", "client-secret"),
-        help="OIDC configuration.",
-    )
-    parser.add_argument(
-        "--allow-emails", action="append", help="OAuth/OIDC configuration."
-    )
-    parser.add_argument(
-        "--allow-domains", action="append", help="OAuth/OIDC configuration."
-    )
-    parser.add_argument("--scopes", action="append", help="OAuth/OIDC configuration.")
-    parser.add_argument(
-        "--proxy-proto",
-        choices=["", "1", "2"],
-        help="The version of PROXY protocol to use with this listener “1”, “2”, or “” if not using.",
-    )
-    parser.add_argument(
-        "--remove-request-header",
-        action="append",
-        help="Removes a header from requests to this edge. Call multiple times to add additional values.",
-    )
-    parser.add_argument(
-        "--remove-response-header",
-        action="append",
-        help="Removes a header from responses from this edge Call multiple times to add additional values..",
-    )
-    parser.add_argument(
-        "--request-header",
-        action="append",
-        nargs=2,
-        metavar=("header", "value"),
-        help="Adds a header to all requests to this edge. Call multiple times to add additional values.",
-    )
-    parser.add_argument(
-        "--response-header",
-        action="append",
-        nargs=2,
-        metavar=("header", "value"),
-        help="Adds a header to all responses coming from this edge. Call multiple times to add additional values.",
-    )
-    parser.add_argument(
-        "--scheme",
-        choices=["HTTPS", "HTTP"],
-        help="The scheme that this edge should use. Defaults to HTTPS.",
-    )
-    parser.add_argument(
-        "--webhook-verification",
-        nargs=2,
-        metavar=("provider", "secret"),
-        help="WebhookVerification configuration.",
-    )
-    parser.add_argument(
-        "--websocket-tcp-conversion",
-        action="store_true",
-        help="Convert incoming websocket connections to TCP-like streams.",
-    )
-    # uvicorn options
-    parser.add_argument("--host", help="Hostname or IP address")
-    parser.add_argument("--port", help="Port number", type=int)
-    parser.add_argument("--uds", help="Unix domain socket")
-    parser.add_argument("--fd", help="File descriptor")
-    # gunicorn options
-    parser.add_argument("--config", "-c", help="Config file not supported")
-    parser.add_argument(
-        "--bind",
-        "-b",
-        help="Specify a server socket to bind. Server sockets can be any of $(HOST), $(HOST):$(PORT), "
-        + "fd://$(FD), or unix:$(PATH). An IP is a valid $(HOST).",
-    )
-    return parser
+import argparse
+
+
+def get_pass_through_args():
+    return {"host", "port", "uds", "fd", "config", "bind"}
+
+
+def get_parser():
+    # argument parsing
+    parser = argparse.ArgumentParser(
+        prog="ngrok-asgi",
+        description="ASGI wrapper for ngrok",
+        epilog="Online in One Line",
+    )
+    parser.add_argument(
+        "command", choices=["gunicorn", "uvicorn"], help="gunicorn or uvicorn"
+    )
+    # ngrok session options
+    parser.add_argument(
+        "--authtoken",
+        help="Ngrok authtoken, otherwise uses NGROK_AUTH_TOKEN environment variable",
+    )
+    parser.add_argument(
+        "--session-metadata",
+        help="Configures the opaque, machine-readable metadata string for this session.",
+    )
+
+    # ngrok listener options
+    parser.add_argument(
+        "--allow-cidr",
+        action="append",
+        help="Restriction placed on the origin of incoming connections to the edge to only allow these CIDR ranges. Call multiple times to add additional CIDR ranges.",
+    )
+    parser.add_argument(
+        "--basic-auth",
+        nargs=2,
+        metavar=("username", "password"),
+        help="Credentials for basic authentication.",
+    )
+    parser.add_argument(
+        "--circuit-breaker",
+        help="Reject requests when 5XX responses exceed this ratio. Disabled when 0.",
+    )
+    parser.add_argument(
+        "--compression",
+        action="store_true",
+        help="Enable gzip compression for HTTP responses.",
+    )
+    parser.add_argument(
+        "--deny-cidr",
+        action="append",
+        help="Restriction placed on the origin of incoming connections to the edge to deny these CIDR ranges. Call multiple times to add additional CIDR ranges.",
+    )
+    parser.add_argument("--domain", help="The domain to request for this edge.")
+    parser.add_argument(
+        "--forwards-to",
+        help="Listener backend metadata. Viewable via the dashboard and API, but has no bearing on listener behavior.",
+    )
+    parser.add_argument(
+        "--metadata", help="Listener-specific opaque metadata. Viewable via the API."
+    )
+    parser.add_argument(
+        "--mutual-tlsca",
+        help="Filename of certificates to use for client authentication at the ngrok edge.",
+    )
+    parser.add_argument("--oauth-provider", help="OAuth provider configuration.")
+    parser.add_argument(
+        "--oidc",
+        nargs=3,
+        metavar=("issuer-url", "client-id", "client-secret"),
+        help="OIDC configuration.",
+    )
+    parser.add_argument(
+        "--allow-emails", action="append", help="OAuth/OIDC configuration."
+    )
+    parser.add_argument(
+        "--allow-domains", action="append", help="OAuth/OIDC configuration."
+    )
+    parser.add_argument("--scopes", action="append", help="OAuth/OIDC configuration.")
+    parser.add_argument(
+        "--proxy-proto",
+        choices=["", "1", "2"],
+        help="The version of PROXY protocol to use with this listener “1”, “2”, or “” if not using.",
+    )
+    parser.add_argument(
+        "--remove-request-header",
+        action="append",
+        help="Removes a header from requests to this edge. Call multiple times to add additional values.",
+    )
+    parser.add_argument(
+        "--remove-response-header",
+        action="append",
+        help="Removes a header from responses from this edge Call multiple times to add additional values..",
+    )
+    parser.add_argument(
+        "--request-header",
+        action="append",
+        nargs=2,
+        metavar=("header", "value"),
+        help="Adds a header to all requests to this edge. Call multiple times to add additional values.",
+    )
+    parser.add_argument(
+        "--response-header",
+        action="append",
+        nargs=2,
+        metavar=("header", "value"),
+        help="Adds a header to all responses coming from this edge. Call multiple times to add additional values.",
+    )
+    parser.add_argument(
+        "--scheme",
+        choices=["HTTPS", "HTTP"],
+        help="The scheme that this edge should use. Defaults to HTTPS.",
+    )
+    parser.add_argument(
+        "--webhook-verification",
+        nargs=2,
+        metavar=("provider", "secret"),
+        help="WebhookVerification configuration.",
+    )
+    parser.add_argument(
+        "--websocket-tcp-conversion",
+        action="store_true",
+        help="Convert incoming websocket connections to TCP-like streams.",
+    )
+    # uvicorn options
+    parser.add_argument("--host", help="Hostname or IP address")
+    parser.add_argument("--port", help="Port number", type=int)
+    parser.add_argument("--uds", help="Unix domain socket")
+    parser.add_argument("--fd", help="File descriptor")
+    # gunicorn options
+    parser.add_argument("--config", "-c", help="Config file not supported")
+    parser.add_argument(
+        "--bind",
+        "-b",
+        help="Specify a server socket to bind. Server sockets can be any of $(HOST), $(HOST):$(PORT), "
+        + "fd://$(FD), or unix:$(PATH). An IP is a valid $(HOST).",
+    )
+    return parser
```

## ngrok/__init__.py

 * *Ordering differences only*

```diff
@@ -1,5 +1,5 @@
-from .ngrok import *
-
-__doc__ = ngrok.__doc__
-if hasattr(ngrok, "__all__"):
-    __all__ = ngrok.__all__
+from .ngrok import *
+
+__doc__ = ngrok.__doc__
+if hasattr(ngrok, "__all__"):
+    __all__ = ngrok.__all__
```

## ngrok/__main__.py

 * *Ordering differences only*

```diff
@@ -1,224 +1,224 @@
-import asyncio
-import logging
-import ngrok
-from ngrok import ngrok_parser
-import os
-import re
-import shlex
-import sys
-
-DEFAULT_HOST = "localhost"
-DEFAULT_PORT = "8000"
-
-
-def configure_session(args):
-    builder = ngrok.SessionBuilder()
-    if args.authtoken:
-        builder.authtoken(args.authtoken)
-    else:
-        builder.authtoken_from_env()
-
-    if args.session_metadata:
-        builder.metadata(args.session_metadata)
-    return builder
-
-
-def configure_listener(session, args):
-    builder = session.http_endpoint()
-    if args.allow_cidr:
-        for cidr in args.allow_cidr:
-            builder.allow_cidr(cidr)
-    if args.basic_auth:
-        builder.basic_auth(args.basic_auth[0], args.basic_auth[1])
-    if args.circuit_breaker:
-        builder.circuit_breaker(float(args.circuit_breaker))
-    if args.compression:
-        builder.compression()
-    if args.deny_cidr:
-        for cidr in args.deny_cidr:
-            builder.deny_cidr(cidr)
-    if args.domain:
-        builder.domain(args.domain)
-    if args.forwards_to:
-        builder.forwards_to(args.forwards_to)
-    if args.metadata:
-        builder.metadata(args.metadata)
-    if args.mutual_tlsca:
-        with open(args.mutual_tlsca, "r") as crt:
-            builder.mutual_tlsca(bytearray(crt.read().encode()))
-    if args.oauth_provider:
-        builder.oauth(
-            args.oauth_provider, args.allow_emails, args.allow_domains, args.scopes
-        )
-    if args.oidc:
-        builder.oidc(
-            args.oidc[0],
-            args.oidc[1],
-            args.oidc[2],
-            args.allow_emails,
-            args.allow_domains,
-            args.scopes,
-        )
-    if args.proxy_proto:
-        builder.proxy_proto(args.proxy_proto)
-    if args.remove_request_header:
-        for header in args.remove_request_header:
-            builder.remove_request_header(header)
-    if args.remove_response_header:
-        for header in args.remove_response_header:
-            builder.remove_response_header(header)
-    if args.request_header:
-        for header in args.request_header:
-            builder.request_header(header[0], header[1])
-    if args.response_header:
-        for header in args.response_header:
-            builder.response_header(header[0], header[1])
-    if args.scheme:
-        builder.scheme(args.scheme)
-    if args.webhook_verification:
-        builder.webhook_verification(
-            args.webhook_verification[0], args.webhook_verification[1]
-        )
-    if args.websocket_tcp_conversion:
-        builder.websocket_tcp_conversion(args.websocket_tcp_conversion)
-    return builder
-
-
-def gunicorn():
-    from gunicorn.app.wsgiapp import run
-
-    run()
-
-
-def uvicorn():
-    import uvicorn
-
-    uvicorn.main()
-
-
-def get_pipe_string(args):
-    pipe_string = None
-    if args.uds:
-        pipe_string = args.uds
-    if args.bind and args.bind.startswith("unix:"):
-        pipe_string = args.bind[5:]
-    return pipe_string
-
-
-def fallback_port(args):
-    fallback_port = DEFAULT_PORT
-    if args.command == "gunicorn" and "PORT" in os.environ:
-        fallback_port = os.getenv("PORT")
-    return fallback_port
-
-
-def get_tcp_string(args):
-    tcp_string = None
-    if args.host and args.port:
-        tcp_string = args.host + ":" + str(args.port)
-    elif args.host:
-        tcp_string = args.host + ":" + fallback_port(args)
-    elif args.port:
-        tcp_string = DEFAULT_HOST + ":" + str(args.port)
-    elif (
-        args.bind
-        and not args.bind.startswith("fd://")
-        and not args.bind.startswith("unix:")
-    ):
-        tcp_string = args.bind
-        # check if missing host
-        if re.search("^:\d+$", tcp_string):
-            tcp_string = DEFAULT_HOST + tcp_string
-        # check if missing port
-        if not re.search(":\d+$", tcp_string):
-            tcp_string += ":" + fallback_port(args)
-    return tcp_string
-
-
-def setup_forwarding(listener, args, tcp_string=None):
-    if tcp_string:
-        listener.forward(tcp_string)
-        return True
-
-    # prefer pipe over tcp
-    pipe_string = get_pipe_string(args)
-    if pipe_string:
-        listener.forward(pipe_string)
-    else:
-        tcp_string = get_tcp_string(args)
-        if not tcp_string:
-            return False
-        listener.forward(tcp_string)
-
-    return True
-
-
-async def bind(parser, args):
-    session = await configure_session(args).connect()
-    listener = await configure_listener(session, args).listen()
-    listener_success = setup_forwarding(listener, args)
-
-    # if we don't have what we need, check gunicorn environment variable
-    if (
-        not listener_success
-        and args.command == "gunicorn"
-        and "GUNICORN_CMD_ARGS" in os.environ
-    ):
-        env_cmd_args = shlex.split(os.getenv("GUNICORN_CMD_ARGS"))
-        env_args, unknown = parser.parse_known_args(env_cmd_args)
-        listener_success = setup_forwarding(listener, env_args)
-
-    # fallback to the default host and port for these runners
-    if not listener_success:
-        listener_success = setup_forwarding(
-            listener, args, tcp_string=f"{DEFAULT_HOST}:{fallback_port(args)}"
-        )
-
-    # give up
-    if not listener_success:
-        logging.fatal("No listener created. Exiting.")
-        sys.exit(1)
-
-    return listener
-
-
-def main(args):
-    logging.basicConfig(level=logging.INFO)
-
-    # argument parsing
-    parser = ngrok_parser.get_parser()
-    args, unknown = parser.parse_known_args()
-
-    # validation
-    if args.config:
-        logging.fatal("Config file not supported. Exiting.")
-        sys.exit(2)
-    if args.fd or (args.bind and args.bind.startswith("fd://")):
-        logging.fatal("File Descriptor not supported. Exiting.")
-        sys.exit(3)
-
-    # bind to ngrok
-    listener = asyncio.run(bind(parser, args))
-
-    # now pretend we don't exist
-    pass_args = [args.command]
-    # pass through some args
-    pass_through_args = ngrok_parser.get_pass_through_args()
-    for key, val in vars(args).items():
-        if key in pass_through_args and val:
-            pass_args.append(f"--{key}")
-            pass_args.append(str(val))
-    # pass through all unknown args
-    sys.argv = pass_args + unknown
-    if args.command == "gunicorn":
-        gunicorn()
-    elif args.command == "uvicorn":
-        uvicorn()
-
-
-def asgi_cli():
-    main(sys.argv)
-
-
-if __name__ == "__main__":
-    main(sys.argv)
+import asyncio
+import logging
+import ngrok
+from ngrok import ngrok_parser
+import os
+import re
+import shlex
+import sys
+
+DEFAULT_HOST = "localhost"
+DEFAULT_PORT = "8000"
+
+
+def configure_session(args):
+    builder = ngrok.SessionBuilder()
+    if args.authtoken:
+        builder.authtoken(args.authtoken)
+    else:
+        builder.authtoken_from_env()
+
+    if args.session_metadata:
+        builder.metadata(args.session_metadata)
+    return builder
+
+
+def configure_listener(session, args):
+    builder = session.http_endpoint()
+    if args.allow_cidr:
+        for cidr in args.allow_cidr:
+            builder.allow_cidr(cidr)
+    if args.basic_auth:
+        builder.basic_auth(args.basic_auth[0], args.basic_auth[1])
+    if args.circuit_breaker:
+        builder.circuit_breaker(float(args.circuit_breaker))
+    if args.compression:
+        builder.compression()
+    if args.deny_cidr:
+        for cidr in args.deny_cidr:
+            builder.deny_cidr(cidr)
+    if args.domain:
+        builder.domain(args.domain)
+    if args.forwards_to:
+        builder.forwards_to(args.forwards_to)
+    if args.metadata:
+        builder.metadata(args.metadata)
+    if args.mutual_tlsca:
+        with open(args.mutual_tlsca, "r") as crt:
+            builder.mutual_tlsca(bytearray(crt.read().encode()))
+    if args.oauth_provider:
+        builder.oauth(
+            args.oauth_provider, args.allow_emails, args.allow_domains, args.scopes
+        )
+    if args.oidc:
+        builder.oidc(
+            args.oidc[0],
+            args.oidc[1],
+            args.oidc[2],
+            args.allow_emails,
+            args.allow_domains,
+            args.scopes,
+        )
+    if args.proxy_proto:
+        builder.proxy_proto(args.proxy_proto)
+    if args.remove_request_header:
+        for header in args.remove_request_header:
+            builder.remove_request_header(header)
+    if args.remove_response_header:
+        for header in args.remove_response_header:
+            builder.remove_response_header(header)
+    if args.request_header:
+        for header in args.request_header:
+            builder.request_header(header[0], header[1])
+    if args.response_header:
+        for header in args.response_header:
+            builder.response_header(header[0], header[1])
+    if args.scheme:
+        builder.scheme(args.scheme)
+    if args.webhook_verification:
+        builder.webhook_verification(
+            args.webhook_verification[0], args.webhook_verification[1]
+        )
+    if args.websocket_tcp_conversion:
+        builder.websocket_tcp_conversion(args.websocket_tcp_conversion)
+    return builder
+
+
+def gunicorn():
+    from gunicorn.app.wsgiapp import run
+
+    run()
+
+
+def uvicorn():
+    import uvicorn
+
+    uvicorn.main()
+
+
+def get_pipe_string(args):
+    pipe_string = None
+    if args.uds:
+        pipe_string = args.uds
+    if args.bind and args.bind.startswith("unix:"):
+        pipe_string = args.bind[5:]
+    return pipe_string
+
+
+def fallback_port(args):
+    fallback_port = DEFAULT_PORT
+    if args.command == "gunicorn" and "PORT" in os.environ:
+        fallback_port = os.getenv("PORT")
+    return fallback_port
+
+
+def get_tcp_string(args):
+    tcp_string = None
+    if args.host and args.port:
+        tcp_string = args.host + ":" + str(args.port)
+    elif args.host:
+        tcp_string = args.host + ":" + fallback_port(args)
+    elif args.port:
+        tcp_string = DEFAULT_HOST + ":" + str(args.port)
+    elif (
+        args.bind
+        and not args.bind.startswith("fd://")
+        and not args.bind.startswith("unix:")
+    ):
+        tcp_string = args.bind
+        # check if missing host
+        if re.search("^:\d+$", tcp_string):
+            tcp_string = DEFAULT_HOST + tcp_string
+        # check if missing port
+        if not re.search(":\d+$", tcp_string):
+            tcp_string += ":" + fallback_port(args)
+    return tcp_string
+
+
+def setup_forwarding(listener, args, tcp_string=None):
+    if tcp_string:
+        listener.forward(tcp_string)
+        return True
+
+    # prefer pipe over tcp
+    pipe_string = get_pipe_string(args)
+    if pipe_string:
+        listener.forward(pipe_string)
+    else:
+        tcp_string = get_tcp_string(args)
+        if not tcp_string:
+            return False
+        listener.forward(tcp_string)
+
+    return True
+
+
+async def bind(parser, args):
+    session = await configure_session(args).connect()
+    listener = await configure_listener(session, args).listen()
+    listener_success = setup_forwarding(listener, args)
+
+    # if we don't have what we need, check gunicorn environment variable
+    if (
+        not listener_success
+        and args.command == "gunicorn"
+        and "GUNICORN_CMD_ARGS" in os.environ
+    ):
+        env_cmd_args = shlex.split(os.getenv("GUNICORN_CMD_ARGS"))
+        env_args, unknown = parser.parse_known_args(env_cmd_args)
+        listener_success = setup_forwarding(listener, env_args)
+
+    # fallback to the default host and port for these runners
+    if not listener_success:
+        listener_success = setup_forwarding(
+            listener, args, tcp_string=f"{DEFAULT_HOST}:{fallback_port(args)}"
+        )
+
+    # give up
+    if not listener_success:
+        logging.fatal("No listener created. Exiting.")
+        sys.exit(1)
+
+    return listener
+
+
+def main(args):
+    logging.basicConfig(level=logging.INFO)
+
+    # argument parsing
+    parser = ngrok_parser.get_parser()
+    args, unknown = parser.parse_known_args()
+
+    # validation
+    if args.config:
+        logging.fatal("Config file not supported. Exiting.")
+        sys.exit(2)
+    if args.fd or (args.bind and args.bind.startswith("fd://")):
+        logging.fatal("File Descriptor not supported. Exiting.")
+        sys.exit(3)
+
+    # bind to ngrok
+    listener = asyncio.run(bind(parser, args))
+
+    # now pretend we don't exist
+    pass_args = [args.command]
+    # pass through some args
+    pass_through_args = ngrok_parser.get_pass_through_args()
+    for key, val in vars(args).items():
+        if key in pass_through_args and val:
+            pass_args.append(f"--{key}")
+            pass_args.append(str(val))
+    # pass through all unknown args
+    sys.argv = pass_args + unknown
+    if args.command == "gunicorn":
+        gunicorn()
+    elif args.command == "uvicorn":
+        uvicorn()
+
+
+def asgi_cli():
+    main(sys.argv)
+
+
+if __name__ == "__main__":
+    main(sys.argv)
```

## Comparing `ngrok-1.2.0.dist-info/METADATA` & `ngrok-1.3.0.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ngrok
-Version: 1.2.0
+Version: 1.3.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Utilities
@@ -21,450 +21,456 @@
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 Summary: The ngrok Agent SDK for Python
 Keywords: ngrok,python,pypi,pyo3,ingress,networking
 License: MIT OR Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: changelog, https://github.com/ngrok/ngrok-python/blob/main/CHANGELOG.md
-Project-URL: repository, https://github.com/ngrok/ngrok-python
 Project-URL: homepage, https://ngrok.com
+Project-URL: repository, https://github.com/ngrok/ngrok-python
+Project-URL: changelog, https://github.com/ngrok/ngrok-python/blob/main/CHANGELOG.md
+
+# Python SDK for ngrok
+
+[![PyPI][pypi-badge]][pypi-url]
+[![Supported Versions][ver-badge]][ver-url]
+[![MIT licensed][mit-badge]][mit-url]
+[![Apache-2.0 licensed][apache-badge]][apache-url]
+[![Continuous integration][ci-badge]][ci-url]
+
+[pypi-badge]: https://img.shields.io/pypi/v/ngrok
+[pypi-url]: https://pypi.org/project/ngrok
+[ver-badge]: https://img.shields.io/pypi/pyversions/ngrok.svg
+[ver-url]: https://pypi.org/project/ngrok
+[mit-badge]: https://img.shields.io/badge/license-MIT-blue.svg
+[mit-url]: https://github.com/ngrok/ngrok-rust/blob/main/LICENSE-MIT
+[apache-badge]: https://img.shields.io/badge/license-Apache_2.0-blue.svg
+[apache-url]: https://github.com/ngrok/ngrok-rust/blob/main/LICENSE-APACHE
+[ci-badge]: https://github.com/ngrok/ngrok-python/actions/workflows/ci.yml/badge.svg
+[ci-url]: https://github.com/ngrok/ngrok-python/actions/workflows/ci.yml
+
+`ngrok-python` is the official Python SDK for ngrok that requires no binaries. Quickly enable secure production-ready connectivity to your applications and services directly from your code.
+
+[ngrok](https://ngrok.com) is a globally distributed gateway that provides secure connectivity for applications and services running in any environment.
 
-# Python SDK for ngrok
-
-[![PyPI][pypi-badge]][pypi-url]
-[![Supported Versions][ver-badge]][ver-url]
-[![MIT licensed][mit-badge]][mit-url]
-[![Apache-2.0 licensed][apache-badge]][apache-url]
-[![Continuous integration][ci-badge]][ci-url]
-
-[pypi-badge]: https://img.shields.io/pypi/v/ngrok
-[pypi-url]: https://pypi.org/project/ngrok
-[ver-badge]: https://img.shields.io/pypi/pyversions/ngrok.svg
-[ver-url]: https://pypi.org/project/ngrok
-[mit-badge]: https://img.shields.io/badge/license-MIT-blue.svg
-[mit-url]: https://github.com/ngrok/ngrok-rust/blob/main/LICENSE-MIT
-[apache-badge]: https://img.shields.io/badge/license-Apache_2.0-blue.svg
-[apache-url]: https://github.com/ngrok/ngrok-rust/blob/main/LICENSE-APACHE
-[ci-badge]: https://github.com/ngrok/ngrok-python/actions/workflows/ci.yml/badge.svg
-[ci-url]: https://github.com/ngrok/ngrok-python/actions/workflows/ci.yml
-
-`ngrok-python` is the official Python SDK for ngrok that requires no binaries. Quickly enable secure production-ready connectivity to your applications and services directly from your code.
-
-[ngrok](https://ngrok.com) is a globally distributed gateway that provides secure connectivity for applications and services running in any environment.
-
-# Installation
-
-The `ngrok-python` SDK can be installed from [PyPI](https://pypi.org/project/ngrok) via `pip`:
-
-```shell
-pip install ngrok
-```
-
-# Quickstart
-
-1. [Install `ngrok-python`](#installation)
-2. Export your [authtoken from the ngrok dashboard](https://dashboard.ngrok.com/get-started/your-authtoken) as `NGROK_AUTHTOKEN` in your terminal
-3. Add the following code to your application to establish connectivity via the [forward method](https://github.com/ngrok/ngrok-python/blob/main/examples/ngrok-forward-minimal.py) through port `9000` on `localhost`:
-
-    ```python
-    # import ngrok python sdk
-    import ngrok
-    
-    # Establish connectivity
-    listener = ngrok.forward(9000, authtoken_from_env=True)
-    
-    # Output ngrok url to console
-    print(f"Ingress established at {listener.url()}")
-    ```
-
-That's it! Your application should now be available through the url output in your terminal. 
-
-> **Note**
-> You can find more examples in [the examples directory](https://github.com/ngrok/ngrok-python/tree/main/examples).
-
-# Documentation
-
-A full quickstart guide and API reference can be found in the [ngrok-python documentation](https://ngrok.github.io/ngrok-python/).
-
-### Authentication
-
-To use most of ngrok's features, you'll need an authtoken. To obtain one, sign up for free at [ngrok.com](https://dashboard.ngrok.com/signup) and retrieve it from the [authtoken page in your ngrok dashboard](https://dashboard.ngrok.com/get-started/your-authtoken). Once you have copied your authtoken, you can reference it in several ways.
-
-You can set it in the `NGROK_AUTHTOKEN` environment variable and pass `authtoken_from_env=True` to the [forward](https://ngrok.github.io/ngrok-python/module.html) method:
-
-```python
-ngrok.forward(authtoken_from_env=True, ...)
-```
-
-Or pass the authtoken directly to the [forward](https://ngrok.github.io/ngrok-python/module.html) method:
-
-```python
-ngrok.forward(authtoken=token, ...)
-```
-
-Or set it for all connections with the [set_auth_token](https://ngrok.github.io/ngrok-python/module.html) method:
-
-```python
-ngrok.set_auth_token(token)
-```
-
-### Connection
-
-The [forward](https://ngrok.github.io/ngrok-python/module.html) method is the easiest way to start an ngrok session and establish a listener to a specified address. If an asynchronous runtime is running, the [forward](https://ngrok.github.io/ngrok-python/module.html) method returns a promise that resolves to the public listener object.
-
-With no arguments, the [forward](https://ngrok.github.io/ngrok-python/module.html) method will start an HTTP listener to `localhost` port `80`:
-
-```python
-listener = ngrok.forward()
-```
-
-You can pass the port number to forward on `localhost`:
-
-```python
-listener = ngrok.forward(4242)
-```
-
-Or you can specify the host and port via a string:
-
-```python
-listener = ngrok.forward("localhost:4242")
-```
-
-More options can be passed to the `forward` method to customize the connection:
-
-```python
-listener = ngrok.forward(8080, basic_auth="ngrok:online1line"})
-listener = ngrok.forward(8080, oauth_provider="google", oauth_allow_domains="example.com")
-```
-
-The second (optional) argument is the listener type, which defaults to `http`. To create a TCP listener:
-
-```python
-listener = ngrok.forward(25565, "tcp")
-```
-
-Since the options are kwargs, you can also use the `**` operator to pass a dictionary for configuration:
-
-```python
-options = {"authtoken_from_env":True, "response_header_add":"X-Awesome:yes"}
-listener = ngrok.forward(8080, **options)
-```
-
-See [Full Configuration](#full-configuration) for the list of possible configuration options.
-
-### Disconnection
-
-To close a listener use the [disconnect](https://ngrok.github.io/ngrok-python/module.html) method with the `url` of the listener to close. If there is an asynchronous runtime running the [disconnect](https://ngrok.github.io/ngrok-python/module.html) method returns a promise that resolves when the call is complete.
-
-```python
-ngrok.disconnect(url)
-```
-
-Or omit the `url` to close all listeners:
-
-```python
-ngrok.disconnect()
-```
-
-The [close](https://ngrok.github.io/ngrok-python/ngrok_listener.html) method on a listener will shut it down, and also stop the ngrok session if it is no longer needed. This method returns a promise that resolves when the listener is closed.
-
-```python
-await listener.close()
-```
-
-### List all Listeners
-
-To list all current non-closed listeners use the [get_listeners](https://ngrok.github.io/ngrok-python/module.html) method. If there is an asynchronous runtime running the [get_listeners](https://ngrok.github.io/ngrok-python/module.html) method returns a promise that resolves to the list of listener objects.
-
-```python
-listeners = ngrok.get_listeners()
-```
-
-### TLS Backends
-
-As of version `0.10.0` there is backend TLS connection support, validated by a filepath specified in the `SSL_CERT_FILE` environment variable, or falling back to the host OS installed trusted certificate authorities. So it is now possible to do this to connect:
-
-```python
-ngrok.forward("https://127.0.0.1:3000", authtoken_from_env=True)
-```
-
-If the service is using certs not trusted by the OS, such as self-signed certificates, add an environment variable like this before running: `SSL_CERT_FILE=/path/to/ca.crt`.
-
-### Unix Sockets
-
-You may also choose to use Unix Sockets instead of TCP. You can view an example of this [here](https://github.com/ngrok/ngrok-python/blob/main/examples/ngrok-http-full.py).
-
-A socket address may be passed directly into the listener `forward()` call as well by prefixing the address with `unix:`, for example `unix:/tmp/socket-123`.
-
-### Builders
-
-For more control over Sessions and Listeners, the builder classes can be used.
-
-A minimal example using the builder class looks like [the following](https://github.com/ngrok/ngrok-python/blob/main/examples/ngrok-http-minimal.py):
-
-```python
-async def create_listener():
-    session = await ngrok.NgrokSessionBuilder().authtoken_from_env().connect()
-    listener = await session.http_endpoint().listen()
-    print (f"Ingress established at {listener.url()}")
-    listener.forward("localhost:9000")
-```
-
-See here for a [Full Configuration Example](https://github.com/ngrok/ngrok-python/blob/main/examples/ngrok-http-full.py)
-
-### Full Configuration
-
-This example shows [all the possible configuration items of ngrok.forward](https://github.com/ngrok/ngrok-python/blob/main/examples/ngrok-forward-full.py):
-
-```python
-listener = ngrok.forward(
-    # session configuration
-    addr="localhost:8080",
-    authtoken="<authtoken>",
-    authtoken_from_env=True,
-    app_protocol="http2",
-    session_metadata="Online in One Line",
-    # listener configuration
-    metadata="example listener metadata from python",
-    domain="<domain>",
-    schemes=["HTTPS"],
-    proto="http",
-    proxy_proto="",  # One of: "", "1", "2"
-    labels="edge:edghts_2G...",  # Along with proto="labeled"
-    # module configuration
-    basic_auth=["ngrok:online1line"],
-    circuit_breaker=0.1,
-    compression=True,
-    allow_user_agent="^mozilla.*",
-    deny_user_agent="^curl.*",
-    allow_cidr="0.0.0.0/0",
-    deny_cidr="10.1.1.1/32",
-    crt=load_file("crt.pem"),
-    key=load_file("key.pem"),
-    mutual_tls_cas=load_file("ca.crt"),
-    oauth_provider="google",
-    oauth_allow_domains=["<domain>"],
-    oauth_allow_emails=["<email>"],
-    oauth_scopes=["<scope>"],
-    oauth_client_id="<id>",
-    oauth_client_secret="<id>",
-    oidc_issuer_url="<url>",
-    oidc_client_id="<id>",
-    oidc_client_secret="<secret>",
-    oidc_allow_domains=["<domain>"],
-    oidc_allow_emails=["<email>"],
-    oidc_scopes=["<scope>"],
-    policy="<policy_json>",
-    request_header_remove="X-Req-Nope",
-    response_header_remove="X-Res-Nope",
-    request_header_add="X-Req-Yup:true",
-    response_header_add="X-Res-Yup:true",
-    verify_webhook_provider="twilio",
-    verify_webhook_secret="asdf",
-    websocket_tcp_converter=True,
-)
-```
-
-# ASGI Runner
-
-`ngrok-python` comes bundled with an ASGI (Asynchronous Server Gateway Interface) runner `ngrok-asgi` that can be used for Uvicorn, Gunicorn, Django and more, with no code. 
-
-To use prefix your start up command for a Uvicorn or Gunicorn web server with either `ngrok-asgi` or `python -m ngrok`. 
-
-Any TCP or Unix Domain Socket arguments will be used to establish connectivity automatically. The ngrok listener can be configured using command flags, for instance adding `--basic-auth ngrok online1line` will introduce basic authentication to the ingress listener.
-
-### Uvicorn
-
-```shell
-# Basic Usage
-ngrok-asgi uvicorn mysite.asgi:application
-
-# With custom host and port
-ngrok-asgi uvicorn mysite.asgi:application \
-    --host localhost \
-    --port 1234
-
-# Using basic auth
-ngrok-asgi uvicorn mysite.asgi:application \
-    --host localhost \
-    --port 1234 \
-    --basic-auth ngrok online1line
-
-# Using custom sock file
-ngrok-asgi uvicorn mysite.asgi:application \
-    --uds /tmp/uvicorn.sock
-
-# Using module name
-python -m ngrok uvicorn mysite.asgi:application \
-    --oauth-provider google \
-    --allow-emails bob@example.com
-```
-
-### Gunicorn
-
-```shell
-# Basic Usage
-ngrok-asgi gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker
-
-# With custom host and port
-ngrok-asgi gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker \
-    --bind localhost:1234
-
-# Using webhook verifications
-ngrok-asgi gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker \
-    --webhook-verification twilio s3cr3t
-
-# Using custom sock file
-ngrok-asgi gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker \
-    --bind unix:/tmp/gunicorn.sock
-
-# Using module name
-python -m ngrok gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker --response-header X-Awesome True
-```
-
-# Examples
-
-#### Listeners
-  - [HTTP](https://github.com/ngrok/ngrok-python/tree/main/examples/ngrok-http-minimal.py)
-    - [Full Configuration Example](https://github.com/ngrok/ngrok-python/tree/main/examples/ngrok-http-full.py)
-  - [Labeled](https://github.com/ngrok/ngrok-python/tree/main/examples/ngrok-labeled.py)
-  - [TCP](https://github.com/ngrok/ngrok-python/tree/main/examples/ngrok-tcp.py)
-  - [TLS](https://github.com/ngrok/ngrok-python/tree/main/examples/ngrok-tls.py)
-
-#### Frameworks
-  - [AIOHTTP](https://github.com/ngrok/ngrok-python/tree/main/examples/aiohttp-ngrok.py)
-  - [AWS APP Runner](https://github.com/ngrok/ngrok-sdk-serverless-example)
-    - with [changes for Python](https://docs.aws.amazon.com/apprunner/latest/dg/service-source-code-python.html)
-  - Django
-    - [Single File Example](https://github.com/ngrok/ngrok-python/tree/main/examples/django-single-file.py)
-    - [Modify manage.py Example](https://github.com/ngrok/ngrok-python/tree/main/examples/djangosite/manage.py)
-    - [Modify asgi.py Example](https://github.com/ngrok/ngrok-python/tree/main/examples/djangosite/djangosite/ngrok-asgi.py)
-    - or [via `ngrok-asgi`](#asgi-runner)
-  - [Flask](https://github.com/ngrok/ngrok-python/tree/main/examples/flask-ngrok.py)
-  - [Gunicorn](#gunicorn)
-  - [Hypercorn](https://github.com/ngrok/ngrok-python/tree/main/examples/hypercorn-http2-ngrok.py)
-  - [Streamlit](https://github.com/ngrok/ngrok-python/tree/main/examples/streamlit/streamlit-ngrok.py)
-  - [Tornado](https://github.com/ngrok/ngrok-python/tree/main/examples/tornado-ngrok.py)
-  - [Uvicorn](https://github.com/ngrok/ngrok-python/tree/main/examples/uvicorn-ngrok.py)
-
-#### Machine Learning
-  - Gradio
-    - [ngrok-asgi Example](https://github.com/ngrok/ngrok-python/tree/main/examples/gradio/gradio-asgi.py)
-    - [gradio CLI Example](https://github.com/ngrok/ngrok-python/tree/main/examples/gradio/gradio-ngrok.py)
-  - [OpenPlayground](https://github.com/ngrok/ngrok-python/tree/main/examples/openplayground/run.py)
-  - [GPT4ALL](https://github.com/ngrok/ngrok-python/tree/main/examples/gpt4all/run.py)
-  - [Stable Diffusion WebUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui/) by AUTOMATIC1111
-    - `ngrok-python` is now built-in, see the `--ngrok` and `--ngrok-options` arguments.
-  - [Text Generation WebUI](https://github.com/oobabooga/text-generation-webui) by oobabooga
-    - `ngrok-python` is now built-in, see the `--extension ngrok` argument.
-
-# Platform Support
-
-Pre-built binaries are provided on PyPI for the following platforms:
-
-| OS         | i686 | x64 | aarch64 | arm |
-| ---------- | -----|-----|---------|-----|
-| Windows    |   ✓  |  ✓  |    *    |     |
-| MacOS      |      |  ✓  |    ✓    |     |
-| Linux      |      |  ✓  |    ✓    |  ✓  |
-| Linux musl |      |  ✓  |    ✓    |     |
-| FreeBSD    |      |  *  |         |     |
-
-> **Note**
-> `ngrok-python`, and [ngrok-rust](https://github.com/ngrok/ngrok-rust/) which it depends on, are open source, so it may be possible to build them for other platforms.
-> - Windows-aarch64 will be supported after the next release of [Ring](https://github.com/briansmith/ring/issues/1167).
-> - FreeBSD-x64 is built by the release process, but PyPI won't accept BSD flavors.
-
-# Dependencies
-
-- This project relies on [PyO3](https://pyo3.rs/), an excellent system to ease development and building of Rust plugins for Python.
-- Thank you to [OpenIoTHub](https://github.com/OpenIoTHub/ngrok) for handing over the ngrok name on PyPI.
-
-# Changelog
-
-Changes to `ngrok-python` are tracked under [CHANGELOG.md](https://github.com/ngrok/ngrok-python/blob/main/CHANGELOG.md).
-
-# Join the ngrok Community
-
-- Check out [our official docs](https://docs.ngrok.com)
-- Read about updates on [our blog](https://blog.ngrok.com)
-- Open an [issue](https://github.com/ngrok/ngrok-python/issues) or [pull request](https://github.com/ngrok/ngrok-python/pulls)
-- Join our [Slack community](https://ngrok.com/slack)
-- Follow us on [X / Twitter (@ngrokHQ)](https://twitter.com/ngrokhq)
-- Subscribe to our [Youtube channel (@ngrokHQ)](https://www.youtube.com/@ngrokhq)
-
-# License
-
-This project is dual-licensed under [Apache, Version 2.0](LICENSE-APACHE) and [MIT](LICENSE-MIT).
-You can choose between one of them if you use this work.
-
-### Contributions
-
-Unless you explicitly state otherwise, any contribution intentionally submitted
-for inclusion in `ngrok-python` by you, as defined in the Apache-2.0 license, shall be
-dual licensed as above, without any additional terms or conditions.
-
-# Development: Getting Started
-
-**Prerequisites:**
-- a valid Ngrok `authtoken`
--  `make` available in your PATH
-
-1. Update [Cargo.toml](./Cargo.toml) with the _latest supported_ ```ngrok = { version = "=VERSION_HERE" }``` from [ngrok-rust](https://github.com/ngrok/ngrok-rust/blob/main/ngrok/Cargo.toml#L3). `ngrok-rust` is used for the bindings in [src/rust_files_here.rs](./src)
-
-2. Run `make build` (builds the `rust` bindings / `python` dependencies)
-
-3. Happy developing!
-
-<br/>
-
-**Example Commands**:
-
-_building the project_
-```shell
-make develop
-```
-
-_running the entire test suite_
-```shell
-# running the entire test suite
-export NGROK_AUTHTOKEN="YOUR_AUTHTOKEN_HERE"; make test
-```
-
-_running an individual test_
-```shell
-# running an individual test
-export NGROK_AUTHTOKEN="YOUR_AUTHTOKEN_HERE"; make test="-k TEST_CLASS.NAME_OF_TEST" test
-```
-
-[See the MakeFile for more examples](./Makefile)
-
-### HTTP2 
-
-The examples include a minimal `hypercorn` HTTP/2 example if you run `make http2`. You can curl the endpoint logged with `INFO:ngrok.listener:Created` and verify the HTTP/2 response from `hypercorn`.
-
-```bash
-curl --http2 -v https://<YOUR_LISTENER_URL>
-*   Trying <YOUR_IP>:443...
-* Connected to a6278d6c07ce.ngrok.app (<YOUR_IP>) port 443 (#0)
-* ALPN, offering h2
-* ALPN, offering http/1.1
-...
-> GET / HTTP/2
-> Host: a6278d6c07ce.ngrok.app
-> user-agent: curl/7.81.0
-> accept: */*
->
-...
-< HTTP/2 200
-< content-type: text/plain
-< date: Fri, 01 Mar 2024 18:50:23 GMT
-< ngrok-agent-ips: <YOUR_AGENT_IP>
-< ngrok-trace-id: ed038ace04876818149cf0769bd43e38
-< server: hypercorn-h2
-<
-* TLSv1.2 (IN), TLS header, Supplemental data (23):
-* TLSv1.2 (IN), TLS header, Supplemental data (23):
-* Connection #0 to host <YOUR_LISTENER_URL> left intact
-hello
+# Installation
+
+The `ngrok-python` SDK can be installed from [PyPI](https://pypi.org/project/ngrok) via `pip`:
+
+```shell
+pip install ngrok
 ```
+
+# Quickstart
+
+1. [Install `ngrok-python`](#installation)
+2. Export your [authtoken from the ngrok dashboard](https://dashboard.ngrok.com/get-started/your-authtoken) as `NGROK_AUTHTOKEN` in your terminal
+3. Add the following code to your application to establish connectivity via the [forward method](https://github.com/ngrok/ngrok-python/blob/main/examples/ngrok-forward-minimal.py) through port `9000` on `localhost`:
+
+    ```python
+    # import ngrok python sdk
+    import ngrok
+    
+    # Establish connectivity
+    listener = ngrok.forward(9000, authtoken_from_env=True)
+    
+    # Output ngrok url to console
+    print(f"Ingress established at {listener.url()}")
+    ```
+
+That's it! Your application should now be available through the url output in your terminal. 
+
+> **Note**
+> You can find more examples in [the examples directory](https://github.com/ngrok/ngrok-python/tree/main/examples).
+
+# Documentation
+
+A full quickstart guide and API reference can be found in the [ngrok-python documentation](https://ngrok.github.io/ngrok-python/).
+
+### Authentication
+
+To use most of ngrok's features, you'll need an authtoken. To obtain one, sign up for free at [ngrok.com](https://dashboard.ngrok.com/signup) and retrieve it from the [authtoken page in your ngrok dashboard](https://dashboard.ngrok.com/get-started/your-authtoken). Once you have copied your authtoken, you can reference it in several ways.
+
+You can set it in the `NGROK_AUTHTOKEN` environment variable and pass `authtoken_from_env=True` to the [forward](https://ngrok.github.io/ngrok-python/module.html) method:
+
+```python
+ngrok.forward(authtoken_from_env=True, ...)
+```
+
+Or pass the authtoken directly to the [forward](https://ngrok.github.io/ngrok-python/module.html) method:
+
+```python
+ngrok.forward(authtoken=token, ...)
+```
+
+Or set it for all connections with the [set_auth_token](https://ngrok.github.io/ngrok-python/module.html) method:
+
+```python
+ngrok.set_auth_token(token)
+```
+
+### Connection
+
+The [forward](https://ngrok.github.io/ngrok-python/module.html) method is the easiest way to start an ngrok session and establish a listener to a specified address. If an asynchronous runtime is running, the [forward](https://ngrok.github.io/ngrok-python/module.html) method returns a promise that resolves to the public listener object.
+
+With no arguments, the [forward](https://ngrok.github.io/ngrok-python/module.html) method will start an HTTP listener to `localhost` port `80`:
+
+```python
+listener = ngrok.forward()
+```
+
+You can pass the port number to forward on `localhost`:
+
+```python
+listener = ngrok.forward(4242)
+```
+
+Or you can specify the host and port via a string:
+
+```python
+listener = ngrok.forward("localhost:4242")
+```
+
+More options can be passed to the `forward` method to customize the connection:
+
+```python
+listener = ngrok.forward(8080, basic_auth="ngrok:online1line"})
+listener = ngrok.forward(8080, oauth_provider="google", oauth_allow_domains="example.com")
+```
+
+The second (optional) argument is the listener type, which defaults to `http`. To create a TCP listener:
+
+```python
+listener = ngrok.forward(25565, "tcp")
+```
+
+Since the options are kwargs, you can also use the `**` operator to pass a dictionary for configuration:
+
+```python
+options = {"authtoken_from_env":True, "response_header_add":"X-Awesome:yes"}
+listener = ngrok.forward(8080, **options)
+```
+
+See [Full Configuration](#full-configuration) for the list of possible configuration options.
+
+### Disconnection
+
+To close a listener use the [disconnect](https://ngrok.github.io/ngrok-python/module.html) method with the `url` of the listener to close. If there is an asynchronous runtime running the [disconnect](https://ngrok.github.io/ngrok-python/module.html) method returns a promise that resolves when the call is complete.
+
+```python
+ngrok.disconnect(url)
+```
+
+Or omit the `url` to close all listeners:
+
+```python
+ngrok.disconnect()
+```
+
+The [close](https://ngrok.github.io/ngrok-python/ngrok_listener.html) method on a listener will shut it down, and also stop the ngrok session if it is no longer needed. This method returns a promise that resolves when the listener is closed.
+
+```python
+await listener.close()
+```
+
+### List all Listeners
+
+To list all current non-closed listeners use the [get_listeners](https://ngrok.github.io/ngrok-python/module.html) method. If there is an asynchronous runtime running the [get_listeners](https://ngrok.github.io/ngrok-python/module.html) method returns a promise that resolves to the list of listener objects.
+
+```python
+listeners = ngrok.get_listeners()
+```
+
+### TLS Backends
+
+As of version `0.10.0` there is backend TLS connection support, validated by a filepath specified in the `SSL_CERT_FILE` environment variable, or falling back to the host OS installed trusted certificate authorities. So it is now possible to do this to connect:
+
+```python
+ngrok.forward("https://127.0.0.1:3000", authtoken_from_env=True)
+```
+
+If the service is using certs not trusted by the OS, such as self-signed certificates, add an environment variable like this before running: `SSL_CERT_FILE=/path/to/ca.crt`. There is also a `verify_upstream_tls=False` option to disable certification verification.
+
+### Unix Sockets
+
+You may also choose to use Unix Sockets instead of TCP. You can view an example of this [here](https://github.com/ngrok/ngrok-python/blob/main/examples/ngrok-http-full.py).
+
+A socket address may be passed directly into the listener `forward()` call as well by prefixing the address with `unix:`, for example `unix:/tmp/socket-123`.
+
+### Builders
+
+For more control over Sessions and Listeners, the builder classes can be used.
+
+A minimal example using the builder class looks like [the following](https://github.com/ngrok/ngrok-python/blob/main/examples/ngrok-http-minimal.py):
+
+```python
+async def create_listener():
+    session = await ngrok.NgrokSessionBuilder().authtoken_from_env().connect()
+    listener = await session.http_endpoint().listen()
+    print (f"Ingress established at {listener.url()}")
+    listener.forward("localhost:9000")
+```
+
+See here for a [Full Configuration Example](https://github.com/ngrok/ngrok-python/blob/main/examples/ngrok-http-full.py)
+
+### Full Configuration
+
+This example shows [all the possible configuration items of ngrok.forward](https://github.com/ngrok/ngrok-python/blob/main/examples/ngrok-forward-full.py):
+
+```python
+listener = ngrok.forward(
+    # session configuration
+    addr="localhost:8080",
+    authtoken="<authtoken>",
+    authtoken_from_env=True,
+    app_protocol="http2",
+    session_metadata="Online in One Line",
+    # advanced session connection configuration
+    server_addr="example.com:443",
+    root_cas="trusted",
+    session_ca_cert=load_file("ca.pem"),
+    # listener configuration
+    metadata="example listener metadata from python",
+    domain="<domain>",
+    schemes=["HTTPS"],
+    proto="http",
+    proxy_proto="",  # One of: "", "1", "2"
+    labels="edge:edghts_2G...",  # Along with proto="labeled"
+    # module configuration
+    basic_auth=["ngrok:online1line"],
+    circuit_breaker=0.1,
+    compression=True,
+    allow_user_agent="^mozilla.*",
+    deny_user_agent="^curl.*",
+    allow_cidr="0.0.0.0/0",
+    deny_cidr="10.1.1.1/32",
+    crt=load_file("crt.pem"),
+    key=load_file("key.pem"),
+    mutual_tls_cas=load_file("ca.crt"),
+    oauth_provider="google",
+    oauth_allow_domains=["<domain>"],
+    oauth_allow_emails=["<email>"],
+    oauth_scopes=["<scope>"],
+    oauth_client_id="<id>",
+    oauth_client_secret="<id>",
+    oidc_issuer_url="<url>",
+    oidc_client_id="<id>",
+    oidc_client_secret="<secret>",
+    oidc_allow_domains=["<domain>"],
+    oidc_allow_emails=["<email>"],
+    oidc_scopes=["<scope>"],
+    policy="<policy_json>",
+    request_header_remove="X-Req-Nope",
+    response_header_remove="X-Res-Nope",
+    request_header_add="X-Req-Yup:true",
+    response_header_add="X-Res-Yup:true",
+    verify_upstream_tls=False,
+    verify_webhook_provider="twilio",
+    verify_webhook_secret="asdf",
+    websocket_tcp_converter=True,
+)
+```
+
+# ASGI Runner
+
+`ngrok-python` comes bundled with an ASGI (Asynchronous Server Gateway Interface) runner `ngrok-asgi` that can be used for Uvicorn, Gunicorn, Django and more, with no code. 
+
+To use prefix your start up command for a Uvicorn or Gunicorn web server with either `ngrok-asgi` or `python -m ngrok`. 
+
+Any TCP or Unix Domain Socket arguments will be used to establish connectivity automatically. The ngrok listener can be configured using command flags, for instance adding `--basic-auth ngrok online1line` will introduce basic authentication to the ingress listener.
+
+### Uvicorn
+
+```shell
+# Basic Usage
+ngrok-asgi uvicorn mysite.asgi:application
+
+# With custom host and port
+ngrok-asgi uvicorn mysite.asgi:application \
+    --host localhost \
+    --port 1234
+
+# Using basic auth
+ngrok-asgi uvicorn mysite.asgi:application \
+    --host localhost \
+    --port 1234 \
+    --basic-auth ngrok online1line
+
+# Using custom sock file
+ngrok-asgi uvicorn mysite.asgi:application \
+    --uds /tmp/uvicorn.sock
+
+# Using module name
+python -m ngrok uvicorn mysite.asgi:application \
+    --oauth-provider google \
+    --allow-emails bob@example.com
+```
+
+### Gunicorn
+
+```shell
+# Basic Usage
+ngrok-asgi gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker
+
+# With custom host and port
+ngrok-asgi gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker \
+    --bind localhost:1234
+
+# Using webhook verifications
+ngrok-asgi gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker \
+    --webhook-verification twilio s3cr3t
+
+# Using custom sock file
+ngrok-asgi gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker \
+    --bind unix:/tmp/gunicorn.sock
+
+# Using module name
+python -m ngrok gunicorn mysite.asgi:application -k uvicorn.workers.UvicornWorker --response-header X-Awesome True
+```
+
+# Examples
+
+#### Listeners
+  - [HTTP](https://github.com/ngrok/ngrok-python/tree/main/examples/ngrok-http-minimal.py)
+    - [Full Configuration Example](https://github.com/ngrok/ngrok-python/tree/main/examples/ngrok-http-full.py)
+  - [Labeled](https://github.com/ngrok/ngrok-python/tree/main/examples/ngrok-labeled.py)
+  - [TCP](https://github.com/ngrok/ngrok-python/tree/main/examples/ngrok-tcp.py)
+  - [TLS](https://github.com/ngrok/ngrok-python/tree/main/examples/ngrok-tls.py)
+
+#### Frameworks
+  - [AIOHTTP](https://github.com/ngrok/ngrok-python/tree/main/examples/aiohttp-ngrok.py)
+  - [AWS APP Runner](https://github.com/ngrok/ngrok-sdk-serverless-example)
+    - with [changes for Python](https://docs.aws.amazon.com/apprunner/latest/dg/service-source-code-python.html)
+  - Django
+    - [Single File Example](https://github.com/ngrok/ngrok-python/tree/main/examples/django-single-file.py)
+    - [Modify manage.py Example](https://github.com/ngrok/ngrok-python/tree/main/examples/djangosite/manage.py)
+    - [Modify asgi.py Example](https://github.com/ngrok/ngrok-python/tree/main/examples/djangosite/djangosite/ngrok-asgi.py)
+    - or [via `ngrok-asgi`](#asgi-runner)
+  - [Flask](https://github.com/ngrok/ngrok-python/tree/main/examples/flask-ngrok.py)
+  - [Gunicorn](#gunicorn)
+  - [Hypercorn](https://github.com/ngrok/ngrok-python/tree/main/examples/hypercorn-http2-ngrok.py)
+  - [Streamlit](https://github.com/ngrok/ngrok-python/tree/main/examples/streamlit/streamlit-ngrok.py)
+  - [Tornado](https://github.com/ngrok/ngrok-python/tree/main/examples/tornado-ngrok.py)
+  - [Uvicorn](https://github.com/ngrok/ngrok-python/tree/main/examples/uvicorn-ngrok.py)
+
+#### Machine Learning
+  - Gradio
+    - [ngrok-asgi Example](https://github.com/ngrok/ngrok-python/tree/main/examples/gradio/gradio-asgi.py)
+    - [gradio CLI Example](https://github.com/ngrok/ngrok-python/tree/main/examples/gradio/gradio-ngrok.py)
+  - [OpenPlayground](https://github.com/ngrok/ngrok-python/tree/main/examples/openplayground/run.py)
+  - [GPT4ALL](https://github.com/ngrok/ngrok-python/tree/main/examples/gpt4all/run.py)
+  - [Stable Diffusion WebUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui/) by AUTOMATIC1111
+    - `ngrok-python` is now built-in, see the `--ngrok` and `--ngrok-options` arguments.
+  - [Text Generation WebUI](https://github.com/oobabooga/text-generation-webui) by oobabooga
+    - `ngrok-python` is now built-in, see the `--extension ngrok` argument.
+
+# Platform Support
+
+Pre-built binaries are provided on PyPI for the following platforms:
+
+| OS         | i686 | x64 | aarch64 | arm |
+| ---------- | -----|-----|---------|-----|
+| Windows    |   ✓  |  ✓  |    *    |     |
+| MacOS      |      |  ✓  |    ✓    |     |
+| Linux      |      |  ✓  |    ✓    |  ✓  |
+| Linux musl |      |  ✓  |    ✓    |     |
+| FreeBSD    |      |  *  |         |     |
+
+> **Note**
+> `ngrok-python`, and [ngrok-rust](https://github.com/ngrok/ngrok-rust/) which it depends on, are open source, so it may be possible to build them for other platforms.
+> - Windows-aarch64 will be supported after the next release of [Ring](https://github.com/briansmith/ring/issues/1167).
+> - FreeBSD-x64 is built by the release process, but PyPI won't accept BSD flavors.
+
+# Dependencies
+
+- This project relies on [PyO3](https://pyo3.rs/), an excellent system to ease development and building of Rust plugins for Python.
+- Thank you to [OpenIoTHub](https://github.com/OpenIoTHub/ngrok) for handing over the ngrok name on PyPI.
+
+# Changelog
+
+Changes to `ngrok-python` are tracked under [CHANGELOG.md](https://github.com/ngrok/ngrok-python/blob/main/CHANGELOG.md).
+
+# Join the ngrok Community
+
+- Check out [our official docs](https://docs.ngrok.com)
+- Read about updates on [our blog](https://blog.ngrok.com)
+- Open an [issue](https://github.com/ngrok/ngrok-python/issues) or [pull request](https://github.com/ngrok/ngrok-python/pulls)
+- Join our [Slack community](https://ngrok.com/slack)
+- Follow us on [X / Twitter (@ngrokHQ)](https://twitter.com/ngrokhq)
+- Subscribe to our [Youtube channel (@ngrokHQ)](https://www.youtube.com/@ngrokhq)
+
+# License
+
+This project is dual-licensed under [Apache, Version 2.0](LICENSE-APACHE) and [MIT](LICENSE-MIT).
+You can choose between one of them if you use this work.
+
+### Contributions
+
+Unless you explicitly state otherwise, any contribution intentionally submitted
+for inclusion in `ngrok-python` by you, as defined in the Apache-2.0 license, shall be
+dual licensed as above, without any additional terms or conditions.
+
+# Development: Getting Started
+
+**Prerequisites:**
+- a valid Ngrok `authtoken`
+-  `make` available in your PATH
+
+1. Update [Cargo.toml](./Cargo.toml) with the _latest supported_ ```ngrok = { version = "=VERSION_HERE" }``` from [ngrok-rust](https://github.com/ngrok/ngrok-rust/blob/main/ngrok/Cargo.toml#L3). `ngrok-rust` is used for the bindings in [src/rust_files_here.rs](./src)
+
+2. Run `make build` (builds the `rust` bindings / `python` dependencies)
+
+3. Happy developing!
+
+<br/>
+
+**Example Commands**:
+
+_building the project_
+```shell
+make develop
+```
+
+_running the entire test suite_
+```shell
+# running the entire test suite
+export NGROK_AUTHTOKEN="YOUR_AUTHTOKEN_HERE"; make test
+```
+
+_running an individual test_
+```shell
+# running an individual test
+export NGROK_AUTHTOKEN="YOUR_AUTHTOKEN_HERE"; make test="-k TEST_CLASS.NAME_OF_TEST" test
+```
+
+[See the MakeFile for more examples](./Makefile)
+
+### HTTP2 
+
+The examples include a minimal `hypercorn` HTTP/2 example if you run `make http2`. You can curl the endpoint logged with `INFO:ngrok.listener:Created` and verify the HTTP/2 response from `hypercorn`.
+
+```bash
+curl --http2 -v https://<YOUR_LISTENER_URL>
+*   Trying <YOUR_IP>:443...
+* Connected to a6278d6c07ce.ngrok.app (<YOUR_IP>) port 443 (#0)
+* ALPN, offering h2
+* ALPN, offering http/1.1
+...
+> GET / HTTP/2
+> Host: a6278d6c07ce.ngrok.app
+> user-agent: curl/7.81.0
+> accept: */*
+>
+...
+< HTTP/2 200
+< content-type: text/plain
+< date: Fri, 01 Mar 2024 18:50:23 GMT
+< ngrok-agent-ips: <YOUR_AGENT_IP>
+< ngrok-trace-id: ed038ace04876818149cf0769bd43e38
+< server: hypercorn-h2
+<
+* TLSv1.2 (IN), TLS header, Supplemental data (23):
+* TLSv1.2 (IN), TLS header, Supplemental data (23):
+* Connection #0 to host <YOUR_LISTENER_URL> left intact
+hello
+```
+
```

## Comparing `ngrok-1.2.0.dist-info/license_files/LICENSE-APACHE` & `ngrok-1.3.0.dist-info/license_files/LICENSE-APACHE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

## Comparing `ngrok-1.2.0.dist-info/license_files/LICENSE-MIT` & `ngrok-1.3.0.dist-info/license_files/LICENSE-MIT`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2022 ngrok, Inc.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright 2022 ngrok, Inc.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

## Comparing `ngrok-1.2.0.dist-info/RECORD` & `ngrok-1.3.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-ngrok-1.2.0.dist-info/METADATA,sha256=ZoCab2-iBao_EDoctMkM_XI33sLyBE4_d86whggzxCo,19032
-ngrok-1.2.0.dist-info/WHEEL,sha256=ZnSmVnashXVUiLCKmp20reANrPJdUjOt4GHgJoJkZ3E,96
-ngrok-1.2.0.dist-info/entry_points.txt,sha256=qIWUBK__RJ7O3GDMiCU9dKnLLqlzJdXpJxat7IQ1cZU,53
-ngrok-1.2.0.dist-info/license_files/LICENSE-APACHE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-ngrok-1.2.0.dist-info/license_files/LICENSE-MIT,sha256=k2H9oRPELrEi8YIKhwwvdIYmJTrpic5YINff621X-Fw,1056
-ngrok/mypy.ini,sha256=0HSIknBt36prarR7YT4-2ouN8FIKYviozBoFdkGv_es,34
-ngrok/ngrok.pyi,sha256=cfM7PfU6BlMXammXitFHAulC-RVCakgZO0Vi8ma6Sts,7330
-ngrok/ngrok_parser.py,sha256=L4imEl-Ce1gIzm54lz1q1WQGASPxcFHcNqK3jGm-XJs,5149
+ngrok-1.3.0.dist-info/METADATA,sha256=glIOSPcCAGxeIn5XiJdHV30PwzaQQu4-Dp6Eco2xgfQ,18864
+ngrok-1.3.0.dist-info/WHEEL,sha256=ChFH4DfmYfghq6b_fFI-43bbDR_dKhx-VMkCzopdRlI,106
+ngrok-1.3.0.dist-info/entry_points.txt,sha256=qIWUBK__RJ7O3GDMiCU9dKnLLqlzJdXpJxat7IQ1cZU,53
+ngrok-1.3.0.dist-info/license_files/LICENSE-APACHE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+ngrok-1.3.0.dist-info/license_files/LICENSE-MIT,sha256=wmZKSCSYH5ESlCdSKshPJ4zUma0hxKfzX8RAHZYYlrk,1050
+ngrok.libs/libgcc_s-60abea67.so.1,sha256=5Ymeh-PwFBkI5B-deNMLyVYu2EYmgIu7iQGitm7d2t4,724137
+ngrok/__main__.py,sha256=Sr3uOOqqGHugFUuMlova3d21ljtZV7mhZ24StWddr_E,6323
+ngrok/__init__.py,sha256=Sl_WfBL8squMtOUw_9jo51R5uqOKMfUxMAIoHAP0vi0,104
 ngrok/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ngrok/__init__.py,sha256=SVQFcbYIelbBItRJLTUbvEnhgLsOvauDlC3_hMuj-Ck,109
-ngrok/__main__.py,sha256=OO0UBQTbA93gsBi75ZSOi8eaY-_o1SG1HXkWVzMHCrk,6547
-ngrok/ngrok.pyd,sha256=mIR7ibjwbUN9D7kz5c-RHL_tH-xPzZtoF19MrGINgAc,8264192
-ngrok-1.2.0.dist-info/RECORD,,
+ngrok/ngrok.pyi,sha256=W9Q_puL6bn0i47g0WaVFmfMtbpCTImxNxTvIS7IdumM,7613
+ngrok/mypy.ini,sha256=xMNPYqFoi-LjalA_e6r7ey8X_RG5YotZ2WunPjsAI3g,32
+ngrok/ngrok_parser.py,sha256=je_O422GC4Vb54AVLWN_WQXOcZxawmVpfhJWJCipRTo,5011
+ngrok/ngrok.abi3.so,sha256=5jqQ7SFohSZHm3ynWhq3uYRSWzP7sn_ZhLrUZT_evNo,6491521
+ngrok-1.3.0.dist-info/RECORD,,
```

