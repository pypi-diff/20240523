# Comparing `tmp/otpme-0.3.0a63.tar.gz` & `tmp/otpme-0.3.0a64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otpme-0.3.0a63.tar", last modified: Thu May 23 11:25:55 2024, max compression
+gzip compressed data, was "otpme-0.3.0a64.tar", last modified: Thu May 23 13:27:40 2024, max compression
```

## Comparing `otpme-0.3.0a63.tar` & `otpme-0.3.0a64.tar`

### file list

```diff
@@ -1,510 +1,510 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.895501 otpme-0.3.0a63/
--rw-r--r--   0 root         (0) root         (0)    35121 2024-05-23 11:25:55.000000 otpme-0.3.0a63/LICENSE
--rw-r--r--   0 root         (0) root         (0)      665 2024-05-23 11:25:55.000000 otpme-0.3.0a63/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      680 2024-05-23 11:25:55.895501 otpme-0.3.0a63/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3821 2024-05-23 11:25:55.000000 otpme-0.3.0a63/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.847500 otpme-0.3.0a63/bash_completion/
--rw-r--r--   0 root         (0) root         (0)     1937 2024-05-23 11:25:55.000000 otpme-0.3.0a63/bash_completion/otpme
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.847500 otpme-0.3.0a63/deploy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.851500 otpme-0.3.0a63/deploy/dicts/
--rw-r--r--   0 root         (0) root         (0)     2535 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/dicts/abbreviations-it.gz
--rw-r--r--   0 root         (0) root         (0)    18683 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/dicts/at-surnames.gz
--rw-r--r--   0 root         (0) root         (0)   197269 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/dicts/common-passwords.gz
--rwxr-xr-x   0 root         (0) root         (0)      532 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/dicts/convert_dict.sh
--rw-r--r--   0 root         (0) root         (0)     3286 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/dicts/de-female.gz
--rw-r--r--   0 root         (0) root         (0)     3070 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/dicts/de-male.gz
--rw-r--r--   0 root         (0) root         (0)    11343 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/dicts/de-surnames.gz
--rw-r--r--   0 root         (0) root         (0)    34845 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/dicts/de-top10000.gz
--rw-r--r--   0 root         (0) root         (0)    30600 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/dicts/en-top10000.gz
--rw-r--r--   0 root         (0) root         (0)   127983 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/dicts/english-guessing.gz
--rw-r--r--   0 root         (0) root         (0)  1041710 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/dicts/english.gz
--rw-r--r--   0 root         (0) root         (0)   547291 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/dicts/german-guessing.gz
--rw-r--r--   0 root         (0) root         (0)   544600 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/dicts/german.gz
--rw-r--r--   0 root         (0) root         (0)    13539 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/dicts/us-female.gz
--rw-r--r--   0 root         (0) root         (0)     4089 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/dicts/us-male.gz
--rw-r--r--   0 root         (0) root         (0)    35682 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/dicts/us-surnames.gz
--rw-r--r--   0 root         (0) root         (0)    13331 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/otpme.conf.dist
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.851500 otpme-0.3.0a63/deploy/pam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.851500 otpme-0.3.0a63/deploy/pam/pam-python/
--rw-r--r--   0 root         (0) root         (0)      511 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/pam/pam-python/README
--rw-r--r--   0 root         (0) root         (0)     2436 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/pam/pam_otpme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.851500 otpme-0.3.0a63/deploy/radius/
--rw-r--r--   0 root         (0) root         (0)    13085 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/radius/dictionary
--rw-r--r--   0 root         (0) root         (0)     3851 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/radius/dictionary.freeradius
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.851500 otpme-0.3.0a63/deploy/schema/
--rw-r--r--   0 root         (0) root         (0)    21610 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/schema/core.schema
--rw-r--r--   0 root         (0) root         (0)    73993 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/schema/cosine.schema
--rw-r--r--   0 root         (0) root         (0)     6267 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/schema/inetorgperson.schema
--rw-r--r--   0 root         (0) root         (0)     7632 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/schema/nis.schema
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.851500 otpme-0.3.0a63/deploy/scripts/
--rw-r--r--   0 root         (0) root         (0)     8600 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/scripts/agent_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/scripts/auth_script.sh
--rw-r--r--   0 root         (0) root         (0)    21045 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/scripts/key_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/scripts/login_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/scripts/node_vote_script.sh
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 11:25:55.000000 otpme-0.3.0a63/deploy/scripts/push_script.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.851500 otpme-0.3.0a63/otpme/
--rw-r--r--   0 root         (0) root         (0)      965 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    12722 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.859501 otpme-0.3.0a63/otpme/lib/
--rw-r--r--   0 root         (0) root         (0)    10486 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2037 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/arp.py
--rw-r--r--   0 root         (0) root         (0)     3569 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/auth_script.py
--rw-r--r--   0 root         (0) root         (0)    48110 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.859501 otpme-0.3.0a63/otpme/lib/backends/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/backends/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.859501 otpme-0.3.0a63/otpme/lib/backends/file/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/backends/file/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90252 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/backends/file/file.py
--rw-r--r--   0 root         (0) root         (0)    13013 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/backends/file/index.py
--rw-r--r--   0 root         (0) root         (0)     5898 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/backends/file/models.py
--rw-r--r--   0 root         (0) root         (0)    67261 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/backends/file/transaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.859501 otpme-0.3.0a63/otpme/lib/cache/
--rw-r--r--   0 root         (0) root         (0)    27634 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3226 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cache/dogpile.py
--rw-r--r--   0 root         (0) root         (0)    19511 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cache/funccache.py
--rw-r--r--   0 root         (0) root         (0)     3515 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cache/lru.py
--rw-r--r--   0 root         (0) root         (0)    14416 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cache/memcache.py
--rw-r--r--   0 root         (0) root         (0)     6500 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cache/memcached.py
--rw-r--r--   0 root         (0) root         (0)     7344 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cache/memcachedb.py
--rw-r--r--   0 root         (0) root         (0)    27195 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cache/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.863500 otpme-0.3.0a63/otpme/lib/classes/
--rw-r--r--   0 root         (0) root         (0)      959 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86247 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/accessgroup.py
--rw-r--r--   0 root         (0) root         (0)    14874 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/agent_conn.py
--rw-r--r--   0 root         (0) root         (0)   125856 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/auth_handler.py
--rw-r--r--   0 root         (0) root         (0)    56674 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/ca.py
--rw-r--r--   0 root         (0) root         (0)    40808 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/client.py
--rw-r--r--   0 root         (0) root         (0)   230568 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/command_handler.py
--rw-r--r--   0 root         (0) root         (0)     8730 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/conn_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.867501 otpme-0.3.0a63/otpme/lib/classes/data_objects/
--rw-r--r--   0 root         (0) root         (0)      880 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/data_objects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2386 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/data_objects/cert.py
--rw-r--r--   0 root         (0) root         (0)     6865 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/data_objects/data_revision.py
--rw-r--r--   0 root         (0) root         (0)     6880 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/data_objects/failed_pass.py
--rw-r--r--   0 root         (0) root         (0)     8125 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/data_objects/last_assigned_id.py
--rw-r--r--   0 root         (0) root         (0)    10579 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/data_objects/revoked_signature.py
--rw-r--r--   0 root         (0) root         (0)     2570 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/data_objects/rsa_key.py
--rw-r--r--   0 root         (0) root         (0)     7020 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/data_objects/skip_sync.py
--rw-r--r--   0 root         (0) root         (0)     5811 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/data_objects/token_counter.py
--rw-r--r--   0 root         (0) root         (0)     5646 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/data_objects/used_hash.py
--rw-r--r--   0 root         (0) root         (0)     5989 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/data_objects/used_otp.py
--rw-r--r--   0 root         (0) root         (0)     5997 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/data_objects/used_slp.py
--rw-r--r--   0 root         (0) root         (0)     5992 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/data_objects/used_sotp.py
--rw-r--r--   0 root         (0) root         (0)    28682 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/dictionary.py
--rw-r--r--   0 root         (0) root         (0)    39185 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/group.py
--rw-r--r--   0 root         (0) root         (0)    52065 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/host.py
--rw-r--r--   0 root         (0) root         (0)    12296 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/login_handler.py
--rw-r--r--   0 root         (0) root         (0)     5370 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/mgmt_client.py
--rw-r--r--   0 root         (0) root         (0)    38858 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/node.py
--rw-r--r--   0 root         (0) root         (0)    24441 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/object_config.py
--rw-r--r--   0 root         (0) root         (0)    77129 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/otpme_agent.py
--rw-r--r--   0 root         (0) root         (0)    49704 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/otpme_host.py
--rw-r--r--   0 root         (0) root         (0)   318862 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/otpme_object.py
--rw-r--r--   0 root         (0) root         (0)    23357 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/policy.py
--rw-r--r--   0 root         (0) root         (0)    62493 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/realm.py
--rw-r--r--   0 root         (0) root         (0)    74478 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/resolver.py
--rw-r--r--   0 root         (0) root         (0)    45067 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/role.py
--rw-r--r--   0 root         (0) root         (0)    34240 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/script.py
--rw-r--r--   0 root         (0) root         (0)    52940 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/session.py
--rw-r--r--   0 root         (0) root         (0)    31485 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/signing.py
--rw-r--r--   0 root         (0) root         (0)   107251 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/site.py
--rw-r--r--   0 root         (0) root         (0)     7054 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/ssh_agent.py
--rw-r--r--   0 root         (0) root         (0)   134917 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/token.py
--rw-r--r--   0 root         (0) root         (0)    49462 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/unit.py
--rw-r--r--   0 root         (0) root         (0)   182238 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/classes/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.867501 otpme-0.3.0a63/otpme/lib/cli/
--rw-r--r--   0 root         (0) root         (0)    64641 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12952 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cli/accessgroup.py
--rw-r--r--   0 root         (0) root         (0)     7186 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cli/ca.py
--rw-r--r--   0 root         (0) root         (0)    13309 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cli/client.py
--rw-r--r--   0 root         (0) root         (0)     5710 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cli/dictionary.py
--rw-r--r--   0 root         (0) root         (0)    13060 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cli/group.py
--rw-r--r--   0 root         (0) root         (0)    13124 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cli/host.py
--rw-r--r--   0 root         (0) root         (0)    11041 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cli/node.py
--rw-r--r--   0 root         (0) root         (0)     6232 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cli/policy.py
--rw-r--r--   0 root         (0) root         (0)     6241 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cli/realm.py
--rw-r--r--   0 root         (0) root         (0)     6667 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cli/resolver.py
--rw-r--r--   0 root         (0) root         (0)    20315 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cli/role.py
--rw-r--r--   0 root         (0) root         (0)     7450 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cli/script.py
--rw-r--r--   0 root         (0) root         (0)     7591 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cli/site.py
--rw-r--r--   0 root         (0) root         (0)    17421 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cli/token.py
--rw-r--r--   0 root         (0) root         (0)     5490 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cli/unit.py
--rw-r--r--   0 root         (0) root         (0)     7663 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/cli/user.py
--rw-r--r--   0 root         (0) root         (0)    24934 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/compgen.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.867501 otpme-0.3.0a63/otpme/lib/compression/
--rw-r--r--   0 root         (0) root         (0)      514 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/compression/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4149 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/compression/base.py
--rw-r--r--   0 root         (0) root         (0)    14344 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/connections.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.871501 otpme-0.3.0a63/otpme/lib/daemon/
--rw-r--r--   0 root         (0) root         (0)      685 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3852 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/daemon/authd.py
--rw-r--r--   0 root         (0) root         (0)   109032 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/daemon/clusterd.py
--rw-r--r--   0 root         (0) root         (0)    47618 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/daemon/controld.py
--rw-r--r--   0 root         (0) root         (0)    76830 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/daemon/hostd.py
--rw-r--r--   0 root         (0) root         (0)     3141 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/daemon/joind.py
--rw-r--r--   0 root         (0) root         (0)     6780 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/daemon/ldapd.py
--rw-r--r--   0 root         (0) root         (0)     3070 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/daemon/mgmtd.py
--rw-r--r--   0 root         (0) root         (0)    15943 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/daemon/otpme_daemon.py
--rw-r--r--   0 root         (0) root         (0)    11458 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/daemon/scriptd.py
--rw-r--r--   0 root         (0) root         (0)     3084 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/daemon/syncd.py
--rw-r--r--   0 root         (0) root         (0)     6941 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/daemon/unix_daemon.py
--rw-r--r--   0 root         (0) root         (0)    19072 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/debug.py
--rw-r--r--   0 root         (0) root         (0)     2157 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/doc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.871501 otpme-0.3.0a63/otpme/lib/encoding/
--rw-r--r--   0 root         (0) root         (0)      496 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/encoding/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1846 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/encoding/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.871501 otpme-0.3.0a63/otpme/lib/encryption/
--rw-r--r--   0 root         (0) root         (0)     4020 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/encryption/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3363 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/encryption/aes.py
--rw-r--r--   0 root         (0) root         (0)     1546 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/encryption/aes_cfb.py
--rw-r--r--   0 root         (0) root         (0)     7967 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/encryption/argon2.py
--rw-r--r--   0 root         (0) root         (0)    10307 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/encryption/asymmetric_key_handler.py
--rw-r--r--   0 root         (0) root         (0)     4318 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/encryption/ec.py
--rw-r--r--   0 root         (0) root         (0)     2979 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/encryption/fernet.py
--rw-r--r--   0 root         (0) root         (0)     3304 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/encryption/hkdf.py
--rw-r--r--   0 root         (0) root         (0)     3794 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/encryption/pbkdf2.py
--rw-r--r--   0 root         (0) root         (0)     7891 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/encryption/rsa.py
--rw-r--r--   0 root         (0) root         (0)     4391 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.871501 otpme-0.3.0a63/otpme/lib/extensions/
--rw-r--r--   0 root         (0) root         (0)      396 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/extensions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.871501 otpme-0.3.0a63/otpme/lib/extensions/base/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/extensions/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12345 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/extensions/base/base.py
--rw-r--r--   0 root         (0) root         (0)    40219 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/extensions/ldif_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.871501 otpme-0.3.0a63/otpme/lib/extensions/posix/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/extensions/posix/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14353 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/extensions/posix/posix.py
--rw-r--r--   0 root         (0) root         (0)     3707 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/extensions/utils.py
--rw-r--r--   0 root         (0) root         (0)    34148 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/filetools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.871501 otpme-0.3.0a63/otpme/lib/freeradius/
--rw-r--r--   0 root         (0) root         (0)     9186 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/freeradius/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18752 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/freeradius/otpme.py
--rw-r--r--   0 root         (0) root         (0)     1297 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/freeradius/radiusd.py
--rw-r--r--   0 root         (0) root         (0)     1203 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/freeradius/radiusd_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.871501 otpme-0.3.0a63/otpme/lib/gpg/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/gpg/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    28565 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/gpg/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.875501 otpme-0.3.0a63/otpme/lib/help/
--rwxr-xr-x   0 root         (0) root         (0)    26596 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23053 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/accessgroup.py
--rw-r--r--   0 root         (0) root         (0)     5552 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/agent.py
--rw-r--r--   0 root         (0) root         (0)     1924 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/auth.py
--rw-r--r--   0 root         (0) root         (0)    15774 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/ca.py
--rw-r--r--   0 root         (0) root         (0)    16991 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/client.py
--rw-r--r--   0 root         (0) root         (0)     1635 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/cluster.py
--rw-r--r--   0 root         (0) root         (0)     5852 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/controld.py
--rw-r--r--   0 root         (0) root         (0)    11455 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/dictionary.py
--rw-r--r--   0 root         (0) root         (0)      589 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/get_authorized_keys.py
--rw-r--r--   0 root         (0) root         (0)    19939 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/group.py
--rw-r--r--   0 root         (0) root         (0)    24503 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/host.py
--rw-r--r--   0 root         (0) root         (0)    21376 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/node.py
--rw-r--r--   0 root         (0) root         (0)      544 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/pinentry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.875501 otpme-0.3.0a63/otpme/lib/help/policy/
--rw-r--r--   0 root         (0) root         (0)     8806 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/policy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3777 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/policy/authonaction.py
--rw-r--r--   0 root         (0) root         (0)     1314 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/policy/autodisable.py
--rw-r--r--   0 root         (0) root         (0)     1818 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/policy/defaultgroups.py
--rw-r--r--   0 root         (0) root         (0)     1626 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/policy/defaultpolicies.py
--rw-r--r--   0 root         (0) root         (0)     1488 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/policy/defaultroles.py
--rw-r--r--   0 root         (0) root         (0)     1903 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/policy/defaultunits.py
--rw-r--r--   0 root         (0) root         (0)     1559 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/policy/forcetoken.py
--rw-r--r--   0 root         (0) root         (0)     2297 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/policy/idrange.py
--rw-r--r--   0 root         (0) root         (0)     3292 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/policy/logintimes.py
--rw-r--r--   0 root         (0) root         (0)     1165 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/policy/objecttemplates.py
--rw-r--r--   0 root         (0) root         (0)     2985 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/policy/password.py
--rw-r--r--   0 root         (0) root         (0)     2846 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/policy/tokenacls.py
--rw-r--r--   0 root         (0) root         (0)    20104 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/realm.py
--rw-r--r--   0 root         (0) root         (0)     1508 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/register.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.875501 otpme-0.3.0a63/otpme/lib/help/resolver/
--rw-r--r--   0 root         (0) root         (0)    12589 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4532 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/resolver/ldap.py
--rw-r--r--   0 root         (0) root         (0)    18265 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/role.py
--rw-r--r--   0 root         (0) root         (0)    15178 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/script.py
--rw-r--r--   0 root         (0) root         (0)     2911 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/session.py
--rw-r--r--   0 root         (0) root         (0)    22555 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.879501 otpme-0.3.0a63/otpme/lib/help/token/
--rw-r--r--   0 root         (0) root         (0)    20570 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/token/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1452 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/token/fido2.py
--rw-r--r--   0 root         (0) root         (0)     5686 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/token/hotp.py
--rw-r--r--   0 root         (0) root         (0)     6406 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/token/motp.py
--rw-r--r--   0 root         (0) root         (0)     2058 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/token/otp_push.py
--rw-r--r--   0 root         (0) root         (0)     5018 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/token/otpme.py
--rw-r--r--   0 root         (0) root         (0)     3947 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/token/password.py
--rw-r--r--   0 root         (0) root         (0)     7318 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/token/ssh.py
--rw-r--r--   0 root         (0) root         (0)     6044 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/token/totp.py
--rw-r--r--   0 root         (0) root         (0)     5870 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/token/yubikey_hmac.py
--rw-r--r--   0 root         (0) root         (0)     1320 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/token/yubikey_hotp.py
--rw-r--r--   0 root         (0) root         (0)    25002 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/tool.py
--rw-r--r--   0 root         (0) root         (0)    15235 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/unit.py
--rw-r--r--   0 root         (0) root         (0)    29476 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/help/user.py
--rw-r--r--   0 root         (0) root         (0)    16408 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/host.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.879501 otpme-0.3.0a63/otpme/lib/humanize/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/humanize/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4258 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/humanize/units.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.879501 otpme-0.3.0a63/otpme/lib/index/
--rw-r--r--   0 root         (0) root         (0)      449 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24015 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/index/mysql.py
--rw-r--r--   0 root         (0) root         (0)    24609 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/index/postgres.py
--rw-r--r--   0 root         (0) root         (0)     8403 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/index/sqlite3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.879501 otpme-0.3.0a63/otpme/lib/job/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20748 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/job/callback.py
--rw-r--r--   0 root         (0) root         (0)    12916 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/job/otpme_job.py
--rw-r--r--   0 root         (0) root         (0)    37164 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/join.py
--rw-r--r--   0 root         (0) root         (0)     4924 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/json.py
--rw-r--r--   0 root         (0) root         (0)     2009 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/jwt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.879501 otpme-0.3.0a63/otpme/lib/ldap/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/ldap/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1421 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/ldap/client.py
--rw-r--r--   0 root         (0) root         (0)    11129 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/ldap/schema.py
--rw-r--r--   0 root         (0) root         (0)    50550 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/ldap/server.py
--rw-r--r--   0 root         (0) root         (0)    19776 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/locking.py
--rw-r--r--   0 root         (0) root         (0)     9497 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/log.py
--rw-r--r--   0 root         (0) root         (0)     1596 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/messages.py
--rw-r--r--   0 root         (0) root         (0)     6048 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/mschap.py
--rw-r--r--   0 root         (0) root         (0)     2433 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/mschap_util.py
--rw-r--r--   0 root         (0) root         (0)    35811 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/multiprocessing.py
--rw-r--r--   0 root         (0) root         (0)    10317 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/net.py
--rw-r--r--   0 root         (0) root         (0)    27211 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/nsscache.py
--rw-r--r--   0 root         (0) root         (0)    63395 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/offline_token.py
--rw-r--r--   0 root         (0) root         (0)    23845 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/oid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.879501 otpme-0.3.0a63/otpme/lib/otp/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/otp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.879501 otpme-0.3.0a63/otpme/lib/otp/oath/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/otp/oath/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1794 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/otp/oath/hotp.py
--rw-r--r--   0 root         (0) root         (0)     1648 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/otp/oath/totp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.879501 otpme-0.3.0a63/otpme/lib/otp/otpme/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/otp/otpme/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3154 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/otp/otpme/otpme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.879501 otpme-0.3.0a63/otpme/lib/otp/yubico/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/otp/yubico/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3093 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/otp/yubico/yubiotp.py
--rw-r--r--   0 root         (0) root         (0)    19904 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/otpme_acl.py
--rw-r--r--   0 root         (0) root         (0)   115839 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/otpme_config.py
--rw-r--r--   0 root         (0) root         (0)     3586 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/otpme_pass.py
--rw-r--r--   0 root         (0) root         (0)    70426 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/pam.py
--rw-r--r--   0 root         (0) root         (0)     2042 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/pickle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.879501 otpme-0.3.0a63/otpme/lib/pinentry/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/pinentry/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27532 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/pinentry/pinentry.py
--rwxr-xr-x   0 root         (0) root         (0)     7947 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/pinentry/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.879501 otpme-0.3.0a63/otpme/lib/pki/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/pki/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9864 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/pki/cert.py
--rw-r--r--   0 root         (0) root         (0)    23217 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/pki/utils.py
--rw-r--r--   0 root         (0) root         (0)    16957 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/pki/utils_openssl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.879501 otpme-0.3.0a63/otpme/lib/policy/
--rw-r--r--   0 root         (0) root         (0)     2166 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.879501 otpme-0.3.0a63/otpme/lib/policy/authonaction/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/authonaction/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32730 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/authonaction/authonaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.879501 otpme-0.3.0a63/otpme/lib/policy/autodisable/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/autodisable/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15785 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/autodisable/autodisable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.883501 otpme-0.3.0a63/otpme/lib/policy/defaultgroups/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/defaultgroups/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17637 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/defaultgroups/defaultgroups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.883501 otpme-0.3.0a63/otpme/lib/policy/defaultpolicies/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/defaultpolicies/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14577 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/defaultpolicies/defaultpolicies.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.883501 otpme-0.3.0a63/otpme/lib/policy/defaultroles/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/defaultroles/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/defaultroles/defaultroles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.883501 otpme-0.3.0a63/otpme/lib/policy/defaultunits/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/defaultunits/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15704 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/defaultunits/defaultunits.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.883501 otpme-0.3.0a63/otpme/lib/policy/forcetoken/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/forcetoken/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14269 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/forcetoken/forcetoken.py
--rw-r--r--   0 root         (0) root         (0)     1243 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/get_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.883501 otpme-0.3.0a63/otpme/lib/policy/idrange/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/idrange/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27323 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/idrange/idrange.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.883501 otpme-0.3.0a63/otpme/lib/policy/logintimes/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/logintimes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23084 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/logintimes/logintimes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.883501 otpme-0.3.0a63/otpme/lib/policy/objecttemplates/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/objecttemplates/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15021 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/objecttemplates/objecttemplates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.883501 otpme-0.3.0a63/otpme/lib/policy/password/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/password/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29048 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/password/password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.883501 otpme-0.3.0a63/otpme/lib/policy/tokenacls/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/tokenacls/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24964 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/tokenacls/tokenacls.py
--rw-r--r--   0 root         (0) root         (0)      558 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/policy/utils.py
--rw-r--r--   0 root         (0) root         (0)     9399 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/preload.py
--rw-r--r--   0 root         (0) root         (0)     2533 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.883501 otpme-0.3.0a63/otpme/lib/protocols/
--rw-r--r--   0 root         (0) root         (0)      371 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.883501 otpme-0.3.0a63/otpme/lib/protocols/client/
--rw-r--r--   0 root         (0) root         (0)      722 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1954 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/client/agent1.py
--rw-r--r--   0 root         (0) root         (0)      899 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/client/auth1.py
--rw-r--r--   0 root         (0) root         (0)    14368 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/client/cluster1.py
--rw-r--r--   0 root         (0) root         (0)     1113 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/client/get_class.py
--rw-r--r--   0 root         (0) root         (0)     4712 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/client/host1.py
--rw-r--r--   0 root         (0) root         (0)      899 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/client/join1.py
--rwxr-xr-x   0 root         (0) root         (0)    11372 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/client/mgmt1.py
--rw-r--r--   0 root         (0) root         (0)    68042 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/client/sync1.py
--rw-r--r--   0 root         (0) root         (0)   160760 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/otpme_client.py
--rw-r--r--   0 root         (0) root         (0)    81487 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/otpme_server.py
--rw-r--r--   0 root         (0) root         (0)     1668 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/request.py
--rw-r--r--   0 root         (0) root         (0)     1837 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.887501 otpme-0.3.0a63/otpme/lib/protocols/server/
--rw-r--r--   0 root         (0) root         (0)      894 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40286 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/server/agent1.py
--rw-r--r--   0 root         (0) root         (0)    12909 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/server/auth1.py
--rw-r--r--   0 root         (0) root         (0)    32369 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/server/cluster1.py
--rw-r--r--   0 root         (0) root         (0)     1979 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/server/get_class.py
--rw-r--r--   0 root         (0) root         (0)    26675 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/server/host1.py
--rw-r--r--   0 root         (0) root         (0)    52629 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/server/join1.py
--rw-r--r--   0 root         (0) root         (0)    70933 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/server/mgmt1.py
--rw-r--r--   0 root         (0) root         (0)    45500 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/server/sync1.py
--rw-r--r--   0 root         (0) root         (0)      594 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/status_codes.py
--rw-r--r--   0 root         (0) root         (0)     7004 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/protocols/utils.py
--rw-r--r--   0 root         (0) root         (0)     2224 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/push_script.py
--rw-r--r--   0 root         (0) root         (0)     1206 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/qrcode.py
--rw-r--r--   0 root         (0) root         (0)      545 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/re.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.887501 otpme-0.3.0a63/otpme/lib/register/
--rw-r--r--   0 root         (0) root         (0)     9783 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/register/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.887501 otpme-0.3.0a63/otpme/lib/resolver/
--rw-r--r--   0 root         (0) root         (0)      552 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1225 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/resolver/get_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.887501 otpme-0.3.0a63/otpme/lib/resolver/ldap/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/resolver/ldap/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39505 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/resolver/ldap/ldap.py
--rw-r--r--   0 root         (0) root         (0)      518 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/resolver/utils.py
--rw-r--r--   0 root         (0) root         (0)    10086 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/script.py
--rw-r--r--   0 root         (0) root         (0)     3072 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/sign_key_cache.py
--rw-r--r--   0 root         (0) root         (0)      604 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/slp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.887501 otpme-0.3.0a63/otpme/lib/smartcard/
--rw-r--r--   0 root         (0) root         (0)      690 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/smartcard/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.887501 otpme-0.3.0a63/otpme/lib/smartcard/fido2/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/smartcard/fido2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10228 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/smartcard/fido2/fido2.py
--rw-r--r--   0 root         (0) root         (0)      925 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/smartcard/get_class.py
--rw-r--r--   0 root         (0) root         (0)     1733 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/smartcard/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.887501 otpme-0.3.0a63/otpme/lib/smartcard/yubikey/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/smartcard/yubikey/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12018 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/smartcard/yubikey/deploy.py
--rw-r--r--   0 root         (0) root         (0)     2049 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/smartcard/yubikey/usb.py
--rw-r--r--   0 root         (0) root         (0)     8142 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/smartcard/yubikey/yubikey.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.887501 otpme-0.3.0a63/otpme/lib/smartcard/yubikey_gpg/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/smartcard/yubikey_gpg/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6431 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.887501 otpme-0.3.0a63/otpme/lib/smartcard/yubikey_hmac/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/smartcard/yubikey_hmac/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12022 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.887501 otpme-0.3.0a63/otpme/lib/smartcard/yubikey_hotp/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/smartcard/yubikey_hotp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5099 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.887501 otpme-0.3.0a63/otpme/lib/socket/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/socket/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13219 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/socket/connect.py
--rw-r--r--   0 root         (0) root         (0)     8517 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/socket/handler.py
--rw-r--r--   0 root         (0) root         (0)    31029 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/socket/listen.py
--rw-r--r--   0 root         (0) root         (0)     2897 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/socket/send_recv1.py
--rw-r--r--   0 root         (0) root         (0)     4475 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/sotp.py
--rwxr-xr-x   0 root         (0) root         (0)    37180 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/spsc.py
--rw-r--r--   0 root         (0) root         (0)      611 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/srp.py
--rw-r--r--   0 root         (0) root         (0)    23521 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/ssh.py
--rw-r--r--   0 root         (0) root         (0)    63740 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/stuff.py
--rw-r--r--   0 root         (0) root         (0)    12405 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/sync_cache.py
--rw-r--r--   0 root         (0) root         (0)     4703 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/system_command.py
--rw-r--r--   0 root         (0) root         (0)     5703 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.887501 otpme-0.3.0a63/otpme/lib/third_party/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.891501 otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/
--rw-r--r--   0 root         (0) root         (0)     1981 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/advanced.py
--rw-r--r--   0 root         (0) root         (0)     9859 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/caching_query.py
--rw-r--r--   0 root         (0) root         (0)     2250 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/environment.py
--rw-r--r--   0 root         (0) root         (0)     1764 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/fixture_data.py
--rw-r--r--   0 root         (0) root         (0)     2248 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/helloworld.py
--rw-r--r--   0 root         (0) root         (0)     3310 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/local_session_caching.py
--rw-r--r--   0 root         (0) root         (0)     3033 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/model.py
--rw-r--r--   0 root         (0) root         (0)     1040 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/relationship_caching.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.891501 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/
--rw-r--r--   0 root         (0) root         (0)     1140 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.891501 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/caches/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/caches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9083 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/caches/caches.py
--rw-r--r--   0 root         (0) root         (0)    14341 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/caches/files.py
--rw-r--r--   0 root         (0) root         (0)     1044 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/config.py
--rw-r--r--   0 root         (0) root         (0)     1959 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/error.py
--rw-r--r--   0 root         (0) root         (0)     7963 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.891501 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/maps/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/maps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2389 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/maps/group.py
--rw-r--r--   0 root         (0) root         (0)    11745 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/maps/maps.py
--rw-r--r--   0 root         (0) root         (0)     2554 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/maps/passwd.py
--rw-r--r--   0 root         (0) root         (0)     2387 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/maps/shadow.py
--rw-r--r--   0 root         (0) root         (0)     4140 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/nss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.891501 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/update/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/update/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5487 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/update/files_updater.py
--rw-r--r--   0 root         (0) root         (0)     5826 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/update/map_updater.py
--rw-r--r--   0 root         (0) root         (0)    10980 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/update/updater.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.891501 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/util/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4117 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/nss_cache/util/file_formats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.891501 otpme-0.3.0a63/otpme/lib/third_party/oath_toolkit/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/oath_toolkit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1592 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/oath_toolkit/_compat.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/third_party/oath_toolkit/uri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.891501 otpme-0.3.0a63/otpme/lib/token/
--rw-r--r--   0 root         (0) root         (0)     1020 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.891501 otpme-0.3.0a63/otpme/lib/token/fido2/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/fido2/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15006 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/fido2/fido2.py
--rw-r--r--   0 root         (0) root         (0)     1123 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/get_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.891501 otpme-0.3.0a63/otpme/lib/token/hotp/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/hotp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39413 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/hotp/hotp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.891501 otpme-0.3.0a63/otpme/lib/token/link/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/link/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9723 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/link/link.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.895501 otpme-0.3.0a63/otpme/lib/token/motp/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/motp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27837 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/motp/motp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.895501 otpme-0.3.0a63/otpme/lib/token/oath/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/oath/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19688 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/oath/oath.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.895501 otpme-0.3.0a63/otpme/lib/token/otp_push/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/otp_push/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23460 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/otp_push/otp_push.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.895501 otpme-0.3.0a63/otpme/lib/token/otpme/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/otpme/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24771 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/otpme/otpme.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.895501 otpme-0.3.0a63/otpme/lib/token/password/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/password/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26135 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/password/password.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.895501 otpme-0.3.0a63/otpme/lib/token/script_otp/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/script_otp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9744 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/script_otp/script_otp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.895501 otpme-0.3.0a63/otpme/lib/token/script_static/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/script_static/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9744 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/script_static/script_static.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.895501 otpme-0.3.0a63/otpme/lib/token/ssh/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/ssh/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39614 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/ssh/ssh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.895501 otpme-0.3.0a63/otpme/lib/token/totp/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/totp/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35465 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/totp/totp.py
--rw-r--r--   0 root         (0) root         (0)      547 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.895501 otpme-0.3.0a63/otpme/lib/token/yubikey_hmac/
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/yubikey_hmac/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25178 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme/lib/token/yubikey_hmac/yubikey_hmac.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 11:25:55.855500 otpme-0.3.0a63/otpme.egg-info/
--rw-r--r--   0 root         (0) root         (0)      680 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13377 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1080 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      969 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-23 11:25:55.000000 otpme-0.3.0a63/otpme.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 11:25:55.895501 otpme-0.3.0a63/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8760 2024-05-23 11:25:55.000000 otpme-0.3.0a63/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.659927 otpme-0.3.0a64/
+-rw-r--r--   0 root         (0) root         (0)    35121 2024-05-23 13:27:40.000000 otpme-0.3.0a64/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      665 2024-05-23 13:27:40.000000 otpme-0.3.0a64/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      680 2024-05-23 13:27:40.659927 otpme-0.3.0a64/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3821 2024-05-23 13:27:40.000000 otpme-0.3.0a64/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.611926 otpme-0.3.0a64/bash_completion/
+-rw-r--r--   0 root         (0) root         (0)     1937 2024-05-23 13:27:40.000000 otpme-0.3.0a64/bash_completion/otpme
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.611926 otpme-0.3.0a64/deploy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.615926 otpme-0.3.0a64/deploy/dicts/
+-rw-r--r--   0 root         (0) root         (0)     2535 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/dicts/abbreviations-it.gz
+-rw-r--r--   0 root         (0) root         (0)    18683 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/dicts/at-surnames.gz
+-rw-r--r--   0 root         (0) root         (0)   197269 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/dicts/common-passwords.gz
+-rwxr-xr-x   0 root         (0) root         (0)      532 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/dicts/convert_dict.sh
+-rw-r--r--   0 root         (0) root         (0)     3286 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/dicts/de-female.gz
+-rw-r--r--   0 root         (0) root         (0)     3070 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/dicts/de-male.gz
+-rw-r--r--   0 root         (0) root         (0)    11343 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/dicts/de-surnames.gz
+-rw-r--r--   0 root         (0) root         (0)    34845 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/dicts/de-top10000.gz
+-rw-r--r--   0 root         (0) root         (0)    30600 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/dicts/en-top10000.gz
+-rw-r--r--   0 root         (0) root         (0)   127983 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/dicts/english-guessing.gz
+-rw-r--r--   0 root         (0) root         (0)  1041710 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/dicts/english.gz
+-rw-r--r--   0 root         (0) root         (0)   547291 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/dicts/german-guessing.gz
+-rw-r--r--   0 root         (0) root         (0)   544600 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/dicts/german.gz
+-rw-r--r--   0 root         (0) root         (0)    13539 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/dicts/us-female.gz
+-rw-r--r--   0 root         (0) root         (0)     4089 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/dicts/us-male.gz
+-rw-r--r--   0 root         (0) root         (0)    35682 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/dicts/us-surnames.gz
+-rw-r--r--   0 root         (0) root         (0)    13331 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/otpme.conf.dist
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.615926 otpme-0.3.0a64/deploy/pam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.615926 otpme-0.3.0a64/deploy/pam/pam-python/
+-rw-r--r--   0 root         (0) root         (0)      511 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/pam/pam-python/README
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/pam/pam_otpme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.615926 otpme-0.3.0a64/deploy/radius/
+-rw-r--r--   0 root         (0) root         (0)    13085 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/radius/dictionary
+-rw-r--r--   0 root         (0) root         (0)     3851 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/radius/dictionary.freeradius
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.619926 otpme-0.3.0a64/deploy/schema/
+-rw-r--r--   0 root         (0) root         (0)    21610 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/schema/core.schema
+-rw-r--r--   0 root         (0) root         (0)    73993 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/schema/cosine.schema
+-rw-r--r--   0 root         (0) root         (0)     6267 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/schema/inetorgperson.schema
+-rw-r--r--   0 root         (0) root         (0)     7632 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/schema/nis.schema
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.619926 otpme-0.3.0a64/deploy/scripts/
+-rw-r--r--   0 root         (0) root         (0)     8600 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/scripts/agent_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/scripts/auth_script.sh
+-rw-r--r--   0 root         (0) root         (0)    21045 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/scripts/key_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/scripts/login_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/scripts/node_vote_script.sh
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-23 13:27:40.000000 otpme-0.3.0a64/deploy/scripts/push_script.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.619926 otpme-0.3.0a64/otpme/
+-rw-r--r--   0 root         (0) root         (0)      965 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    12722 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.623926 otpme-0.3.0a64/otpme/lib/
+-rw-r--r--   0 root         (0) root         (0)    10486 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/arp.py
+-rw-r--r--   0 root         (0) root         (0)     3569 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/auth_script.py
+-rw-r--r--   0 root         (0) root         (0)    48110 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.623926 otpme-0.3.0a64/otpme/lib/backends/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/backends/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.623926 otpme-0.3.0a64/otpme/lib/backends/file/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/backends/file/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90252 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/backends/file/file.py
+-rw-r--r--   0 root         (0) root         (0)    13013 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/backends/file/index.py
+-rw-r--r--   0 root         (0) root         (0)     5898 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/backends/file/models.py
+-rw-r--r--   0 root         (0) root         (0)    67261 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/backends/file/transaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.627926 otpme-0.3.0a64/otpme/lib/cache/
+-rw-r--r--   0 root         (0) root         (0)    27634 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3226 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cache/dogpile.py
+-rw-r--r--   0 root         (0) root         (0)    19511 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cache/funccache.py
+-rw-r--r--   0 root         (0) root         (0)     3515 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cache/lru.py
+-rw-r--r--   0 root         (0) root         (0)    14416 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cache/memcache.py
+-rw-r--r--   0 root         (0) root         (0)     6500 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cache/memcached.py
+-rw-r--r--   0 root         (0) root         (0)     7344 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cache/memcachedb.py
+-rw-r--r--   0 root         (0) root         (0)    27195 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cache/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.631926 otpme-0.3.0a64/otpme/lib/classes/
+-rw-r--r--   0 root         (0) root         (0)      959 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86247 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/accessgroup.py
+-rw-r--r--   0 root         (0) root         (0)    14874 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/agent_conn.py
+-rw-r--r--   0 root         (0) root         (0)   126103 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/auth_handler.py
+-rw-r--r--   0 root         (0) root         (0)    56674 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/ca.py
+-rw-r--r--   0 root         (0) root         (0)    40808 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/client.py
+-rw-r--r--   0 root         (0) root         (0)   230568 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/command_handler.py
+-rw-r--r--   0 root         (0) root         (0)     8730 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/conn_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.631926 otpme-0.3.0a64/otpme/lib/classes/data_objects/
+-rw-r--r--   0 root         (0) root         (0)      880 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/data_objects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2386 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/data_objects/cert.py
+-rw-r--r--   0 root         (0) root         (0)     6865 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/data_objects/data_revision.py
+-rw-r--r--   0 root         (0) root         (0)     6880 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/data_objects/failed_pass.py
+-rw-r--r--   0 root         (0) root         (0)     8125 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/data_objects/last_assigned_id.py
+-rw-r--r--   0 root         (0) root         (0)    10579 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/data_objects/revoked_signature.py
+-rw-r--r--   0 root         (0) root         (0)     2570 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/data_objects/rsa_key.py
+-rw-r--r--   0 root         (0) root         (0)     7020 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/data_objects/skip_sync.py
+-rw-r--r--   0 root         (0) root         (0)     5811 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/data_objects/token_counter.py
+-rw-r--r--   0 root         (0) root         (0)     5646 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/data_objects/used_hash.py
+-rw-r--r--   0 root         (0) root         (0)     5989 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/data_objects/used_otp.py
+-rw-r--r--   0 root         (0) root         (0)     5997 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/data_objects/used_slp.py
+-rw-r--r--   0 root         (0) root         (0)     5992 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/data_objects/used_sotp.py
+-rw-r--r--   0 root         (0) root         (0)    28682 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)    39185 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/group.py
+-rw-r--r--   0 root         (0) root         (0)    52065 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/host.py
+-rw-r--r--   0 root         (0) root         (0)    12296 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/login_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/mgmt_client.py
+-rw-r--r--   0 root         (0) root         (0)    38858 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/node.py
+-rw-r--r--   0 root         (0) root         (0)    24441 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/object_config.py
+-rw-r--r--   0 root         (0) root         (0)    77129 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/otpme_agent.py
+-rw-r--r--   0 root         (0) root         (0)    49704 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/otpme_host.py
+-rw-r--r--   0 root         (0) root         (0)   318862 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/otpme_object.py
+-rw-r--r--   0 root         (0) root         (0)    23357 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/policy.py
+-rw-r--r--   0 root         (0) root         (0)    62493 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/realm.py
+-rw-r--r--   0 root         (0) root         (0)    74478 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/resolver.py
+-rw-r--r--   0 root         (0) root         (0)    45067 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/role.py
+-rw-r--r--   0 root         (0) root         (0)    34240 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/script.py
+-rw-r--r--   0 root         (0) root         (0)    52987 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/session.py
+-rw-r--r--   0 root         (0) root         (0)    31485 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/signing.py
+-rw-r--r--   0 root         (0) root         (0)   107251 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/site.py
+-rw-r--r--   0 root         (0) root         (0)     7054 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/ssh_agent.py
+-rw-r--r--   0 root         (0) root         (0)   134917 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/token.py
+-rw-r--r--   0 root         (0) root         (0)    49462 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/unit.py
+-rw-r--r--   0 root         (0) root         (0)   182238 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/classes/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.631926 otpme-0.3.0a64/otpme/lib/cli/
+-rw-r--r--   0 root         (0) root         (0)    64641 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12952 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cli/accessgroup.py
+-rw-r--r--   0 root         (0) root         (0)     7186 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cli/ca.py
+-rw-r--r--   0 root         (0) root         (0)    13309 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cli/client.py
+-rw-r--r--   0 root         (0) root         (0)     5710 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cli/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)    13060 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cli/group.py
+-rw-r--r--   0 root         (0) root         (0)    13124 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cli/host.py
+-rw-r--r--   0 root         (0) root         (0)    11041 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cli/node.py
+-rw-r--r--   0 root         (0) root         (0)     6232 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cli/policy.py
+-rw-r--r--   0 root         (0) root         (0)     6241 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cli/realm.py
+-rw-r--r--   0 root         (0) root         (0)     6667 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cli/resolver.py
+-rw-r--r--   0 root         (0) root         (0)    20315 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cli/role.py
+-rw-r--r--   0 root         (0) root         (0)     7450 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cli/script.py
+-rw-r--r--   0 root         (0) root         (0)     7591 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cli/site.py
+-rw-r--r--   0 root         (0) root         (0)    17421 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cli/token.py
+-rw-r--r--   0 root         (0) root         (0)     5490 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cli/unit.py
+-rw-r--r--   0 root         (0) root         (0)     7663 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/cli/user.py
+-rw-r--r--   0 root         (0) root         (0)    24934 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/compgen.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.631926 otpme-0.3.0a64/otpme/lib/compression/
+-rw-r--r--   0 root         (0) root         (0)      514 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/compression/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4149 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/compression/base.py
+-rw-r--r--   0 root         (0) root         (0)    14344 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/connections.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.635926 otpme-0.3.0a64/otpme/lib/daemon/
+-rw-r--r--   0 root         (0) root         (0)      685 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3852 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/daemon/authd.py
+-rw-r--r--   0 root         (0) root         (0)   109032 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/daemon/clusterd.py
+-rw-r--r--   0 root         (0) root         (0)    47618 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/daemon/controld.py
+-rw-r--r--   0 root         (0) root         (0)    76830 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/daemon/hostd.py
+-rw-r--r--   0 root         (0) root         (0)     3141 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/daemon/joind.py
+-rw-r--r--   0 root         (0) root         (0)     6780 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/daemon/ldapd.py
+-rw-r--r--   0 root         (0) root         (0)     3070 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/daemon/mgmtd.py
+-rw-r--r--   0 root         (0) root         (0)    15943 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/daemon/otpme_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    11458 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/daemon/scriptd.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/daemon/syncd.py
+-rw-r--r--   0 root         (0) root         (0)     6941 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/daemon/unix_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    19072 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/debug.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/doc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.635926 otpme-0.3.0a64/otpme/lib/encoding/
+-rw-r--r--   0 root         (0) root         (0)      496 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/encoding/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/encoding/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.635926 otpme-0.3.0a64/otpme/lib/encryption/
+-rw-r--r--   0 root         (0) root         (0)     4020 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/encryption/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/encryption/aes.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/encryption/aes_cfb.py
+-rw-r--r--   0 root         (0) root         (0)     7967 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/encryption/argon2.py
+-rw-r--r--   0 root         (0) root         (0)    10307 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/encryption/asymmetric_key_handler.py
+-rw-r--r--   0 root         (0) root         (0)     4318 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/encryption/ec.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/encryption/fernet.py
+-rw-r--r--   0 root         (0) root         (0)     3304 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/encryption/hkdf.py
+-rw-r--r--   0 root         (0) root         (0)     3794 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/encryption/pbkdf2.py
+-rw-r--r--   0 root         (0) root         (0)     7891 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/encryption/rsa.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.635926 otpme-0.3.0a64/otpme/lib/extensions/
+-rw-r--r--   0 root         (0) root         (0)      396 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/extensions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.635926 otpme-0.3.0a64/otpme/lib/extensions/base/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/extensions/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12345 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/extensions/base/base.py
+-rw-r--r--   0 root         (0) root         (0)    40219 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/extensions/ldif_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.635926 otpme-0.3.0a64/otpme/lib/extensions/posix/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/extensions/posix/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14353 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/extensions/posix/posix.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/extensions/utils.py
+-rw-r--r--   0 root         (0) root         (0)    34148 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/filetools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.635926 otpme-0.3.0a64/otpme/lib/freeradius/
+-rw-r--r--   0 root         (0) root         (0)     9186 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/freeradius/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18752 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/freeradius/otpme.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/freeradius/radiusd.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/freeradius/radiusd_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.635926 otpme-0.3.0a64/otpme/lib/gpg/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/gpg/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    28565 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/gpg/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.639927 otpme-0.3.0a64/otpme/lib/help/
+-rwxr-xr-x   0 root         (0) root         (0)    26596 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23053 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/accessgroup.py
+-rw-r--r--   0 root         (0) root         (0)     5552 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/agent.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/auth.py
+-rw-r--r--   0 root         (0) root         (0)    15774 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/ca.py
+-rw-r--r--   0 root         (0) root         (0)    16991 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/client.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5852 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/controld.py
+-rw-r--r--   0 root         (0) root         (0)    11455 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/dictionary.py
+-rw-r--r--   0 root         (0) root         (0)      589 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/get_authorized_keys.py
+-rw-r--r--   0 root         (0) root         (0)    19939 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/group.py
+-rw-r--r--   0 root         (0) root         (0)    24503 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/host.py
+-rw-r--r--   0 root         (0) root         (0)    21376 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/node.py
+-rw-r--r--   0 root         (0) root         (0)      544 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/pinentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.639927 otpme-0.3.0a64/otpme/lib/help/policy/
+-rw-r--r--   0 root         (0) root         (0)     8806 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/policy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3777 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/policy/authonaction.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/policy/autodisable.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/policy/defaultgroups.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/policy/defaultpolicies.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/policy/defaultroles.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/policy/defaultunits.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/policy/forcetoken.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/policy/idrange.py
+-rw-r--r--   0 root         (0) root         (0)     3292 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/policy/logintimes.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/policy/objecttemplates.py
+-rw-r--r--   0 root         (0) root         (0)     2985 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/policy/password.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/policy/tokenacls.py
+-rw-r--r--   0 root         (0) root         (0)    20104 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/realm.py
+-rw-r--r--   0 root         (0) root         (0)     1508 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/register.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.639927 otpme-0.3.0a64/otpme/lib/help/resolver/
+-rw-r--r--   0 root         (0) root         (0)    12589 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4532 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/resolver/ldap.py
+-rw-r--r--   0 root         (0) root         (0)    18265 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/role.py
+-rw-r--r--   0 root         (0) root         (0)    15178 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/script.py
+-rw-r--r--   0 root         (0) root         (0)     2911 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/session.py
+-rw-r--r--   0 root         (0) root         (0)    22555 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.643926 otpme-0.3.0a64/otpme/lib/help/token/
+-rw-r--r--   0 root         (0) root         (0)    20570 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/token/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/token/fido2.py
+-rw-r--r--   0 root         (0) root         (0)     5686 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/token/hotp.py
+-rw-r--r--   0 root         (0) root         (0)     6406 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/token/motp.py
+-rw-r--r--   0 root         (0) root         (0)     2058 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/token/otp_push.py
+-rw-r--r--   0 root         (0) root         (0)     5018 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/token/otpme.py
+-rw-r--r--   0 root         (0) root         (0)     3947 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/token/password.py
+-rw-r--r--   0 root         (0) root         (0)     7318 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/token/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/token/totp.py
+-rw-r--r--   0 root         (0) root         (0)     5870 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/token/yubikey_hmac.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/token/yubikey_hotp.py
+-rw-r--r--   0 root         (0) root         (0)    25002 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/tool.py
+-rw-r--r--   0 root         (0) root         (0)    15235 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/unit.py
+-rw-r--r--   0 root         (0) root         (0)    29476 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/help/user.py
+-rw-r--r--   0 root         (0) root         (0)    16408 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/host.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.643926 otpme-0.3.0a64/otpme/lib/humanize/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/humanize/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4258 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/humanize/units.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.643926 otpme-0.3.0a64/otpme/lib/index/
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24015 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/index/mysql.py
+-rw-r--r--   0 root         (0) root         (0)    24609 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/index/postgres.py
+-rw-r--r--   0 root         (0) root         (0)     8403 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/index/sqlite3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.643926 otpme-0.3.0a64/otpme/lib/job/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20748 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/job/callback.py
+-rw-r--r--   0 root         (0) root         (0)    12916 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/job/otpme_job.py
+-rw-r--r--   0 root         (0) root         (0)    37164 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/join.py
+-rw-r--r--   0 root         (0) root         (0)     4924 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/json.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/jwt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.643926 otpme-0.3.0a64/otpme/lib/ldap/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/ldap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/ldap/client.py
+-rw-r--r--   0 root         (0) root         (0)    11129 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/ldap/schema.py
+-rw-r--r--   0 root         (0) root         (0)    50550 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/ldap/server.py
+-rw-r--r--   0 root         (0) root         (0)    19776 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/locking.py
+-rw-r--r--   0 root         (0) root         (0)     9497 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/log.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/messages.py
+-rw-r--r--   0 root         (0) root         (0)     6048 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/mschap.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/mschap_util.py
+-rw-r--r--   0 root         (0) root         (0)    35811 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/multiprocessing.py
+-rw-r--r--   0 root         (0) root         (0)    10317 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/net.py
+-rw-r--r--   0 root         (0) root         (0)    27211 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/nsscache.py
+-rw-r--r--   0 root         (0) root         (0)    63395 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/offline_token.py
+-rw-r--r--   0 root         (0) root         (0)    23845 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/oid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.643926 otpme-0.3.0a64/otpme/lib/otp/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/otp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.643926 otpme-0.3.0a64/otpme/lib/otp/oath/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/otp/oath/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/otp/oath/hotp.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/otp/oath/totp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.643926 otpme-0.3.0a64/otpme/lib/otp/otpme/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/otp/otpme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3154 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/otp/otpme/otpme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.643926 otpme-0.3.0a64/otpme/lib/otp/yubico/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/otp/yubico/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/otp/yubico/yubiotp.py
+-rw-r--r--   0 root         (0) root         (0)    19904 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/otpme_acl.py
+-rw-r--r--   0 root         (0) root         (0)   115839 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/otpme_config.py
+-rw-r--r--   0 root         (0) root         (0)     3586 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/otpme_pass.py
+-rw-r--r--   0 root         (0) root         (0)    70426 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/pam.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/pickle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.643926 otpme-0.3.0a64/otpme/lib/pinentry/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/pinentry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27532 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/pinentry/pinentry.py
+-rwxr-xr-x   0 root         (0) root         (0)     7947 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/pinentry/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.643926 otpme-0.3.0a64/otpme/lib/pki/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/pki/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9864 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/pki/cert.py
+-rw-r--r--   0 root         (0) root         (0)    23217 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/pki/utils.py
+-rw-r--r--   0 root         (0) root         (0)    16957 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/pki/utils_openssl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.643926 otpme-0.3.0a64/otpme/lib/policy/
+-rw-r--r--   0 root         (0) root         (0)     2166 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.647927 otpme-0.3.0a64/otpme/lib/policy/authonaction/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/authonaction/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32730 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/authonaction/authonaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.647927 otpme-0.3.0a64/otpme/lib/policy/autodisable/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/autodisable/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15785 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/autodisable/autodisable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.647927 otpme-0.3.0a64/otpme/lib/policy/defaultgroups/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/defaultgroups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17637 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/defaultgroups/defaultgroups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.647927 otpme-0.3.0a64/otpme/lib/policy/defaultpolicies/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/defaultpolicies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14577 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/defaultpolicies/defaultpolicies.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.647927 otpme-0.3.0a64/otpme/lib/policy/defaultroles/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/defaultroles/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/defaultroles/defaultroles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.647927 otpme-0.3.0a64/otpme/lib/policy/defaultunits/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/defaultunits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15704 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/defaultunits/defaultunits.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.647927 otpme-0.3.0a64/otpme/lib/policy/forcetoken/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/forcetoken/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14269 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/forcetoken/forcetoken.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/get_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.647927 otpme-0.3.0a64/otpme/lib/policy/idrange/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/idrange/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27323 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/idrange/idrange.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.647927 otpme-0.3.0a64/otpme/lib/policy/logintimes/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/logintimes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23084 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/logintimes/logintimes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.647927 otpme-0.3.0a64/otpme/lib/policy/objecttemplates/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/objecttemplates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15021 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/objecttemplates/objecttemplates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.647927 otpme-0.3.0a64/otpme/lib/policy/password/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/password/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29048 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/password/password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.647927 otpme-0.3.0a64/otpme/lib/policy/tokenacls/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/tokenacls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24964 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/tokenacls/tokenacls.py
+-rw-r--r--   0 root         (0) root         (0)      558 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/policy/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9399 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/preload.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/progress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.647927 otpme-0.3.0a64/otpme/lib/protocols/
+-rw-r--r--   0 root         (0) root         (0)      371 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.651927 otpme-0.3.0a64/otpme/lib/protocols/client/
+-rw-r--r--   0 root         (0) root         (0)      722 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/client/agent1.py
+-rw-r--r--   0 root         (0) root         (0)      899 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/client/auth1.py
+-rw-r--r--   0 root         (0) root         (0)    14368 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/client/cluster1.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/client/get_class.py
+-rw-r--r--   0 root         (0) root         (0)     4712 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/client/host1.py
+-rw-r--r--   0 root         (0) root         (0)      899 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/client/join1.py
+-rwxr-xr-x   0 root         (0) root         (0)    11372 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/client/mgmt1.py
+-rw-r--r--   0 root         (0) root         (0)    68042 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/client/sync1.py
+-rw-r--r--   0 root         (0) root         (0)   160760 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/otpme_client.py
+-rw-r--r--   0 root         (0) root         (0)    81487 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/otpme_server.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/request.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.651927 otpme-0.3.0a64/otpme/lib/protocols/server/
+-rw-r--r--   0 root         (0) root         (0)      894 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40286 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/server/agent1.py
+-rw-r--r--   0 root         (0) root         (0)    12909 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/server/auth1.py
+-rw-r--r--   0 root         (0) root         (0)    32369 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/server/cluster1.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/server/get_class.py
+-rw-r--r--   0 root         (0) root         (0)    26675 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/server/host1.py
+-rw-r--r--   0 root         (0) root         (0)    52629 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/server/join1.py
+-rw-r--r--   0 root         (0) root         (0)    70933 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/server/mgmt1.py
+-rw-r--r--   0 root         (0) root         (0)    45500 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/server/sync1.py
+-rw-r--r--   0 root         (0) root         (0)      594 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/status_codes.py
+-rw-r--r--   0 root         (0) root         (0)     7004 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/protocols/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/push_script.py
+-rw-r--r--   0 root         (0) root         (0)     1206 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/qrcode.py
+-rw-r--r--   0 root         (0) root         (0)      545 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/re.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.651927 otpme-0.3.0a64/otpme/lib/register/
+-rw-r--r--   0 root         (0) root         (0)     9783 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/register/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.651927 otpme-0.3.0a64/otpme/lib/resolver/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/resolver/get_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.651927 otpme-0.3.0a64/otpme/lib/resolver/ldap/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/resolver/ldap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39505 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/resolver/ldap/ldap.py
+-rw-r--r--   0 root         (0) root         (0)      518 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/resolver/utils.py
+-rw-r--r--   0 root         (0) root         (0)    10086 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/script.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/sign_key_cache.py
+-rw-r--r--   0 root         (0) root         (0)      604 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/slp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.651927 otpme-0.3.0a64/otpme/lib/smartcard/
+-rw-r--r--   0 root         (0) root         (0)      690 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/smartcard/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.651927 otpme-0.3.0a64/otpme/lib/smartcard/fido2/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/smartcard/fido2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10228 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/smartcard/fido2/fido2.py
+-rw-r--r--   0 root         (0) root         (0)      925 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/smartcard/get_class.py
+-rw-r--r--   0 root         (0) root         (0)     1733 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/smartcard/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.651927 otpme-0.3.0a64/otpme/lib/smartcard/yubikey/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/smartcard/yubikey/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12018 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/smartcard/yubikey/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/smartcard/yubikey/usb.py
+-rw-r--r--   0 root         (0) root         (0)     8142 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/smartcard/yubikey/yubikey.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.651927 otpme-0.3.0a64/otpme/lib/smartcard/yubikey_gpg/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/smartcard/yubikey_gpg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6431 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.651927 otpme-0.3.0a64/otpme/lib/smartcard/yubikey_hmac/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/smartcard/yubikey_hmac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12022 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.651927 otpme-0.3.0a64/otpme/lib/smartcard/yubikey_hotp/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/smartcard/yubikey_hotp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.651927 otpme-0.3.0a64/otpme/lib/socket/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/socket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13219 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/socket/connect.py
+-rw-r--r--   0 root         (0) root         (0)     8517 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/socket/handler.py
+-rw-r--r--   0 root         (0) root         (0)    31029 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/socket/listen.py
+-rw-r--r--   0 root         (0) root         (0)     2897 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/socket/send_recv1.py
+-rw-r--r--   0 root         (0) root         (0)     4475 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/sotp.py
+-rwxr-xr-x   0 root         (0) root         (0)    37180 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/spsc.py
+-rw-r--r--   0 root         (0) root         (0)      611 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/srp.py
+-rw-r--r--   0 root         (0) root         (0)    23521 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/ssh.py
+-rw-r--r--   0 root         (0) root         (0)    63740 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/stuff.py
+-rw-r--r--   0 root         (0) root         (0)    12405 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/sync_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4703 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/system_command.py
+-rw-r--r--   0 root         (0) root         (0)     5703 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.655927 otpme-0.3.0a64/otpme/lib/third_party/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.655927 otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/
+-rw-r--r--   0 root         (0) root         (0)     1981 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/advanced.py
+-rw-r--r--   0 root         (0) root         (0)     9859 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/caching_query.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/environment.py
+-rw-r--r--   0 root         (0) root         (0)     1764 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/fixture_data.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/helloworld.py
+-rw-r--r--   0 root         (0) root         (0)     3310 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/local_session_caching.py
+-rw-r--r--   0 root         (0) root         (0)     3033 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/model.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/relationship_caching.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.655927 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/
+-rw-r--r--   0 root         (0) root         (0)     1140 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.655927 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/caches/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/caches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9083 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/caches/caches.py
+-rw-r--r--   0 root         (0) root         (0)    14341 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/caches/files.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/config.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/error.py
+-rw-r--r--   0 root         (0) root         (0)     7963 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.655927 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/maps/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/maps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/maps/group.py
+-rw-r--r--   0 root         (0) root         (0)    11745 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/maps/maps.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/maps/passwd.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/maps/shadow.py
+-rw-r--r--   0 root         (0) root         (0)     4140 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/nss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.655927 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/update/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/update/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5487 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/update/files_updater.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/update/map_updater.py
+-rw-r--r--   0 root         (0) root         (0)    10980 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/update/updater.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.655927 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4117 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/nss_cache/util/file_formats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.655927 otpme-0.3.0a64/otpme/lib/third_party/oath_toolkit/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/oath_toolkit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/oath_toolkit/_compat.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/third_party/oath_toolkit/uri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.655927 otpme-0.3.0a64/otpme/lib/token/
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.655927 otpme-0.3.0a64/otpme/lib/token/fido2/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/fido2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15006 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/fido2/fido2.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/get_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.655927 otpme-0.3.0a64/otpme/lib/token/hotp/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/hotp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39413 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/hotp/hotp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.655927 otpme-0.3.0a64/otpme/lib/token/link/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/link/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9723 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/link/link.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.659927 otpme-0.3.0a64/otpme/lib/token/motp/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/motp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27837 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/motp/motp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.659927 otpme-0.3.0a64/otpme/lib/token/oath/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/oath/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19688 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/oath/oath.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.659927 otpme-0.3.0a64/otpme/lib/token/otp_push/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/otp_push/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23460 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/otp_push/otp_push.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.659927 otpme-0.3.0a64/otpme/lib/token/otpme/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/otpme/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24771 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/otpme/otpme.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.659927 otpme-0.3.0a64/otpme/lib/token/password/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/password/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26135 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/password/password.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.659927 otpme-0.3.0a64/otpme/lib/token/script_otp/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/script_otp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9744 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/script_otp/script_otp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.659927 otpme-0.3.0a64/otpme/lib/token/script_static/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/script_static/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9744 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/script_static/script_static.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.659927 otpme-0.3.0a64/otpme/lib/token/ssh/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/ssh/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39614 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/ssh/ssh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.659927 otpme-0.3.0a64/otpme/lib/token/totp/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/totp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35465 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/totp/totp.py
+-rw-r--r--   0 root         (0) root         (0)      547 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.659927 otpme-0.3.0a64/otpme/lib/token/yubikey_hmac/
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/yubikey_hmac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25178 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme/lib/token/yubikey_hmac/yubikey_hmac.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:27:40.619926 otpme-0.3.0a64/otpme.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      680 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13377 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      973 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-23 13:27:40.000000 otpme-0.3.0a64/otpme.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 13:27:40.659927 otpme-0.3.0a64/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8833 2024-05-23 13:27:40.000000 otpme-0.3.0a64/setup.py
```

### Comparing `otpme-0.3.0a63/LICENSE` & `otpme-0.3.0a64/LICENSE`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/MANIFEST.in` & `otpme-0.3.0a64/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/PKG-INFO` & `otpme-0.3.0a64/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otpme
-Version: 0.3.0a63
+Version: 0.3.0a64
 Summary: OTPme: A flexible One-Time-Password system.
 Home-page: http://www.otpme.org
 Author: the2nd
 Author-email: the2nd@otpme.org
 Maintainer: the2nd
 Maintainer-email: the2nd@otpme.org
 License: GPLv2
```

