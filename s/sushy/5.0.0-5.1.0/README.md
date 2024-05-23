# Comparing `tmp/sushy-5.0.0.tar.gz` & `tmp/sushy-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sushy-5.0.0.tar", last modified: Thu Feb 22 15:01:13 2024, max compression
+gzip compressed data, was "sushy-5.1.0.tar", last modified: Thu May 23 07:55:13 2024, max compression
```

## Comparing `sushy-5.0.0.tar` & `sushy-5.1.0.tar`

### file list

```diff
@@ -1,487 +1,489 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.680539 sushy-5.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:00:44.000000 sushy-5.0.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-02-22 15:00:44.000000 sushy-5.0.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2024-02-22 15:00:44.000000 sushy-5.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3041 2024-02-22 15:01:13.000000 sushy-5.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-02-22 15:00:44.000000 sushy-5.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17948 2024-02-22 15:01:13.000000 sushy-5.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-02-22 15:00:44.000000 sushy-5.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-02-22 15:00:44.000000 sushy-5.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2230 2024-02-22 15:01:13.680539 sushy-5.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2024-02-22 15:00:44.000000 sushy-5.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-02-22 15:00:44.000000 sushy-5.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.632535 sushy-5.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-02-22 15:00:44.000000 sushy-5.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.632535 sushy-5.0.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3047 2024-02-22 15:00:44.000000 sushy-5.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.632535 sushy-5.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3142 2024-02-22 15:00:44.000000 sushy-5.0.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2024-02-22 15:00:44.000000 sushy-5.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.632535 sushy-5.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2024-02-22 15:00:44.000000 sushy-5.0.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.632535 sushy-5.0.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2024-02-22 15:00:44.000000 sushy-5.0.0/doc/source/reference/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10228 2024-02-22 15:00:44.000000 sushy-5.0.0/doc/source/reference/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.628535 sushy-5.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.644536 sushy-5.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/action-parameter-missing-7d234b96b5b1d81a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-apply-time-support-to-bios-315ebad429dcab3d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-bios-bf69ac56c4ae8f50.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-bios-update-status-cc59816c374b78e4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-chassis-linkage-d8e567f9c791169d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-chassis-support-5b97daffe1c61a2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-custom-connector-support-0a49c6649d5f7eaf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-default-identity-10c5dd23bed0e915.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-drive-led-97b687013fec88c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-drive-revision-a0c069fff236479d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-drive-volumes-971d80644c3bd1e0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-endpoint-subresource-to-fabric-b03e5fd99ece1bf4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-fabric-support-1520f7fcb0e12539.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-http-boot-uri-support-5c25816e13ccdb27.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-initial-redfish-oem-extension-support-50c9849bb7b6b25c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-mapped-list-field-04c671f7a73d83f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-network-adapter-26d01d8d9fb1d7ad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-network-device-function-and-port-e880d8f461e3723d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-odata-version-header-96dc8179c0e2e9bd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-partial-key-match-27bed73d577b1187.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-power-resource-e141ddf298673305.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-processor-id-and-status-b81d4c6e6c14c25f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-raid-type-properties-2090da5bea37c660.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-read-and-connect-timeout-9f7dc3ed63c192c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-response-cb-65d448ee2690d0b2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-simple-storage-915464811737bb05.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-storage-and-simple-storage-attributes-to-system-16e81f9b15b1897d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-storage-da766d3dbf9fb385.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-sushy-root-to-resources-1f221794557aa5fc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-system-bootprogress-42ee452cfa279c63.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-system-manager-linkage-86be69c9df4cb359.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-system-status-field-41b3f2a8c4b85f38.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-system-type-mapping-bf456c5c15a90877.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-task-monitor-support-21f711927ad6ec91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-task-service-c751ce51e0b8dc11.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-thermal-resource-5c965a3c940f9028.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-virtual-media-support-f522fbec4420341c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add_composition_service-84750d8d1d96474a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add_ethernet_interface-df308f814f0e4bce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add_keyword_argument_for_connector-cea5dc4e6c01b548.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add_product_and_protocol_features_supported-59de3f89b7382434.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add_update_service-b54c9bb0177e3468.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/allow_empty_context_eventdestination-9a96c34dd7edbeca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/apply-time-support-for-volume-ops-f2ebc412e3b4290a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/bios-attribute-registry-a55c2d81c730a795.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/bug-1754514-ca6ebe16c4e4b3b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/catch-general-requests-exceptions-b5fd706597708fb6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/certificate-collection-acc67488c240274c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/change-bootdev-smc-ab30317eaf5c37d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/change-vmedia-write-protected-attr-586370a552288801.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/check-for-boot-attrs-in-settingsuri-1cad07b6eb1c81b3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/config-server-side-retries-d16824019bd709a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/decouple-boot-params-c75e80f5951abb12.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/deprecate-system-leds-f1a72422c53d281e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/disable-conn-pooling-3456782afe56ac94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      807 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/do-not-offer-compression-encoding-884ca8a7458cb096.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/drop-py-2-7-cc931c210ce08e33.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/enhance-oem-extension-design-3143717e710b3eaf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/enhance-storage-volume-drive-support-16314d30f3631fb3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/enums-3aff03d940012f33.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/event-service-d6607420effc3df8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/expand-drive-schema-042901f919be646c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-2008198-bios-factory-reset-400-bad-request-3f4a7a2aada0835b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-eject-media-empty-dict-573b4c9e06f52ce7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-exceeding-retries-663ab543cc14f261.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-extended-info-error-handling-73fecb6bf5c852ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-insert-media-payload-b5d4c707f81d9603.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-malformed-boot-mode-1ba1117cad8dcc47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-manager-action-d71fd415cea29aa6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-missing-etags-ded8c0bb31fafef7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-oem-loading-52da045252b6c33e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-refine-resource-refresh-86c21ce230967251.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-required-oem-attribute-parsing-205e4186275aa293.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-retry_volume_operation-on_sys518-009f2b16e5c38a27.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-return-full-weak-etag-04265472cbea9c0e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-simple-storage-device-capacity-bytes-null-0672eed36d9da70a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-simple-update-e88838fab4170920.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-software-firmware-inventory-3e0e79e052aa76d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-subprocessors-3b619434dba4636d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-taskmonitor-init-calls-in-volume-module-0f8a747acd0cfe3f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-to-close-session-on-dealloc-c3687d4dcb1441b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-update-service-constants-b8c3f48ccee6ce1f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-use-headers-for-options-736940b87c06c189.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-virtual-media-fallback-15a559414a65c014.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-volume-actions-not-required-730fd637dd2587ce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-volume-delete-configuration-unsuported-operational_time_property-f53f650d8612a847.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fixes-ilo5-redfish-firmware-update-issue-273862b2a11e3536.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/get-retry-9ca311caf8a0b7bb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/handle-basic-auth-access-errors-393b368b31f5cad2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/handle_transfer_method-a51d5a17e381ebee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/health_literals_change-0e3fc0c439b765e3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/increase-server-retries-5f11edde8ee0b461.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/indicator-led-mappings-e7b34da03f6abb06.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/lazily-load-registries-0e9441e435c2471d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/make-leds-settable-c82cb513de0171f5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/make-volume-ops-blocking-de5c2ae032041d5d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/message-parsing-resilience-534da532515a15da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/message-registry-logging-39624ae114c02e15.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/monitor_firmware_update-664b0c6c1a0307cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/more-transferprotocoltype-739ce8bdedbcb51c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/no-passwords-295207ac891d27ab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/non-default-language-registries-f73bdecc98ba2cc8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/property-missing-7602c421ec177e9a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/raise-error-on-async-task-failure-b67c7bc189a4d6ca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/re-raise-1fe9f912691e893e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/reauthentication-session-fallback-failure-fixes-4f0dcfdad1afd2d7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/redfish-response-log-294f3f10b770e356.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1522 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/refactor-taskmonitor-update-volume-ba99380188395852.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/releasenote-d7138d1e1d414632.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/remove-deprecated-task-monitors-58c505d43e1fa6a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/retry-if-transferprototype-missing-9cae57f3ecf470a9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/retry-ilo-not-ready-error-0b4dce882282eaac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/secure-boot-76c5b80371ea85d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/secure-boot-database-7fae673722d7cf4f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/sessions.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/standard-registry-license-0ded489afd6cfad1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/storage-controllers-resource-7ab112f5d2c34ca0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/story-2006246-reset-bios-return-http-error-415-08170df7fe6300f8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/story-2007216-fix-to-message-registry-cff37659f03ba815.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/sushy-system-virtualmedia-7a61bd77780f7b0e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/update-apply-time-support-53c5445b58cd3b42.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/update_sushy_models-9b8ea0350eb4d4d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/use-sessions-url-from-root-8b8eca57dc450705.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/use-settingsobject-if-supported-12a332f9905d64ce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/vmedia-1.4.0-9957460fed59d85c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/vmedia-certificate-06c367c6ef33d139.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/vmedia-credentials-14b7705c3c94cc07.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/workaround-sushy-requests-verify-handling-6879c273b651246f.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.644536 sushy-5.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.644536 sushy-5.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.644536 sushy-5.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9025 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2024-02-22 15:00:44.000000 sushy-5.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1032 2024-02-22 15:01:13.680539 sushy-5.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-02-22 15:00:44.000000 sushy-5.0.0/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.648537 sushy-5.0.0/sushy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1672 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11601 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22799 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6058 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25817 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/main.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.648537 sushy-5.0.0/sushy/resources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31234 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.648537 sushy-5.0.0/sushy/resources/certificateservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/certificateservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4199 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/certificateservice/certificate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3599 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/certificateservice/certificateservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3138 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/certificateservice/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.648537 sushy-5.0.0/sushy/resources/chassis/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12166 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/chassis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5618 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.648537 sushy-5.0.0/sushy/resources/chassis/power/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/power/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/power/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4605 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/power/power.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.652537 sushy-5.0.0/sushy/resources/chassis/thermal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/thermal/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/thermal/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4909 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/thermal/thermal.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3657 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/common.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.652537 sushy-5.0.0/sushy/resources/compositionservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/compositionservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4043 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/compositionservice/compositionservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3311 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/compositionservice/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4346 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/compositionservice/resourceblock.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/compositionservice/resourcezone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12477 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.652537 sushy-5.0.0/sushy/resources/eventservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/eventservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1759 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/eventservice/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4539 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/eventservice/eventdestination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6073 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/eventservice/eventservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.652537 sushy-5.0.0/sushy/resources/fabric/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/fabric/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3340 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/fabric/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5613 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/fabric/endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3663 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/fabric/fabric.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2757 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/ipaddresses.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.652537 sushy-5.0.0/sushy/resources/manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5544 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/manager/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9951 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/manager/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11234 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/manager/virtual_media.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.652537 sushy-5.0.0/sushy/resources/oem/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/oem/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2814 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/oem/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4426 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/oem/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1374 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/oem/fake.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.652537 sushy-5.0.0/sushy/resources/registry/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/registry/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3423 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/registry/attribute_registry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/registry/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5414 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/registry/message_registry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7463 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/registry/message_registry_file.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.652537 sushy-5.0.0/sushy/resources/sessionservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/sessionservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3221 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/sessionservice/session.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4952 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/sessionservice/sessionservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6580 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/settings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.656537 sushy-5.0.0/sushy/resources/system/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9571 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/bios.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13947 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2547 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/ethernet_interface.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.656537 sushy-5.0.0/sushy/resources/system/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/network/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3157 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/network/adapter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3803 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/network/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6971 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/network/device_function.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2362 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/network/port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6612 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/processor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5550 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/secure_boot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4168 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/secure_boot_database.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2868 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/simple_storage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.656537 sushy-5.0.0/sushy/resources/system/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6283 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/storage/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6111 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/storage/controller.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3861 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/storage/drive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7410 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/storage/storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9575 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/storage/volume.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23551 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/system.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.656537 sushy-5.0.0/sushy/resources/taskservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/taskservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1495 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/taskservice/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3666 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/taskservice/task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/taskservice/taskservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.656537 sushy-5.0.0/sushy/resources/updateservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/updateservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1937 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/updateservice/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3863 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/updateservice/softwareinventory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7602 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/updateservice/updateservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.660537 sushy-5.0.0/sushy/standard_registries/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26502 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/standard_registries/Base.1.0.0.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29190 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/standard_registries/Base.1.2.0.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30123 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/standard_registries/Base.1.3.0.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30283 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/standard_registries/Base.1.3.1.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30875 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/standard_registries/Base.1.4.0.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7854 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/taskmonitor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.660537 sushy-5.0.0/sushy/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.660537 sushy-5.0.0/sushy/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.672538 sushy-5.0.0/sushy/tests/unit/json_samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/TestRegistry.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/bare_minimum_root.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1855 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/bios.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/bios_attribute_registry.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/bios_attribute_registry_file.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/bios_attribute_registry_file_zthardware.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2301 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/bios_attribute_registry_zthardware.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1270 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/bios_settings.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11114 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/bios_zt.json
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3793 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/certificate.json
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      567 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/certificate_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/certificate_locations.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/certificateservice.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3166 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/chassis.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/chassis_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      683 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/compositionservice.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1544 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/drive.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1685 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/drive2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1797 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/drive3.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/endpoint.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/endpoint_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1885 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/error_single_ext_info.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1166 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/ethernet_interfaces.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/ethernet_interfaces_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/eventdestination1.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/eventdestination2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/eventdestination3.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      508 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/eventdestination_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      836 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/eventservice.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      689 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/fabric.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/fabric_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/firmwareinventory_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2505 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/manager.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/manager_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2589 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/managerv1_18.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1482 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/message_registry.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/message_registry_file.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/message_registry_file_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2553 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/network_adapter.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/network_adapter_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2541 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/network_device_function.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/network_device_function_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1655 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/network_port.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/network_port_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4211 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/power.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/processor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/processor2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/processor_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1344 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/resourceblock.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/resourceblock_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/resourcezone.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/resourcezone_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1638 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/root.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/secure_boot.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/secure_boot_database.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1370 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/secure_boot_database_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/session.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/session_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/session_creation_headers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/session_creation_headers_no_location.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/session_error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/session_service.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/settings-body-bootsourceoverridemode-only.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/settings-body-lenovo-se450.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/settings-body-nokia.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/settings-lenovo-se450.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/settings-nokia.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/settings.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2039 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/simple_storage.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      607 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/simple_storage_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/softwareinventory.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/storage.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/storage_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1499 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/storage_controller.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/storage_controller_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/storage_controller_settings.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/subprocessor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/subprocessor_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5222 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/system.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/system_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4277 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/systemv1_20.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/task.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/task2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/task_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/task_monitor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/taskservice.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1323 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/thermal.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/transfer_method_required_error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/transfer_proto_required_error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/transfer_proto_required_error2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/transfer_proto_required_error3.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      950 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/updateservice.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      748 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/updateservice_no_inv.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/virtual_media.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/virtual_media_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/virtual_media_collectionv1_6.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/virtual_mediav1_6.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1514 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/volume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1392 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/volume2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/volume3.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1407 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/volume4.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/volume_collection.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.672538 sushy-5.0.0/sushy/tests/unit/resources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.672538 sushy-5.0.0/sushy/tests/unit/resources/certificateservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/certificateservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5657 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/certificateservice/test_certificate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3683 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/certificateservice/test_certificateservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.672538 sushy-5.0.0/sushy/tests/unit/resources/chassis/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/chassis/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12179 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/chassis/test_chassis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9406 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/chassis/test_power.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5962 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/chassis/test_thermal.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.672538 sushy-5.0.0/sushy/tests/unit/resources/compositionservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/compositionservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2861 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/compositionservice/test_compositionservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4894 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/compositionservice/test_resourceblock.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4027 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/compositionservice/test_resourcezone.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.676539 sushy-5.0.0/sushy/tests/unit/resources/eventservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/eventservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6786 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/eventservice/test_evendestination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4988 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/eventservice/test_eventservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.676539 sushy-5.0.0/sushy/tests/unit/resources/fabric/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/fabric/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2083 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/fabric/test_endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5434 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/fabric/test_fabric.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.676539 sushy-5.0.0/sushy/tests/unit/resources/manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14409 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/manager/test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16423 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/manager/test_virtual_media.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.676539 sushy-5.0.0/sushy/tests/unit/resources/oem/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/oem/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9148 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/oem/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2315 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/oem/test_fake.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.676539 sushy-5.0.0/sushy/tests/unit/resources/registry/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/registry/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4998 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/registry/test_attribute_registry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15477 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/registry/test_message_registry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14996 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/registry/test_message_registry_file.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.676539 sushy-5.0.0/sushy/tests/unit/resources/sessionservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/sessionservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4310 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/sessionservice/test_session.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6993 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/sessionservice/test_sessionservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.676539 sushy-5.0.0/sushy/tests/unit/resources/system/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.676539 sushy-5.0.0/sushy/tests/unit/resources/system/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/network/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8673 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/network/test_adapter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7679 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/network/test_device_function.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5056 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/network/test_port.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.680539 sushy-5.0.0/sushy/tests/unit/resources/system/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6366 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/storage/test_controller.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4394 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/storage/test_drive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17404 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/storage/test_storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16030 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/storage/test_volume.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20207 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/test_bios.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4757 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/test_ethernet_interfaces.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8840 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/test_processor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5169 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/test_secure_boot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6392 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/test_secure_boot_database.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5848 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/test_simple_storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45204 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/test_system.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.680539 sushy-5.0.0/sushy/tests/unit/resources/taskservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/taskservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7219 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/taskservice/test_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/taskservice/test_taskservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20136 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4938 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/test_settings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.680539 sushy-5.0.0/sushy/tests/unit/resources/updateservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/updateservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5604 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/updateservice/test_softwareinventory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9466 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/updateservice/test_updateservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22169 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40991 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/test_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28538 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/test_main.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11533 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/test_taskmonitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11237 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13472 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.648537 sushy-5.0.0/sushy.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2230 2024-02-22 15:01:13.000000 sushy-5.0.0/sushy.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22054 2024-02-22 15:01:13.000000 sushy-5.0.0/sushy.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 15:01:13.000000 sushy-5.0.0/sushy.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-02-22 15:01:13.000000 sushy-5.0.0/sushy.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 15:01:13.000000 sushy-5.0.0/sushy.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-22 15:01:13.000000 sushy-5.0.0/sushy.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-02-22 15:01:13.000000 sushy-5.0.0/sushy.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2024-02-22 15:01:13.000000 sushy-5.0.0/sushy.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2024-02-22 15:00:44.000000 sushy-5.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.680539 sushy-5.0.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2644 2024-02-22 15:00:44.000000 sushy-5.0.0/tools/generate-enum.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3311 2024-02-22 15:00:44.000000 sushy-5.0.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.680539 sushy-5.0.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2024-02-22 15:00:44.000000 sushy-5.0.0/zuul.d/project.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-02-22 15:00:44.000000 sushy-5.0.0/zuul.d/sushy-jobs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.139894 sushy-5.1.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 07:54:08.000000 sushy-5.1.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-05-23 07:54:08.000000 sushy-5.1.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2024-05-23 07:54:08.000000 sushy-5.1.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3071 2024-05-23 07:55:12.000000 sushy-5.1.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-05-23 07:54:08.000000 sushy-5.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18300 2024-05-23 07:55:12.000000 sushy-5.1.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-05-23 07:54:08.000000 sushy-5.1.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-23 07:54:08.000000 sushy-5.1.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2230 2024-05-23 07:55:13.139894 sushy-5.1.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2024-05-23 07:54:08.000000 sushy-5.1.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-05-23 07:54:08.000000 sushy-5.1.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.075894 sushy-5.1.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-05-23 07:54:08.000000 sushy-5.1.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.075894 sushy-5.1.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3047 2024-05-23 07:54:08.000000 sushy-5.1.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.075894 sushy-5.1.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3142 2024-05-23 07:54:08.000000 sushy-5.1.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2024-05-23 07:54:08.000000 sushy-5.1.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.075894 sushy-5.1.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2024-05-23 07:54:08.000000 sushy-5.1.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.075894 sushy-5.1.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2024-05-23 07:54:08.000000 sushy-5.1.0/doc/source/reference/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10228 2024-05-23 07:54:08.000000 sushy-5.1.0/doc/source/reference/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.067894 sushy-5.1.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.095894 sushy-5.1.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/accept-encoding-4646ea43998f80bd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/action-parameter-missing-7d234b96b5b1d81a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-apply-time-support-to-bios-315ebad429dcab3d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-bios-bf69ac56c4ae8f50.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-bios-update-status-cc59816c374b78e4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-chassis-linkage-d8e567f9c791169d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-chassis-support-5b97daffe1c61a2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-custom-connector-support-0a49c6649d5f7eaf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-default-identity-10c5dd23bed0e915.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-drive-led-97b687013fec88c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-drive-revision-a0c069fff236479d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-drive-volumes-971d80644c3bd1e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-endpoint-subresource-to-fabric-b03e5fd99ece1bf4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-fabric-support-1520f7fcb0e12539.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-http-boot-uri-support-5c25816e13ccdb27.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-initial-redfish-oem-extension-support-50c9849bb7b6b25c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-mapped-list-field-04c671f7a73d83f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-network-adapter-26d01d8d9fb1d7ad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-network-device-function-and-port-e880d8f461e3723d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-odata-version-header-96dc8179c0e2e9bd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-partial-key-match-27bed73d577b1187.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-power-resource-e141ddf298673305.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-processor-id-and-status-b81d4c6e6c14c25f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-raid-type-properties-2090da5bea37c660.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-read-and-connect-timeout-9f7dc3ed63c192c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-response-cb-65d448ee2690d0b2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-simple-storage-915464811737bb05.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-storage-and-simple-storage-attributes-to-system-16e81f9b15b1897d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-storage-da766d3dbf9fb385.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-sushy-root-to-resources-1f221794557aa5fc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-system-bootprogress-42ee452cfa279c63.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-system-manager-linkage-86be69c9df4cb359.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-system-status-field-41b3f2a8c4b85f38.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-system-type-mapping-bf456c5c15a90877.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-task-monitor-support-21f711927ad6ec91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-task-service-c751ce51e0b8dc11.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-thermal-resource-5c965a3c940f9028.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add-virtual-media-support-f522fbec4420341c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add_composition_service-84750d8d1d96474a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add_ethernet_interface-df308f814f0e4bce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add_keyword_argument_for_connector-cea5dc4e6c01b548.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add_product_and_protocol_features_supported-59de3f89b7382434.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/add_update_service-b54c9bb0177e3468.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/allow_empty_context_eventdestination-9a96c34dd7edbeca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/apply-time-support-for-volume-ops-f2ebc412e3b4290a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/bios-attribute-registry-a55c2d81c730a795.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/bug-1754514-ca6ebe16c4e4b3b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/catch-general-requests-exceptions-b5fd706597708fb6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/certificate-collection-acc67488c240274c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/change-bootdev-smc-ab30317eaf5c37d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/change-vmedia-write-protected-attr-586370a552288801.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/check-for-boot-attrs-in-settingsuri-1cad07b6eb1c81b3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/config-server-side-retries-d16824019bd709a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/decouple-boot-params-c75e80f5951abb12.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/deprecate-system-leds-f1a72422c53d281e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/disable-conn-pooling-3456782afe56ac94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      807 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/do-not-offer-compression-encoding-884ca8a7458cb096.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/drop-py-2-7-cc931c210ce08e33.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/enhance-oem-extension-design-3143717e710b3eaf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/enhance-storage-volume-drive-support-16314d30f3631fb3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/enums-3aff03d940012f33.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/event-service-d6607420effc3df8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/expand-drive-schema-042901f919be646c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-2008198-bios-factory-reset-400-bad-request-3f4a7a2aada0835b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-eject-media-empty-dict-573b4c9e06f52ce7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-exceeding-retries-663ab543cc14f261.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-extended-info-error-handling-73fecb6bf5c852ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-insert-media-payload-b5d4c707f81d9603.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-malformed-boot-mode-1ba1117cad8dcc47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-manager-action-d71fd415cea29aa6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-missing-etags-ded8c0bb31fafef7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-oem-loading-52da045252b6c33e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-refine-resource-refresh-86c21ce230967251.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-required-oem-attribute-parsing-205e4186275aa293.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-retry_volume_operation-on_sys518-009f2b16e5c38a27.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-return-full-weak-etag-04265472cbea9c0e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-simple-storage-device-capacity-bytes-null-0672eed36d9da70a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-simple-update-e88838fab4170920.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-software-firmware-inventory-3e0e79e052aa76d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-subprocessors-3b619434dba4636d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-taskmonitor-init-calls-in-volume-module-0f8a747acd0cfe3f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-to-close-session-on-dealloc-c3687d4dcb1441b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-update-service-constants-b8c3f48ccee6ce1f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-use-headers-for-options-736940b87c06c189.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-virtual-media-fallback-15a559414a65c014.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-volume-actions-not-required-730fd637dd2587ce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fix-volume-delete-configuration-unsuported-operational_time_property-f53f650d8612a847.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/fixes-ilo5-redfish-firmware-update-issue-273862b2a11e3536.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/get-retry-9ca311caf8a0b7bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/handle-basic-auth-access-errors-393b368b31f5cad2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/handle_transfer_method-a51d5a17e381ebee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/health_literals_change-0e3fc0c439b765e3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/increase-server-retries-5f11edde8ee0b461.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/indicator-led-mappings-e7b34da03f6abb06.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/lazily-load-registries-0e9441e435c2471d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/make-leds-settable-c82cb513de0171f5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/make-volume-ops-blocking-de5c2ae032041d5d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/message-parsing-resilience-534da532515a15da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/message-registry-logging-39624ae114c02e15.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/monitor_firmware_update-664b0c6c1a0307cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/more-transferprotocoltype-739ce8bdedbcb51c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/no-passwords-295207ac891d27ab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/non-default-language-registries-f73bdecc98ba2cc8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/property-missing-7602c421ec177e9a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/raise-error-on-async-task-failure-b67c7bc189a4d6ca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/re-raise-1fe9f912691e893e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/reauthentication-session-fallback-failure-fixes-4f0dcfdad1afd2d7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/redfish-response-log-294f3f10b770e356.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1522 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/refactor-taskmonitor-update-volume-ba99380188395852.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/releasenote-d7138d1e1d414632.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/remove-deprecated-task-monitors-58c505d43e1fa6a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/retry-if-transferprototype-missing-9cae57f3ecf470a9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/retry-ilo-not-ready-error-0b4dce882282eaac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/secure-boot-76c5b80371ea85d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/secure-boot-database-7fae673722d7cf4f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/sessions.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/standard-registry-license-0ded489afd6cfad1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/storage-controllers-resource-7ab112f5d2c34ca0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/story-2006246-reset-bios-return-http-error-415-08170df7fe6300f8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/story-2007216-fix-to-message-registry-cff37659f03ba815.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/sushy-system-virtualmedia-7a61bd77780f7b0e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/update-apply-time-support-53c5445b58cd3b42.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/update_sushy_models-9b8ea0350eb4d4d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/use-sessions-url-from-root-8b8eca57dc450705.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/use-settingsobject-if-supported-12a332f9905d64ce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/vmedia-1.4.0-9957460fed59d85c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/vmedia-certificate-06c367c6ef33d139.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/vmedia-credentials-14b7705c3c94cc07.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/notes/workaround-sushy-requests-verify-handling-6879c273b651246f.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.095894 sushy-5.1.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.095894 sushy-5.1.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.095894 sushy-5.1.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9025 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2024-05-23 07:54:08.000000 sushy-5.1.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2024-05-23 07:54:08.000000 sushy-5.1.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1032 2024-05-23 07:55:13.139894 sushy-5.1.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-05-23 07:54:08.000000 sushy-5.1.0/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.099894 sushy-5.1.0/sushy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1672 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11601 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23842 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6223 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25817 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/main.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.099894 sushy-5.1.0/sushy/resources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31234 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.103894 sushy-5.1.0/sushy/resources/certificateservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/certificateservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4199 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/certificateservice/certificate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3599 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/certificateservice/certificateservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3138 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/certificateservice/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.103894 sushy-5.1.0/sushy/resources/chassis/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/chassis/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12166 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/chassis/chassis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5618 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/chassis/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.103894 sushy-5.1.0/sushy/resources/chassis/power/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/chassis/power/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/chassis/power/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4605 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/chassis/power/power.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.103894 sushy-5.1.0/sushy/resources/chassis/thermal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/chassis/thermal/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/chassis/thermal/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4909 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/chassis/thermal/thermal.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3657 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/common.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.103894 sushy-5.1.0/sushy/resources/compositionservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/compositionservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4043 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/compositionservice/compositionservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3311 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/compositionservice/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4346 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/compositionservice/resourceblock.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/compositionservice/resourcezone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12477 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.103894 sushy-5.1.0/sushy/resources/eventservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/eventservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1759 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/eventservice/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4539 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/eventservice/eventdestination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6073 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/eventservice/eventservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.103894 sushy-5.1.0/sushy/resources/fabric/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/fabric/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3340 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/fabric/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5613 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/fabric/endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3663 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/fabric/fabric.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2757 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/ipaddresses.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.107894 sushy-5.1.0/sushy/resources/manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5544 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/manager/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9951 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/manager/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11234 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/manager/virtual_media.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.107894 sushy-5.1.0/sushy/resources/oem/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/oem/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2814 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/oem/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4426 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/oem/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1374 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/oem/fake.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.107894 sushy-5.1.0/sushy/resources/registry/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/registry/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3423 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/registry/attribute_registry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/registry/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5422 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/registry/message_registry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7463 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/registry/message_registry_file.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.107894 sushy-5.1.0/sushy/resources/sessionservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/sessionservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3221 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/sessionservice/session.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4952 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/sessionservice/sessionservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6580 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/settings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.107894 sushy-5.1.0/sushy/resources/system/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9571 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/bios.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13947 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2547 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/ethernet_interface.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.111894 sushy-5.1.0/sushy/resources/system/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/network/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3157 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/network/adapter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3803 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/network/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6971 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/network/device_function.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2362 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/network/port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6612 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/processor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5550 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/secure_boot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4168 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/secure_boot_database.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2868 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/simple_storage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.111894 sushy-5.1.0/sushy/resources/system/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6283 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/storage/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6111 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/storage/controller.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3861 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/storage/drive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7410 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/storage/storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9575 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/storage/volume.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23551 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/system/system.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.111894 sushy-5.1.0/sushy/resources/taskservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/taskservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1495 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/taskservice/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3666 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/taskservice/task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/taskservice/taskservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.111894 sushy-5.1.0/sushy/resources/updateservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/updateservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1937 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/updateservice/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3863 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/updateservice/softwareinventory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7602 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/resources/updateservice/updateservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.111894 sushy-5.1.0/sushy/standard_registries/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26502 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/standard_registries/Base.1.0.0.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29190 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/standard_registries/Base.1.2.0.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30123 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/standard_registries/Base.1.3.0.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30283 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/standard_registries/Base.1.3.1.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30875 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/standard_registries/Base.1.4.0.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7854 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/taskmonitor.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.111894 sushy-5.1.0/sushy/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.115894 sushy-5.1.0/sushy/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.131894 sushy-5.1.0/sushy/tests/unit/json_samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/TestRegistry.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/bare_minimum_root.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1855 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/bios.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/bios_attribute_registry.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/bios_attribute_registry_file.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/bios_attribute_registry_file_zthardware.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2301 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/bios_attribute_registry_zthardware.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1270 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/bios_settings.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11114 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/bios_zt.json
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3793 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/certificate.json
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      567 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/certificate_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/certificate_locations.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/certificateservice.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3166 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/chassis.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/chassis_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      683 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/compositionservice.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1544 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/drive.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1685 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/drive2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1797 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/drive3.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/endpoint.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/endpoint_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1885 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/error_single_ext_info.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1166 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/ethernet_interfaces.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/ethernet_interfaces_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/eventdestination1.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/eventdestination2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/eventdestination3.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      508 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/eventdestination_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      836 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/eventservice.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      689 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/fabric.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/fabric_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/firmwareinventory_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2505 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/manager.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/manager_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2589 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/managerv1_18.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1482 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/message_registry.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/message_registry_file.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/message_registry_file_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2553 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/network_adapter.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/network_adapter_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2541 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/network_device_function.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/network_device_function_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1655 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/network_port.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/network_port_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4211 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/power.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/processor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/processor2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/processor_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1344 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/resourceblock.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/resourceblock_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/resourcezone.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/resourcezone_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1638 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/root.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/secure_boot.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/secure_boot_database.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1370 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/secure_boot_database_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/session.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/session_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/session_creation_headers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/session_creation_headers_no_location.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/session_error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/session_service.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/settings-body-bootsourceoverridemode-only.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/settings-body-lenovo-se450.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/settings-body-nokia.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/settings-lenovo-se450.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/settings-nokia.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/settings.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2039 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/simple_storage.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      607 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/simple_storage_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/softwareinventory.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/storage.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/storage_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1499 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/storage_controller.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/storage_controller_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/storage_controller_settings.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/subprocessor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/subprocessor_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5222 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/system.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/system_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4277 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/systemv1_20.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/task.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/task2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/task_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/task_monitor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/taskservice.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1323 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/thermal.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/transfer_method_required_error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/transfer_proto_required_error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/transfer_proto_required_error2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/transfer_proto_required_error3.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      950 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/updateservice.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      748 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/updateservice_no_inv.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/virtual_media.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/virtual_media_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/virtual_media_collectionv1_6.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/virtual_mediav1_6.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1514 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/volume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1392 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/volume2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/volume3.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1407 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/volume4.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/json_samples/volume_collection.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.131894 sushy-5.1.0/sushy/tests/unit/resources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.131894 sushy-5.1.0/sushy/tests/unit/resources/certificateservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/certificateservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5657 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/certificateservice/test_certificate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3683 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/certificateservice/test_certificateservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.131894 sushy-5.1.0/sushy/tests/unit/resources/chassis/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/chassis/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12179 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/chassis/test_chassis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9406 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/chassis/test_power.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5962 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/chassis/test_thermal.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.131894 sushy-5.1.0/sushy/tests/unit/resources/compositionservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/compositionservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2861 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/compositionservice/test_compositionservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4894 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/compositionservice/test_resourceblock.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4027 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/compositionservice/test_resourcezone.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.131894 sushy-5.1.0/sushy/tests/unit/resources/eventservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/eventservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6786 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/eventservice/test_evendestination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4988 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/eventservice/test_eventservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.131894 sushy-5.1.0/sushy/tests/unit/resources/fabric/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/fabric/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2083 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/fabric/test_endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5434 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/fabric/test_fabric.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.131894 sushy-5.1.0/sushy/tests/unit/resources/manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14409 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/manager/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16423 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/manager/test_virtual_media.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.135894 sushy-5.1.0/sushy/tests/unit/resources/oem/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/oem/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9148 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/oem/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2315 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/oem/test_fake.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.135894 sushy-5.1.0/sushy/tests/unit/resources/registry/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/registry/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4998 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/registry/test_attribute_registry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15477 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/registry/test_message_registry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14996 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/registry/test_message_registry_file.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.135894 sushy-5.1.0/sushy/tests/unit/resources/sessionservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/sessionservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4310 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/sessionservice/test_session.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6993 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/sessionservice/test_sessionservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.135894 sushy-5.1.0/sushy/tests/unit/resources/system/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/system/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.135894 sushy-5.1.0/sushy/tests/unit/resources/system/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/system/network/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8673 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/system/network/test_adapter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7679 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/system/network/test_device_function.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5056 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/system/network/test_port.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.135894 sushy-5.1.0/sushy/tests/unit/resources/system/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/system/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6366 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/system/storage/test_controller.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4394 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/system/storage/test_drive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17404 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/system/storage/test_storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16030 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/system/storage/test_volume.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20207 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/system/test_bios.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4757 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/system/test_ethernet_interfaces.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8840 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/system/test_processor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5169 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/system/test_secure_boot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6392 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/system/test_secure_boot_database.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5848 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/system/test_simple_storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45204 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/system/test_system.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.139894 sushy-5.1.0/sushy/tests/unit/resources/taskservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/taskservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7219 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/taskservice/test_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/taskservice/test_taskservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20136 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4938 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/test_settings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.139894 sushy-5.1.0/sushy/tests/unit/resources/updateservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/updateservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5604 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/updateservice/test_softwareinventory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9466 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/resources/updateservice/test_updateservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22169 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42663 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/test_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28538 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/test_main.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11533 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/test_taskmonitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11237 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13472 2024-05-23 07:54:08.000000 sushy-5.1.0/sushy/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.099894 sushy-5.1.0/sushy.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2230 2024-05-23 07:55:12.000000 sushy-5.1.0/sushy.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22142 2024-05-23 07:55:13.000000 sushy-5.1.0/sushy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 07:55:12.000000 sushy-5.1.0/sushy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-05-23 07:55:12.000000 sushy-5.1.0/sushy.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-23 07:55:12.000000 sushy-5.1.0/sushy.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-23 07:55:12.000000 sushy-5.1.0/sushy.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-05-23 07:55:12.000000 sushy-5.1.0/sushy.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2024-05-23 07:55:12.000000 sushy-5.1.0/sushy.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2024-05-23 07:54:08.000000 sushy-5.1.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.139894 sushy-5.1.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2644 2024-05-23 07:54:08.000000 sushy-5.1.0/tools/generate-enum.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3311 2024-05-23 07:54:08.000000 sushy-5.1.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-23 07:55:13.139894 sushy-5.1.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2024-05-23 07:54:08.000000 sushy-5.1.0/zuul.d/project.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-05-23 07:54:08.000000 sushy-5.1.0/zuul.d/sushy-jobs.yaml
```

### Comparing `sushy-5.0.0/AUTHORS` & `sushy-5.1.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 Takashi Kajinami <kajinamit@oss.nttdata.com>
 Takashi Natsume <takanattie@gmail.com>
 Thomas Goirand <zigo@debian.org>
 Vanou Ishii <ishii.vanou@fujitsu.com>
 Varsha <varsha.verma.eee15@itbhu.ac.in>
 Vu Cong Tuan <tuanvc@vn.fujitsu.com>
 Winicius Silva <winiciusab12@gmail.com>
