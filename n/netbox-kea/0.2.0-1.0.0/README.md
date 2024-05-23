# Comparing `tmp/netbox_kea-0.2.0.tar.gz` & `tmp/netbox_kea-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_kea-0.2.0.tar", max compression
+gzip compressed data, was "netbox_kea-1.0.0.tar", max compression
```

## Comparing `netbox_kea-0.2.0.tar` & `netbox_kea-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,30 @@
--rw-r--r--   0        0        0    11358 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/LICENSE
--rw-r--r--   0        0        0     3173 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/README.md
--rw-r--r--   0        0        0      288 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/__init__.py
--rw-r--r--   0        0        0        0 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/api/__init__.py
--rw-r--r--   0        0        0      719 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/api/serializers.py
--rw-r--r--   0        0        0      190 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/api/urls.py
--rw-r--r--   0        0        0      322 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/api/views.py
--rw-r--r--   0        0        0      364 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/constants.py
--rw-r--r--   0        0        0      229 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/filtersets.py
--rw-r--r--   0        0        0     6620 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/forms.py
--rw-r--r--   0        0        0      404 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/graphql.py
--rw-r--r--   0        0        0     2563 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/kea.py
--rw-r--r--   0        0        0     1633 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/migrations/0001_initial.py
--rw-r--r--   0        0        0      650 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/migrations/0002_alter_server_options_server_dhcp4_server_dhcp6.py
--rw-r--r--   0        0        0        0 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/migrations/__init__.py
--rw-r--r--   0        0        0     3895 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/models.py
--rw-r--r--   0        0        0      620 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/navigation.py
--rw-r--r--   0        0        0     7597 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/tables.py
--rw-r--r--   0        0        0      360 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/templates/netbox_kea/exception_htmx.html
--rw-r--r--   0        0        0      505 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/templates/netbox_kea/inc/configure_table.html
--rw-r--r--   0        0        0      991 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/templates/netbox_kea/server.html
--rw-r--r--   0        0        0       51 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/templates/netbox_kea/server_base.html
--rw-r--r--   0        0        0      492 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/templates/netbox_kea/server_dhcp_leases.html
--rw-r--r--   0        0        0     4547 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/templates/netbox_kea/server_dhcp_leases_htmx.html
--rw-r--r--   0        0        0     1103 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/templates/netbox_kea/server_dhcp_subnets.html
--rw-r--r--   0        0        0     1180 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/templates/netbox_kea/server_leases_delete.html
--rw-r--r--   0        0        0      563 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/templates/netbox_kea/server_status.html
--rw-r--r--   0        0        0      419 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/templates/netbox_kea/service_disabled.html
--rw-r--r--   0        0        0      772 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/urls.py
--rw-r--r--   0        0        0     2792 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/utilities.py
--rw-r--r--   0        0        0    18214 2023-08-23 03:09:55.714019 netbox_kea-0.2.0/netbox_kea/views.py
--rw-r--r--   0        0        0      648 2023-08-23 03:09:55.718019 netbox_kea-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3638 1970-01-01 00:00:00.000000 netbox_kea-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-23 18:48:06.935831 netbox_kea-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3173 2024-05-23 18:48:06.935831 netbox_kea-1.0.0/README.md
+-rw-r--r--   0        0        0      288 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/api/__init__.py
+-rw-r--r--   0        0        0      778 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/api/serializers.py
+-rw-r--r--   0        0        0      190 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/api/urls.py
+-rw-r--r--   0        0        0      322 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/api/views.py
+-rw-r--r--   0        0        0      364 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/constants.py
+-rw-r--r--   0        0        0      229 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/filtersets.py
+-rw-r--r--   0        0        0     6666 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/forms.py
+-rw-r--r--   0        0        0      459 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/graphql.py
+-rw-r--r--   0        0        0     2532 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/kea.py
+-rw-r--r--   0        0        0     1633 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/migrations/0001_initial.py
+-rw-r--r--   0        0        0      650 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/migrations/0002_alter_server_options_server_dhcp4_server_dhcp6.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/migrations/__init__.py
+-rw-r--r--   0        0        0     3895 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/models.py
+-rw-r--r--   0        0        0      490 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/navigation.py
+-rw-r--r--   0        0        0     7060 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/tables.py
+-rw-r--r--   0        0        0      360 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/templates/netbox_kea/exception_htmx.html
+-rw-r--r--   0        0        0     1314 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/templates/netbox_kea/inc/server_dhcp_leases_paginator.html
+-rw-r--r--   0        0        0      946 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/templates/netbox_kea/server.html
+-rw-r--r--   0        0        0      599 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/templates/netbox_kea/server_dhcp_leases.html
+-rw-r--r--   0        0        0     3238 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/templates/netbox_kea/server_dhcp_leases_htmx.html
+-rw-r--r--   0        0        0      764 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/templates/netbox_kea/server_dhcp_subnets.html
+-rw-r--r--   0        0        0      563 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/templates/netbox_kea/server_status.html
+-rw-r--r--   0        0        0      772 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/urls.py
+-rw-r--r--   0        0        0     2780 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/utilities.py
+-rw-r--r--   0        0        0    18368 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/netbox_kea/views.py
+-rw-r--r--   0        0        0      673 2024-05-23 18:48:06.939831 netbox_kea-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3692 1970-01-01 00:00:00.000000 netbox_kea-1.0.0/PKG-INFO
```

### Comparing `netbox_kea-0.2.0/LICENSE` & `netbox_kea-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.2.0/README.md` & `netbox_kea-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 
 - Kea doesn't provide a way to get a list of subnets without an additional hook library.
   Thus, this plugin lists subnets using the `config-get` command. This means that the entire config will be fetched just to get the configured subnets!
   This may be an expensive operation.
 
 ## Requirements
 