### Comparing `otpme-0.3.0a63/README` & `otpme-0.3.0a64/README`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/bash_completion/otpme` & `otpme-0.3.0a64/bash_completion/otpme`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/dicts/abbreviations-it.gz` & `otpme-0.3.0a64/deploy/dicts/abbreviations-it.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/dicts/at-surnames.gz` & `otpme-0.3.0a64/deploy/dicts/at-surnames.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/dicts/common-passwords.gz` & `otpme-0.3.0a64/deploy/dicts/common-passwords.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/dicts/convert_dict.sh` & `otpme-0.3.0a64/deploy/dicts/convert_dict.sh`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/dicts/de-female.gz` & `otpme-0.3.0a64/deploy/dicts/de-female.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/dicts/de-male.gz` & `otpme-0.3.0a64/deploy/dicts/de-male.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/dicts/de-surnames.gz` & `otpme-0.3.0a64/deploy/dicts/de-surnames.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/dicts/de-top10000.gz` & `otpme-0.3.0a64/deploy/dicts/de-top10000.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/dicts/en-top10000.gz` & `otpme-0.3.0a64/deploy/dicts/en-top10000.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/dicts/english-guessing.gz` & `otpme-0.3.0a64/deploy/dicts/english-guessing.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/dicts/english.gz` & `otpme-0.3.0a64/deploy/dicts/english.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/dicts/german-guessing.gz` & `otpme-0.3.0a64/deploy/dicts/german-guessing.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/dicts/german.gz` & `otpme-0.3.0a64/deploy/dicts/german.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/dicts/us-female.gz` & `otpme-0.3.0a64/deploy/dicts/us-female.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/dicts/us-male.gz` & `otpme-0.3.0a64/deploy/dicts/us-male.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/dicts/us-surnames.gz` & `otpme-0.3.0a64/deploy/dicts/us-surnames.gz`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/otpme.conf.dist` & `otpme-0.3.0a64/deploy/otpme.conf.dist`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/pam/pam_otpme.py` & `otpme-0.3.0a64/deploy/pam/pam_otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/radius/dictionary` & `otpme-0.3.0a64/deploy/radius/dictionary`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/radius/dictionary.freeradius` & `otpme-0.3.0a64/deploy/radius/dictionary.freeradius`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/schema/core.schema` & `otpme-0.3.0a64/deploy/schema/core.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/schema/cosine.schema` & `otpme-0.3.0a64/deploy/schema/cosine.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/schema/inetorgperson.schema` & `otpme-0.3.0a64/deploy/schema/inetorgperson.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/schema/nis.schema` & `otpme-0.3.0a64/deploy/schema/nis.schema`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/scripts/agent_script.sh` & `otpme-0.3.0a64/deploy/scripts/agent_script.sh`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/deploy/scripts/key_script.sh` & `otpme-0.3.0a64/deploy/scripts/key_script.sh`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/__init__.py` & `otpme-0.3.0a64/otpme/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 __project_url__ = "http://www.otpme.org"
 __copyright__ = "Copyright 2014-2024 the2nd <the2nd@otpme.org>"
 __project_description__ = "OTPme: A flexible One-Time-Password system."
 __author__ = "the2nd"
 __email__ = "the2nd@otpme.org"
 __credits__ = []
 __license__ = "GPLv2"