+Youngjun <yj.yoo@okestro.com>
 Yusef Shaban <yshaban@godaddy.com>
 ajya <mail@clusums.eu>
 ankit <ankit.dhn31@gmail.com>
 chengebj5238 <chengebj@inspur.com>
 dnuka <csx@tuta.io>
 ghanshyam <gmann@ghanshyammann.com>
 inspurericzhang <zhanglf01@inspur.com>
```

### Comparing `sushy-5.0.0/CONTRIBUTING.rst` & `sushy-5.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/ChangeLog` & `sushy-5.1.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 CHANGES
 =======
 
+5.1.0
+-----
+
+* reno: Update master for unmaintained/zed
+* Handle NotAcceptable when Accept-Encoding: identity is not allowed
+* reno: Update master for unmaintained/xena
+* reno: Update master for unmaintained/wallaby
+* reno: Update master for unmaintained/victoria
+* refectoring: Fix parameter and annotation mismatch
+* Update master for stable/2024.1
+
 5.0.0
 -----
 
 * reno: Update master for unmaintained/yoga
 * Force constraints when installing a package during tox test
 * [codespell] Adding CI target for Tox Codespell
 * [codespell] Adding Tox Target for Codespell
```

### Comparing `sushy-5.0.0/LICENSE` & `sushy-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/PKG-INFO` & `sushy-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sushy
-Version: 5.0.0
+Version: 5.1.0
 Summary: Sushy is a small Python library to communicate with Redfish based systems
 Home-page: https://docs.openstack.org/sushy/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Overview
         ========