-- NetBox > v3.5
+- NetBox >= v4.0
 - [Kea Control Agent](https://kea.readthedocs.io/en/latest/arm/agent.html)
 - [`lease_cmds`](https://kea.readthedocs.io/en/latest/arm/hooks.html#lease-cmds-lease-commands-for-easier-lease-management) hook library
 
 ## Compatibility
 
-- This plugin was tested with Kea v2.2.0 with the `memfile` lease database.
+- This plugin is tested with Kea v2.4.1 with the `memfile` lease database.
   Other versions and lease databases may also work.
 
 ## Installation
 
 1. Add `netbox-kea` to `local_requirements.txt`.
 
 2. Enable the plugin in `configuration.py`
```

### Comparing `netbox_kea-0.2.0/netbox_kea/forms.py` & `netbox_kea-1.0.0/netbox_kea/forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Any, Dict, Literal, Optional
+from typing import Any, Literal, Optional
 
 from django import forms
 from django.core.exceptions import ValidationError
 from netaddr import EUI, AddrFormatError, IPAddress, IPNetwork, mac_unix_expanded
 from netbox.forms import NetBoxModelFilterSetForm, NetBoxModelForm
-from utilities.forms import BOOLEAN_WITH_BLANK_CHOICES, BootstrapMixin
+from utilities.forms import BOOLEAN_WITH_BLANK_CHOICES
 from utilities.forms.fields import TagFilterField
 
 from . import constants
 from .models import Server
 from .utilities import is_hex_string
 
 
@@ -51,19 +51,19 @@
     dhcp6 = forms.NullBooleanField(
         label="DHCPv6",
         required=False,
         widget=forms.Select(choices=BOOLEAN_WITH_BLANK_CHOICES),
     )
 
 
-class BaseLeasesSarchForm(BootstrapMixin, forms.Form):
+class BaseLeasesSarchForm(forms.Form):
     q = forms.CharField(label="Search")
     page = forms.CharField(required=False, widget=VeryHiddenInput)
 
-    def clean(self) -> Optional[Dict[str, Any]]:
+    def clean(self) -> Optional[dict[str, Any]]:
         ip_version = self.Meta.ip_version
         cleaned_data = super().clean()
         q = cleaned_data.get("q")
         by = cleaned_data.get("by")
 
         if q and not by:
             raise ValidationError({"by": "Search attribute is empty."})
@@ -77,65 +77,59 @@
                 net = IPNetwork(q, version=ip_version)
                 if net.ip != net.cidr.ip:
                     raise ValidationError(
                         {"q": f"{net} is not a valid prefix. Did you mean {net.cidr}?"}
                     )
                 cleaned_data["q"] = net
             except (AddrFormatError, TypeError, ValueError) as e:
-                raise ValidationError(
-                    {"q": f"Invalid IPv{ip_version} subnet: {cleaned_data['q']}"}
-                ) from e
+                raise ValidationError({"q": f"Invalid IPv{ip_version} subnet."}) from e
         elif by == constants.BY_SUBNET_ID:
             try:
                 i = int(q)
                 if i <= 0:
-                    raise ValidationError({"q": f"Invalid subnet ID: {q}"})
+                    raise ValidationError({"q": "Invalid subnet ID."})
                 cleaned_data["q"] = i
             except ValueError as e:
-                raise ValidationError(
-                    {"q": f"Subnet ID must be an integer: {q}"}
-                ) from e
+                raise ValidationError({"q": "Subnet ID must be an integer."}) from e
         elif by == constants.BY_IP:
             try:
                 # use IPAddress to normalize values
                 cleaned_data["q"] = str(IPAddress(q, version=ip_version))
             except (AddrFormatError, TypeError, ValueError) as e:
-                raise ValidationError(
-                    {"q": f"Invalid IPv{ip_version} address: {q}"}
-                ) from e
-        elif by in (constants.BY_HW_ADDRESS):
+                raise ValidationError({"q": f"Invalid IPv{ip_version} address."}) from e
+        elif by == constants.BY_HW_ADDRESS:
             try:
                 cleaned_data["q"] = str(EUI(q, version=48, dialect=mac_unix_expanded))
             except (AddrFormatError, TypeError, ValueError) as e:
-                raise ValidationError({"q": f"Invalid hardware address: {q}"}) from e
-        elif by in constants.BY_DUID:
+                raise ValidationError({"q": "Invalid hardware address."}) from e
+        elif by == constants.BY_DUID:
             if not is_hex_string(
                 q, constants.DUID_MIN_OCTETS, constants.DUID_MAX_OCTETS
             ):
-                raise ValidationError({"q": f"Invalid DUID: {q}"})
+                raise ValidationError({"q": "Invalid DUID."})
             cleaned_data["q"] = q.replace("-", "")
-        elif by in constants.BY_CLIENT_ID:
+        elif by == constants.BY_CLIENT_ID:
             if not is_hex_string(
                 q, constants.CLIENT_ID_MIN_OCTETS, constants.DUID_MAX_OCTETS
             ):
-                raise ValidationError({"q": f"Invalid client ID: {q}"})
+                raise ValidationError({"q": "Invalid client ID."})
             cleaned_data["q"] = q.replace("-", "")
 
         page = cleaned_data["page"]
         if page:
             if by != constants.BY_SUBNET:
                 raise ValidationError({"page": "page is only supported with subnet."})
             try:
                 page_ip = IPAddress(page, version=ip_version)
                 if page_ip not in cleaned_data["q"]:
                     raise ValidationError({"page": "page is not in the given subnet"})
 
                 cleaned_data["page"] = str(page_ip)
             except AddrFormatError as e:
-                raise ValidationError({"page": f"Invalid IP: {page}"}) from e
+                raise ValidationError({"page": "Invalid IP."}) from e
 
 
 class Leases4SearchForm(BaseLeasesSarchForm):
     by = forms.ChoiceField(
         label="Attribute",
         choices=(
             (constants.BY_IP, "IP Address"),
@@ -174,19 +168,29 @@
         self._version = version
         super().__init__(*args, widget=forms.MultipleHiddenInput, **kwargs)
 
     def clean(self, value: Any) -> Any:
         if not isinstance(value, list):
             raise forms.ValidationError(f"Expected a list, got {type(value)}.")
 
+        if len(value) == 0:
+            raise forms.ValidationError("IP address list is empty.")
+
         try:
             return [str(IPAddress(ip, version=self._version)) for ip in value]
         except (AddrFormatError, ValueError) as e:
             raise forms.ValidationError("Invalid IP address.") from e
 
 
-class Lease6DeleteForm(forms.Form):
+class BaseLeaseDeleteForm(forms.Form):
+    return_url = forms.CharField(
+        required=False,
+        widget=forms.HiddenInput(),
+    )
+
+
+class Lease6DeleteForm(BaseLeaseDeleteForm):
     pk = MultipleIPField(6)
 
 
-class Lease4DeleteForm(forms.Form):
+class Lease4DeleteForm(BaseLeaseDeleteForm):
     pk = MultipleIPField(4)
```

### Comparing `netbox_kea-0.2.0/netbox_kea/kea.py` & `netbox_kea-1.0.0/netbox_kea/kea.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from typing import Any, Dict, List, Optional, Sequence, TypedDict, Union
+from typing import Any, Optional, Sequence, TypedDict
 
 import requests
 from requests.models import HTTPBasicAuth
 
 
 class KeaResponse(TypedDict):
     result: int
-    arguments: Optional[Dict[str, Any]]
+    arguments: Optional[dict[str, Any]]
     text: Optional[str]
 
 
 class KeaClient:
     def __init__(
         self,
         url: str,
         username: Optional[str] = None,
         password: Optional[str] = None,
-        verify: Optional[Union[bool, str]] = None,
+        verify: Optional[bool | str] = None,
         client_cert: Optional[str] = None,
         client_key: Optional[str] = None,
         timeout: int = 30,
     ):
         if (client_cert is not None and client_key is None) or (
             client_cert is None and client_key is not None
         ):
@@ -36,19 +36,19 @@
             self._session.auth = HTTPBasicAuth(username, password)
         if client_cert is not None and client_key is not None:
             self._session.cert = (client_cert, client_key)
 
     def command(
         self,
         command: str,
-        service: Optional[List[str]] = None,
-        arguments: Optional[Dict[str, Any]] = None,
-        check: Union[None, Sequence[int]] = (0,),
-    ) -> List[KeaResponse]:
-        body: Dict[str, Any] = {"command": command}
+        service: Optional[list[str]] = None,
+        arguments: Optional[dict[str, Any]] = None,
+        check: None | Sequence[int] = (0,),
+    ) -> list[KeaResponse]:
+        body: dict[str, Any] = {"command": command}
 
         if service is not None:
             body["service"] = service
 
         if arguments is not None:
             body["arguments"] = arguments
 
@@ -70,12 +70,12 @@
 
         if msg is None:
             msg = f"Kea returned result[{index}] {self.response.get('result')}"
         message = f"{msg}: {self.response.get('text')}"
         super().__init__(message)
 
 
-def check_response(resp: List[KeaResponse], ok_codes: Sequence[int]) -> None:
+def check_response(resp: list[KeaResponse], ok_codes: Sequence[int]) -> None:
     """Raise a KeaException for any non 0 responses."""
     for idx, kr in enumerate(resp):
         if kr["result"] not in ok_codes:
             raise KeaException(kr, index=idx)
```

### Comparing `netbox_kea-0.2.0/netbox_kea/migrations/0001_initial.py` & `netbox_kea-1.0.0/netbox_kea/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.2.0/netbox_kea/migrations/0002_alter_server_options_server_dhcp4_server_dhcp6.py` & `netbox_kea-1.0.0/netbox_kea/migrations/0002_alter_server_options_server_dhcp4_server_dhcp6.py`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.2.0/netbox_kea/models.py` & `netbox_kea-1.0.0/netbox_kea/models.py`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.2.0/netbox_kea/tables.py` & `netbox_kea-1.0.0/netbox_kea/tables.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import django_tables2 as tables
 from django.urls import reverse
-from netbox.tables import BaseTable, BooleanColumn, NetBoxTable, ToggleColumn
+from django.utils.http import urlencode
+from netbox.tables import BaseTable, BooleanColumn, NetBoxTable, ToggleColumn, columns
 
 from netbox_kea.utilities import format_duration
 
 from .models import Server
 
-SUBNET_ACTIONS = """<span class="dropdown">
+SUBNET_ACTIONS = """<span class="btn-group dropdown">
   <a class="btn btn-sm btn-secondary dropdown-toggle" href="#" type="button" data-bs-toggle="dropdown">
   <i class="mdi mdi-magnify"></i></a>
   <ul class="dropdown-menu">
-    {% if record.id %}
+    {% if record.pk %}
     <li>
-      <a href="{% url "ipam:prefix" pk=record.id %}" class="dropdown-item">
+      <a href="{% url "ipam:prefix" pk=record.pk %}" class="dropdown-item">
         <i class="mdi mdi-open-in-app" aria-hidden="true" title="View prefix"></i>
         View prefix
       </a>
     </li>
     {% endif %}
     {% if record.subnet %}
     <li>
@@ -27,15 +28,15 @@
     </li>
     {% endif %}
   </ul>
 </span>
 """  # noqa: E501
 
 
-LEASE_ACTIONS = """<span class="dropdown">
+LEASE_ACTIONS = """<span class="btn-group dropdown">
     <a class="btn btn-sm btn-secondary dropdown-toggle" href="#" type="button" data-bs-toggle="dropdown">
     <i class="mdi mdi-magnify"></i></a>
     <ul class="dropdown-menu">
         {% if record.ip_address %}
         <li>
             <a href="{% url "ipam:ipaddress_list" %}?address={{ record.ip_address }}" class="dropdown-item">
                 <i class="mdi mdi-magnify" aria-hidden="true" title="Search IPs"></i>
@@ -123,72 +124,55 @@
 class GenericTable(BaseTable):
     exempt_columns = ("actions", "pk")
 
     class Meta(BaseTable.Meta):
         empty_text = "No rows"
         fields = ()
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
     @property
     def objects_count(self):
         return len(self.data)
 
-    def configure(self, request):
-        # Save ordering preference
-        if request.user.is_authenticated:
-            table_name = self.__class__.__name__
-            if self.prefixed_order_by_field in request.GET:
-                # If an ordering has been specified as a query parameter, save it as the
-                # user's preferred ordering for this table.
-                ordering = request.GET.getlist(self.prefixed_order_by_field)
-                request.user.config.set(
-                    f"tables.{table_name}.ordering", ordering, commit=True
-                )
-            elif ordering := request.user.config.get(f"tables.{table_name}.ordering"):
-                # If no ordering has been specified,
-                # set the preferred ordering (if any).
-                self.order_by = ordering
-
 
 class SubnetTable(GenericTable):
     id = tables.Column(verbose_name="ID")
     subnet = tables.Column(
-        linkify=lambda record, table: reverse(table.leases_view, args=[table.server_pk])
-        + f"?by=subnet&q={record['subnet']}"
-        if record.get("id")
-        else None,
+        linkify=lambda record, table: (
+            (
+                reverse(
+                    f"plugins:netbox_kea:server_leases{record['dhcp_version']}",
+                    args=[record["server_pk"]],
+                )
+                + "?"
+                + urlencode({"by": "subnet", "q": record["subnet"]})
+            )
+            if record.get("subnet")
+            else None
+        ),
     )
     shared_network = tables.Column(verbose_name="Shared Network")
-    actions = ActionsColumn(SUBNET_ACTIONS)
+    actions = columns.ActionsColumn(actions=tuple(), extra_buttons=SUBNET_ACTIONS)
 
-    class Meta(GenericTable.Meta):
+    class Meta(NetBoxTable.Meta):
         empty_text = "No subnets"
         fields = ("id", "subnet", "shared_network", "actions")
         default_columns = ("id", "subnet", "shared_network")
 
-    def __init__(self, leases_view: str, server_pk: int, *args, **kwargs):
-        self.leases_view = leases_view
-        self.server_pk = server_pk
-        super().__init__(*args, **kwargs)
-
 
 class BaseLeaseTable(GenericTable):
     # This column is for the select checkboxes.
     pk = ToggleColumn(verbose_name="IP Address", accessor="ip_address", visible=True)
     ip_address = tables.Column(verbose_name="IP Address")
     hostname = tables.Column(verbose_name="Hostname")
     subnet_id = tables.Column(verbose_name="Subnet ID")
     hw_address = MonospaceColumn(verbose_name="Hardware Address")
     valid_lft = DurationColumn(verbose_name="Valid Lifetime")
-    cltt = tables.DateTimeColumn(verbose_name="Client Last Transaction Time")
-    expires_at = tables.DateTimeColumn(verbose_name="Expires At")
+    cltt = columns.DateTimeColumn(verbose_name="Client Last Transaction Time")
+    expires_at = columns.DateTimeColumn(verbose_name="Expires At")
     expires_in = DurationColumn(verbose_name="Expires In")
-    state = tables.Column()
     actions = ActionsColumn(LEASE_ACTIONS)
 
     class Meta(GenericTable.Meta):
         empty_text = "No leases found."
         fields = (
             "ip_address",
             "hostname",
@@ -214,7 +198,16 @@
     type = tables.Column(verbose_name="Type", accessor="type")
     preferred_lft = DurationColumn(verbose_name="Preferred Lifetime")
     duid = MonospaceColumn(verbose_name="DUID")
     iaid = MonospaceColumn(verbose_name="IAID")
 
     class Meta(BaseLeaseTable.Meta):
         fields = ("type", "duid", "iaid", *BaseLeaseTable.Meta.fields)
+
+
+class LeaseDeleteTable(GenericTable):
+    ip_address = tables.Column(verbose_name="IP Address", accessor="ip")
+
+    class Meta(NetBoxTable.Meta):
+        empty_text = "No leases"
+        fields = ("ip_address",)
+        default_columns = ("ip_address",)
```

### Comparing `netbox_kea-0.2.0/netbox_kea/templates/netbox_kea/server.html` & `netbox_kea-1.0.0/netbox_kea/templates/netbox_kea/server.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 {% extends "generic/object.html" %}
 
-{% load render_table from django_tables2 %}
-
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Server</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
-{% extends "generic/object.html" %} {% load render_table from django_tables2 %}
-{% block content %}
+{% extends "generic/object.html" %} {% block content %}
 **** SSeerrvveerr ****
 NNaammee       {{ object.name }}
 SSeerrvveerr UURRLL {{ object.server_url }}
 DDHHCCPPvv66     {% checkmark object.dhcp6 %}
 DDHHCCPPvv44     {% checkmark object.dhcp4 %}
 {% include "inc/panels/tags.html" %}
 {% endblock content %}
```

### Comparing `netbox_kea-0.2.0/netbox_kea/templates/netbox_kea/server_dhcp_leases_htmx.html` & `netbox_kea-1.0.0/netbox_kea/templates/netbox_kea/server_dhcp_leases_htmx.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,285 +1,203 @@
 00000000: 7b25 206c 6f61 6420 666f 726d 5f68 656c  {% load form_hel
 00000010: 7065 7273 2025 7d0a 7b25 206c 6f61 6420  pers %}.{% load 
 00000020: 6865 6c70 6572 7320 257d 0a7b 2520 6c6f  helpers %}.{% lo
 00000030: 6164 2072 656e 6465 725f 7461 626c 6520  ad render_table 
 00000040: 6672 6f6d 2064 6a61 6e67 6f5f 7461 626c  from django_tabl
 00000050: 6573 3220 257d 0a0a 3c64 6976 2069 643d  es2 %}..<div id=
-00000060: 226c 6561 7365 2d73 6561 7263 6822 3e0a  "lease-search">.
-00000070: 2020 3c64 6976 2063 6c61 7373 3d22 726f    <div class="ro
-00000080: 7720 7078 2d33 223e 0a20 2020 203c 6469  w px-3">.    <di
-00000090: 7620 636c 6173 733d 2263 6f6c 2063 6f6c  v class="col col
-000000a0: 2d36 206f 6666 7365 742d 3320 7079 2d33  -6 offset-3 py-3
-000000b0: 223e 0a20 2020 2020 203c 666f 726d 0a20  ">.      <form. 
-000000c0: 2020 2020 2020 2063 6c61 7373 3d22 666f         class="fo
-000000d0: 726d 2066 6f72 6d2d 686f 7269 7a6f 6e74  rm form-horizont
-000000e0: 616c 220a 2020 2020 2020 2020 6878 2d67  al".        hx-g
-000000f0: 6574 3d22 2e22 0a20 2020 2020 2020 2068  et=".".        h
-00000100: 782d 7461 7267 6574 3d22 236c 6561 7365  x-target="#lease
-00000110: 2d73 6561 7263 6822 0a20 2020 2020 2020  -search".       
-00000120: 2068 782d 696e 6469 6361 746f 723d 2223   hx-indicator="#
-00000130: 7365 6172 6368 2d69 6e64 6963 6174 6f72  search-indicator
-00000140: 220a 2020 2020 2020 2020 6878 2d70 7573  ".        hx-pus
-00000150: 682d 7572 6c3d 2274 7275 6522 0a20 2020  h-url="true".   
-00000160: 2020 2020 207b 2520 6966 2066 6f72 6d2e       {% if form.
-00000170: 6973 5f62 6f75 6e64 2061 6e64 2069 735f  is_bound and is_
-00000180: 656d 6265 6464 6564 2061 6e64 2066 6f72  embedded and for
-00000190: 6d2e 6973 5f76 616c 6964 2025 7d68 782d  m.is_valid %}hx-
-000001a0: 7472 6967 6765 723d 226c 6f61 6422 7b25  trigger="load"{%
-000001b0: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-000001c0: 3e0a 2020 2020 2020 2020 7b25 2069 6620  >.        {% if 
-000001d0: 666f 726d 2e63 6c65 616e 6564 5f64 6174  form.cleaned_dat
-000001e0: 612e 7061 6765 2025 7d0a 2020 2020 2020  a.page %}.      
-000001f0: 2020 2020 7b23 204f 6e6c 7920 696e 636c      {# Only incl
-00000200: 7564 6520 6f6e 2066 756c 6c20 7061 6765  ude on full page
-00000210: 206c 6f61 6420 736f 2074 6861 7420 7468   load so that th
-00000220: 6520 7573 6572 206c 616e 6473 206f 6e20  e user lands on 
-00000230: 7468 6520 636f 7272 6563 7420 7061 6765  the correct page
-00000240: 2e20 237d 0a20 2020 2020 2020 2020 203c  . #}.          <
-00000250: 696e 7075 7420 7479 7065 3d22 6869 6464  input type="hidd
-00000260: 656e 2220 6964 3d22 6964 5f70 6167 6522  en" id="id_page"
-00000270: 206e 616d 653d 2270 6167 6522 2076 616c   name="page" val
-00000280: 7565 3d22 7b7b 2066 6f72 6d2e 636c 6561  ue="{{ form.clea
-00000290: 6e65 645f 6461 7461 2e70 6167 6520 7d7d  ned_data.page }}
-000002a0: 223e 0a20 2020 2020 2020 207b 2520 656e  ">.        {% en
-000002b0: 6469 6620 257d 0a20 2020 2020 2020 207b  dif %}.        {
-000002c0: 2520 666f 7220 6520 696e 2066 6f72 6d2e  % for e in form.
-000002d0: 6572 726f 7273 2e70 6167 6520 257d 0a20  errors.page %}. 
-000002e0: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
-000002f0: 6173 733d 2261 6c65 7274 2061 6c65 7274  ass="alert alert
-00000300: 2d64 616e 6765 7222 2072 6f6c 653d 2261  -danger" role="a
-00000310: 6c65 7274 223e 7b7b 2065 207d 7d3c 2f64  lert">{{ e }}</d
-00000320: 6976 3e0a 2020 2020 2020 2020 7b25 2065  iv>.        {% e
-00000330: 6e64 666f 7220 257d 0a20 2020 2020 2020  ndfor %}.       
-00000340: 207b 2520 7265 6e64 6572 5f66 6f72 6d20   {% render_form 
-00000350: 666f 726d 2025 7d0a 2020 2020 2020 2020  form %}.        
-00000360: 3c64 6976 2063 6c61 7373 3d22 7465 7874  <div class="text
-00000370: 2d65 6e64 223e 0a20 2020 2020 2020 2020  -end">.         
-00000380: 203c 6469 7620 6964 3d22 7365 6172 6368   <div id="search
-00000390: 2d69 6e64 6963 6174 6f72 2220 636c 6173  -indicator" clas
-000003a0: 733d 2273 7069 6e6e 6572 2d62 6f72 6465  s="spinner-borde
-000003b0: 7220 642d 696e 6c69 6e65 2d62 6c6f 636b  r d-inline-block
-000003c0: 2061 6c69 676e 2d6d 6964 646c 6520 6874   align-middle ht
-000003d0: 6d78 2d69 6e64 6963 6174 6f72 206d 652d  mx-indicator me-
-000003e0: 3222 2072 6f6c 653d 2273 7461 7475 7322  2" role="status"
-000003f0: 3e0a 2020 2020 2020 2020 2020 2020 3c73  >.            <s
-00000400: 7061 6e20 636c 6173 733d 2276 6973 7561  pan class="visua
-00000410: 6c6c 792d 6869 6464 656e 223e 4c6f 6164  lly-hidden">Load
-00000420: 696e 672e 2e2e 3c2f 7370 616e 3e0a 2020  ing...</span>.  
-00000430: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00000440: 2020 2020 2020 2020 203c 6275 7474 6f6e           <button
-00000450: 2074 7970 653d 2273 7562 6d69 7422 2063   type="submit" c
-00000460: 6c61 7373 3d22 6274 6e20 6274 6e2d 7072  lass="btn btn-pr
-00000470: 696d 6172 7922 3e0a 2020 2020 2020 2020  imary">.        
-00000480: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
-00000490: 226d 6469 206d 6469 2d6d 6167 6e69 6679  "mdi mdi-magnify
-000004a0: 2220 6172 6961 2d68 6964 6465 6e3d 2274  " aria-hidden="t
-000004b0: 7275 6522 3e3c 2f73 7061 6e3e 2053 6561  rue"></span> Sea
-000004c0: 7263 680a 2020 2020 2020 2020 2020 3c2f  rch.          </
-000004d0: 6275 7474 6f6e 3e0a 2020 2020 2020 2020  button>.        
-000004e0: 3c2f 6469 763e 0a20 2020 2020 203c 2f66  </div>.      </f
-000004f0: 6f72 6d3e 0a20 2020 203c 2f64 6976 3e0a  orm>.    </div>.
-00000500: 2020 3c2f 6469 763e 0a0a 2020 7b25 2069    </div>..  {% i
-00000510: 6620 6e6f 7420 6973 5f65 6d62 6564 6465  f not is_embedde
-00000520: 6420 616e 6420 666f 726d 2e69 735f 7661  d and form.is_va
-00000530: 6c69 6420 257d 0a20 2020 207b 2520 696e  lid %}.    {% in
-00000540: 636c 7564 6520 226e 6574 626f 785f 6b65  clude "netbox_ke
-00000550: 612f 696e 632f 636f 6e66 6967 7572 655f  a/inc/configure_
-00000560: 7461 626c 652e 6874 6d6c 2220 7769 7468  table.html" with
-00000570: 2074 6162 6c65 5f6d 6f64 616c 3d22 4f62   table_modal="Ob
-00000580: 6a65 6374 5461 626c 655f 636f 6e66 6967  jectTable_config
-00000590: 2220 257d 0a20 2020 203c 666f 726d 206d  " %}.    <form m
-000005a0: 6574 686f 643d 2270 6f73 7422 2061 6374  ethod="post" act
-000005b0: 696f 6e3d 227b 7b20 6465 6c65 7465 5f61  ion="{{ delete_a
-000005c0: 6374 696f 6e20 7d7d 223e 0a20 2020 2020  ction }}">.     
-000005d0: 207b 2520 6373 7266 5f74 6f6b 656e 2025   {% csrf_token %
-000005e0: 7d0a 2020 2020 2020 3c69 6e70 7574 2074  }.      <input t
-000005f0: 7970 653d 2268 6964 6465 6e22 206e 616d  ype="hidden" nam
-00000600: 653d 2272 6574 7572 6e5f 7572 6c22 2076  e="return_url" v
-00000610: 616c 7565 3d22 7b7b 2072 6571 7565 7374  alue="{{ request
-00000620: 2e70 6174 6820 7d7d 3f7b 7b20 7265 7175  .path }}?{{ requ
-00000630: 6573 742e 4745 542e 7572 6c65 6e63 6f64  est.GET.urlencod
-00000640: 6520 7d7d 2220 2f3e 0a20 2020 2020 203c  e }}" />.      <
-00000650: 6469 7620 636c 6173 733d 2263 6172 6422  div class="card"
-00000660: 3e0a 2020 2020 2020 2020 3c64 6976 2063  >.        <div c
-00000670: 6c61 7373 3d22 6361 7264 2d62 6f64 7922  lass="card-body"
-00000680: 3e0a 2020 2020 2020 2020 2020 2020 7b25  >.            {%
-00000690: 2072 656e 6465 725f 7461 626c 6520 7461   render_table ta
-000006a0: 626c 6520 257d 0a20 2020 2020 2020 2020  ble %}.         
-000006b0: 203c 6469 7620 636c 6173 733d 2272 6f77   <div class="row
-000006c0: 223e 0a20 2020 2020 2020 2020 2020 203c  ">.            <
-000006d0: 6469 7620 636c 6173 733d 2263 6f6c 2063  div class="col c
-000006e0: 6f6c 2d6d 642d 3620 6d62 2d30 223e 0a20  ol-md-6 mb-0">. 
-000006f0: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00000700: 6966 2070 6167 696e 6174 6520 257d 0a20  if paginate %}. 
-00000710: 2020 2020 2020 2020 2020 2020 2020 203c                 <
-00000720: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
-00000730: 2020 2020 636c 6173 733d 2262 746e 2062      class="btn b
-00000740: 746e 2d73 6d20 6274 6e2d 6f75 746c 696e  tn-sm btn-outlin
-00000750: 652d 7365 636f 6e64 6172 797b 2520 6966  e-secondary{% if
-00000760: 206e 6f74 206e 6578 745f 7061 6765 2025   not next_page %
-00000770: 7d20 6469 7361 626c 6564 7b25 2065 6e64  } disabled{% end
-00000780: 6966 2025 7d22 0a20 2020 2020 2020 2020  if %}".         
-00000790: 2020 2020 2020 2020 2072 6f6c 653d 2262           role="b
-000007a0: 7574 746f 6e22 0a20 2020 2020 2020 2020  utton".         
-000007b0: 2020 2020 2020 2020 207b 2520 6966 206e           {% if n
-000007c0: 6578 745f 7061 6765 2025 7d0a 2020 2020  ext_page %}.    
-000007d0: 2020 2020 2020 2020 2020 2020 2020 6878                hx
-000007e0: 2d67 6574 3d22 7b25 2071 7565 7279 7374  -get="{% queryst
-000007f0: 7269 6e67 2072 6571 7565 7374 2070 6167  ring request pag
-00000800: 653d 6e65 7874 5f70 6167 6520 257d 220a  e=next_page %}".
-00000810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000820: 2020 6878 2d74 6172 6765 743d 2223 6c65    hx-target="#le
-00000830: 6173 652d 7365 6172 6368 220a 2020 2020  ase-search".    
-00000840: 2020 2020 2020 2020 2020 2020 2020 6878                hx
-00000850: 2d69 6e64 6963 6174 6f72 3d22 236e 6578  -indicator="#nex
-00000860: 742d 696e 6469 6361 746f 7222 0a20 2020  t-indicator".   
-00000870: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-00000880: 782d 7075 7368 2d75 726c 3d22 7472 7565  x-push-url="true
-00000890: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-000008a0: 2020 2020 7b25 2065 6c73 6520 257d 0a20      {% else %}. 
-000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008c0: 2061 7269 612d 6469 7361 626c 6564 3d22   aria-disabled="
-000008d0: 7472 7565 220a 2020 2020 2020 2020 2020  true".          
-000008e0: 2020 2020 2020 2020 7b25 2065 6e64 6966          {% endif
-000008f0: 2025 7d0a 2020 2020 2020 2020 2020 2020   %}.            
-00000900: 2020 2020 3e4e 6578 743c 2f61 3e0a 2020      >Next</a>.  
-00000910: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-00000920: 6976 2069 643d 226e 6578 742d 696e 6469  iv id="next-indi
-00000930: 6361 746f 7222 2063 6c61 7373 3d22 7370  cator" class="sp
-00000940: 696e 6e65 722d 626f 7264 6572 2073 7069  inner-border spi
-00000950: 6e6e 6572 2d62 6f72 6465 722d 736d 2064  nner-border-sm d
-00000960: 2d69 6e6c 696e 652d 626c 6f63 6b20 616c  -inline-block al
-00000970: 6967 6e2d 6d69 6464 6c65 2068 746d 782d  ign-middle htmx-
-00000980: 696e 6469 6361 746f 7222 2072 6f6c 653d  indicator" role=
-00000990: 2273 7461 7475 7322 3e0a 2020 2020 2020  "status">.      
-000009a0: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
-000009b0: 6e20 636c 6173 733d 2276 6973 7561 6c6c  n class="visuall
-000009c0: 792d 6869 6464 656e 223e 4c6f 6164 696e  y-hidden">Loadin
-000009d0: 672e 2e2e 3c2f 7370 616e 3e0a 2020 2020  g...</span>.    
-000009e0: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-000009f0: 763e 0a20 2020 2020 2020 2020 2020 2020  v>.             
-00000a00: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
-00000a10: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00000a20: 2020 2020 2020 2020 2020 2020 3c64 6976              <div
-00000a30: 2063 6c61 7373 3d22 636f 6c20 636f 6c2d   class="col col-
-00000a40: 6d64 2d36 206d 622d 3020 7465 7874 2d65  md-6 mb-0 text-e
-00000a50: 6e64 223e 0a20 2020 2020 2020 2020 2020  nd">.           
-00000a60: 2020 207b 2520 6966 2070 6167 696e 6174     {% if paginat
-00000a70: 6520 257d 0a20 2020 2020 2020 2020 2020  e %}.           
-00000a80: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-00000a90: 2264 726f 7064 6f77 6e20 6472 6f70 7570  "dropdown dropup
-00000aa0: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00000ab0: 2020 2020 203c 6275 7474 6f6e 2063 6c61       <button cla
-00000ac0: 7373 3d22 6274 6e20 6274 6e2d 736d 2062  ss="btn btn-sm b
-00000ad0: 746e 2d6f 7574 6c69 6e65 2d73 6563 6f6e  tn-outline-secon
-00000ae0: 6461 7279 2064 726f 7064 6f77 6e2d 746f  dary dropdown-to
-00000af0: 6767 6c65 2220 7479 7065 3d22 6275 7474  ggle" type="butt
-00000b00: 6f6e 2220 6461 7461 2d62 732d 746f 6767  on" data-bs-togg
-00000b10: 6c65 3d22 6472 6f70 646f 776e 223e 0a20  le="dropdown">. 
-00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b30: 2050 6572 2050 6167 650a 2020 2020 2020   Per Page.      
-00000b40: 2020 2020 2020 2020 2020 2020 3c2f 6275              </bu
-00000b50: 7474 6f6e 3e0a 2020 2020 2020 2020 2020  tton>.          
-00000b60: 2020 2020 2020 2020 3c75 6c20 636c 6173          <ul clas
-00000b70: 733d 2264 726f 7064 6f77 6e2d 6d65 6e75  s="dropdown-menu
-00000b80: 223e 0a20 2020 2020 2020 2020 2020 2020  ">.             
-00000b90: 2020 2020 2020 207b 2520 666f 7220 6e20         {% for n 
-00000ba0: 696e 2070 6167 655f 6c65 6e67 7468 7320  in page_lengths 
-00000bb0: 257d 0a20 2020 2020 2020 2020 2020 2020  %}.             
-00000bc0: 2020 2020 2020 2020 203c 6c69 3e0a 2020           <li>.  
-00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000be0: 2020 2020 2020 3c61 2068 7265 663d 2223        <a href="#
-00000bf0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00000c00: 2020 2020 2020 2020 2020 2020 2068 782d               hx-
-00000c10: 6765 743d 227b 2520 7175 6572 7973 7472  get="{% querystr
-00000c20: 696e 6720 7265 7175 6573 7420 7065 725f  ing request per_
-00000c30: 7061 6765 3d6e 2025 7d22 0a20 2020 2020  page=n %}".     
-00000c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c50: 2020 2020 2020 6878 2d74 6172 6765 743d        hx-target=
-00000c60: 2223 6c65 6173 652d 7365 6172 6368 220a  "#lease-search".
-00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c80: 2020 2020 2020 2020 2020 2068 782d 7075             hx-pu
-00000c90: 7368 2d75 726c 3d22 7472 7565 220a 2020  sh-url="true".  
-00000ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cb0: 2020 2020 2020 2020 2063 6c61 7373 3d22           class="
-00000cc0: 6472 6f70 646f 776e 2d69 7465 6d22 0a20  dropdown-item". 
-00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ce0: 2020 2020 2020 203e 7b7b 206e 207d 7d3c         >{{ n }}<
-00000cf0: 2f61 3e0a 2020 2020 2020 2020 2020 2020  /a>.            
-00000d00: 2020 2020 2020 2020 2020 3c2f 6c69 3e0a            </li>.
-00000d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d20: 2020 2020 7b25 2065 6e64 666f 7220 257d      {% endfor %}
-00000d30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000d40: 2020 203c 2f75 6c3e 0a20 2020 2020 2020     </ul>.       
-00000d50: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00000d60: 2020 2020 2020 2020 2020 2020 2020 7b25                {%
-00000d70: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
-00000d80: 2020 2020 2020 2020 3c73 6d61 6c6c 2063          <small c
-00000d90: 6c61 7373 3d22 7465 7874 2d65 6e64 2074  lass="text-end t
-00000da0: 6578 742d 6d75 7465 6422 3e53 686f 7769  ext-muted">Showi
-00000db0: 6e67 207b 7b20 7461 626c 652e 726f 7773  ng {{ table.rows
-00000dc0: 7c6c 656e 6774 6820 7d7d 206c 6561 7365  |length }} lease
-00000dd0: 2873 293c 2f73 6d61 6c6c 3e0a 2020 2020  (s)</small>.    
-00000de0: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00000df0: 2020 2020 2020 2020 203c 2f64 6976 3e0a           </div>.
-00000e00: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
-00000e10: 2020 2020 203c 2f64 6976 3e0a 2020 2020       </div>.    
-00000e20: 2020 3c64 6976 2063 6c61 7373 3d22 6e6f    <div class="no
-00000e30: 7072 696e 7420 6275 6c6b 2d62 7574 746f  print bulk-butto
-00000e40: 6e73 223e 0a20 2020 2020 2020 203c 6469  ns">.        <di
-00000e50: 7620 636c 6173 733d 2262 756c 6b2d 6275  v class="bulk-bu
-00000e60: 7474 6f6e 2d67 726f 7570 223e 0a20 2020  tton-group">.   
-00000e70: 2020 2020 2020 203c 6275 7474 6f6e 2074         <button t
-00000e80: 7970 653d 2273 7562 6d69 7422 2063 6c61  ype="submit" cla
-00000e90: 7373 3d22 6274 6e20 6274 6e2d 736d 2062  ss="btn btn-sm b
-00000ea0: 746e 2d64 616e 6765 7222 3e3c 6920 636c  tn-danger"><i cl
-00000eb0: 6173 733d 226d 6469 206d 6469 2d74 7261  ass="mdi mdi-tra
-00000ec0: 7368 2d63 616e 2d6f 7574 6c69 6e65 2220  sh-can-outline" 
-00000ed0: 6172 6961 2d68 6964 6465 6e3d 2274 7275  aria-hidden="tru
-00000ee0: 6522 3e3c 2f69 3e20 4465 6c65 7465 2053  e"></i> Delete S
-00000ef0: 656c 6563 7465 640a 2020 2020 2020 2020  elected.        
-00000f00: 2020 3c2f 6275 7474 6f6e 3e0a 2020 2020    </button>.    
-00000f10: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-00000f20: 2020 203c 6469 7620 636c 6173 733d 2262     <div class="b
-00000f30: 756c 6b2d 6275 7474 6f6e 2d67 726f 7570  ulk-button-group
-00000f40: 223e 0a20 2020 2020 2020 2020 203c 6469  ">.          <di
-00000f50: 7620 636c 6173 733d 2264 726f 7064 6f77  v class="dropdow
-00000f60: 6e22 3e0a 2020 2020 2020 2020 2020 2020  n">.            
-00000f70: 3c62 7574 746f 6e20 7479 7065 3d22 6275  <button type="bu
-00000f80: 7474 6f6e 2220 636c 6173 733d 2262 746e  tton" class="btn
-00000f90: 2062 746e 2d73 6d20 6274 6e2d 7075 7270   btn-sm btn-purp
-00000fa0: 6c65 2064 726f 7064 6f77 6e2d 746f 6767  le dropdown-togg
-00000fb0: 6c65 2220 6461 7461 2d62 732d 746f 6767  le" data-bs-togg
-00000fc0: 6c65 3d22 6472 6f70 646f 776e 2220 6172  le="dropdown" ar
-00000fd0: 6961 2d68 6173 706f 7075 703d 2274 7275  ia-haspopup="tru
-00000fe0: 6522 2061 7269 612d 6578 7061 6e64 6564  e" aria-expanded
-00000ff0: 3d22 6661 6c73 6522 3e0a 2020 2020 2020  ="false">.      
-00001000: 2020 2020 2020 2020 3c69 2063 6c61 7373          <i class
-00001010: 3d22 6d64 6920 6d64 692d 646f 776e 6c6f  ="mdi mdi-downlo
-00001020: 6164 223e 3c2f 693e 266e 6273 703b 4578  ad"></i>&nbsp;Ex
-00001030: 706f 7274 0a20 2020 2020 2020 2020 2020  port.           
-00001040: 203c 2f62 7574 746f 6e3e 0a20 2020 2020   </button>.     
-00001050: 2020 2020 2020 203c 756c 2063 6c61 7373         <ul class
-00001060: 3d22 6472 6f70 646f 776e 2d6d 656e 7520  ="dropdown-menu 
-00001070: 6472 6f70 646f 776e 2d6d 656e 752d 656e  dropdown-menu-en
-00001080: 6422 3e0a 2020 2020 2020 2020 2020 2020  d">.            
-00001090: 2020 3c6c 693e 3c61 2063 6c61 7373 3d22    <li><a class="
-000010a0: 6472 6f70 646f 776e 2d69 7465 6d22 2068  dropdown-item" h
-000010b0: 7265 663d 227b 2520 7175 6572 7973 7472  ref="{% querystr
-000010c0: 696e 6720 7265 7175 6573 7420 6578 706f  ing request expo
-000010d0: 7274 3d22 7461 626c 6522 2025 7d22 3e43  rt="table" %}">C
-000010e0: 7572 7265 6e74 2056 6965 773c 2f61 3e3c  urrent View</a><
-000010f0: 2f6c 693e 0a20 2020 2020 2020 2020 2020  /li>.           
-00001100: 2020 203c 6c69 3e3c 6120 636c 6173 733d     <li><a class=
-00001110: 2264 726f 7064 6f77 6e2d 6974 656d 2220  "dropdown-item" 
-00001120: 6872 6566 3d22 7b25 2071 7565 7279 7374  href="{% queryst
-00001130: 7269 6e67 2072 6571 7565 7374 2065 7870  ring request exp
-00001140: 6f72 743d 2222 2025 7d22 3e41 6c6c 2044  ort="" %}">All D
-00001150: 6174 6120 2843 5356 293c 2f61 3e3c 2f6c  ata (CSV)</a></l
-00001160: 693e 0a20 2020 2020 2020 2020 2020 203c  i>.            <
-00001170: 2f75 6c3e 0a20 2020 2020 2020 2020 203c  /ul>.          <
-00001180: 2f64 6976 3e0a 2020 2020 2020 2020 3c2f  /div>.        </
-00001190: 6469 763e 0a20 2020 2020 203c 2f64 6976  div>.      </div
-000011a0: 3e0a 2020 2020 3c2f 666f 726d 3e0a 2020  >.    </form>.  
-000011b0: 7b25 2065 6e64 6966 2025 7d0a 3c2f 6469  {% endif %}.</di
-000011c0: 763e 0a                                  v>.
+00000060: 226c 6561 7365 2d73 6561 7263 6822 2068  "lease-search" h
+00000070: 782d 7461 7267 6574 3d22 236c 6561 7365  x-target="#lease
+00000080: 2d73 6561 7263 6822 2068 782d 7377 6170  -search" hx-swap
+00000090: 3d22 6f75 7465 7248 544d 4c22 2068 782d  ="outerHTML" hx-
+000000a0: 7075 7368 2d75 726c 3d22 7472 7565 223e  push-url="true">
+000000b0: 0a20 203c 6469 7620 636c 6173 733d 2272  .  <div class="r
+000000c0: 6f77 2070 782d 3322 3e0a 2020 2020 3c64  ow px-3">.    <d
+000000d0: 6976 2063 6c61 7373 3d22 636f 6c20 636f  iv class="col co
+000000e0: 6c2d 3620 6f66 6673 6574 2d33 2070 792d  l-6 offset-3 py-
+000000f0: 3322 3e0a 2020 2020 2020 3c66 6f72 6d0a  3">.      <form.
+00000100: 2020 2020 2020 2020 636c 6173 733d 2266          class="f
+00000110: 6f72 6d20 666f 726d 2d68 6f72 697a 6f6e  orm form-horizon
+00000120: 7461 6c22 0a20 2020 2020 2020 2068 782d  tal".        hx-
+00000130: 6765 743d 222e 220a 2020 2020 2020 2020  get=".".        
+00000140: 6878 2d69 6e64 6963 6174 6f72 3d22 2373  hx-indicator="#s
+00000150: 6561 7263 682d 696e 6469 6361 746f 7222  earch-indicator"
+00000160: 0a20 2020 2020 2020 2068 782d 6469 7361  .        hx-disa
+00000170: 626c 6564 2d65 6c74 3d22 236c 6561 7365  bled-elt="#lease
+00000180: 2d73 6561 7263 682d 6274 6e22 0a20 2020  -search-btn".   
+00000190: 2020 2020 207b 2520 6966 2066 6f72 6d2e       {% if form.
+000001a0: 6973 5f62 6f75 6e64 2061 6e64 2069 735f  is_bound and is_
+000001b0: 656d 6265 6464 6564 2061 6e64 2066 6f72  embedded and for
+000001c0: 6d2e 6973 5f76 616c 6964 2025 7d68 782d  m.is_valid %}hx-
+000001d0: 7472 6967 6765 723d 226c 6f61 6422 7b25  trigger="load"{%
+000001e0: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
+000001f0: 3e0a 2020 2020 2020 2020 7b25 2069 6620  >.        {% if 
+00000200: 666f 726d 2e63 6c65 616e 6564 5f64 6174  form.cleaned_dat
+00000210: 612e 7061 6765 2025 7d0a 2020 2020 2020  a.page %}.      
+00000220: 2020 2020 7b23 204f 6e6c 7920 696e 636c      {# Only incl
+00000230: 7564 6520 6f6e 2066 756c 6c20 7061 6765  ude on full page
+00000240: 206c 6f61 6420 736f 2074 6861 7420 7468   load so that th
+00000250: 6520 7573 6572 206c 616e 6473 206f 6e20  e user lands on 
+00000260: 7468 6520 636f 7272 6563 7420 7061 6765  the correct page
+00000270: 2e20 237d 0a20 2020 2020 2020 2020 203c  . #}.          <
+00000280: 696e 7075 7420 7479 7065 3d22 6869 6464  input type="hidd
+00000290: 656e 2220 6964 3d22 6964 5f70 6167 6522  en" id="id_page"
+000002a0: 206e 616d 653d 2270 6167 6522 2076 616c   name="page" val
+000002b0: 7565 3d22 7b7b 2066 6f72 6d2e 636c 6561  ue="{{ form.clea
+000002c0: 6e65 645f 6461 7461 2e70 6167 6520 7d7d  ned_data.page }}
+000002d0: 223e 0a20 2020 2020 2020 207b 2520 656e  ">.        {% en
+000002e0: 6469 6620 257d 0a20 2020 2020 2020 207b  dif %}.        {
+000002f0: 2520 666f 7220 6520 696e 2066 6f72 6d2e  % for e in form.
+00000300: 6572 726f 7273 2e70 6167 6520 257d 0a20  errors.page %}. 
+00000310: 2020 2020 2020 2020 203c 6469 7620 636c           <div cl
+00000320: 6173 733d 2261 6c65 7274 2061 6c65 7274  ass="alert alert
+00000330: 2d64 616e 6765 7222 2072 6f6c 653d 2261  -danger" role="a
+00000340: 6c65 7274 223e 7b7b 2065 207d 7d3c 2f64  lert">{{ e }}</d
+00000350: 6976 3e0a 2020 2020 2020 2020 7b25 2065  iv>.        {% e
+00000360: 6e64 666f 7220 257d 0a20 2020 2020 2020  ndfor %}.       
+00000370: 207b 2520 7265 6e64 6572 5f66 6f72 6d20   {% render_form 
+00000380: 666f 726d 2025 7d0a 2020 2020 2020 2020  form %}.        
+00000390: 3c64 6976 2063 6c61 7373 3d22 7465 7874  <div class="text
+000003a0: 2d65 6e64 223e 0a20 2020 2020 2020 2020  -end">.         
+000003b0: 203c 6469 7620 6964 3d22 7365 6172 6368   <div id="search
+000003c0: 2d69 6e64 6963 6174 6f72 2220 636c 6173  -indicator" clas
+000003d0: 733d 2273 7069 6e6e 6572 2d62 6f72 6465  s="spinner-borde
+000003e0: 7220 642d 696e 6c69 6e65 2d62 6c6f 636b  r d-inline-block
+000003f0: 2061 6c69 676e 2d6d 6964 646c 6520 6874   align-middle ht
+00000400: 6d78 2d69 6e64 6963 6174 6f72 206d 652d  mx-indicator me-
+00000410: 3222 2072 6f6c 653d 2273 7461 7475 7322  2" role="status"
+00000420: 3e0a 2020 2020 2020 2020 2020 2020 3c73  >.            <s
+00000430: 7061 6e20 636c 6173 733d 2276 6973 7561  pan class="visua
+00000440: 6c6c 792d 6869 6464 656e 223e 4c6f 6164  lly-hidden">Load
+00000450: 696e 672e 2e2e 3c2f 7370 616e 3e0a 2020  ing...</span>.  
+00000460: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00000470: 2020 2020 2020 2020 203c 6275 7474 6f6e           <button
+00000480: 2069 643d 226c 6561 7365 2d73 6561 7263   id="lease-searc
+00000490: 682d 6274 6e22 2074 7970 653d 2273 7562  h-btn" type="sub
+000004a0: 6d69 7422 2063 6c61 7373 3d22 6274 6e20  mit" class="btn 
+000004b0: 6274 6e2d 7072 696d 6172 7922 3e0a 2020  btn-primary">.  
+000004c0: 2020 2020 2020 2020 2020 3c73 7061 6e20            <span 
+000004d0: 636c 6173 733d 226d 6469 206d 6469 2d6d  class="mdi mdi-m
+000004e0: 6167 6e69 6679 2220 6172 6961 2d68 6964  agnify" aria-hid
+000004f0: 6465 6e3d 2274 7275 6522 3e3c 2f73 7061  den="true"></spa
+00000500: 6e3e 2053 6561 7263 680a 2020 2020 2020  n> Search.      
+00000510: 2020 2020 3c2f 6275 7474 6f6e 3e0a 2020      </button>.  
+00000520: 2020 2020 2020 3c2f 6469 763e 0a20 2020        </div>.   
+00000530: 2020 203c 2f66 6f72 6d3e 0a20 2020 203c     </form>.    <
+00000540: 2f64 6976 3e0a 2020 3c2f 6469 763e 0a0a  /div>.  </div>..
+00000550: 2020 7b25 2069 6620 6e6f 7420 6973 5f65    {% if not is_e
+00000560: 6d62 6564 6465 6420 616e 6420 666f 726d  mbedded and form
+00000570: 2e69 735f 7661 6c69 6420 257d 0a20 2020  .is_valid %}.   
+00000580: 207b 2520 696e 636c 7564 6520 2269 6e63   {% include "inc
+00000590: 2f74 6162 6c65 5f63 6f6e 7472 6f6c 735f  /table_controls_
+000005a0: 6874 6d78 2e68 746d 6c22 2077 6974 6820  htmx.html" with 
+000005b0: 7461 626c 655f 6d6f 6461 6c3d 224c 6561  table_modal="Lea
+000005c0: 7365 7354 6162 6c65 5f63 6f6e 6669 6722  sesTable_config"
+000005d0: 2025 7d0a 2020 2020 7b25 2077 6974 6820   %}.    {% with 
+000005e0: 7072 6566 6572 656e 6365 737c 6765 745f  preferences|get_
+000005f0: 6b65 793a 2270 6167 696e 6174 696f 6e2e  key:"pagination.
+00000600: 706c 6163 656d 656e 7422 2061 7320 7061  placement" as pa
+00000610: 6769 6e61 746f 725f 706c 6163 656d 656e  ginator_placemen
+00000620: 7420 257d 0a20 2020 2020 203c 666f 726d  t %}.      <form
+00000630: 206d 6574 686f 643d 2270 6f73 7422 2061   method="post" a
+00000640: 6374 696f 6e3d 227b 7b20 6465 6c65 7465  ction="{{ delete
+00000650: 5f61 6374 696f 6e20 7d7d 223e 0a20 2020  _action }}">.   
+00000660: 2020 2020 207b 2520 6373 7266 5f74 6f6b       {% csrf_tok
+00000670: 656e 2025 7d0a 2020 2020 2020 2020 3c69  en %}.        <i
+00000680: 6e70 7574 2074 7970 653d 2268 6964 6465  nput type="hidde
+00000690: 6e22 206e 616d 653d 2272 6574 7572 6e5f  n" name="return_
+000006a0: 7572 6c22 2076 616c 7565 3d22 7b7b 2072  url" value="{{ r
+000006b0: 6571 7565 7374 2e70 6174 6820 7d7d 3f7b  equest.path }}?{
+000006c0: 7b20 7265 7175 6573 742e 4745 542e 7572  { request.GET.ur
+000006d0: 6c65 6e63 6f64 6520 7d7d 2220 2f3e 0a20  lencode }}" />. 
+000006e0: 2020 2020 2020 203c 6469 7620 636c 6173         <div clas
+000006f0: 733d 2263 6172 6422 3e0a 2020 2020 2020  s="card">.      
+00000700: 2020 2020 7b25 2069 6620 7061 6769 6e61      {% if pagina
+00000710: 746f 725f 706c 6163 656d 656e 7420 3d3d  tor_placement ==
+00000720: 2027 746f 7027 206f 7220 7061 6769 6e61   'top' or pagina
+00000730: 746f 725f 706c 6163 656d 656e 7420 3d3d  tor_placement ==
+00000740: 2027 626f 7468 2720 257d 0a20 2020 2020   'both' %}.     
+00000750: 2020 2020 2020 207b 2520 696e 636c 7564         {% includ
+00000760: 6520 226e 6574 626f 785f 6b65 612f 696e  e "netbox_kea/in
+00000770: 632f 7365 7276 6572 5f64 6863 705f 6c65  c/server_dhcp_le
+00000780: 6173 6573 5f70 6167 696e 6174 6f72 2e68  ases_paginator.h
+00000790: 746d 6c22 2077 6974 6820 7461 626c 653d  tml" with table=
+000007a0: 7461 626c 6520 7061 6769 6e61 7465 3d70  table paginate=p
+000007b0: 6167 696e 6174 6520 706c 6163 656d 656e  aginate placemen
+000007c0: 743d 2274 6f70 2220 257d 0a20 2020 2020  t="top" %}.     
+000007d0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
+000007e0: 0a20 2020 2020 2020 2020 207b 2520 7265  .          {% re
+000007f0: 6e64 6572 5f74 6162 6c65 2074 6162 6c65  nder_table table
+00000800: 2022 696e 632f 7461 626c 655f 6874 6d78   "inc/table_htmx
+00000810: 2e68 746d 6c22 2025 7d0a 2020 2020 2020  .html" %}.      
+00000820: 2020 2020 7b25 2069 6620 7061 6769 6e61      {% if pagina
+00000830: 746f 725f 706c 6163 656d 656e 7420 213d  tor_placement !=
+00000840: 2022 746f 7022 2025 7d0a 2020 2020 2020   "top" %}.      
+00000850: 2020 2020 2020 7b25 2069 6e63 6c75 6465        {% include
+00000860: 2022 6e65 7462 6f78 5f6b 6561 2f69 6e63   "netbox_kea/inc
+00000870: 2f73 6572 7665 725f 6468 6370 5f6c 6561  /server_dhcp_lea
+00000880: 7365 735f 7061 6769 6e61 746f 722e 6874  ses_paginator.ht
+00000890: 6d6c 2220 7769 7468 2074 6162 6c65 3d74  ml" with table=t
+000008a0: 6162 6c65 2070 6167 696e 6174 653d 7061  able paginate=pa
+000008b0: 6769 6e61 7465 2070 6c61 6365 6d65 6e74  ginate placement
+000008c0: 3d22 626f 7474 6f6d 2220 257d 0a20 2020  ="bottom" %}.   
+000008d0: 2020 2020 2020 207b 2520 656e 6469 6620         {% endif 
+000008e0: 257d 0a20 2020 2020 2020 203c 2f64 6976  %}.        </div
+000008f0: 3e0a 2020 2020 2020 2020 3c64 6976 2063  >.        <div c
+00000900: 6c61 7373 3d22 642d 7072 696e 742d 6e6f  lass="d-print-no
+00000910: 6e65 2064 2d66 6c65 7820 6a75 7374 6966  ne d-flex justif
+00000920: 792d 636f 6e74 656e 742d 6265 7477 6565  y-content-betwee
+00000930: 6e20 6d74 2d32 223e 0a20 2020 2020 2020  n mt-2">.       
+00000940: 2020 203c 6469 763e 0a20 2020 2020 2020     <div>.       
+00000950: 2020 2020 207b 2520 6966 2063 616e 5f64       {% if can_d
+00000960: 656c 6574 6520 257d 0a20 2020 2020 2020  elete %}.       
+00000970: 2020 2020 2020 203c 6275 7474 6f6e 2074         <button t
+00000980: 7970 653d 2273 7562 6d69 7422 2063 6c61  ype="submit" cla
+00000990: 7373 3d22 6274 6e20 6274 6e2d 736d 2062  ss="btn btn-sm b
+000009a0: 746e 2d64 616e 6765 7222 3e3c 6920 636c  tn-danger"><i cl
+000009b0: 6173 733d 226d 6469 206d 6469 2d74 7261  ass="mdi mdi-tra
+000009c0: 7368 2d63 616e 2d6f 7574 6c69 6e65 2220  sh-can-outline" 
+000009d0: 6172 6961 2d68 6964 6465 6e3d 2274 7275  aria-hidden="tru
+000009e0: 6522 3e3c 2f69 3e20 4465 6c65 7465 2053  e"></i> Delete S
+000009f0: 656c 6563 7465 643c 2f62 7574 746f 6e3e  elected</button>
+00000a00: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
+00000a10: 656e 6469 6620 257d 0a20 2020 2020 2020  endif %}.       
+00000a20: 2020 203c 2f64 6976 3e0a 0a20 2020 2020     </div>..     
+00000a30: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00000a40: 2264 726f 7064 6f77 6e22 3e0a 2020 2020  "dropdown">.    
+00000a50: 2020 2020 2020 2020 3c62 7574 746f 6e20          <button 
+00000a60: 7479 7065 3d22 6275 7474 6f6e 2220 636c  type="button" cl
+00000a70: 6173 733d 2262 746e 2062 746e 2d70 7572  ass="btn btn-pur
+00000a80: 706c 6520 6472 6f70 646f 776e 2d74 6f67  ple dropdown-tog
+00000a90: 676c 6522 2064 6174 612d 6273 2d74 6f67  gle" data-bs-tog
+00000aa0: 676c 653d 2264 726f 7064 6f77 6e22 2061  gle="dropdown" a
+00000ab0: 7269 612d 6861 7370 6f70 7570 3d22 7472  ria-haspopup="tr
+00000ac0: 7565 2220 6172 6961 2d65 7870 616e 6465  ue" aria-expande
+00000ad0: 643d 2266 616c 7365 223e 0a20 2020 2020  d="false">.     
+00000ae0: 2020 2020 2020 2020 203c 6920 636c 6173           <i clas
+00000af0: 733d 226d 6469 206d 6469 2d64 6f77 6e6c  s="mdi mdi-downl
+00000b00: 6f61 6422 3e3c 2f69 3e20 4578 706f 7274  oad"></i> Export
+00000b10: 0a20 2020 2020 2020 2020 2020 203c 2f62  .            </b
+00000b20: 7574 746f 6e3e 0a20 2020 2020 2020 2020  utton>.         
+00000b30: 2020 203c 756c 2063 6c61 7373 3d22 6472     <ul class="dr
+00000b40: 6f70 646f 776e 2d6d 656e 7520 6472 6f70  opdown-menu drop
+00000b50: 646f 776e 2d6d 656e 752d 656e 6422 3e0a  down-menu-end">.
+00000b60: 2020 2020 2020 2020 2020 2020 2020 3c6c                <l
+00000b70: 693e 3c61 2063 6c61 7373 3d22 6472 6f70  i><a class="drop
+00000b80: 646f 776e 2d69 7465 6d22 2068 7265 663d  down-item" href=
+00000b90: 227b 2520 7175 6572 7973 7472 696e 6720  "{% querystring 
+00000ba0: 7265 7175 6573 7420 6578 706f 7274 3d22  request export="
+00000bb0: 7461 626c 6522 2025 7d22 3e43 7572 7265  table" %}">Curre
+00000bc0: 6e74 2056 6965 773c 2f61 3e3c 2f6c 693e  nt View</a></li>
+00000bd0: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
+00000be0: 6c69 3e3c 6120 636c 6173 733d 2264 726f  li><a class="dro
+00000bf0: 7064 6f77 6e2d 6974 656d 2220 6872 6566  pdown-item" href
+00000c00: 3d22 7b25 2071 7565 7279 7374 7269 6e67  ="{% querystring
+00000c10: 2072 6571 7565 7374 2065 7870 6f72 743d   request export=
+00000c20: 2222 2025 7d22 3e41 6c6c 2044 6174 6120  "" %}">All Data 
+00000c30: 2843 5356 293c 2f61 3e3c 2f6c 693e 0a20  (CSV)</a></li>. 
+00000c40: 2020 2020 2020 2020 2020 203c 2f75 6c3e             </ul>
+00000c50: 0a20 2020 2020 2020 2020 203c 2f64 6976  .          </div
+00000c60: 3e0a 2020 2020 2020 2020 3c2f 6469 763e  >.        </div>
+00000c70: 0a20 2020 2020 203c 2f66 6f72 6d3e 0a20  .      </form>. 
+00000c80: 2020 207b 2520 656e 6477 6974 6820 257d     {% endwith %}
+00000c90: 0a20 207b 2520 656e 6469 6620 257d 0a3c  .  {% endif %}.<
+00000ca0: 2f64 6976 3e0a                           /div>.
```

### Comparing `netbox_kea-0.2.0/netbox_kea/templates/netbox_kea/server_status.html` & `netbox_kea-1.0.0/netbox_kea/templates/netbox_kea/server_status.html`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.2.0/netbox_kea/urls.py` & `netbox_kea-1.0.0/netbox_kea/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_kea-0.2.0/netbox_kea/utilities.py` & `netbox_kea-1.0.0/netbox_kea/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 from datetime import datetime
-from typing import Any, Callable, Dict, List, Literal, Optional
+from typing import Any, Callable, Literal, Optional
 
 from django.http import HttpResponse
 from django.shortcuts import redirect
 from django_tables2 import Table
 from django_tables2.export import TableExport
 from utilities.views import ViewTab
 
@@ -16,15 +16,15 @@
     if s is None:
         return None
     hours, rest = divmod(s, 3600)
     minutes, seconds = divmod(rest, 60)
     return f"{hours:02}:{minutes:02}:{seconds:02}"
 
 
-def _enrich_lease(now: datetime, lease: Dict[str, Any]) -> Dict[str, Any]:
+def _enrich_lease(now: datetime, lease: dict[str, Any]) -> dict[str, Any]:
     """Add expires at and expires in to a lease."""
 
     # Need to replace "-" so we can access the values in a template
     lease = {k.replace("-", "_"): v for k, v in lease.items()}
     if "cltt" not in lease and "valid_lft" not in lease:
         return lease
 
@@ -36,15 +36,15 @@
     expires_at = datetime.fromtimestamp(cltt + valid_lft)
     lease["expires_at"] = expires_at
     lease["expires_in"] = (expires_at - now).seconds
     lease["cltt"] = datetime.fromtimestamp(cltt)
     return lease
 
 
-def format_leases(leases: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
+def format_leases(leases: list[dict[str, Any]]) -> list[dict[str, Any]]:
     now = datetime.now()
     return [_enrich_lease(now, ls) for ls in leases]
 
 
 def export_table(
     table: Table,
     filename: str,
```

### Comparing `netbox_kea-0.2.0/netbox_kea/views.py` & `netbox_kea-1.0.0/netbox_kea/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import logging
 from abc import ABCMeta
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Optional
 
 from django.contrib import messages
-from django.http import HttpResponse
+from django.http import HttpResponse, HttpResponseForbidden
 from django.http.request import HttpRequest
 from django.shortcuts import redirect, render
 from django.urls import reverse
 from netaddr import IPAddress, IPNetwork
 from netbox.views import generic
 from utilities.exceptions import AbortRequest
-from utilities.htmx import is_htmx
 from utilities.paginator import EnhancedPaginator, get_paginate_count
 from utilities.views import GetReturnURLMixin, ViewTab, register_model_view
 
 from . import constants, forms, tables
 from .filtersets import ServerFilterSet
 from .kea import KeaClient
 from .models import Server
@@ -57,15 +56,15 @@
 
 @register_model_view(Server, "status")
 class ServerStatusView(generic.ObjectView):
     queryset = Server.objects.all()
     tab = ViewTab(label="Status", weight=1000)
     template_name = "netbox_kea/server_status.html"
 
-    def _get_ca_status(self, client: KeaClient) -> Dict[str, Any]:
+    def _get_ca_status(self, client: KeaClient) -> dict[str, Any]:
         """Get the control agent status"""
         status = client.command("status-get")
         args = status[0]["arguments"]
         assert args is not None
 
         version = client.command("version-get")
         version_args = version[0]["arguments"]
@@ -76,16 +75,16 @@
             "Uptime": format_duration(int(args["uptime"])),
             "Time since reload": format_duration(int(args["reload"])),
             "Version": version_args["extended"],
         }
 
     def _get_dhcp_status(
         self, server: Server, client: KeaClient
-    ) -> Dict[str, Dict[str, Any]]:
-        resp: Dict[str, Dict[str, Any]] = {}
+    ) -> dict[str, dict[str, Any]]:
+        resp: dict[str, dict[str, Any]] = {}
 
         # Map of name to pretty name
         service_names = {"dhcp6": "DHCPv6", "dhcp4": "DHCPv4"}
         services = []
         if server.dhcp6:
             services.append("dhcp6")
         if server.dhcp4:
@@ -139,33 +138,33 @@
                         ),
                     }
                 )
         return resp
 
     def _get_statuses(
         self, server: Server, client: KeaClient
-    ) -> Dict[str, Dict[str, Any]]:
+    ) -> dict[str, dict[str, Any]]:
         return {
             "Control Agent": self._get_ca_status(client),
             **self._get_dhcp_status(server, client),
         }
 
     def get_extra_context(
         self, request: HttpResponse, instance: Server
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         return {"statuses": self._get_statuses(instance, instance.get_client())}
 
 
 class BaseServerLeasesView(generic.ObjectView):
     template_name = "netbox_kea/server_dhcp_leases.html"
     queryset = Server.objects.all()
 
     def get_leases_page(
         self, client: KeaClient, subnet: IPNetwork, page: Optional[str], per_page: int
-    ) -> Tuple[List[Dict[str, Any]], Optional[str]]:
+    ) -> tuple[list[dict[str, Any]], Optional[str]]:
         if page:
             frm = page
         elif int(subnet.network) == 0:
             frm = str(subnet.network)
         else:
             frm = str(subnet.network - 1)
 
@@ -177,29 +176,30 @@
         )
 
         if resp[0]["result"] == 3:
             return [], None
 
         args = resp[0]["arguments"]
         assert args is not None
-        subnet_leases = args["leases"]
-        next = (
-            f"{subnet_leases[-1]['ip-address']}" if args["count"] == per_page else None
-        )
-        for i, lease in enumerate(args["leases"]):
+
+        raw_leases = args["leases"]
+        next = f"{raw_leases[-1]['ip-address']}" if args["count"] == per_page else None
+        for i, lease in enumerate(raw_leases):
             lease_ip = IPAddress(lease["ip-address"])
             if lease_ip not in subnet:
-                subnet_leases = subnet_leases[:i]
+                raw_leases = raw_leases[:i]
                 next = None
                 break
 
-        return format_leases(subnet_leases), next
+        subnet_leases = format_leases(raw_leases)
 
-    def get_leases(self, client: KeaClient, q: Any, by: str) -> List[Dict[str, Any]]:
-        arguments: Dict[str, Any]
+        return subnet_leases, next
+
+    def get_leases(self, client: KeaClient, q: Any, by: str) -> list[dict[str, Any]]:
+        arguments: dict[str, Any]
         command = ""
         multiple = True
 
         if by == constants.BY_IP:
             arguments = {"ip-address": q}
             multiple = False
         elif by == constants.BY_HW_ADDRESS:
@@ -235,15 +235,15 @@
         assert args is not None
         if multiple is True:
             return format_leases(args["leases"])
         return format_leases([args])
 
     def get_extra_context(
         self, request: HttpRequest, _instance: Server
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         # For non-htmx requests.
 
         table = self.table([], user=request.user)
         form = self.form(request.GET) if "q" in request.GET else self.form()
         return {"form": form, "table": table}
 
     def get_export(self, request: HttpRequest, **kwargs) -> HttpResponse:
@@ -255,15 +255,15 @@
         instance = self.get_object(**kwargs)
 
         by = form.cleaned_data["by"]
         q = form.cleaned_data["q"]
         client = instance.get_client()
         if by == constants.BY_SUBNET:
             leases = []
-            page = ""  # start from the beginning
+            page: Optional[str] = ""  # start from the beginning
             while page is not None:
                 page_leases, page = self.get_leases_page(
                     client,
                     q,
                     page,
                     per_page=get_paginate_count(request),
                 )
@@ -273,25 +273,25 @@
 
         table = self.table(leases, user=request.user)
         return export_table(
             table, "leases.csv", use_selected_columns=request.GET["export"] == "table"
         )
 
     def get(self, request: HttpRequest, **kwargs) -> HttpResponse:
-        logger = logging.getLogger("netbox_kea.views.BaseServerDHCPLeasesVie")
+        logger = logging.getLogger("netbox_kea.views.BaseServerDHCPLeasesView")
 
         instance: Server = self.get_object(**kwargs)
 
         if resp := check_dhcp_enabled(instance, self.dhcp_version):
             return resp
 
         if "export" in request.GET:
             return self.get_export(request, **kwargs)
 
-        if not is_htmx(request):
+        if not request.htmx:
             return super().get(request, **kwargs)
 
         try:
             form = self.form(request.GET)
             if not form.is_valid():
                 return render(
                     request,
@@ -316,32 +316,41 @@
                 )
                 paginate = True
             else:
                 paginate = False
                 next_page = None
                 leases = self.get_leases(client, q, by)
 
+            table = self.table(leases, user=request.user)
+            can_delete = request.user.has_perm(
+                "netbox_kea.bulk_delete_lease_from_server",
+                obj=instance,
+            )
+            if not can_delete:
+                table.columns.hide("pk")
+
             return render(
                 request,
                 "netbox_kea/server_dhcp_leases_htmx.html",
                 {
+                    "can_delete": can_delete,
                     "is_embedded": False,
                     "delete_action": reverse(
                         f"plugins:netbox_kea:server_leases{self.dhcp_version}_delete",
                         args=[instance.pk],
                     ),
                     "form": form,
-                    "table": self.table(leases, user=request.user),
+                    "table": table,
                     "next_page": next_page,
                     "paginate": paginate,
                     "page_lengths": EnhancedPaginator.default_page_lengths,
                 },
             )
         except Exception as e:
-            logger.exception("Got exception on DHCP leases HTMX handler")
+            logger.exception("exception on DHCP leases HTMX handler")
             return render(
                 request,
                 "netbox_kea/exception_htmx.html",
                 {"type_": type(e).__name__, "exception": str(e)},
             )
 
 
@@ -361,14 +370,23 @@
         label="DHCPv4 Leases", weight=1020, is_enabled=lambda s: s.dhcp4
     )
     form = forms.Leases4SearchForm
     table = tables.LeaseTable4
     dhcp_version = 4
 
 
+class FakeLeaseModelMeta:
+    verbose_name_plural = "leases"
+
+
+# Fake model to allow us to use the bulk_delete.html template.
+class FakeLeaseModel:
+    _meta = FakeLeaseModelMeta
+
+
 class BaseServerLeasesDeleteView(
     GetReturnURLMixin, generic.ObjectView, metaclass=ABCMeta
 ):
     queryset = Server.objects.all()
     default_return_url = "plugins:netbox_kea:server_list"
 
     def delete_lease(self, client: KeaClient, ip: str) -> None:
@@ -380,30 +398,39 @@
         )
 
     def get(self, request: HttpRequest, **kwargs):
         return redirect(self.get_return_url(request, obj=self.get_object(**kwargs)))
 
     def post(self, request: HttpRequest, **kwargs) -> HttpResponse:
         instance: Server = self.get_object(**kwargs)
+
+        if not request.user.has_perm(
+            "netbox_kea.bulk_delete_lease_from_server", obj=instance
+        ):
+            return HttpResponseForbidden(
+                "This user does not have permission to delete DHCP leases."
+            )
+
         form = self.form(request.POST)
 
         if not form.is_valid():
             messages.warning(request, str(form.errors))
             return redirect(self.get_return_url(request, obj=instance))
 
         lease_ips = form.cleaned_data["pk"]
         if "_confirm" not in request.POST:
-            if len(lease_ips) == 0:
-                messages.warning(request, "No leases were selected for deletion.")
-                return redirect(self.get_return_url(request, obj=instance))
             return render(
                 request,
-                "netbox_kea/server_leases_delete.html",
+                "generic/bulk_delete.html",
                 {
-                    "lease_ips": form.cleaned_data["pk"],
+                    "model": FakeLeaseModel,
+                    "table": tables.LeaseDeleteTable(
+                        ({"ip": ip} for ip in lease_ips),
+                        orderable=False,
+                    ),
                     "form": form,
                     "return_url": self.get_return_url(request, obj=instance),
                 },
             )
 
         client = instance.get_client()
 
@@ -426,47 +453,67 @@
 
 
 class ServerLeases4DeleteView(BaseServerLeasesDeleteView):
     form = forms.Lease4DeleteForm
     dhcp_version = 4
 
 
-class BaseServerDHCPSubnetsView(generic.ObjectView, metaclass=ABCMeta):
+class BaseServerDHCPSubnetsView(generic.ObjectChildrenView):
+    table = tables.SubnetTable
     queryset = Server.objects.all()
     template_name = "netbox_kea/server_dhcp_subnets.html"
 
-    def get_subnet_table(
-        self, request: HttpRequest, instance: Server
-    ) -> tables.SubnetTable:
-        client = instance.get_client()
-        subnets = self.get_subnets(client)
-        table = tables.SubnetTable(
-            f"plugins:netbox_kea:server_leases{self.dhcp_version}",
-            instance.pk,
-            subnets,
-            user=request.user,
-        )
-        table.configure(request)
-        return table
+    def get_children(
+        self, request: HttpRequest, parent: Server
+    ) -> list[dict[str, Any]]:
+        return self.get_subnets(parent)
+
+    def get_subnets(self, server: Server) -> list[dict[str, Any]]:
+        client = server.get_client()
+        config = client.command("config-get", service=[f"dhcp{self.dhcp_version}"])
+        assert config[0]["arguments"] is not None
+        subnets = config[0]["arguments"][f"Dhcp{self.dhcp_version}"][
+            f"subnet{self.dhcp_version}"
+        ]
+        subnet_list = [
+            dict(
+                id=s["id"],
+                subnet=s["subnet"],
+                dhcp_version=self.dhcp_version,
+                server_pk=server.pk,
+            )
+            for s in subnets
+            if "id" in s and "subnet" in s
+        ]
 
-    def get_extra_context(
-        self, request: HttpRequest, instance: Server
-    ) -> Dict[str, Any]:
-        return {"table": self.get_subnet_table(request, instance)}
+        for sn in config[0]["arguments"][f"Dhcp{self.dhcp_version}"]["shared-networks"]:
+            for s in sn[f"subnet{self.dhcp_version}"]:
+                subnet_list.append(
+                    dict(
+                        id=s["id"],
+                        subnet=s["subnet"],
+                        shared_network=sn["name"],
+                        dhcp_version=self.dhcp_version,
+                        server_pk=server.pk,
+                    )
+                )
+
+        return subnet_list
 
     def get(self, request: HttpRequest, **kwargs) -> HttpResponse:
         instance = self.get_object(**kwargs)
-
         if resp := check_dhcp_enabled(instance, self.dhcp_version):
             return resp
 
         if "export" not in request.GET:
             return super().get(request, **kwargs)
 
-        table = self.get_subnet_table(request, instance)
+        child_objects = self.get_children(request, instance)
+        table_data = self.prep_table_data(request, child_objects, instance)
+        table = self.get_table(table_data, request, False)
 
         return export_table(
             table,
             filename=f"kea-dhcpv{self.dhcp_version}-subnets.csv",
             use_selected_columns=request.GET["export"] == "table",
         )
 
@@ -474,50 +521,14 @@
 @register_model_view(Server, "subnets6")
 class ServerDHCP6SubnetsView(BaseServerDHCPSubnetsView):
     tab = OptionalViewTab(
         label="DHCPv6 Subnets", weight=1030, is_enabled=lambda s: s.dhcp6
     )
     dhcp_version = 6
 
-    def get_subnets(self, client: KeaClient) -> List[Dict[str, Any]]:
-        config = client.command("config-get", service=["dhcp6"])
-        assert config[0]["arguments"] is not None
-        subnets = config[0]["arguments"]["Dhcp6"]["subnet6"]
-        subnet_list = [
-            {"id": s["id"], "subnet": s["subnet"]}
-            for s in subnets
-            if "id" in s and "subnet" in s
-        ]
-
-        for sn in config[0]["arguments"]["Dhcp6"]["shared-networks"]:
-            for s in sn["subnet6"]:
-                subnet_list.append(
-                    dict(id=s["id"], subnet=s["subnet"], shared_network=sn["name"])
-                )
-
-        return subnet_list
-
 
 @register_model_view(Server, "subnets4")
 class ServerDHCP4SubnetsView(BaseServerDHCPSubnetsView):
     tab = OptionalViewTab(
         label="DHCPv4 Subnets", weight=1040, is_enabled=lambda s: s.dhcp4
     )
     dhcp_version = 4
-
-    def get_subnets(self, client: KeaClient) -> List[Dict[str, Any]]:
-        config = client.command("config-get", service=["dhcp4"])
-        assert config[0]["arguments"] is not None
-        subnets = config[0]["arguments"]["Dhcp4"]["subnet4"]
-        subnet_list = [
-            {"id": s["id"], "subnet": s["subnet"]}
-            for s in subnets
-            if "id" in s and "subnet" in s
-        ]
-
-        for sn in config[0]["arguments"]["Dhcp4"]["shared-networks"]:
-            for s in sn["subnet4"]:
-                subnet_list.append(
-                    dict(id=s["id"], subnet=s["subnet"], shared_network=sn["name"])
-                )
-
-        return subnet_list
```

### Comparing `netbox_kea-0.2.0/pyproject.toml` & `netbox_kea-1.0.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "netbox-kea"
-version = "0.2.0"
+version = "1.0.0"
 description = ""
 authors = ["Devon Mar <devonm+netbox-kea@mdmm.ca>"]
 readme = "README.md"
 packages = [{include = "netbox_kea"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 requests = "^2"
-netaddr = "^0.8"
+netaddr = ">=0.8,<=1.2.1"
 
 [tool.poetry.group.dev.dependencies]
-django-stubs = {extras = ["compatible-mypy"], version = "^4"}
+django-stubs = {extras = ["compatible-mypy"], version = "^5"}
 mypy = "^1.2"
 types-requests = "^2"
-pytest = "^7"
+pytest = "^8"
 pynetbox = "^7"
-flake8 = "^6.0"
-pytest-playwright = "^0.4"
+flake8 = "^7.0"
+pytest-playwright = "^0.5"
+black = "^24.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `netbox_kea-0.2.0/PKG-INFO` & `netbox_kea-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: netbox-kea
-Version: 0.2.0
+Version: 1.0.0
 Summary: 
 Author: Devon Mar
 Author-email: devonm+netbox-kea@mdmm.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: netaddr (>=0.8,<0.9)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: netaddr (>=0.8,<=1.2.1)
 Requires-Dist: requests (>=2,<3)
 Description-Content-Type: text/markdown
 
 # NetBox plugin for the Kea DHCP server
 
 This plugin allows you to view Kea status, leases and subnets in NetBox. Go directly from a NetBox device/VM to a DHCP lease and back!
 
@@ -38,21 +39,21 @@
 
 - Kea doesn't provide a way to get a list of subnets without an additional hook library.
   Thus, this plugin lists subnets using the `config-get` command. This means that the entire config will be fetched just to get the configured subnets!
   This may be an expensive operation.
 
 ## Requirements
 
-- NetBox > v3.5
+- NetBox >= v4.0
 - [Kea Control Agent](https://kea.readthedocs.io/en/latest/arm/agent.html)
 - [`lease_cmds`](https://kea.readthedocs.io/en/latest/arm/hooks.html#lease-cmds-lease-commands-for-easier-lease-management) hook library
 
 ## Compatibility
 
-- This plugin was tested with Kea v2.2.0 with the `memfile` lease database.
+- This plugin is tested with Kea v2.4.1 with the `memfile` lease database.
   Other versions and lease databases may also work.
 
 ## Installation
 
 1. Add `netbox-kea` to `local_requirements.txt`.
 
 2. Enable the plugin in `configuration.py`
```