-__version__ = "0.3.0a63"
+__version__ = "0.3.0a64"
 __status__ = "Development Status :: 3 - Alpha"
 # In future versions :D
 #__status__ = "Development Status :: 4 - Beta"
 #__status__ = "Development Status :: 5 - Production/Stable"
 __pkg_name__ = __project_name__
 __maintainer__ = __author__
 __author_email__  = __email__
```

### Comparing `otpme-0.3.0a63/otpme/command.py` & `otpme-0.3.0a64/otpme/command.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/__init__.py` & `otpme-0.3.0a64/otpme/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/arp.py` & `otpme-0.3.0a64/otpme/lib/arp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/auth_script.py` & `otpme-0.3.0a64/otpme/lib/auth_script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/backend.py` & `otpme-0.3.0a64/otpme/lib/backend.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/backends/file/file.py` & `otpme-0.3.0a64/otpme/lib/backends/file/file.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/backends/file/index.py` & `otpme-0.3.0a64/otpme/lib/backends/file/index.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/backends/file/models.py` & `otpme-0.3.0a64/otpme/lib/backends/file/models.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/backends/file/transaction.py` & `otpme-0.3.0a64/otpme/lib/backends/file/transaction.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cache/__init__.py` & `otpme-0.3.0a64/otpme/lib/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cache/dogpile.py` & `otpme-0.3.0a64/otpme/lib/cache/dogpile.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cache/funccache.py` & `otpme-0.3.0a64/otpme/lib/cache/funccache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cache/lru.py` & `otpme-0.3.0a64/otpme/lib/cache/lru.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cache/memcache.py` & `otpme-0.3.0a64/otpme/lib/cache/memcache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cache/memcached.py` & `otpme-0.3.0a64/otpme/lib/cache/memcached.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cache/memcachedb.py` & `otpme-0.3.0a64/otpme/lib/cache/memcachedb.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cache/redis.py` & `otpme-0.3.0a64/otpme/lib/cache/redis.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/__init__.py` & `otpme-0.3.0a64/otpme/lib/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/accessgroup.py` & `otpme-0.3.0a64/otpme/lib/classes/accessgroup.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/agent_conn.py` & `otpme-0.3.0a64/otpme/lib/classes/agent_conn.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/auth_handler.py` & `otpme-0.3.0a64/otpme/lib/classes/auth_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,17 +504,19 @@
             processed_sessions.append(session_uuid)
             # Get session instance.
             session_id = user_sessions[session_uuid]['session_id'][0]
             session = backend.get_object(object_type="session",
                                         uuid=session_uuid)
             if not session:
                 continue