```

### Comparing `sushy-5.0.0/README.rst` & `sushy-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/doc/source/conf.py` & `sushy-5.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/doc/source/contributor/index.rst` & `sushy-5.1.0/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/doc/source/index.rst` & `sushy-5.1.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/doc/source/reference/usage.rst` & `sushy-5.1.0/doc/source/reference/usage.rst`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/releasenotes/notes/apply-time-support-for-volume-ops-f2ebc412e3b4290a.yaml` & `sushy-5.1.0/releasenotes/notes/apply-time-support-for-volume-ops-f2ebc412e3b4290a.yaml`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/releasenotes/notes/check-for-boot-attrs-in-settingsuri-1cad07b6eb1c81b3.yaml` & `sushy-5.1.0/releasenotes/notes/check-for-boot-attrs-in-settingsuri-1cad07b6eb1c81b3.yaml`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/releasenotes/notes/do-not-offer-compression-encoding-884ca8a7458cb096.yaml` & `sushy-5.1.0/releasenotes/notes/do-not-offer-compression-encoding-884ca8a7458cb096.yaml`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/releasenotes/notes/enhance-oem-extension-design-3143717e710b3eaf.yaml` & `sushy-5.1.0/releasenotes/notes/enhance-oem-extension-design-3143717e710b3eaf.yaml`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/releasenotes/notes/enums-3aff03d940012f33.yaml` & `sushy-5.1.0/releasenotes/notes/enums-3aff03d940012f33.yaml`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/releasenotes/notes/fix-insert-media-payload-b5d4c707f81d9603.yaml` & `sushy-5.1.0/releasenotes/notes/fix-insert-media-payload-b5d4c707f81d9603.yaml`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/releasenotes/notes/reauthentication-session-fallback-failure-fixes-4f0dcfdad1afd2d7.yaml` & `sushy-5.1.0/releasenotes/notes/reauthentication-session-fallback-failure-fixes-4f0dcfdad1afd2d7.yaml`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/releasenotes/notes/refactor-taskmonitor-update-volume-ba99380188395852.yaml` & `sushy-5.1.0/releasenotes/notes/refactor-taskmonitor-update-volume-ba99380188395852.yaml`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/releasenotes/notes/releasenote-d7138d1e1d414632.yaml` & `sushy-5.1.0/releasenotes/notes/releasenote-d7138d1e1d414632.yaml`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/releasenotes/notes/update-apply-time-support-53c5445b58cd3b42.yaml` & `sushy-5.1.0/releasenotes/notes/update-apply-time-support-53c5445b58cd3b42.yaml`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/releasenotes/source/conf.py` & `sushy-5.1.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/requirements.txt` & `sushy-5.1.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/setup.cfg` & `sushy-5.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/setup.py` & `sushy-5.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/__init__.py` & `sushy-5.1.0/sushy/__init__.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/auth.py` & `sushy-5.1.0/sushy/auth.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/connector.py` & `sushy-5.1.0/sushy/connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,23 +47,14 @@
         # by allowing us to understand that we should stop authentication.
         self._sessions_uri = None
         # NOTE(etingof): field studies reveal that some BMCs choke at
         # long-running persistent HTTP connections (or TCP connections).
         # By default, we ask HTTP server to shut down HTTP connection we've
         # just used.
         self._session.headers['Connection'] = 'close'
-        # NOTE(TheJulia): Depending on the BMC, offering compression as an
-        # acceptable response changes the ETag behavior to offering an
-        # automatic "weak" ETag response, which is appropriate because the
-        # body content *may* not be a byte for byte match given compression.
-        # Overall, the value of compression is less than the value of concise
-        # interaction with the BMC. Setting to identity basically means
-        # "without modification or compression". By default, python-requests
-        # indicates responses can be compressed.
-        self._session.headers['Accept-Encoding'] = 'identity'
 
         if username or password:
             LOG.warning('Passing username and password to Connector is '
                         'deprecated. Authentication is passed through '
                         'set_auth now, support for these arguments will '
                         'be removed in the future')
             self.set_http_basic_auth(username, password)
@@ -111,15 +102,16 @@
             **extra_session_req_kwargs):
         """Generic RESTful request handler.
 
         :param method: The HTTP method to be used, e.g: GET, POST,
             PUT, PATCH, etc...
         :param path: The sub-URI or absolute URL path to the resource.
         :param data: Optional JSON data.
-        :param headers: Optional dictionary of headers.
+        :param headers: Optional dictionary of headers. Use None value
+                        to remove a default header.
         :param blocking: Whether to block for asynchronous operations.
         :param timeout: Max time in seconds to wait for blocking async call or
                         for requests library to connect and read. If a custom
                         timeout for requests is provided in
                         extra_session_req_kwargs, it will be used instead for
                         those calls.
         :param server_side_retries_left: Remaining retries. If not provided
@@ -134,20 +126,33 @@
         :raises: HTTPError
         """
         if server_side_retries_left is None:
             server_side_retries_left = self._server_side_retries
 
         url = path if urlparse.urlparse(path).netloc else urlparse.urljoin(
             self._url, path)
-        headers = headers or {}
+        headers = (headers or {}).copy()
         lc_headers = [k.lower() for k in headers]
         if data is not None and 'content-type' not in lc_headers:
             headers['Content-Type'] = 'application/json'
         if 'odata-version' not in lc_headers:
             headers['OData-Version'] = '4.0'
+        # NOTE(TheJulia): Depending on the BMC, offering compression as an
+        # acceptable response changes the ETag behavior to offering an
+        # automatic "weak" ETag response, which is appropriate because the
+        # body content *may* not be a byte for byte match given compression.
+        # Overall, the value of compression is less than the value of concise
+        # interaction with the BMC. Setting to identity basically means
+        # "without modification or compression". By default, python-requests
+        # indicates responses can be compressed.
+        if 'accept-encoding' not in lc_headers:
+            headers['Accept-Encoding'] = 'identity'
+        # Allow removing default headers
+        headers = {k: v for k, v in headers.items() if v is not None}
+
         # TODO(lucasagomes): We should mask the data to remove sensitive
         # information
         LOG.debug('HTTP request: %(method)s %(url)s; headers: %(headers)s; '
                   'body: %(data)s; blocking: %(blocking)s; timeout: '
                   '%(timeout)s; session arguments: %(session)s;',
                   {'method': method, 'url': url,
                    'headers': utils.sanitize(headers),
@@ -264,14 +269,29 @@
                 return self._op(
                     method, path, data=data, headers=headers,
                     blocking=blocking, timeout=timeout,
                     server_side_retries_left=server_side_retries_left,
                     **extra_session_req_kwargs)
             else:
                 raise
+        except exceptions.NotAcceptableError as e:
+            # NOTE(dtantsur): some HPE Gen 10 Plus machines do not allow
+            # identity encoding when fetching registries.
+            if (method.lower() == 'get'
+                    and headers.get('Accept-Encoding') == 'identity'):
+                LOG.warning('Server has indicated a NotAcceptable for %s, '
+                            'retrying without identity encoding', e)
+                headers = dict(headers, **{'Accept-Encoding': None})
+                return self._op(
+                    method, path, data=data, headers=headers,
+                    blocking=blocking, timeout=timeout,
+                    server_side_retries_left=server_side_retries_left,
+                    **extra_session_req_kwargs)
+            else:
+                raise
         if blocking and response.status_code == 202:
             if not response.headers.get('Location'):
                 m = ('HTTP response for %(method)s request to %(url)s '
                      'returned status 202, but no Location header'
                      % {'method': method, 'url': url})
                 raise exceptions.ConnectionError(url=url, error=m)
```