-            # Check if session exists (e.g. expired sessions get removed when
-            # they are loaded).
-            if not session.exists(outdate=True):
+            # Outdate expired session.
+            try:
+                if not session.exists(outdate=True):
+                    continue
+            except LockWaitAbort:
                 continue
 
             ## We can only verify sessions that match the requests auth type.
             #if self.auth_type != session.session_type:
             #    self.logger.debug("Ignoring %s session for %s request."
             #                % (session.session_type, self.auth_type))
             #    continue
@@ -594,18 +596,22 @@
         # Get sessions for this user.
         user_sessions = backend.get_sessions(user=self.user.uuid,
                                 access_group=self.auth_group.uuid)
         for session_uuid in user_sessions:
             # Get session instance.
             session = backend.get_object(object_type="session",
                                         uuid=session_uuid)
-            # Check if session exists (e.g. expired sessions get removed when
-            # they are loaded).
             if not session:
                 continue
+            # Outdate sessions.
+            try:
+                if not session.exists(outdate=True):
+                    continue
+            except LockWaitAbort:
+                continue
             # Try to verify session.
             verify_reply = session.verify(password=slp,
                                         check_auth=False,
                                         check_srp=False,
                                         do_reneg=False,
                                         check_sotp=False,
                                         check_slp=True)
@@ -1701,17 +1707,22 @@
                                 access_group=self.auth_group.uuid)
         # Walk through session list.
         session_list = []
         for session_uuid in user_sessions:
             # Get session instance for already existing session.
             session_x = backend.get_object(object_type="session",
                                             uuid=session_uuid)
-            # Skip outdated sessions.
             if not session_x:
                 continue
+            # Outdate sessions.
+            try:
+                if not session_x.exists(outdate=True):
+                    continue
+            except LockWaitAbort:
+                continue
             session_list.append(session_x)
 
         # List that will hold all user session instances.
         # Check if we would (+1) reach max_sessions when adding this session.
         if (len(session_list) + 1) <= self.auth_group.max_sessions:
             return
```

### Comparing `otpme-0.3.0a63/otpme/lib/classes/ca.py` & `otpme-0.3.0a64/otpme/lib/classes/ca.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/client.py` & `otpme-0.3.0a64/otpme/lib/classes/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/command_handler.py` & `otpme-0.3.0a64/otpme/lib/classes/command_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/conn_handler.py` & `otpme-0.3.0a64/otpme/lib/classes/conn_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/data_objects/__init__.py` & `otpme-0.3.0a64/otpme/lib/classes/data_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/data_objects/cert.py` & `otpme-0.3.0a64/otpme/lib/classes/data_objects/cert.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/data_objects/data_revision.py` & `otpme-0.3.0a64/otpme/lib/classes/data_objects/data_revision.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/data_objects/failed_pass.py` & `otpme-0.3.0a64/otpme/lib/classes/data_objects/failed_pass.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/data_objects/last_assigned_id.py` & `otpme-0.3.0a64/otpme/lib/classes/data_objects/last_assigned_id.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/data_objects/revoked_signature.py` & `otpme-0.3.0a64/otpme/lib/classes/data_objects/revoked_signature.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/data_objects/rsa_key.py` & `otpme-0.3.0a64/otpme/lib/classes/data_objects/rsa_key.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/data_objects/skip_sync.py` & `otpme-0.3.0a64/otpme/lib/classes/data_objects/skip_sync.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/data_objects/token_counter.py` & `otpme-0.3.0a64/otpme/lib/classes/data_objects/token_counter.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/data_objects/used_hash.py` & `otpme-0.3.0a64/otpme/lib/classes/data_objects/used_hash.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/data_objects/used_otp.py` & `otpme-0.3.0a64/otpme/lib/classes/data_objects/used_otp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/data_objects/used_slp.py` & `otpme-0.3.0a64/otpme/lib/classes/data_objects/used_slp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/data_objects/used_sotp.py` & `otpme-0.3.0a64/otpme/lib/classes/data_objects/used_sotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/dictionary.py` & `otpme-0.3.0a64/otpme/lib/classes/dictionary.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/group.py` & `otpme-0.3.0a64/otpme/lib/classes/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/host.py` & `otpme-0.3.0a64/otpme/lib/classes/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/login_handler.py` & `otpme-0.3.0a64/otpme/lib/classes/login_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/mgmt_client.py` & `otpme-0.3.0a64/otpme/lib/classes/mgmt_client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/node.py` & `otpme-0.3.0a64/otpme/lib/classes/node.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/object_config.py` & `otpme-0.3.0a64/otpme/lib/classes/object_config.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/otpme_agent.py` & `otpme-0.3.0a64/otpme/lib/classes/otpme_agent.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/otpme_host.py` & `otpme-0.3.0a64/otpme/lib/classes/otpme_host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/otpme_object.py` & `otpme-0.3.0a64/otpme/lib/classes/otpme_object.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/policy.py` & `otpme-0.3.0a64/otpme/lib/classes/policy.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/realm.py` & `otpme-0.3.0a64/otpme/lib/classes/realm.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/resolver.py` & `otpme-0.3.0a64/otpme/lib/classes/resolver.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/role.py` & `otpme-0.3.0a64/otpme/lib/classes/role.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/script.py` & `otpme-0.3.0a64/otpme/lib/classes/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/session.py` & `otpme-0.3.0a64/otpme/lib/classes/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1267,13 +1267,15 @@
                 session = child_sessions[s]
                 session.delete(recursive=recursive,
                                 force=True,
                                 verify_acls=verify_acls)
 
         try:
             backend.delete_object(self.oid, cluster=True)