### Comparing `sushy-5.0.0/sushy/exceptions.py` & `sushy-5.1.0/sushy/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,18 @@
     pass
 
 
 class AccessError(HTTPError):
     pass
 
 
+class NotAcceptableError(HTTPError):
+    pass
+
+
 class MissingXAuthToken(HTTPError):
     message = ('No X-Auth-Token returned from remote host when '
                'attempting to establish a session. Error: %(error)s')
 
 
 def raise_for_response(method, url, response):
     """Raise a correct error class, if needed."""
@@ -172,11 +176,13 @@
     elif response.status_code == http_client.NOT_FOUND:
         raise ResourceNotFoundError(method, url, response)
     elif response.status_code == http_client.BAD_REQUEST:
         raise BadRequestError(method, url, response)
     elif response.status_code in (http_client.UNAUTHORIZED,
                                   http_client.FORBIDDEN):
         raise AccessError(method, url, response)
+    elif response.status_code == http_client.NOT_ACCEPTABLE:
+        raise NotAcceptableError(method, url, response)
     elif response.status_code >= http_client.INTERNAL_SERVER_ERROR:
         raise ServerSideError(method, url, response)
     else:
         raise HTTPError(method, url, response)
```

### Comparing `sushy-5.0.0/sushy/main.py` & `sushy-5.1.0/sushy/main.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/base.py` & `sushy-5.1.0/sushy/resources/base.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/certificateservice/certificate.py` & `sushy-5.1.0/sushy/resources/certificateservice/certificate.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/certificateservice/certificateservice.py` & `sushy-5.1.0/sushy/resources/certificateservice/certificateservice.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/certificateservice/constants.py` & `sushy-5.1.0/sushy/resources/certificateservice/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/chassis/chassis.py` & `sushy-5.1.0/sushy/resources/chassis/chassis.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/chassis/constants.py` & `sushy-5.1.0/sushy/resources/chassis/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/chassis/power/constants.py` & `sushy-5.1.0/sushy/resources/chassis/power/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/chassis/power/power.py` & `sushy-5.1.0/sushy/resources/chassis/power/power.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/chassis/thermal/constants.py` & `sushy-5.1.0/sushy/resources/chassis/thermal/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/chassis/thermal/thermal.py` & `sushy-5.1.0/sushy/resources/chassis/thermal/thermal.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/common.py` & `sushy-5.1.0/sushy/resources/common.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/compositionservice/compositionservice.py` & `sushy-5.1.0/sushy/resources/compositionservice/compositionservice.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/compositionservice/constants.py` & `sushy-5.1.0/sushy/resources/compositionservice/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/compositionservice/resourceblock.py` & `sushy-5.1.0/sushy/resources/compositionservice/resourceblock.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/compositionservice/resourcezone.py` & `sushy-5.1.0/sushy/resources/compositionservice/resourcezone.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/constants.py` & `sushy-5.1.0/sushy/resources/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/eventservice/constants.py` & `sushy-5.1.0/sushy/resources/eventservice/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/eventservice/eventdestination.py` & `sushy-5.1.0/sushy/resources/eventservice/eventdestination.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/eventservice/eventservice.py` & `sushy-5.1.0/sushy/resources/eventservice/eventservice.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/fabric/constants.py` & `sushy-5.1.0/sushy/resources/fabric/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/fabric/endpoint.py` & `sushy-5.1.0/sushy/resources/fabric/endpoint.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/fabric/fabric.py` & `sushy-5.1.0/sushy/resources/fabric/fabric.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/ipaddresses.py` & `sushy-5.1.0/sushy/resources/ipaddresses.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/manager/constants.py` & `sushy-5.1.0/sushy/resources/manager/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/manager/manager.py` & `sushy-5.1.0/sushy/resources/manager/manager.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/manager/virtual_media.py` & `sushy-5.1.0/sushy/resources/manager/virtual_media.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/oem/__init__.py` & `sushy-5.1.0/sushy/resources/oem/__init__.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/oem/base.py` & `sushy-5.1.0/sushy/resources/oem/base.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/oem/common.py` & `sushy-5.1.0/sushy/resources/oem/common.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/oem/fake.py` & `sushy-5.1.0/sushy/resources/oem/fake.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/registry/attribute_registry.py` & `sushy-5.1.0/sushy/resources/registry/attribute_registry.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/registry/constants.py` & `sushy-5.1.0/sushy/resources/registry/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/registry/message_registry.py` & `sushy-5.1.0/sushy/resources/registry/message_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
 
 def parse_message(message_registries, message_field):
     """Parse the messages in registries and substitute any params
 
     Check only registries that support messages.
 
-    :param registries: dict of Message Registries
+    :param message_registries: dict of Message Registries
     :param message_field: settings.MessageListField to parse
 
     :returns: parsed settings.MessageListField with missing attributes filled
     """
 
     reg_msg = None
     if '.' in message_field.message_id:
```

### Comparing `sushy-5.0.0/sushy/resources/registry/message_registry_file.py` & `sushy-5.1.0/sushy/resources/registry/message_registry_file.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/sessionservice/session.py` & `sushy-5.1.0/sushy/resources/sessionservice/session.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/sessionservice/sessionservice.py` & `sushy-5.1.0/sushy/resources/sessionservice/sessionservice.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/settings.py` & `sushy-5.1.0/sushy/resources/settings.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/system/bios.py` & `sushy-5.1.0/sushy/resources/system/bios.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/system/constants.py` & `sushy-5.1.0/sushy/resources/system/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/system/ethernet_interface.py` & `sushy-5.1.0/sushy/resources/system/ethernet_interface.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/system/network/adapter.py` & `sushy-5.1.0/sushy/resources/system/network/adapter.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/system/network/constants.py` & `sushy-5.1.0/sushy/resources/system/network/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/system/network/device_function.py` & `sushy-5.1.0/sushy/resources/system/network/device_function.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/system/network/port.py` & `sushy-5.1.0/sushy/resources/system/network/port.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/system/processor.py` & `sushy-5.1.0/sushy/resources/system/processor.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/system/secure_boot.py` & `sushy-5.1.0/sushy/resources/system/secure_boot.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/system/secure_boot_database.py` & `sushy-5.1.0/sushy/resources/system/secure_boot_database.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/system/simple_storage.py` & `sushy-5.1.0/sushy/resources/system/simple_storage.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/system/storage/constants.py` & `sushy-5.1.0/sushy/resources/system/storage/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/system/storage/controller.py` & `sushy-5.1.0/sushy/resources/system/storage/controller.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/system/storage/drive.py` & `sushy-5.1.0/sushy/resources/system/storage/drive.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/system/storage/storage.py` & `sushy-5.1.0/sushy/resources/system/storage/storage.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/system/storage/volume.py` & `sushy-5.1.0/sushy/resources/system/storage/volume.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/system/system.py` & `sushy-5.1.0/sushy/resources/system/system.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/taskservice/constants.py` & `sushy-5.1.0/sushy/resources/taskservice/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/taskservice/task.py` & `sushy-5.1.0/sushy/resources/taskservice/task.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/taskservice/taskservice.py` & `sushy-5.1.0/sushy/resources/taskservice/taskservice.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/updateservice/constants.py` & `sushy-5.1.0/sushy/resources/updateservice/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/updateservice/softwareinventory.py` & `sushy-5.1.0/sushy/resources/updateservice/softwareinventory.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/resources/updateservice/updateservice.py` & `sushy-5.1.0/sushy/resources/updateservice/updateservice.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/standard_registries/Base.1.0.0.json` & `sushy-5.1.0/sushy/standard_registries/Base.1.0.0.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/standard_registries/Base.1.2.0.json` & `sushy-5.1.0/sushy/standard_registries/Base.1.2.0.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/standard_registries/Base.1.3.0.json` & `sushy-5.1.0/sushy/standard_registries/Base.1.3.0.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/standard_registries/Base.1.3.1.json` & `sushy-5.1.0/sushy/standard_registries/Base.1.3.1.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/standard_registries/Base.1.4.0.json` & `sushy-5.1.0/sushy/standard_registries/Base.1.4.0.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/taskmonitor.py` & `sushy-5.1.0/sushy/taskmonitor.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/base.py` & `sushy-5.1.0/sushy/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/TestRegistry.zip` & `sushy-5.1.0/sushy/tests/unit/json_samples/TestRegistry.zip`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/bios.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/bios.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/bios_attribute_registry.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/bios_attribute_registry.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/bios_attribute_registry_file.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/bios_attribute_registry_file.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/bios_attribute_registry_file_zthardware.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/bios_attribute_registry_file_zthardware.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/bios_attribute_registry_zthardware.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/bios_attribute_registry_zthardware.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/bios_settings.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/bios_settings.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/bios_zt.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/bios_zt.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/certificate.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/certificate.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/certificate_collection.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/certificate_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/certificate_locations.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/certificate_locations.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/certificateservice.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/certificateservice.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/chassis.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/chassis.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/chassis_collection.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/chassis_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/compositionservice.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/compositionservice.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/drive.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/drive.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/drive2.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/drive2.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/drive3.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/drive3.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/endpoint.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/endpoint.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/error.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/error.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/error_single_ext_info.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/error_single_ext_info.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/ethernet_interfaces.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/ethernet_interfaces.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/ethernet_interfaces_collection.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/ethernet_interfaces_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/eventservice.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/eventservice.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/fabric.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/fabric.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/fabric_collection.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/fabric_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/firmwareinventory_collection.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/firmwareinventory_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/manager.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/manager.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/manager_collection.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/manager_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/managerv1_18.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/managerv1_18.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/message_registry.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/message_registry.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/message_registry_file.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/message_registry_file.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/network_adapter.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/network_adapter.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/network_device_function.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/network_device_function.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/network_device_function_collection.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/network_device_function_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/network_port.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/network_port.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/network_port_collection.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/network_port_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/power.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/power.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/processor.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/processor.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/processor2.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/processor2.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/processor_collection.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/processor_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/resourceblock.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/resourceblock.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/resourcezone.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/resourcezone.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/root.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/root.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/secure_boot.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/secure_boot.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/secure_boot_database.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/secure_boot_database.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/secure_boot_database_collection.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/secure_boot_database_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/session.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/session.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/session_creation_headers.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/session_creation_headers.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/session_creation_headers_no_location.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/session_creation_headers_no_location.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/session_error.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/session_error.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/session_service.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/session_service.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/settings-body-nokia.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/settings-body-nokia.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/settings.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/settings.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/simple_storage.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/simple_storage.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/simple_storage_collection.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/simple_storage_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/softwareinventory.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/softwareinventory.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/storage.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/storage.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/storage_collection.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/storage_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/storage_controller.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/storage_controller.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/storage_controller_collection.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/storage_controller_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/system.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/system.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/system_collection.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/system_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/systemv1_20.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/systemv1_20.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/task.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/task.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/task_monitor.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/task_monitor.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/taskservice.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/taskservice.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/thermal.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/thermal.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/transfer_proto_required_error.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/transfer_proto_required_error.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/transfer_proto_required_error3.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/transfer_proto_required_error3.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/updateservice.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/updateservice.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/updateservice_no_inv.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/updateservice_no_inv.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/virtual_media.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/virtual_media.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/virtual_media_collection.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/virtual_media_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/virtual_mediav1_6.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/virtual_mediav1_6.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/volume.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/volume.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/volume2.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/volume2.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/volume3.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/volume3.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/volume4.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/volume4.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/json_samples/volume_collection.json` & `sushy-5.1.0/sushy/tests/unit/json_samples/volume_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/certificateservice/test_certificate.py` & `sushy-5.1.0/sushy/tests/unit/resources/certificateservice/test_certificate.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/certificateservice/test_certificateservice.py` & `sushy-5.1.0/sushy/tests/unit/resources/certificateservice/test_certificateservice.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/chassis/test_chassis.py` & `sushy-5.1.0/sushy/tests/unit/resources/chassis/test_chassis.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/chassis/test_power.py` & `sushy-5.1.0/sushy/tests/unit/resources/chassis/test_power.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/chassis/test_thermal.py` & `sushy-5.1.0/sushy/tests/unit/resources/chassis/test_thermal.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/compositionservice/test_compositionservice.py` & `sushy-5.1.0/sushy/tests/unit/resources/compositionservice/test_compositionservice.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/compositionservice/test_resourceblock.py` & `sushy-5.1.0/sushy/tests/unit/resources/compositionservice/test_resourceblock.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/compositionservice/test_resourcezone.py` & `sushy-5.1.0/sushy/tests/unit/resources/compositionservice/test_resourcezone.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/eventservice/test_evendestination.py` & `sushy-5.1.0/sushy/tests/unit/resources/eventservice/test_evendestination.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/eventservice/test_eventservice.py` & `sushy-5.1.0/sushy/tests/unit/resources/eventservice/test_eventservice.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/fabric/test_endpoint.py` & `sushy-5.1.0/sushy/tests/unit/resources/fabric/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/fabric/test_fabric.py` & `sushy-5.1.0/sushy/tests/unit/resources/fabric/test_fabric.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/manager/test_manager.py` & `sushy-5.1.0/sushy/tests/unit/resources/manager/test_manager.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/manager/test_virtual_media.py` & `sushy-5.1.0/sushy/tests/unit/resources/manager/test_virtual_media.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/oem/test_common.py` & `sushy-5.1.0/sushy/tests/unit/resources/oem/test_common.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/oem/test_fake.py` & `sushy-5.1.0/sushy/tests/unit/resources/oem/test_fake.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/registry/test_attribute_registry.py` & `sushy-5.1.0/sushy/tests/unit/resources/registry/test_attribute_registry.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/registry/test_message_registry.py` & `sushy-5.1.0/sushy/tests/unit/resources/registry/test_message_registry.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/registry/test_message_registry_file.py` & `sushy-5.1.0/sushy/tests/unit/resources/registry/test_message_registry_file.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/sessionservice/test_session.py` & `sushy-5.1.0/sushy/tests/unit/resources/sessionservice/test_session.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/sessionservice/test_sessionservice.py` & `sushy-5.1.0/sushy/tests/unit/resources/sessionservice/test_sessionservice.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/system/network/test_adapter.py` & `sushy-5.1.0/sushy/tests/unit/resources/system/network/test_adapter.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/system/network/test_device_function.py` & `sushy-5.1.0/sushy/tests/unit/resources/system/network/test_device_function.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/system/network/test_port.py` & `sushy-5.1.0/sushy/tests/unit/resources/system/network/test_port.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/system/storage/test_controller.py` & `sushy-5.1.0/sushy/tests/unit/resources/system/storage/test_controller.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/system/storage/test_drive.py` & `sushy-5.1.0/sushy/tests/unit/resources/system/storage/test_drive.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/system/storage/test_storage.py` & `sushy-5.1.0/sushy/tests/unit/resources/system/storage/test_storage.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/system/storage/test_volume.py` & `sushy-5.1.0/sushy/tests/unit/resources/system/storage/test_volume.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/system/test_bios.py` & `sushy-5.1.0/sushy/tests/unit/resources/system/test_bios.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/system/test_ethernet_interfaces.py` & `sushy-5.1.0/sushy/tests/unit/resources/system/test_ethernet_interfaces.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/system/test_processor.py` & `sushy-5.1.0/sushy/tests/unit/resources/system/test_processor.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/system/test_secure_boot.py` & `sushy-5.1.0/sushy/tests/unit/resources/system/test_secure_boot.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/system/test_secure_boot_database.py` & `sushy-5.1.0/sushy/tests/unit/resources/system/test_secure_boot_database.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/system/test_simple_storage.py` & `sushy-5.1.0/sushy/tests/unit/resources/system/test_simple_storage.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/system/test_system.py` & `sushy-5.1.0/sushy/tests/unit/resources/system/test_system.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/taskservice/test_task.py` & `sushy-5.1.0/sushy/tests/unit/resources/taskservice/test_task.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/taskservice/test_taskservice.py` & `sushy-5.1.0/sushy/tests/unit/resources/taskservice/test_taskservice.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/test_base.py` & `sushy-5.1.0/sushy/tests/unit/resources/test_base.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/test_settings.py` & `sushy-5.1.0/sushy/tests/unit/resources/test_settings.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/updateservice/test_softwareinventory.py` & `sushy-5.1.0/sushy/tests/unit/resources/updateservice/test_softwareinventory.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/resources/updateservice/test_updateservice.py` & `sushy-5.1.0/sushy/tests/unit/resources/updateservice/test_updateservice.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/test_auth.py` & `sushy-5.1.0/sushy/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/test_connector.py` & `sushy-5.1.0/sushy/tests/unit/test_connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -164,62 +164,77 @@
         self.auth = mock_auth
         super(ConnectorOpTestCase, self).setUp()
         self.conn = connector.Connector(
             'http://foo.bar:1234', verify=True,
             server_side_retries=10, server_side_retries_delay=3)
         self.conn._auth = mock_auth
         self.data = {'fake': 'data'}
-        self.headers = {'X-Fake': 'header'}
+        self.headers = {'Accept-Encoding': 'identity', 'OData-Version': '4.0'}
         self.session = mock.Mock(spec=requests.Session)
         self.conn._session = self.session
         self.request = self.session.request
         self.request.return_value.status_code = http_client.OK
 
     def test_ok_get(self):
-        self.conn._op('GET', path='fake/path', headers=self.headers)
+        self.conn._op('GET', path='fake/path')
         self.request.assert_called_once_with(
             'GET', 'http://foo.bar:1234/fake/path',
             headers=self.headers, json=None, verify=True, timeout=60)
 
+    def test_ok_get_with_headers(self):
+        self.conn._op('GET', path='fake/path', headers={'answer': '42'})
+        self.request.assert_called_once_with(
+            'GET', 'http://foo.bar:1234/fake/path',
+            headers=dict(self.headers, answer='42'),
+            json=None, verify=True, timeout=60)
+
     def test_response_callback(self):
         mock_response_callback = mock.MagicMock()
         self.conn._response_callback = mock_response_callback
 
         self.conn._op('GET', path='fake/path', headers=self.headers)
         self.assertEqual(1, mock_response_callback.call_count)
 
     def test_ok_get_url_redirect_false(self):
-        self.conn._op('GET', path='fake/path', headers=self.headers,
-                      allow_redirects=False)
+        self.conn._op('GET', path='fake/path', allow_redirects=False)
         self.request.assert_called_once_with(
             'GET', 'http://foo.bar:1234/fake/path',
             headers=self.headers, json=None, allow_redirects=False,
             verify=True, timeout=60)
 
     def test_ok_post(self):
+        self.conn._op('POST', path='fake/path', data=self.data.copy())
+        self.request.assert_called_once_with(
+            'POST', 'http://foo.bar:1234/fake/path',
+            json=self.data,
+            headers=dict(self.headers, **{'Content-Type': 'application/json'}),
+            verify=True, timeout=60)
+
+    def test_ok_post_with_headers(self):
         self.conn._op('POST', path='fake/path', data=self.data.copy(),
-                      headers=self.headers)
+                      headers={'answer': 42})
         self.request.assert_called_once_with(
             'POST', 'http://foo.bar:1234/fake/path',
-            json=self.data, headers=self.headers, verify=True, timeout=60)
+            json=self.data,
+            headers=dict(self.headers, **{'Content-Type': 'application/json',
+                                          'answer': 42}),
+            verify=True, timeout=60)
 
     def test_ok_put(self):
-        self.conn._op('PUT', path='fake/path', data=self.data.copy(),
-                      headers=self.headers)
+        self.conn._op('PUT', path='fake/path', data=self.data.copy())
         self.request.assert_called_once_with(
             'PUT', 'http://foo.bar:1234/fake/path',
-            json=self.data, headers=self.headers, verify=True, timeout=60)
+            headers=dict(self.headers, **{'Content-Type': 'application/json'}),
+            json=self.data, verify=True, timeout=60)
 
     def test_ok_delete(self):
-        expected_headers = self.headers.copy()
-        expected_headers['OData-Version'] = '4.0'
-        self.conn._op('DELETE', path='fake/path', headers=self.headers.copy())
+        self.conn._op('DELETE', path='fake/path')
         self.request.assert_called_once_with(
             'DELETE', 'http://foo.bar:1234/fake/path',
-            headers=expected_headers, json=None, verify=True, timeout=60)
+            headers=self.headers, json=None, verify=True, timeout=60)
 
     def test_ok_post_with_session(self):
         self.conn._session.headers = {}
         self.conn._session.headers['X-Auth-Token'] = 'asdf1234'
         expected_headers = self.headers.copy()
         expected_headers['OData-Version'] = '4.0'
         expected_headers['Content-Type'] = 'application/json'
@@ -238,30 +253,31 @@
         expected_headers['OData-Version'] = '4.0'
         self.request.reset_mock()
         self.conn._op('GET', path=path, headers=headers)
         self.request.assert_called_once_with(
             'GET', 'http://foo.bar:1234' + path,
             headers=expected_headers, json=None, verify=True, timeout=60)
 
-    def test_odata_version_header_redfish_no_headers(self):
-        path = '/redfish/v1/bar'
-        expected_headers = {'OData-Version': '4.0'}
-        self.conn._op('GET', path=path)
+    def test_odata_version_header_redfish_existing_header(self):
+        path = '/redfish/v1/foo'
+        headers = {'OData-Version': '3.0'}
+        expected_headers = dict(self.headers, **headers)
+        self.conn._op('GET', path=path, headers=headers)
         self.request.assert_called_once_with(
             'GET', 'http://foo.bar:1234' + path,
             headers=expected_headers, json=None, verify=True, timeout=60)
 
-    def test_odata_version_header_redfish_existing_header(self):
+    def test_remove_header_accept_encoding(self):
         path = '/redfish/v1/foo'
-        headers = {'OData-Version': '3.0'}
-        expected_headers = dict(headers)
+        headers = {'Accept-Encoding': None}
+        self.headers.pop('Accept-Encoding')
         self.conn._op('GET', path=path, headers=headers)
         self.request.assert_called_once_with(
             'GET', 'http://foo.bar:1234' + path,
-            headers=expected_headers, json=None, verify=True, timeout=60)
+            headers=self.headers, json=None, verify=True, timeout=60)
 
     def test_timed_out_session_unable_to_create_session(self):
         self.conn._auth.can_refresh_session.return_value = False
         self.session.auth = None
         self.conn._session = self.session
         self.request = self.session.request
         self.request.return_value.status_code = http_client.FORBIDDEN
@@ -518,14 +534,37 @@
                 method='DELETE', url='http://foo.bar', response=mock_error)
 
         self.assertRaises(exceptions.ServerSideError, self.conn._op, 'DELETE',
                           'http://foo.bar')
         self.assertEqual(0, mock_sleep.call_count)
         self.assertEqual(1, self.request.call_count)
 
+    def test_op_retry_without_identity(self):
+        self.request.side_effect = [
+            mock.Mock(status_code=http_client.NOT_ACCEPTABLE),
+            mock.Mock(status_code=http_client.OK),
+        ]
+        self.conn._op('GET', 'http://foo.bar')
+
+        self.assertEqual(2, self.request.call_count)
+        headers_no_accept = self.headers.copy()
+        headers_no_accept.pop('Accept-Encoding')
+        self.request.assert_has_calls([
+            mock.call('GET', 'http://foo.bar', headers=self.headers,
+                      json=None, verify=True, timeout=60),
+            mock.call('GET', 'http://foo.bar', headers=headers_no_accept,
+                      json=None, verify=True, timeout=60),
+        ])
+
+    def test_op_retry_without_identity_fails(self):
+        self.request.return_value.status_code = http_client.NOT_ACCEPTABLE
+        self.assertRaises(exceptions.NotAcceptableError, self.conn._op,
+                          'GET', 'http://foo.bar')
+        self.assertEqual(2, self.request.call_count)
+
     def test_access_error(self):
         self.conn._auth = None
 
         self.request.return_value.status_code = http_client.FORBIDDEN
         self.request.return_value.json.side_effect = ValueError('no json')
 
         with self.assertRaisesRegex(exceptions.AccessError,
@@ -711,16 +750,15 @@
                                 blocking=False, timeout=60)
         mock__op.assert_called_once_with(
             self.conn,
             "PATCH",
             '/redfish/v1/Systems/1',
             data={'Boot': {'BootSourceOverrideTarget': 'Cd',
                            'BootSourceOverrideEnabled': 'Once'}},
-            headers={'X-Fake': 'header',
-                     'If-Match': '"3d7b8a7360bf2941d"'},
+            headers=dict(self.headers, **{'If-Match': '"3d7b8a7360bf2941d"'}),
             blocking=False,
             timeout=60)
 
     @mock.patch.object(connector.Connector, '_op', autospec=True)
     def test_etag_handler_weak_etag_ok(self, mock__op):
         self.headers['If-Match'] = 'W/"3d7b8a7360bf2941d"'
         response = mock.MagicMock(spec=requests.Response)
@@ -734,16 +772,16 @@
                                 blocking=False, timeout=60)
         mock__op.assert_called_once_with(
             self.conn,
             "PATCH",
             '/redfish/v1/Systems/1',
             data={'Boot': {'BootSourceOverrideTarget': 'Cd',
                            'BootSourceOverrideEnabled': 'Once'}},
-            headers={'X-Fake': 'header',
-                     'If-Match': 'W/"3d7b8a7360bf2941d"'},
+            headers=dict(self.headers,
+                         **{'If-Match': 'W/"3d7b8a7360bf2941d"'}),
             blocking=False,
             timeout=60)
 
     @mock.patch.object(connector.Connector, '_op', autospec=True)
     def test_etag_handler_no_etag_ok(self, mock__op):
         response = mock.MagicMock(spec=requests.Response)
         response.status_code = http_client.OK
@@ -755,15 +793,15 @@
                                 blocking=False, timeout=60)
         mock__op.assert_called_once_with(
             self.conn,
             "PATCH",
             '/redfish/v1/Systems/1',
             data={'Boot': {'BootSourceOverrideTarget': 'Cd',
                            'BootSourceOverrideEnabled': 'Once'}},
-            headers={'X-Fake': 'header'},
+            headers=self.headers,
             blocking=False,
             timeout=60)
 
     @mock.patch.object(connector.Connector, '_op', autospec=True)
     def test_etag_handler_weak_etag_fallback_to_strong(self, mock__op):
         self.headers['If-Match'] = 'W/"3d7b8a7360bf2941d"'
         target_uri = '/redfish/v1/Systems/1'
@@ -783,16 +821,15 @@
                                 blocking=False, timeout=60)
         mock__op.assert_called_with(
             self.conn,
             "PATCH",
             '/redfish/v1/Systems/1',
             data={'Boot': {'BootSourceOverrideTarget': 'Cd',
                            'BootSourceOverrideEnabled': 'Once'}},
-            headers={'X-Fake': 'header',
-                     'If-Match': '"3d7b8a7360bf2941d"'},
+            headers=dict(self.headers, **{'If-Match': '"3d7b8a7360bf2941d"'}),
             blocking=False,
             timeout=60)
 
     @mock.patch.object(connector.Connector, '_op', autospec=True)
     def test_etag_handler_weak_etag_fallback_to_no_etag(self, mock__op):
         self.headers['If-Match'] = 'W/"3d7b8a7360bf2941d"'
         target_uri = '/redfish/v1/Systems/1'
@@ -814,15 +851,15 @@
                                 blocking=False, timeout=60)
         mock__op.assert_called_with(
             self.conn,
             "PATCH",
             '/redfish/v1/Systems/1',
             data={'Boot': {'BootSourceOverrideTarget': 'Cd',
                            'BootSourceOverrideEnabled': 'Once'}},
-            headers={'X-Fake': 'header'},
+            headers=self.headers,
             blocking=False,
             timeout=60)
 
     @mock.patch.object(connector.Connector, '_op', autospec=True)
     def test_etag_handler_strong_etag_fallback_to_no_etag(self, mock__op):
         self.headers['If-Match'] = '"3d7b8a7360bf2941d"'
         target_uri = '/redfish/v1/Systems/1'
@@ -842,15 +879,15 @@
                                 blocking=False, timeout=60)
         mock__op.assert_called_with(
             self.conn,
             "PATCH",
             '/redfish/v1/Systems/1',
             data={'Boot': {'BootSourceOverrideTarget': 'Cd',
                            'BootSourceOverrideEnabled': 'Once'}},
-            headers={'X-Fake': 'header'},
+            headers=self.headers,
             blocking=False,
             timeout=60)
 
     @mock.patch.object(connector.Connector, '_op', autospec=True)
     def test_etag_handler_fail_other_exception(self, mock__op):
         self.headers['If-Match'] = 'W/"3d7b8a7360bf2941d"'
         target_uri = '/redfish/v1/Systems/1'
```