+        except UnknownObject:
+            pass
         except Exception as e:
             config.raise_exception()
             msg = (_("Error removing session '%s': %s") % (self.name, e))
             return callback.error(msg)
 
         return callback.ok()
```

### Comparing `otpme-0.3.0a63/otpme/lib/classes/signing.py` & `otpme-0.3.0a64/otpme/lib/classes/signing.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/site.py` & `otpme-0.3.0a64/otpme/lib/classes/site.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/ssh_agent.py` & `otpme-0.3.0a64/otpme/lib/classes/ssh_agent.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/token.py` & `otpme-0.3.0a64/otpme/lib/classes/token.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/unit.py` & `otpme-0.3.0a64/otpme/lib/classes/unit.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/classes/user.py` & `otpme-0.3.0a64/otpme/lib/classes/user.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cli/__init__.py` & `otpme-0.3.0a64/otpme/lib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cli/accessgroup.py` & `otpme-0.3.0a64/otpme/lib/cli/accessgroup.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cli/ca.py` & `otpme-0.3.0a64/otpme/lib/cli/ca.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cli/client.py` & `otpme-0.3.0a64/otpme/lib/cli/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cli/dictionary.py` & `otpme-0.3.0a64/otpme/lib/cli/dictionary.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cli/group.py` & `otpme-0.3.0a64/otpme/lib/cli/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cli/host.py` & `otpme-0.3.0a64/otpme/lib/cli/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cli/node.py` & `otpme-0.3.0a64/otpme/lib/cli/node.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cli/policy.py` & `otpme-0.3.0a64/otpme/lib/cli/policy.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cli/realm.py` & `otpme-0.3.0a64/otpme/lib/cli/realm.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cli/resolver.py` & `otpme-0.3.0a64/otpme/lib/cli/resolver.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cli/role.py` & `otpme-0.3.0a64/otpme/lib/cli/role.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cli/script.py` & `otpme-0.3.0a64/otpme/lib/cli/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cli/site.py` & `otpme-0.3.0a64/otpme/lib/cli/site.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cli/token.py` & `otpme-0.3.0a64/otpme/lib/cli/token.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cli/unit.py` & `otpme-0.3.0a64/otpme/lib/cli/unit.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/cli/user.py` & `otpme-0.3.0a64/otpme/lib/cli/user.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/compgen.py` & `otpme-0.3.0a64/otpme/lib/compgen.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/compression/__init__.py` & `otpme-0.3.0a64/otpme/lib/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/compression/base.py` & `otpme-0.3.0a64/otpme/lib/compression/base.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/connections.py` & `otpme-0.3.0a64/otpme/lib/connections.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/daemon/__init__.py` & `otpme-0.3.0a64/otpme/lib/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/daemon/authd.py` & `otpme-0.3.0a64/otpme/lib/daemon/authd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/daemon/clusterd.py` & `otpme-0.3.0a64/otpme/lib/daemon/clusterd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/daemon/controld.py` & `otpme-0.3.0a64/otpme/lib/daemon/controld.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/daemon/hostd.py` & `otpme-0.3.0a64/otpme/lib/daemon/hostd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/daemon/joind.py` & `otpme-0.3.0a64/otpme/lib/daemon/joind.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/daemon/ldapd.py` & `otpme-0.3.0a64/otpme/lib/daemon/ldapd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/daemon/mgmtd.py` & `otpme-0.3.0a64/otpme/lib/daemon/mgmtd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/daemon/otpme_daemon.py` & `otpme-0.3.0a64/otpme/lib/daemon/otpme_daemon.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/daemon/scriptd.py` & `otpme-0.3.0a64/otpme/lib/daemon/scriptd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/daemon/syncd.py` & `otpme-0.3.0a64/otpme/lib/daemon/syncd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/daemon/unix_daemon.py` & `otpme-0.3.0a64/otpme/lib/daemon/unix_daemon.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/debug.py` & `otpme-0.3.0a64/otpme/lib/debug.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/doc.py` & `otpme-0.3.0a64/otpme/lib/doc.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/encoding/base.py` & `otpme-0.3.0a64/otpme/lib/encoding/base.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/encryption/__init__.py` & `otpme-0.3.0a64/otpme/lib/encryption/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/encryption/aes.py` & `otpme-0.3.0a64/otpme/lib/encryption/aes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/encryption/aes_cfb.py` & `otpme-0.3.0a64/otpme/lib/encryption/aes_cfb.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/encryption/argon2.py` & `otpme-0.3.0a64/otpme/lib/encryption/argon2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/encryption/asymmetric_key_handler.py` & `otpme-0.3.0a64/otpme/lib/encryption/asymmetric_key_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/encryption/ec.py` & `otpme-0.3.0a64/otpme/lib/encryption/ec.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/encryption/fernet.py` & `otpme-0.3.0a64/otpme/lib/encryption/fernet.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/encryption/hkdf.py` & `otpme-0.3.0a64/otpme/lib/encryption/hkdf.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/encryption/pbkdf2.py` & `otpme-0.3.0a64/otpme/lib/encryption/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/encryption/rsa.py` & `otpme-0.3.0a64/otpme/lib/encryption/rsa.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/exceptions.py` & `otpme-0.3.0a64/otpme/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/extensions/base/base.py` & `otpme-0.3.0a64/otpme/lib/extensions/base/base.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/extensions/ldif_handler.py` & `otpme-0.3.0a64/otpme/lib/extensions/ldif_handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/extensions/posix/posix.py` & `otpme-0.3.0a64/otpme/lib/extensions/posix/posix.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/extensions/utils.py` & `otpme-0.3.0a64/otpme/lib/extensions/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/filetools.py` & `otpme-0.3.0a64/otpme/lib/filetools.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/freeradius/__init__.py` & `otpme-0.3.0a64/otpme/lib/freeradius/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/freeradius/otpme.py` & `otpme-0.3.0a64/otpme/lib/freeradius/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/freeradius/radiusd.py` & `otpme-0.3.0a64/otpme/lib/freeradius/radiusd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/freeradius/radiusd_test.py` & `otpme-0.3.0a64/otpme/lib/freeradius/radiusd_test.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/gpg/utils.py` & `otpme-0.3.0a64/otpme/lib/gpg/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/__init__.py` & `otpme-0.3.0a64/otpme/lib/help/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/accessgroup.py` & `otpme-0.3.0a64/otpme/lib/help/accessgroup.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/agent.py` & `otpme-0.3.0a64/otpme/lib/help/agent.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/auth.py` & `otpme-0.3.0a64/otpme/lib/help/auth.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/ca.py` & `otpme-0.3.0a64/otpme/lib/help/ca.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/client.py` & `otpme-0.3.0a64/otpme/lib/help/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/cluster.py` & `otpme-0.3.0a64/otpme/lib/help/cluster.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/controld.py` & `otpme-0.3.0a64/otpme/lib/help/controld.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/dictionary.py` & `otpme-0.3.0a64/otpme/lib/help/dictionary.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/get_authorized_keys.py` & `otpme-0.3.0a64/otpme/lib/help/get_authorized_keys.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/group.py` & `otpme-0.3.0a64/otpme/lib/help/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/host.py` & `otpme-0.3.0a64/otpme/lib/help/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/node.py` & `otpme-0.3.0a64/otpme/lib/help/node.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/pinentry.py` & `otpme-0.3.0a64/otpme/lib/help/pinentry.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/policy/__init__.py` & `otpme-0.3.0a64/otpme/lib/help/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/policy/authonaction.py` & `otpme-0.3.0a64/otpme/lib/help/policy/authonaction.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/policy/autodisable.py` & `otpme-0.3.0a64/otpme/lib/help/policy/autodisable.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/policy/defaultgroups.py` & `otpme-0.3.0a64/otpme/lib/help/policy/defaultgroups.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/policy/defaultpolicies.py` & `otpme-0.3.0a64/otpme/lib/help/policy/defaultpolicies.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/policy/defaultroles.py` & `otpme-0.3.0a64/otpme/lib/help/policy/defaultroles.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/policy/defaultunits.py` & `otpme-0.3.0a64/otpme/lib/help/policy/defaultunits.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/policy/forcetoken.py` & `otpme-0.3.0a64/otpme/lib/help/policy/forcetoken.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/policy/idrange.py` & `otpme-0.3.0a64/otpme/lib/help/policy/idrange.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/policy/logintimes.py` & `otpme-0.3.0a64/otpme/lib/help/policy/logintimes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/policy/objecttemplates.py` & `otpme-0.3.0a64/otpme/lib/help/policy/objecttemplates.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/policy/password.py` & `otpme-0.3.0a64/otpme/lib/help/policy/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/policy/tokenacls.py` & `otpme-0.3.0a64/otpme/lib/help/policy/tokenacls.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/realm.py` & `otpme-0.3.0a64/otpme/lib/help/realm.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/register.py` & `otpme-0.3.0a64/otpme/lib/help/register.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/resolver/__init__.py` & `otpme-0.3.0a64/otpme/lib/help/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/resolver/ldap.py` & `otpme-0.3.0a64/otpme/lib/help/resolver/ldap.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/role.py` & `otpme-0.3.0a64/otpme/lib/help/role.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/script.py` & `otpme-0.3.0a64/otpme/lib/help/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/session.py` & `otpme-0.3.0a64/otpme/lib/help/session.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/site.py` & `otpme-0.3.0a64/otpme/lib/help/site.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/token/__init__.py` & `otpme-0.3.0a64/otpme/lib/help/token/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/token/fido2.py` & `otpme-0.3.0a64/otpme/lib/help/token/fido2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/token/hotp.py` & `otpme-0.3.0a64/otpme/lib/help/token/hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/token/motp.py` & `otpme-0.3.0a64/otpme/lib/help/token/motp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/token/otp_push.py` & `otpme-0.3.0a64/otpme/lib/help/token/otp_push.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/token/otpme.py` & `otpme-0.3.0a64/otpme/lib/help/token/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/token/password.py` & `otpme-0.3.0a64/otpme/lib/help/token/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/token/ssh.py` & `otpme-0.3.0a64/otpme/lib/help/token/ssh.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/token/totp.py` & `otpme-0.3.0a64/otpme/lib/help/token/totp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/token/yubikey_hmac.py` & `otpme-0.3.0a64/otpme/lib/help/token/yubikey_hmac.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/token/yubikey_hotp.py` & `otpme-0.3.0a64/otpme/lib/help/token/yubikey_hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/tool.py` & `otpme-0.3.0a64/otpme/lib/help/tool.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/unit.py` & `otpme-0.3.0a64/otpme/lib/help/unit.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/help/user.py` & `otpme-0.3.0a64/otpme/lib/help/user.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/host.py` & `otpme-0.3.0a64/otpme/lib/host.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/humanize/units.py` & `otpme-0.3.0a64/otpme/lib/humanize/units.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/index/mysql.py` & `otpme-0.3.0a64/otpme/lib/index/mysql.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/index/postgres.py` & `otpme-0.3.0a64/otpme/lib/index/postgres.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/index/sqlite3.py` & `otpme-0.3.0a64/otpme/lib/index/sqlite3.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/job/callback.py` & `otpme-0.3.0a64/otpme/lib/job/callback.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/job/otpme_job.py` & `otpme-0.3.0a64/otpme/lib/job/otpme_job.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/join.py` & `otpme-0.3.0a64/otpme/lib/join.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/json.py` & `otpme-0.3.0a64/otpme/lib/json.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/jwt.py` & `otpme-0.3.0a64/otpme/lib/jwt.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/ldap/client.py` & `otpme-0.3.0a64/otpme/lib/ldap/client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/ldap/schema.py` & `otpme-0.3.0a64/otpme/lib/ldap/schema.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/ldap/server.py` & `otpme-0.3.0a64/otpme/lib/ldap/server.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/locking.py` & `otpme-0.3.0a64/otpme/lib/locking.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/log.py` & `otpme-0.3.0a64/otpme/lib/log.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/messages.py` & `otpme-0.3.0a64/otpme/lib/messages.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/mschap.py` & `otpme-0.3.0a64/otpme/lib/mschap.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/mschap_util.py` & `otpme-0.3.0a64/otpme/lib/mschap_util.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/multiprocessing.py` & `otpme-0.3.0a64/otpme/lib/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/net.py` & `otpme-0.3.0a64/otpme/lib/net.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/nsscache.py` & `otpme-0.3.0a64/otpme/lib/nsscache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/offline_token.py` & `otpme-0.3.0a64/otpme/lib/offline_token.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/oid.py` & `otpme-0.3.0a64/otpme/lib/oid.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/otp/oath/hotp.py` & `otpme-0.3.0a64/otpme/lib/otp/oath/hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/otp/oath/totp.py` & `otpme-0.3.0a64/otpme/lib/otp/oath/totp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/otp/otpme/otpme.py` & `otpme-0.3.0a64/otpme/lib/otp/otpme/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/otp/yubico/yubiotp.py` & `otpme-0.3.0a64/otpme/lib/otp/yubico/yubiotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/otpme_acl.py` & `otpme-0.3.0a64/otpme/lib/otpme_acl.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/otpme_config.py` & `otpme-0.3.0a64/otpme/lib/otpme_config.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/otpme_pass.py` & `otpme-0.3.0a64/otpme/lib/otpme_pass.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/pam.py` & `otpme-0.3.0a64/otpme/lib/pam.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/pickle.py` & `otpme-0.3.0a64/otpme/lib/pickle.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/pinentry/pinentry.py` & `otpme-0.3.0a64/otpme/lib/pinentry/pinentry.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/pinentry/wrapper.py` & `otpme-0.3.0a64/otpme/lib/pinentry/wrapper.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/pki/cert.py` & `otpme-0.3.0a64/otpme/lib/pki/cert.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/pki/utils.py` & `otpme-0.3.0a64/otpme/lib/pki/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/pki/utils_openssl.py` & `otpme-0.3.0a64/otpme/lib/pki/utils_openssl.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/policy/__init__.py` & `otpme-0.3.0a64/otpme/lib/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/policy/authonaction/authonaction.py` & `otpme-0.3.0a64/otpme/lib/policy/authonaction/authonaction.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/policy/autodisable/autodisable.py` & `otpme-0.3.0a64/otpme/lib/policy/autodisable/autodisable.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/policy/defaultgroups/defaultgroups.py` & `otpme-0.3.0a64/otpme/lib/policy/defaultgroups/defaultgroups.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/policy/defaultpolicies/defaultpolicies.py` & `otpme-0.3.0a64/otpme/lib/policy/defaultpolicies/defaultpolicies.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/policy/defaultroles/defaultroles.py` & `otpme-0.3.0a64/otpme/lib/policy/defaultroles/defaultroles.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/policy/defaultunits/defaultunits.py` & `otpme-0.3.0a64/otpme/lib/policy/defaultunits/defaultunits.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/policy/forcetoken/forcetoken.py` & `otpme-0.3.0a64/otpme/lib/policy/forcetoken/forcetoken.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/policy/get_class.py` & `otpme-0.3.0a64/otpme/lib/policy/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/policy/idrange/idrange.py` & `otpme-0.3.0a64/otpme/lib/policy/idrange/idrange.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/policy/logintimes/logintimes.py` & `otpme-0.3.0a64/otpme/lib/policy/logintimes/logintimes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/policy/objecttemplates/objecttemplates.py` & `otpme-0.3.0a64/otpme/lib/policy/objecttemplates/objecttemplates.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/policy/password/password.py` & `otpme-0.3.0a64/otpme/lib/policy/password/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/policy/tokenacls/tokenacls.py` & `otpme-0.3.0a64/otpme/lib/policy/tokenacls/tokenacls.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/policy/utils.py` & `otpme-0.3.0a64/otpme/lib/policy/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/preload.py` & `otpme-0.3.0a64/otpme/lib/preload.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/progress.py` & `otpme-0.3.0a64/otpme/lib/progress.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/client/__init__.py` & `otpme-0.3.0a64/otpme/lib/protocols/client/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/client/agent1.py` & `otpme-0.3.0a64/otpme/lib/protocols/client/agent1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/client/auth1.py` & `otpme-0.3.0a64/otpme/lib/protocols/client/auth1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/client/cluster1.py` & `otpme-0.3.0a64/otpme/lib/protocols/client/cluster1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/client/get_class.py` & `otpme-0.3.0a64/otpme/lib/protocols/client/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/client/host1.py` & `otpme-0.3.0a64/otpme/lib/protocols/client/host1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/client/join1.py` & `otpme-0.3.0a64/otpme/lib/protocols/client/join1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/client/mgmt1.py` & `otpme-0.3.0a64/otpme/lib/protocols/client/mgmt1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/client/sync1.py` & `otpme-0.3.0a64/otpme/lib/protocols/client/sync1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/otpme_client.py` & `otpme-0.3.0a64/otpme/lib/protocols/otpme_client.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/otpme_server.py` & `otpme-0.3.0a64/otpme/lib/protocols/otpme_server.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/request.py` & `otpme-0.3.0a64/otpme/lib/protocols/request.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/response.py` & `otpme-0.3.0a64/otpme/lib/protocols/response.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/server/__init__.py` & `otpme-0.3.0a64/otpme/lib/protocols/server/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/server/agent1.py` & `otpme-0.3.0a64/otpme/lib/protocols/server/agent1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/server/auth1.py` & `otpme-0.3.0a64/otpme/lib/protocols/server/auth1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/server/cluster1.py` & `otpme-0.3.0a64/otpme/lib/protocols/server/cluster1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/server/get_class.py` & `otpme-0.3.0a64/otpme/lib/protocols/server/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/server/host1.py` & `otpme-0.3.0a64/otpme/lib/protocols/server/host1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/server/join1.py` & `otpme-0.3.0a64/otpme/lib/protocols/server/join1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/server/mgmt1.py` & `otpme-0.3.0a64/otpme/lib/protocols/server/mgmt1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/server/sync1.py` & `otpme-0.3.0a64/otpme/lib/protocols/server/sync1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/status_codes.py` & `otpme-0.3.0a64/otpme/lib/protocols/status_codes.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/protocols/utils.py` & `otpme-0.3.0a64/otpme/lib/protocols/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/push_script.py` & `otpme-0.3.0a64/otpme/lib/push_script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/qrcode.py` & `otpme-0.3.0a64/otpme/lib/qrcode.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/re.py` & `otpme-0.3.0a64/otpme/lib/re.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/register/__init__.py` & `otpme-0.3.0a64/otpme/lib/register/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/resolver/__init__.py` & `otpme-0.3.0a64/otpme/lib/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/resolver/get_class.py` & `otpme-0.3.0a64/otpme/lib/resolver/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/resolver/ldap/ldap.py` & `otpme-0.3.0a64/otpme/lib/resolver/ldap/ldap.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/resolver/utils.py` & `otpme-0.3.0a64/otpme/lib/resolver/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/script.py` & `otpme-0.3.0a64/otpme/lib/script.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/sign_key_cache.py` & `otpme-0.3.0a64/otpme/lib/sign_key_cache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/slp.py` & `otpme-0.3.0a64/otpme/lib/slp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/smartcard/__init__.py` & `otpme-0.3.0a64/otpme/lib/smartcard/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/smartcard/fido2/fido2.py` & `otpme-0.3.0a64/otpme/lib/smartcard/fido2/fido2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/smartcard/get_class.py` & `otpme-0.3.0a64/otpme/lib/smartcard/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/smartcard/utils.py` & `otpme-0.3.0a64/otpme/lib/smartcard/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/smartcard/yubikey/deploy.py` & `otpme-0.3.0a64/otpme/lib/smartcard/yubikey/deploy.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/smartcard/yubikey/usb.py` & `otpme-0.3.0a64/otpme/lib/smartcard/yubikey/usb.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/smartcard/yubikey/yubikey.py` & `otpme-0.3.0a64/otpme/lib/smartcard/yubikey/yubikey.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py` & `otpme-0.3.0a64/otpme/lib/smartcard/yubikey_gpg/yubikey_gpg.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py` & `otpme-0.3.0a64/otpme/lib/smartcard/yubikey_hmac/yubikey_hmac.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py` & `otpme-0.3.0a64/otpme/lib/smartcard/yubikey_hotp/yubikey_hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/socket/connect.py` & `otpme-0.3.0a64/otpme/lib/socket/connect.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/socket/handler.py` & `otpme-0.3.0a64/otpme/lib/socket/handler.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/socket/listen.py` & `otpme-0.3.0a64/otpme/lib/socket/listen.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/socket/send_recv1.py` & `otpme-0.3.0a64/otpme/lib/socket/send_recv1.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/sotp.py` & `otpme-0.3.0a64/otpme/lib/sotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/spsc.py` & `otpme-0.3.0a64/otpme/lib/spsc.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/srp.py` & `otpme-0.3.0a64/otpme/lib/srp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/ssh.py` & `otpme-0.3.0a64/otpme/lib/ssh.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/stuff.py` & `otpme-0.3.0a64/otpme/lib/stuff.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/sync_cache.py` & `otpme-0.3.0a64/otpme/lib/sync_cache.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/system_command.py` & `otpme-0.3.0a64/otpme/lib/system_command.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/test.py` & `otpme-0.3.0a64/otpme/lib/test.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/__init__.py` & `otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/advanced.py` & `otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/advanced.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/caching_query.py` & `otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/caching_query.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/environment.py` & `otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/environment.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/fixture_data.py` & `otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/fixture_data.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/helloworld.py` & `otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/helloworld.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/local_session_caching.py` & `otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/local_session_caching.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/model.py` & `otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/model.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/dogpile_caching/relationship_caching.py` & `otpme-0.3.0a64/otpme/lib/third_party/dogpile_caching/relationship_caching.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/nss_cache/__init__.py` & `otpme-0.3.0a64/otpme/lib/third_party/nss_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/nss_cache/caches/caches.py` & `otpme-0.3.0a64/otpme/lib/third_party/nss_cache/caches/caches.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/nss_cache/caches/files.py` & `otpme-0.3.0a64/otpme/lib/third_party/nss_cache/caches/files.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/nss_cache/config.py` & `otpme-0.3.0a64/otpme/lib/third_party/nss_cache/config.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/nss_cache/error.py` & `otpme-0.3.0a64/otpme/lib/third_party/nss_cache/error.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/nss_cache/lock.py` & `otpme-0.3.0a64/otpme/lib/third_party/nss_cache/lock.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/nss_cache/maps/group.py` & `otpme-0.3.0a64/otpme/lib/third_party/nss_cache/maps/group.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/nss_cache/maps/maps.py` & `otpme-0.3.0a64/otpme/lib/third_party/nss_cache/maps/maps.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/nss_cache/maps/passwd.py` & `otpme-0.3.0a64/otpme/lib/third_party/nss_cache/maps/passwd.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/nss_cache/maps/shadow.py` & `otpme-0.3.0a64/otpme/lib/third_party/nss_cache/maps/shadow.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/nss_cache/nss.py` & `otpme-0.3.0a64/otpme/lib/third_party/nss_cache/nss.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/nss_cache/update/files_updater.py` & `otpme-0.3.0a64/otpme/lib/third_party/nss_cache/update/files_updater.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/nss_cache/update/map_updater.py` & `otpme-0.3.0a64/otpme/lib/third_party/nss_cache/update/map_updater.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/nss_cache/update/updater.py` & `otpme-0.3.0a64/otpme/lib/third_party/nss_cache/update/updater.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/nss_cache/util/file_formats.py` & `otpme-0.3.0a64/otpme/lib/third_party/nss_cache/util/file_formats.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/oath_toolkit/_compat.py` & `otpme-0.3.0a64/otpme/lib/third_party/oath_toolkit/_compat.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/third_party/oath_toolkit/uri.py` & `otpme-0.3.0a64/otpme/lib/third_party/oath_toolkit/uri.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/token/__init__.py` & `otpme-0.3.0a64/otpme/lib/token/__init__.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/token/fido2/fido2.py` & `otpme-0.3.0a64/otpme/lib/token/fido2/fido2.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/token/get_class.py` & `otpme-0.3.0a64/otpme/lib/token/get_class.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/token/hotp/hotp.py` & `otpme-0.3.0a64/otpme/lib/token/hotp/hotp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/token/link/link.py` & `otpme-0.3.0a64/otpme/lib/token/link/link.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/token/motp/motp.py` & `otpme-0.3.0a64/otpme/lib/token/motp/motp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/token/oath/oath.py` & `otpme-0.3.0a64/otpme/lib/token/oath/oath.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/token/otp_push/otp_push.py` & `otpme-0.3.0a64/otpme/lib/token/otp_push/otp_push.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/token/otpme/otpme.py` & `otpme-0.3.0a64/otpme/lib/token/otpme/otpme.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/token/password/password.py` & `otpme-0.3.0a64/otpme/lib/token/password/password.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/token/script_otp/script_otp.py` & `otpme-0.3.0a64/otpme/lib/token/script_otp/script_otp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/token/script_static/script_static.py` & `otpme-0.3.0a64/otpme/lib/token/script_static/script_static.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/token/ssh/ssh.py` & `otpme-0.3.0a64/otpme/lib/token/ssh/ssh.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/token/totp/totp.py` & `otpme-0.3.0a64/otpme/lib/token/totp/totp.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/token/utils.py` & `otpme-0.3.0a64/otpme/lib/token/utils.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme/lib/token/yubikey_hmac/yubikey_hmac.py` & `otpme-0.3.0a64/otpme/lib/token/yubikey_hmac/yubikey_hmac.py`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme.egg-info/PKG-INFO` & `otpme-0.3.0a64/otpme.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otpme
-Version: 0.3.0a63
+Version: 0.3.0a64
 Summary: OTPme: A flexible One-Time-Password system.
 Home-page: http://www.otpme.org
 Author: the2nd
 Author-email: the2nd@otpme.org
 Maintainer: the2nd
 Maintainer-email: the2nd@otpme.org
 License: GPLv2
```

### Comparing `otpme-0.3.0a63/otpme.egg-info/SOURCES.txt` & `otpme-0.3.0a64/otpme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme.egg-info/entry_points.txt` & `otpme-0.3.0a64/otpme.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `otpme-0.3.0a63/otpme.egg-info/requires.txt` & `otpme-0.3.0a64/otpme.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 SQLAlchemy-Utils>=0.36.8
 SQLAlchemy>=2.0.15
 Twisted>=13.2.0
 argon2>=0.1.10
 arprequest>=0.3
 bson>=0.5.10
 cachetools==5.3.1
-cchardet>=1.1.2
+cchardet>=2.1.7
 chardet>=3.0.4
 colorlog>=4.1.0
-cryptography
+cryptography<3.5
 daemonize>=2.4.7
 dnspython>=1.15.0
 dogpile.cache>=0.9.0
 ecdsa>=0.10
 fido2==1.1.1
 future>=0.15.2
 humanize>=0.5.1
```

### Comparing `otpme-0.3.0a63/setup.py` & `otpme-0.3.0a64/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,16 @@
                 "importlib-metadata",
                 "ipaddr>=2.1.10",
                 "psutil>=5.5.1",
                 "pytz>=2019.3",
                 "pexpect>=4.6.0",
                 "pycryptodomex>=3.7.3",
                 #"cryptography==3.3.2",
-                "cryptography",
+                #"cryptography",
+                "cryptography<3.5",
                 #"pyOpenSSL>=0.13",
                 "pyOpenSSL>=0.15.1",
                 "pysodium>=0.7.10",
                 "pylibacl>=0.5.1",
                 "ecdsa>=0.10",
                 #"ecdsa>=0.13",
                 "dnspython>=1.15.0",
@@ -73,15 +74,16 @@
                 "prettytable>=0.7.2",
                 "setproctitle>=1.1.10",
                 "paramiko>=1.16.0",
                 "arprequest>=0.3",
                 "scapy>=2.4.4",
                 "oath>=1.4.1",
                 "Cython>=0.20",
-                "cchardet>=1.1.2",
+                #"cchardet>=1.1.2",
+                "cchardet>=2.1.7",
                 "chardet>=3.0.4",
                 "argon2>=0.1.10",
                 "future>=0.15.2",
                 "Cython>=0.29.36",
                 "PyJWT==1.7.1",
                 "fido2==1.1.1",
                 "qrcode>=5.1",
```