### Comparing `sushy-5.0.0/sushy/tests/unit/test_main.py` & `sushy-5.1.0/sushy/tests/unit/test_main.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/test_taskmonitor.py` & `sushy-5.1.0/sushy/tests/unit/test_taskmonitor.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/tests/unit/test_utils.py` & `sushy-5.1.0/sushy/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy/utils.py` & `sushy-5.1.0/sushy/utils.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/sushy.egg-info/PKG-INFO` & `sushy-5.1.0/sushy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sushy
-Version: 5.0.0
+Version: 5.1.0
 Summary: Sushy is a small Python library to communicate with Redfish based systems
 Home-page: https://docs.openstack.org/sushy/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Overview
         ========
```

### Comparing `sushy-5.0.0/sushy.egg-info/SOURCES.txt` & `sushy-5.1.0/sushy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 doc/source/conf.py
 doc/source/index.rst
 doc/source/contributor/index.rst
 doc/source/install/index.rst
 doc/source/reference/index.rst
 doc/source/reference/usage.rst
 releasenotes/notes/.placeholder
+releasenotes/notes/accept-encoding-4646ea43998f80bd.yaml
 releasenotes/notes/action-parameter-missing-7d234b96b5b1d81a.yaml
 releasenotes/notes/add-apply-time-support-to-bios-315ebad429dcab3d.yaml
 releasenotes/notes/add-bios-bf69ac56c4ae8f50.yaml
 releasenotes/notes/add-bios-update-status-cc59816c374b78e4.yaml
 releasenotes/notes/add-chassis-linkage-d8e567f9c791169d.yaml
 releasenotes/notes/add-chassis-support-5b97daffe1c61a2b.yaml
 releasenotes/notes/add-custom-connector-support-0a49c6649d5f7eaf.yaml
@@ -147,14 +148,15 @@
 releasenotes/notes/use-settingsobject-if-supported-12a332f9905d64ce.yaml
 releasenotes/notes/vmedia-1.4.0-9957460fed59d85c.yaml
 releasenotes/notes/vmedia-certificate-06c367c6ef33d139.yaml
 releasenotes/notes/vmedia-credentials-14b7705c3c94cc07.yaml
 releasenotes/notes/workaround-sushy-requests-verify-handling-6879c273b651246f.yaml
 releasenotes/source/2023.1.rst
 releasenotes/source/2023.2.rst
+releasenotes/source/2024.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/stein.rst
 releasenotes/source/train.rst
```

### Comparing `sushy-5.0.0/tools/generate-enum.py` & `sushy-5.1.0/tools/generate-enum.py`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/tox.ini` & `sushy-5.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/zuul.d/project.yaml` & `sushy-5.1.0/zuul.d/project.yaml`

 * *Files identical despite different names*

### Comparing `sushy-5.0.0/zuul.d/sushy-jobs.yaml` & `sushy-5.1.0/zuul.d/sushy-jobs.yaml`

 * *Files identical despite different names*

