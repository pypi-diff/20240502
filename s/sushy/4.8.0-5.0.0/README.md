# Comparing `tmp/sushy-4.8.0.tar.gz` & `tmp/sushy-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sushy-4.8.0.tar", last modified: Tue Jan 16 16:34:01 2024, max compression
+gzip compressed data, was "sushy-5.0.0.tar", last modified: Thu Feb 22 15:01:13 2024, max compression
```

## Comparing `sushy-4.8.0.tar` & `sushy-5.0.0.tar`

### file list

```diff
@@ -1,485 +1,487 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.103367 sushy-4.8.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-01-16 16:33:28.000000 sushy-4.8.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-01-16 16:33:28.000000 sushy-4.8.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2024-01-16 16:33:28.000000 sushy-4.8.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2877 2024-01-16 16:34:00.000000 sushy-4.8.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-01-16 16:33:28.000000 sushy-4.8.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17557 2024-01-16 16:34:00.000000 sushy-4.8.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-01-16 16:33:28.000000 sushy-4.8.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-01-16 16:33:28.000000 sushy-4.8.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2279 2024-01-16 16:34:01.103367 sushy-4.8.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2024-01-16 16:33:28.000000 sushy-4.8.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-01-16 16:33:28.000000 sushy-4.8.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.043368 sushy-4.8.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-01-16 16:33:28.000000 sushy-4.8.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.043368 sushy-4.8.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3047 2024-01-16 16:33:28.000000 sushy-4.8.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.043368 sushy-4.8.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3141 2024-01-16 16:33:28.000000 sushy-4.8.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2024-01-16 16:33:28.000000 sushy-4.8.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.043368 sushy-4.8.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2024-01-16 16:33:28.000000 sushy-4.8.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.043368 sushy-4.8.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2024-01-16 16:33:28.000000 sushy-4.8.0/doc/source/reference/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10228 2024-01-16 16:33:28.000000 sushy-4.8.0/doc/source/reference/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.039368 sushy-4.8.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.063367 sushy-4.8.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-apply-time-support-to-bios-315ebad429dcab3d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-bios-bf69ac56c4ae8f50.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-bios-update-status-cc59816c374b78e4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-chassis-linkage-d8e567f9c791169d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-chassis-support-5b97daffe1c61a2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-custom-connector-support-0a49c6649d5f7eaf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-default-identity-10c5dd23bed0e915.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-drive-led-97b687013fec88c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-drive-revision-a0c069fff236479d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-drive-volumes-971d80644c3bd1e0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-endpoint-subresource-to-fabric-b03e5fd99ece1bf4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-fabric-support-1520f7fcb0e12539.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-http-boot-uri-support-5c25816e13ccdb27.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-initial-redfish-oem-extension-support-50c9849bb7b6b25c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-mapped-list-field-04c671f7a73d83f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-network-adapter-26d01d8d9fb1d7ad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-network-device-function-and-port-e880d8f461e3723d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-odata-version-header-96dc8179c0e2e9bd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-partial-key-match-27bed73d577b1187.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-power-resource-e141ddf298673305.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-processor-id-and-status-b81d4c6e6c14c25f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-raid-type-properties-2090da5bea37c660.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-read-and-connect-timeout-9f7dc3ed63c192c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-response-cb-65d448ee2690d0b2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-simple-storage-915464811737bb05.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-storage-and-simple-storage-attributes-to-system-16e81f9b15b1897d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-storage-da766d3dbf9fb385.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-sushy-root-to-resources-1f221794557aa5fc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-system-bootprogress-42ee452cfa279c63.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-system-manager-linkage-86be69c9df4cb359.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-system-status-field-41b3f2a8c4b85f38.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-system-type-mapping-bf456c5c15a90877.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-task-monitor-support-21f711927ad6ec91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-task-service-c751ce51e0b8dc11.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-thermal-resource-5c965a3c940f9028.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add-virtual-media-support-f522fbec4420341c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add_composition_service-84750d8d1d96474a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add_ethernet_interface-df308f814f0e4bce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add_keyword_argument_for_connector-cea5dc4e6c01b548.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add_product_and_protocol_features_supported-59de3f89b7382434.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/add_update_service-b54c9bb0177e3468.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/allow_empty_context_eventdestination-9a96c34dd7edbeca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/apply-time-support-for-volume-ops-f2ebc412e3b4290a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/bios-attribute-registry-a55c2d81c730a795.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/bug-1754514-ca6ebe16c4e4b3b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/catch-general-requests-exceptions-b5fd706597708fb6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/certificate-collection-acc67488c240274c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/change-bootdev-smc-ab30317eaf5c37d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/change-vmedia-write-protected-attr-586370a552288801.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/check-for-boot-attrs-in-settingsuri-1cad07b6eb1c81b3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/config-server-side-retries-d16824019bd709a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/decouple-boot-params-c75e80f5951abb12.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/deprecate-system-leds-f1a72422c53d281e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/disable-conn-pooling-3456782afe56ac94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      807 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/do-not-offer-compression-encoding-884ca8a7458cb096.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/drop-py-2-7-cc931c210ce08e33.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/enhance-oem-extension-design-3143717e710b3eaf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/enhance-storage-volume-drive-support-16314d30f3631fb3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/enums-3aff03d940012f33.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/event-service-d6607420effc3df8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/expand-drive-schema-042901f919be646c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-2008198-bios-factory-reset-400-bad-request-3f4a7a2aada0835b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-eject-media-empty-dict-573b4c9e06f52ce7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-exceeding-retries-663ab543cc14f261.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-extended-info-error-handling-73fecb6bf5c852ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-insert-media-payload-b5d4c707f81d9603.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-malformed-boot-mode-1ba1117cad8dcc47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-manager-action-d71fd415cea29aa6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-missing-etags-ded8c0bb31fafef7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-oem-loading-52da045252b6c33e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-refine-resource-refresh-86c21ce230967251.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-required-oem-attribute-parsing-205e4186275aa293.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-retry_volume_operation-on_sys518-009f2b16e5c38a27.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-return-full-weak-etag-04265472cbea9c0e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-simple-storage-device-capacity-bytes-null-0672eed36d9da70a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-simple-update-e88838fab4170920.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-software-firmware-inventory-3e0e79e052aa76d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-subprocessors-3b619434dba4636d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-taskmonitor-init-calls-in-volume-module-0f8a747acd0cfe3f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-to-close-session-on-dealloc-c3687d4dcb1441b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-update-service-constants-b8c3f48ccee6ce1f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-use-headers-for-options-736940b87c06c189.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-virtual-media-fallback-15a559414a65c014.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-volume-actions-not-required-730fd637dd2587ce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fix-volume-delete-configuration-unsuported-operational_time_property-f53f650d8612a847.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/fixes-ilo5-redfish-firmware-update-issue-273862b2a11e3536.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/get-retry-9ca311caf8a0b7bb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/handle-basic-auth-access-errors-393b368b31f5cad2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/handle_transfer_method-a51d5a17e381ebee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/health_literals_change-0e3fc0c439b765e3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/increase-server-retries-5f11edde8ee0b461.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/indicator-led-mappings-e7b34da03f6abb06.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/lazily-load-registries-0e9441e435c2471d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/make-leds-settable-c82cb513de0171f5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/make-volume-ops-blocking-de5c2ae032041d5d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/message-parsing-resilience-534da532515a15da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/message-registry-logging-39624ae114c02e15.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/monitor_firmware_update-664b0c6c1a0307cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/more-transferprotocoltype-739ce8bdedbcb51c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/no-passwords-295207ac891d27ab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/non-default-language-registries-f73bdecc98ba2cc8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/property-missing-7602c421ec177e9a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/raise-error-on-async-task-failure-b67c7bc189a4d6ca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/re-raise-1fe9f912691e893e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/reauthentication-session-fallback-failure-fixes-4f0dcfdad1afd2d7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/redfish-response-log-294f3f10b770e356.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1522 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/refactor-taskmonitor-update-volume-ba99380188395852.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/releasenote-d7138d1e1d414632.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/remove-deprecated-task-monitors-58c505d43e1fa6a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/retry-if-transferprototype-missing-9cae57f3ecf470a9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/retry-ilo-not-ready-error-0b4dce882282eaac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/secure-boot-76c5b80371ea85d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/secure-boot-database-7fae673722d7cf4f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/sessions.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/standard-registry-license-0ded489afd6cfad1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/storage-controllers-resource-7ab112f5d2c34ca0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/story-2006246-reset-bios-return-http-error-415-08170df7fe6300f8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/story-2007216-fix-to-message-registry-cff37659f03ba815.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/sushy-system-virtualmedia-7a61bd77780f7b0e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/update-apply-time-support-53c5445b58cd3b42.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/update_sushy_models-9b8ea0350eb4d4d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/use-sessions-url-from-root-8b8eca57dc450705.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/use-settingsobject-if-supported-12a332f9905d64ce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/vmedia-1.4.0-9957460fed59d85c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/vmedia-certificate-06c367c6ef33d139.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/vmedia-credentials-14b7705c3c94cc07.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/notes/workaround-sushy-requests-verify-handling-6879c273b651246f.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.063367 sushy-4.8.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.063367 sushy-4.8.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.063367 sushy-4.8.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9025 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-01-16 16:33:28.000000 sushy-4.8.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2024-01-16 16:33:28.000000 sushy-4.8.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2024-01-16 16:34:01.103367 sushy-4.8.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-01-16 16:33:28.000000 sushy-4.8.0/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.067367 sushy-4.8.0/sushy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1672 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11603 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22797 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6058 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25604 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/main.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.067367 sushy-4.8.0/sushy/resources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31234 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.067367 sushy-4.8.0/sushy/resources/certificateservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/certificateservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4199 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/certificateservice/certificate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3599 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/certificateservice/certificateservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3138 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/certificateservice/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.067367 sushy-4.8.0/sushy/resources/chassis/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/chassis/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12166 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/chassis/chassis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5618 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/chassis/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.067367 sushy-4.8.0/sushy/resources/chassis/power/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/chassis/power/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/chassis/power/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4605 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/chassis/power/power.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.067367 sushy-4.8.0/sushy/resources/chassis/thermal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/chassis/thermal/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/chassis/thermal/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4909 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/chassis/thermal/thermal.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3657 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/common.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.071368 sushy-4.8.0/sushy/resources/compositionservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/compositionservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4043 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/compositionservice/compositionservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3311 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/compositionservice/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4346 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/compositionservice/resourceblock.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/compositionservice/resourcezone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12477 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.071368 sushy-4.8.0/sushy/resources/eventservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/eventservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1759 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/eventservice/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4539 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/eventservice/eventdestination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6073 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/eventservice/eventservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.071368 sushy-4.8.0/sushy/resources/fabric/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/fabric/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3340 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/fabric/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5613 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/fabric/endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3663 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/fabric/fabric.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2757 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/ipaddresses.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.071368 sushy-4.8.0/sushy/resources/manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5544 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/manager/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9951 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/manager/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11156 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/manager/virtual_media.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.071368 sushy-4.8.0/sushy/resources/oem/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/oem/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2814 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/oem/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4426 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/oem/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1374 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/oem/fake.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.071368 sushy-4.8.0/sushy/resources/registry/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/registry/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3422 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/registry/attribute_registry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/registry/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5413 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/registry/message_registry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7463 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/registry/message_registry_file.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.071368 sushy-4.8.0/sushy/resources/sessionservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/sessionservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3221 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/sessionservice/session.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4952 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/sessionservice/sessionservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6580 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/settings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.075368 sushy-4.8.0/sushy/resources/system/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9571 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/bios.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13944 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2547 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/ethernet_interface.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.075368 sushy-4.8.0/sushy/resources/system/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/network/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3157 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/network/adapter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3803 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/network/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6971 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/network/device_function.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2362 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/network/port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6612 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/processor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5550 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/secure_boot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4168 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/secure_boot_database.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2868 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/simple_storage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.075368 sushy-4.8.0/sushy/resources/system/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6283 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/storage/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6111 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/storage/controller.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3861 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/storage/drive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7410 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/storage/storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9575 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/storage/volume.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23551 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/system/system.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.075368 sushy-4.8.0/sushy/resources/taskservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/taskservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1495 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/taskservice/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3666 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/taskservice/task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/taskservice/taskservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.075368 sushy-4.8.0/sushy/resources/updateservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/updateservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1937 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/updateservice/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3863 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/updateservice/softwareinventory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7602 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/resources/updateservice/updateservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.079367 sushy-4.8.0/sushy/standard_registries/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26501 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/standard_registries/Base.1.0.0.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29190 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/standard_registries/Base.1.2.0.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30123 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/standard_registries/Base.1.3.0.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30283 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/standard_registries/Base.1.3.1.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30875 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/standard_registries/Base.1.4.0.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7854 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/taskmonitor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.079367 sushy-4.8.0/sushy/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.079367 sushy-4.8.0/sushy/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.095368 sushy-4.8.0/sushy/tests/unit/json_samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/TestRegistry.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/bare_minimum_root.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1855 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/bios.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/bios_attribute_registry.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/bios_attribute_registry_file.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/bios_attribute_registry_file_zthardware.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2301 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/bios_attribute_registry_zthardware.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1270 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/bios_settings.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11114 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/bios_zt.json
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3793 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/certificate.json
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      567 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/certificate_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/certificate_locations.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/certificateservice.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3166 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/chassis.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/chassis_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      683 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/compositionservice.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1544 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/drive.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1685 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/drive2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1797 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/drive3.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/endpoint.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/endpoint_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1885 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/error_single_ext_info.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1166 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/ethernet_interfaces.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/ethernet_interfaces_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/eventdestination1.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/eventdestination2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/eventdestination3.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      508 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/eventdestination_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      836 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/eventservice.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      689 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/fabric.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/fabric_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/firmwareinventory_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2505 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/manager.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/manager_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2589 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/managerv1_18.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1482 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/message_registry.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/message_registry_file.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/message_registry_file_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2553 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/network_adapter.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/network_adapter_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2541 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/network_device_function.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/network_device_function_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1655 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/network_port.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/network_port_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4211 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/power.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/processor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/processor2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/processor_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1344 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/resourceblock.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/resourceblock_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/resourcezone.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/resourcezone_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1638 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/root.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/secure_boot.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/secure_boot_database.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1370 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/secure_boot_database_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/session.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/session_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/session_creation_headers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/session_creation_headers_no_location.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/session_error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/session_service.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/settings-body-bootsourceoverridemode-only.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/settings-body-lenovo-se450.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/settings-body-nokia.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/settings-lenovo-se450.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/settings-nokia.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/settings.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2039 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/simple_storage.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      607 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/simple_storage_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/softwareinventory.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/storage.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/storage_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1499 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/storage_controller.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/storage_controller_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/storage_controller_settings.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/subprocessor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/subprocessor_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5222 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/system.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/system_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4277 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/systemv1_20.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/task.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/task2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/task_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/task_monitor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/taskservice.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1323 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/thermal.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/transfer_method_required_error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/transfer_proto_required_error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/transfer_proto_required_error2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      950 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/updateservice.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      748 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/updateservice_no_inv.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/virtual_media.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/virtual_media_collection.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/virtual_media_collectionv1_6.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/virtual_mediav1_6.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1514 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/volume.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1392 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/volume2.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/volume3.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1407 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/volume4.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/json_samples/volume_collection.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.095368 sushy-4.8.0/sushy/tests/unit/resources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.095368 sushy-4.8.0/sushy/tests/unit/resources/certificateservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/certificateservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5657 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/certificateservice/test_certificate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3683 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/certificateservice/test_certificateservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.095368 sushy-4.8.0/sushy/tests/unit/resources/chassis/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/chassis/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12179 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/chassis/test_chassis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9406 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/chassis/test_power.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5962 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/chassis/test_thermal.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.095368 sushy-4.8.0/sushy/tests/unit/resources/compositionservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/compositionservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2861 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/compositionservice/test_compositionservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4894 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/compositionservice/test_resourceblock.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4027 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/compositionservice/test_resourcezone.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.095368 sushy-4.8.0/sushy/tests/unit/resources/eventservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/eventservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6786 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/eventservice/test_evendestination.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4988 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/eventservice/test_eventservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.095368 sushy-4.8.0/sushy/tests/unit/resources/fabric/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/fabric/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2083 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/fabric/test_endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5434 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/fabric/test_fabric.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.095368 sushy-4.8.0/sushy/tests/unit/resources/manager/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/manager/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14409 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/manager/test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15925 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/manager/test_virtual_media.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.095368 sushy-4.8.0/sushy/tests/unit/resources/oem/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/oem/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9148 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/oem/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2315 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/oem/test_fake.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.099367 sushy-4.8.0/sushy/tests/unit/resources/registry/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/registry/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4998 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/registry/test_attribute_registry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15477 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/registry/test_message_registry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14996 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/registry/test_message_registry_file.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.099367 sushy-4.8.0/sushy/tests/unit/resources/sessionservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/sessionservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4310 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/sessionservice/test_session.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6993 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/sessionservice/test_sessionservice.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.099367 sushy-4.8.0/sushy/tests/unit/resources/system/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/system/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.099367 sushy-4.8.0/sushy/tests/unit/resources/system/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/system/network/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8673 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/system/network/test_adapter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7679 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/system/network/test_device_function.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5056 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/system/network/test_port.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.099367 sushy-4.8.0/sushy/tests/unit/resources/system/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/system/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6366 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/system/storage/test_controller.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4394 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/system/storage/test_drive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17404 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/system/storage/test_storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16030 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/system/storage/test_volume.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20208 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/system/test_bios.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4757 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/system/test_ethernet_interfaces.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8840 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/system/test_processor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5169 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/system/test_secure_boot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6392 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/system/test_secure_boot_database.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5848 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/system/test_simple_storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45204 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/system/test_system.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.099367 sushy-4.8.0/sushy/tests/unit/resources/taskservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/taskservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7219 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/taskservice/test_task.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/taskservice/test_taskservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20136 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4938 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/test_settings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.103367 sushy-4.8.0/sushy/tests/unit/resources/updateservice/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/updateservice/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5604 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/updateservice/test_softwareinventory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9466 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/resources/updateservice/test_updateservice.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22169 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40991 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/test_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27368 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/test_main.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11533 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/test_taskmonitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11237 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13472 2024-01-16 16:33:28.000000 sushy-4.8.0/sushy/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.067367 sushy-4.8.0/sushy.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2279 2024-01-16 16:34:00.000000 sushy-4.8.0/sushy.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21922 2024-01-16 16:34:01.000000 sushy-4.8.0/sushy.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-01-16 16:34:00.000000 sushy-4.8.0/sushy.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-01-16 16:34:00.000000 sushy-4.8.0/sushy.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-01-16 16:34:00.000000 sushy-4.8.0/sushy.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-01-16 16:34:00.000000 sushy-4.8.0/sushy.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-01-16 16:34:00.000000 sushy-4.8.0/sushy.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2024-01-16 16:34:00.000000 sushy-4.8.0/sushy.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2024-01-16 16:33:28.000000 sushy-4.8.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.103367 sushy-4.8.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2644 2024-01-16 16:33:28.000000 sushy-4.8.0/tools/generate-enum.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2930 2024-01-16 16:33:28.000000 sushy-4.8.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-16 16:34:01.103367 sushy-4.8.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2024-01-16 16:33:28.000000 sushy-4.8.0/zuul.d/project.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2024-01-16 16:33:28.000000 sushy-4.8.0/zuul.d/sushy-jobs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.680539 sushy-5.0.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:00:44.000000 sushy-5.0.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-02-22 15:00:44.000000 sushy-5.0.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2024-02-22 15:00:44.000000 sushy-5.0.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3041 2024-02-22 15:01:13.000000 sushy-5.0.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-02-22 15:00:44.000000 sushy-5.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17948 2024-02-22 15:01:13.000000 sushy-5.0.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-02-22 15:00:44.000000 sushy-5.0.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-02-22 15:00:44.000000 sushy-5.0.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2230 2024-02-22 15:01:13.680539 sushy-5.0.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2024-02-22 15:00:44.000000 sushy-5.0.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-02-22 15:00:44.000000 sushy-5.0.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.632535 sushy-5.0.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2024-02-22 15:00:44.000000 sushy-5.0.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.632535 sushy-5.0.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3047 2024-02-22 15:00:44.000000 sushy-5.0.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.632535 sushy-5.0.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3142 2024-02-22 15:00:44.000000 sushy-5.0.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2024-02-22 15:00:44.000000 sushy-5.0.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.632535 sushy-5.0.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2024-02-22 15:00:44.000000 sushy-5.0.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.632535 sushy-5.0.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2024-02-22 15:00:44.000000 sushy-5.0.0/doc/source/reference/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10228 2024-02-22 15:00:44.000000 sushy-5.0.0/doc/source/reference/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.628535 sushy-5.0.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.644536 sushy-5.0.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/action-parameter-missing-7d234b96b5b1d81a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-apply-time-support-to-bios-315ebad429dcab3d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-bios-bf69ac56c4ae8f50.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-bios-update-status-cc59816c374b78e4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-chassis-linkage-d8e567f9c791169d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-chassis-support-5b97daffe1c61a2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-custom-connector-support-0a49c6649d5f7eaf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-default-identity-10c5dd23bed0e915.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-drive-led-97b687013fec88c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-drive-revision-a0c069fff236479d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-drive-volumes-971d80644c3bd1e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-endpoint-subresource-to-fabric-b03e5fd99ece1bf4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-fabric-support-1520f7fcb0e12539.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-http-boot-uri-support-5c25816e13ccdb27.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-initial-redfish-oem-extension-support-50c9849bb7b6b25c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-mapped-list-field-04c671f7a73d83f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-network-adapter-26d01d8d9fb1d7ad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-network-device-function-and-port-e880d8f461e3723d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-odata-version-header-96dc8179c0e2e9bd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-partial-key-match-27bed73d577b1187.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-power-resource-e141ddf298673305.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-processor-id-and-status-b81d4c6e6c14c25f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-raid-type-properties-2090da5bea37c660.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-read-and-connect-timeout-9f7dc3ed63c192c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-response-cb-65d448ee2690d0b2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-simple-storage-915464811737bb05.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-storage-and-simple-storage-attributes-to-system-16e81f9b15b1897d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-storage-da766d3dbf9fb385.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-sushy-root-to-resources-1f221794557aa5fc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-system-bootprogress-42ee452cfa279c63.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-system-manager-linkage-86be69c9df4cb359.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-system-status-field-41b3f2a8c4b85f38.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-system-type-mapping-bf456c5c15a90877.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-task-monitor-support-21f711927ad6ec91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-task-service-c751ce51e0b8dc11.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-thermal-resource-5c965a3c940f9028.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add-virtual-media-support-f522fbec4420341c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add_composition_service-84750d8d1d96474a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add_ethernet_interface-df308f814f0e4bce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add_keyword_argument_for_connector-cea5dc4e6c01b548.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add_product_and_protocol_features_supported-59de3f89b7382434.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/add_update_service-b54c9bb0177e3468.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/allow_empty_context_eventdestination-9a96c34dd7edbeca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/apply-time-support-for-volume-ops-f2ebc412e3b4290a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/bios-attribute-registry-a55c2d81c730a795.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/bug-1754514-ca6ebe16c4e4b3b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/catch-general-requests-exceptions-b5fd706597708fb6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/certificate-collection-acc67488c240274c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/change-bootdev-smc-ab30317eaf5c37d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/change-vmedia-write-protected-attr-586370a552288801.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/check-for-boot-attrs-in-settingsuri-1cad07b6eb1c81b3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/config-server-side-retries-d16824019bd709a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/decouple-boot-params-c75e80f5951abb12.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/deprecate-system-leds-f1a72422c53d281e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/disable-conn-pooling-3456782afe56ac94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      807 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/do-not-offer-compression-encoding-884ca8a7458cb096.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/drop-py-2-7-cc931c210ce08e33.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/enhance-oem-extension-design-3143717e710b3eaf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/enhance-storage-volume-drive-support-16314d30f3631fb3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/enums-3aff03d940012f33.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/event-service-d6607420effc3df8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/expand-drive-schema-042901f919be646c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-2008198-bios-factory-reset-400-bad-request-3f4a7a2aada0835b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-eject-media-empty-dict-573b4c9e06f52ce7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-exceeding-retries-663ab543cc14f261.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-extended-info-error-handling-73fecb6bf5c852ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-insert-media-payload-b5d4c707f81d9603.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-malformed-boot-mode-1ba1117cad8dcc47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-manager-action-d71fd415cea29aa6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-missing-etags-ded8c0bb31fafef7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-oem-loading-52da045252b6c33e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-refine-resource-refresh-86c21ce230967251.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-required-oem-attribute-parsing-205e4186275aa293.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-retry_volume_operation-on_sys518-009f2b16e5c38a27.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-return-full-weak-etag-04265472cbea9c0e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-simple-storage-device-capacity-bytes-null-0672eed36d9da70a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-simple-update-e88838fab4170920.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-software-firmware-inventory-3e0e79e052aa76d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-subprocessors-3b619434dba4636d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-taskmonitor-init-calls-in-volume-module-0f8a747acd0cfe3f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-to-close-session-on-dealloc-c3687d4dcb1441b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-update-service-constants-b8c3f48ccee6ce1f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-use-headers-for-options-736940b87c06c189.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-virtual-media-fallback-15a559414a65c014.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-volume-actions-not-required-730fd637dd2587ce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fix-volume-delete-configuration-unsuported-operational_time_property-f53f650d8612a847.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/fixes-ilo5-redfish-firmware-update-issue-273862b2a11e3536.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/get-retry-9ca311caf8a0b7bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/handle-basic-auth-access-errors-393b368b31f5cad2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/handle_transfer_method-a51d5a17e381ebee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/health_literals_change-0e3fc0c439b765e3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/increase-server-retries-5f11edde8ee0b461.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/indicator-led-mappings-e7b34da03f6abb06.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/lazily-load-registries-0e9441e435c2471d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/make-leds-settable-c82cb513de0171f5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/make-volume-ops-blocking-de5c2ae032041d5d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/message-parsing-resilience-534da532515a15da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/message-registry-logging-39624ae114c02e15.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/monitor_firmware_update-664b0c6c1a0307cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       85 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/more-transferprotocoltype-739ce8bdedbcb51c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/no-passwords-295207ac891d27ab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/non-default-language-registries-f73bdecc98ba2cc8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/property-missing-7602c421ec177e9a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/raise-error-on-async-task-failure-b67c7bc189a4d6ca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/re-raise-1fe9f912691e893e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1432 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/reauthentication-session-fallback-failure-fixes-4f0dcfdad1afd2d7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/redfish-response-log-294f3f10b770e356.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1522 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/refactor-taskmonitor-update-volume-ba99380188395852.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/releasenote-d7138d1e1d414632.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/remove-deprecated-task-monitors-58c505d43e1fa6a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/retry-if-transferprototype-missing-9cae57f3ecf470a9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/retry-ilo-not-ready-error-0b4dce882282eaac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/secure-boot-76c5b80371ea85d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/secure-boot-database-7fae673722d7cf4f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/sessions.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/standard-registry-license-0ded489afd6cfad1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/storage-controllers-resource-7ab112f5d2c34ca0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/story-2006246-reset-bios-return-http-error-415-08170df7fe6300f8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/story-2007216-fix-to-message-registry-cff37659f03ba815.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/sushy-system-virtualmedia-7a61bd77780f7b0e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/update-apply-time-support-53c5445b58cd3b42.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/update_sushy_models-9b8ea0350eb4d4d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/use-sessions-url-from-root-8b8eca57dc450705.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/use-settingsobject-if-supported-12a332f9905d64ce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/vmedia-1.4.0-9957460fed59d85c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/vmedia-certificate-06c367c6ef33d139.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/vmedia-credentials-14b7705c3c94cc07.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/notes/workaround-sushy-requests-verify-handling-6879c273b651246f.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.644536 sushy-5.0.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/2023.2.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.644536 sushy-5.0.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.644536 sushy-5.0.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9025 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-02-22 15:00:44.000000 sushy-5.0.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2024-02-22 15:00:44.000000 sushy-5.0.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1032 2024-02-22 15:01:13.680539 sushy-5.0.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-02-22 15:00:44.000000 sushy-5.0.0/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.648537 sushy-5.0.0/sushy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1672 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11601 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22799 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6058 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25817 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/main.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.648537 sushy-5.0.0/sushy/resources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31234 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.648537 sushy-5.0.0/sushy/resources/certificateservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/certificateservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4199 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/certificateservice/certificate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3599 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/certificateservice/certificateservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3138 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/certificateservice/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.648537 sushy-5.0.0/sushy/resources/chassis/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12166 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/chassis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5618 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.648537 sushy-5.0.0/sushy/resources/chassis/power/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/power/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/power/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4605 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/power/power.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.652537 sushy-5.0.0/sushy/resources/chassis/thermal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/thermal/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/thermal/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4909 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/chassis/thermal/thermal.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3657 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/common.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.652537 sushy-5.0.0/sushy/resources/compositionservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/compositionservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4043 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/compositionservice/compositionservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3311 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/compositionservice/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4346 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/compositionservice/resourceblock.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/compositionservice/resourcezone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12477 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.652537 sushy-5.0.0/sushy/resources/eventservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/eventservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1759 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/eventservice/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4539 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/eventservice/eventdestination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6073 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/eventservice/eventservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.652537 sushy-5.0.0/sushy/resources/fabric/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/fabric/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3340 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/fabric/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5613 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/fabric/endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3663 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/fabric/fabric.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2757 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/ipaddresses.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.652537 sushy-5.0.0/sushy/resources/manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5544 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/manager/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9951 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/manager/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11234 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/manager/virtual_media.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.652537 sushy-5.0.0/sushy/resources/oem/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/oem/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2814 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/oem/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4426 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/oem/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1374 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/oem/fake.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.652537 sushy-5.0.0/sushy/resources/registry/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/registry/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3423 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/registry/attribute_registry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/registry/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5414 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/registry/message_registry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7463 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/registry/message_registry_file.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.652537 sushy-5.0.0/sushy/resources/sessionservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/sessionservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3221 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/sessionservice/session.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4952 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/sessionservice/sessionservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6580 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/settings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.656537 sushy-5.0.0/sushy/resources/system/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9571 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/bios.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13947 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2547 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/ethernet_interface.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.656537 sushy-5.0.0/sushy/resources/system/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/network/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3157 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/network/adapter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3803 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/network/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6971 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/network/device_function.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2362 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/network/port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6612 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/processor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5550 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/secure_boot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4168 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/secure_boot_database.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2868 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/simple_storage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.656537 sushy-5.0.0/sushy/resources/system/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6283 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/storage/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6111 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/storage/controller.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3861 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/storage/drive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7410 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/storage/storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9575 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/storage/volume.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23551 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/system/system.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.656537 sushy-5.0.0/sushy/resources/taskservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/taskservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1495 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/taskservice/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3666 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/taskservice/task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2955 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/taskservice/taskservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.656537 sushy-5.0.0/sushy/resources/updateservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/updateservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1937 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/updateservice/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3863 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/updateservice/softwareinventory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7602 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/resources/updateservice/updateservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.660537 sushy-5.0.0/sushy/standard_registries/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26502 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/standard_registries/Base.1.0.0.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29190 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/standard_registries/Base.1.2.0.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30123 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/standard_registries/Base.1.3.0.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30283 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/standard_registries/Base.1.3.1.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30875 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/standard_registries/Base.1.4.0.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7854 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/taskmonitor.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.660537 sushy-5.0.0/sushy/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.660537 sushy-5.0.0/sushy/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.672538 sushy-5.0.0/sushy/tests/unit/json_samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/TestRegistry.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/bare_minimum_root.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1855 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/bios.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/bios_attribute_registry.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/bios_attribute_registry_file.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/bios_attribute_registry_file_zthardware.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2301 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/bios_attribute_registry_zthardware.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1270 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/bios_settings.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11114 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/bios_zt.json
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3793 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/certificate.json
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      567 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/certificate_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/certificate_locations.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      982 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/certificateservice.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3166 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/chassis.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/chassis_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      683 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/compositionservice.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1544 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/drive.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1685 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/drive2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1797 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/drive3.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/endpoint.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/endpoint_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1885 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/error_single_ext_info.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1166 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/ethernet_interfaces.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/ethernet_interfaces_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/eventdestination1.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/eventdestination2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/eventdestination3.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      508 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/eventdestination_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      836 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/eventservice.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      689 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/fabric.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/fabric_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/firmwareinventory_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2505 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/manager.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/manager_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2589 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/managerv1_18.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1482 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/message_registry.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/message_registry_file.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/message_registry_file_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2553 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/network_adapter.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/network_adapter_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2541 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/network_device_function.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/network_device_function_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1655 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/network_port.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/network_port_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4211 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/power.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/processor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/processor2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/processor_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1344 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/resourceblock.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/resourceblock_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/resourcezone.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/resourcezone_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1638 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/root.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/secure_boot.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/secure_boot_database.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1370 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/secure_boot_database_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/session.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/session_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/session_creation_headers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/session_creation_headers_no_location.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/session_error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/session_service.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/settings-body-bootsourceoverridemode-only.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/settings-body-lenovo-se450.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1209 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/settings-body-nokia.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/settings-lenovo-se450.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/settings-nokia.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/settings.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2039 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/simple_storage.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      607 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/simple_storage_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/softwareinventory.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/storage.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      564 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/storage_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1499 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/storage_controller.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/storage_controller_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/storage_controller_settings.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/subprocessor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/subprocessor_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5222 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/system.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/system_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4277 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/systemv1_20.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/task.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/task2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/task_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/task_monitor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/taskservice.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1323 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/thermal.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/transfer_method_required_error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/transfer_proto_required_error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/transfer_proto_required_error2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/transfer_proto_required_error3.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      950 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/updateservice.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      748 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/updateservice_no_inv.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/virtual_media.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/virtual_media_collection.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/virtual_media_collectionv1_6.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/virtual_mediav1_6.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1514 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/volume.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1392 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/volume2.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/volume3.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1407 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/volume4.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/json_samples/volume_collection.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.672538 sushy-5.0.0/sushy/tests/unit/resources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.672538 sushy-5.0.0/sushy/tests/unit/resources/certificateservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/certificateservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5657 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/certificateservice/test_certificate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3683 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/certificateservice/test_certificateservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.672538 sushy-5.0.0/sushy/tests/unit/resources/chassis/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/chassis/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12179 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/chassis/test_chassis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9406 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/chassis/test_power.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5962 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/chassis/test_thermal.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.672538 sushy-5.0.0/sushy/tests/unit/resources/compositionservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/compositionservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2861 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/compositionservice/test_compositionservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4894 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/compositionservice/test_resourceblock.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4027 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/compositionservice/test_resourcezone.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.676539 sushy-5.0.0/sushy/tests/unit/resources/eventservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/eventservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6786 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/eventservice/test_evendestination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4988 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/eventservice/test_eventservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.676539 sushy-5.0.0/sushy/tests/unit/resources/fabric/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/fabric/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2083 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/fabric/test_endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5434 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/fabric/test_fabric.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.676539 sushy-5.0.0/sushy/tests/unit/resources/manager/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/manager/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14409 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/manager/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16423 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/manager/test_virtual_media.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.676539 sushy-5.0.0/sushy/tests/unit/resources/oem/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/oem/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9148 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/oem/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2315 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/oem/test_fake.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.676539 sushy-5.0.0/sushy/tests/unit/resources/registry/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/registry/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4998 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/registry/test_attribute_registry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15477 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/registry/test_message_registry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14996 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/registry/test_message_registry_file.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.676539 sushy-5.0.0/sushy/tests/unit/resources/sessionservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/sessionservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4310 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/sessionservice/test_session.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6993 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/sessionservice/test_sessionservice.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.676539 sushy-5.0.0/sushy/tests/unit/resources/system/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.676539 sushy-5.0.0/sushy/tests/unit/resources/system/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/network/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8673 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/network/test_adapter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7679 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/network/test_device_function.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5056 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/network/test_port.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.680539 sushy-5.0.0/sushy/tests/unit/resources/system/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6366 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/storage/test_controller.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4394 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/storage/test_drive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17404 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/storage/test_storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16030 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/storage/test_volume.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20207 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/test_bios.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4757 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/test_ethernet_interfaces.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8840 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/test_processor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5169 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/test_secure_boot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6392 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/test_secure_boot_database.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5848 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/test_simple_storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45204 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/system/test_system.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.680539 sushy-5.0.0/sushy/tests/unit/resources/taskservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/taskservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7219 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/taskservice/test_task.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/taskservice/test_taskservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20136 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4938 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/test_settings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.680539 sushy-5.0.0/sushy/tests/unit/resources/updateservice/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/updateservice/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5604 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/updateservice/test_softwareinventory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9466 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/resources/updateservice/test_updateservice.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22169 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40991 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/test_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28538 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/test_main.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11533 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/test_taskmonitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11237 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13472 2024-02-22 15:00:44.000000 sushy-5.0.0/sushy/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.648537 sushy-5.0.0/sushy.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2230 2024-02-22 15:01:13.000000 sushy-5.0.0/sushy.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22054 2024-02-22 15:01:13.000000 sushy-5.0.0/sushy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 15:01:13.000000 sushy-5.0.0/sushy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-02-22 15:01:13.000000 sushy-5.0.0/sushy.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 15:01:13.000000 sushy-5.0.0/sushy.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-22 15:01:13.000000 sushy-5.0.0/sushy.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-02-22 15:01:13.000000 sushy-5.0.0/sushy.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2024-02-22 15:01:13.000000 sushy-5.0.0/sushy.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2024-02-22 15:00:44.000000 sushy-5.0.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.680539 sushy-5.0.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2644 2024-02-22 15:00:44.000000 sushy-5.0.0/tools/generate-enum.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3311 2024-02-22 15:00:44.000000 sushy-5.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:01:13.680539 sushy-5.0.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2024-02-22 15:00:44.000000 sushy-5.0.0/zuul.d/project.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-02-22 15:00:44.000000 sushy-5.0.0/zuul.d/sushy-jobs.yaml
```

### Comparing `sushy-4.8.0/AUTHORS` & `sushy-5.0.0/AUTHORS`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 Bob Fournier <bfournie@redhat.com>
 Christopher Dearborn <Christopher.Dearborn@dell.com>
 Debayan Ray <debayan.ray@gmail.com>
 Derek Higgins <derekh@redhat.com>
 Dmitry Tantsur <divius.inside@gmail.com>
 Dmitry Tantsur <dtantsur@protonmail.com>
 Doug Hellmann <doug@doughellmann.com>
+Fabian Wiesel <fabian.wiesel@sap.com>
+Fedor Tarasenko <feodor.tarasenko@gmail.com>
 Gabriela Soria <soria.gaby@gmail.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Ha Manh Dong <donghm@vn.fujitsu.com>
 Hervé Beraud <hberaud@redhat.com>
 Ilya Etingof <etingof@gmail.com>
 Iury Gregory Melo Ferreira <imelofer@redhat.com>
 Iury Gregory Melo Ferreira <iurygregory@gmail.com>
@@ -43,16 +45,18 @@
 Riccardo Pittau <elfosardo@gmail.com>
 Richard G. Pioso <richard.pioso@dell.com>
 Richard Pioso <richard.pioso@dell.com>
 Ruby Loo <ruby.loo@intel.com>
 Samuel Kunkel <samuel.kunkel@mail.schwarz>
 Sayali Kutwal <sayalikutwal26@gmail.com>
 Sean McGinnis <sean.mcginnis@gmail.com>
+Sharpz7 <adam.mcarthur62@gmail.com>
 Shivanand Tendulker <stendulker@gmail.com>
 Steve Baker <sbaker@redhat.com>
+Takashi Kajinami <kajinamit@oss.nttdata.com>
 Takashi Natsume <takanattie@gmail.com>
 Thomas Goirand <zigo@debian.org>
 Vanou Ishii <ishii.vanou@fujitsu.com>
 Varsha <varsha.verma.eee15@itbhu.ac.in>
 Vu Cong Tuan <tuanvc@vn.fujitsu.com>
 Winicius Silva <winiciusab12@gmail.com>
 Yusef Shaban <yshaban@godaddy.com>
```

### Comparing `sushy-4.8.0/CONTRIBUTING.rst` & `sushy-5.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/ChangeLog` & `sushy-5.0.0/ChangeLog`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 CHANGES
 =======
 
+5.0.0
+-----
+
+* reno: Update master for unmaintained/yoga
+* Force constraints when installing a package during tox test
+* [codespell] Adding CI target for Tox Codespell
+* [codespell] Adding Tox Target for Codespell
+* [codespell] Fixing Spelling Mistakes
+* Update supported python versions
+
 4.8.0
 -----
 
 * Allows System to access VirtualMedia in Sushy
+* Handle a different related properties for missing TransferProtocolType
 * Add release version to release notes
 * Handle exceptions after re-authentication
 * Remove version field from iLO error
 * Add a boot progress indicator
 
 4.7.0
 -----
@@ -22,14 +33,15 @@
 * Update master for stable/2023.2
 * Fix wrong \_get\_registry logic in ResourceBase
 
 4.5.1
 -----
 
 * Requests must always have a read/connect timeout
+* Handle session-uri in body
 
 4.5.0
 -----
 
 * Retry on ilo state error
 * Update pep8 dep hacking to latest: v6
 * Handle TransferMethod in vmedia insertion
```

### Comparing `sushy-4.8.0/LICENSE` & `sushy-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/PKG-INFO` & `sushy-5.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sushy
-Version: 4.8.0
+Version: 5.0.0
 Summary: Sushy is a small Python library to communicate with Redfish based systems
 Home-page: https://docs.openstack.org/sushy/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Overview
         ========
@@ -38,13 +38,12 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
```

### Comparing `sushy-4.8.0/README.rst` & `sushy-5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/doc/source/conf.py` & `sushy-5.0.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/doc/source/contributor/index.rst` & `sushy-5.0.0/doc/source/contributor/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 .. code-block:: sh
 
   sushy-emulator
 
   # Or, running with custom parameters
   sushy-emulator --port 8000 --libvirt-uri "qemu:///system"
 
-That's it, now you can test Sushy against the ``http://locahost:8000``
+That's it, now you can test Sushy against the ``http://localhost:8000``
 endpoint.
 
 
 Enabling SSL
 ~~~~~~~~~~~~
 
 Both mockup servers supports `SSL`_ if you want Sushy with it. To set it
```

### Comparing `sushy-4.8.0/doc/source/index.rst` & `sushy-5.0.0/doc/source/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 * System mappings
 * System processor
 * Storage management
 * Systems power management (Both soft and hard; Including NMI injection)
 * Changing systems boot device, frequency (Once or permanently) and mode
   (UEFI or BIOS)
 * Chassis management
-* OEM extention
+* OEM extension
 * Virtual media management
 * Session Management
 
 Documentation
 =============
 
 .. toctree::
```

### Comparing `sushy-4.8.0/doc/source/reference/usage.rst` & `sushy-5.0.0/doc/source/reference/usage.rst`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/releasenotes/notes/apply-time-support-for-volume-ops-f2ebc412e3b4290a.yaml` & `sushy-5.0.0/releasenotes/notes/apply-time-support-for-volume-ops-f2ebc412e3b4290a.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/releasenotes/notes/check-for-boot-attrs-in-settingsuri-1cad07b6eb1c81b3.yaml` & `sushy-5.0.0/releasenotes/notes/check-for-boot-attrs-in-settingsuri-1cad07b6eb1c81b3.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/releasenotes/notes/do-not-offer-compression-encoding-884ca8a7458cb096.yaml` & `sushy-5.0.0/releasenotes/notes/do-not-offer-compression-encoding-884ca8a7458cb096.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/releasenotes/notes/enhance-oem-extension-design-3143717e710b3eaf.yaml` & `sushy-5.0.0/releasenotes/notes/enhance-oem-extension-design-3143717e710b3eaf.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/releasenotes/notes/enums-3aff03d940012f33.yaml` & `sushy-5.0.0/releasenotes/notes/enums-3aff03d940012f33.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/releasenotes/notes/fix-insert-media-payload-b5d4c707f81d9603.yaml` & `sushy-5.0.0/releasenotes/notes/fix-insert-media-payload-b5d4c707f81d9603.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/releasenotes/notes/reauthentication-session-fallback-failure-fixes-4f0dcfdad1afd2d7.yaml` & `sushy-5.0.0/releasenotes/notes/reauthentication-session-fallback-failure-fixes-4f0dcfdad1afd2d7.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/releasenotes/notes/refactor-taskmonitor-update-volume-ba99380188395852.yaml` & `sushy-5.0.0/releasenotes/notes/refactor-taskmonitor-update-volume-ba99380188395852.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/releasenotes/notes/releasenote-d7138d1e1d414632.yaml` & `sushy-5.0.0/releasenotes/notes/releasenote-d7138d1e1d414632.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/releasenotes/notes/update-apply-time-support-53c5445b58cd3b42.yaml` & `sushy-5.0.0/releasenotes/notes/update-apply-time-support-53c5445b58cd3b42.yaml`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/releasenotes/source/conf.py` & `sushy-5.0.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/requirements.txt` & `sushy-5.0.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/setup.cfg` & `sushy-5.0.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -2,36 +2,38 @@
 name = sushy
 summary = Sushy is a small Python library to communicate with Redfish based systems
 description_file = 
 	README.rst
 author = OpenStack
 author_email = openstack-discuss@lists.openstack.org
 home_page = https://docs.openstack.org/sushy/latest/
-python_requires = >=3.6
+python_requires = >=3.8
 classifier = 
 	Environment :: OpenStack
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [files]
 packages = 
 	sushy
 
 [entry_points]
 sushy.resources.system.oems = 
 	contoso = sushy.resources.oem.fake:get_extension
 
+[codespell]
+quiet-level = 4
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sushy-4.8.0/setup.py` & `sushy-5.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/__init__.py` & `sushy-5.0.0/sushy/__init__.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/auth.py` & `sushy-5.0.0/sushy/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     def set_context(self, root_resource, connector):
         """Set the context of the authentication object.
 
         :param root_resource: Root sushy object
         :param connector: Connector for http connections
         """
         # Set the root resource, and connector to use
-        # for normal opreations.
+        # for normal operations.
         self._root_resource = root_resource
         self._connector = connector
         self._connector.set_auth(self)
 
     def authenticate(self):
         """Perform authentication.
 
@@ -271,16 +271,16 @@
             LOG.debug('Encountered a connectivity failure while attempting '
                       'to authenticate. We will not explicitly fallback. '
                       'Error: %(exception)s',
                       {'exception': e})
             # Previously we would silently eat the failure as SushyError
             # and fallback as it is a general fault. Callers on direct
             # invocations through a connector _op method call can still
-            # receieve these exceptions, and applicaitons like Ironic do
-            # consider a client re-use disqualifier if there has been
+            # receive these exceptions, and applications like Ironic do
+            # consider a client reuse disqualifier if there has been
             # a connection failure, so it is okay for us to fix the behavior
             # here.
             raise
         except exceptions.SushyError as e:
             LOG.debug('Received exception "%(exception)s" while '
                       'attempting to establish a session. '
                       'Falling back to basic authentication.',
```

### Comparing `sushy-4.8.0/sushy/connector.py` & `sushy-5.0.0/sushy/connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             if (method == 'POST'
                     and self._sessions_uri is not None
                     and self._sessions_uri in url):
                 LOG.error('Authentication to the session service failed. '
                           'Please check credentials and try again.')
                 raise
             if not allow_reauth:
-                LOG.error("Failure occured while attempting to retry "
+                LOG.error("Failure occurred while attempting to retry "
                           "request after refreshing the session: %s", e)
                 raise
             if self._auth is not None:
                 # self._session.auth value is only set when basic auth is used
                 if self._session.auth is not None:
                     LOG.warning('We have encountered an AccessError when '
                                 'using \'basic\' authentication. %(err)s',
@@ -207,15 +207,15 @@
                         LOG.warning('Session authentication appears to have '
                                     'been lost at some point in time. '
                                     'Connectivity may have been lost during '
                                     'a prior session refresh. Attempting to '
                                     're-authenticate.')
                         self._auth.authenticate()
                 except exceptions.AccessError as refresh_exc:
-                    LOG.error("A failure occured while attempting to refresh "
+                    LOG.error("A failure occurred while attempting to refresh "
                               "the session. Error: %s", refresh_exc.message)
                     raise
                 LOG.debug("Authentication refreshed successfully, "
                           "retrying the call.")
                 return self._op(
                     method, path, data=data, headers=headers,
                     blocking=blocking, timeout=timeout,
```

### Comparing `sushy-4.8.0/sushy/exceptions.py` & `sushy-5.0.0/sushy/exceptions.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/main.py` & `sushy-5.0.0/sushy/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,15 +391,15 @@
         """Returns the Sessions url"""
         # NOTE(TheJulia): This method is the standard discovery method
         # advised by the DMTF DSP0266 standard to find the session service.
         try:
             links_url = self.json.get('Links')
             sessions_uri = links_url['Sessions']['@odata.id']
             # Save the session URL for post detection and prevention
-            # of recursive autentication attempts.
+            # of recursive authentication attempts.
             self._conn._sessions_uri = sessions_uri
             return sessions_uri
         except (TypeError, KeyError):
             raise exceptions.MissingAttributeError(
                 attribute='Links/Sessions/@data.id', resource=self.path)
 
     def get_session(self, identity):
@@ -461,14 +461,21 @@
         session_key = rsp.headers.get('X-Auth-Token')
         if session_key is None:
             raise exceptions.MissingXAuthToken(
                 method='POST', url=session_service_path, response=rsp)
 
         session_uri = rsp.headers.get('Location')
         if session_uri is None:
+            try:
+                body = rsp.json()
+                session_uri = body.get("@odata.id")
+            except ValueError:  # JSON decoding failed
+                pass
+
+        if session_uri is None:
             LOG.warning("Received X-Auth-Token but NO session uri.")
 
         return session_key, session_uri
 
     def get_update_service(self):
         """Get the UpdateService object
```

### Comparing `sushy-4.8.0/sushy/resources/base.py` & `sushy-5.0.0/sushy/resources/base.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/certificateservice/certificate.py` & `sushy-5.0.0/sushy/resources/certificateservice/certificate.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/certificateservice/certificateservice.py` & `sushy-5.0.0/sushy/resources/certificateservice/certificateservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/certificateservice/constants.py` & `sushy-5.0.0/sushy/resources/certificateservice/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/chassis/chassis.py` & `sushy-5.0.0/sushy/resources/chassis/chassis.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/chassis/constants.py` & `sushy-5.0.0/sushy/resources/chassis/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/chassis/power/constants.py` & `sushy-5.0.0/sushy/resources/chassis/power/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/chassis/power/power.py` & `sushy-5.0.0/sushy/resources/chassis/power/power.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/chassis/thermal/constants.py` & `sushy-5.0.0/sushy/resources/chassis/thermal/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/chassis/thermal/thermal.py` & `sushy-5.0.0/sushy/resources/chassis/thermal/thermal.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/common.py` & `sushy-5.0.0/sushy/resources/common.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/compositionservice/compositionservice.py` & `sushy-5.0.0/sushy/resources/compositionservice/compositionservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/compositionservice/constants.py` & `sushy-5.0.0/sushy/resources/compositionservice/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/compositionservice/resourceblock.py` & `sushy-5.0.0/sushy/resources/compositionservice/resourceblock.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/compositionservice/resourcezone.py` & `sushy-5.0.0/sushy/resources/compositionservice/resourcezone.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/constants.py` & `sushy-5.0.0/sushy/resources/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/eventservice/constants.py` & `sushy-5.0.0/sushy/resources/eventservice/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/eventservice/eventdestination.py` & `sushy-5.0.0/sushy/resources/eventservice/eventdestination.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/eventservice/eventservice.py` & `sushy-5.0.0/sushy/resources/eventservice/eventservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/fabric/constants.py` & `sushy-5.0.0/sushy/resources/fabric/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/fabric/endpoint.py` & `sushy-5.0.0/sushy/resources/fabric/endpoint.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/fabric/fabric.py` & `sushy-5.0.0/sushy/resources/fabric/fabric.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/ipaddresses.py` & `sushy-5.0.0/sushy/resources/ipaddresses.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/manager/constants.py` & `sushy-5.0.0/sushy/resources/manager/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/manager/manager.py` & `sushy-5.0.0/sushy/resources/manager/manager.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/manager/virtual_media.py` & `sushy-5.0.0/sushy/resources/manager/virtual_media.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,16 @@
         if (error.code.endswith('GeneralError')
            and 'TransferProtocolType' in error.detail):
             return True
 
         return (
             (error.code.endswith(".ActionParameterMissing")
              or error.code.endswith(".PropertyMissing"))
-            and "#/TransferProtocolType" in error.related_properties
+            and (("#/TransferProtocolType" in error.related_properties)
+                 or ("/TransferProtocolType" in error.related_properties))
         )
 
     def is_transfer_method_required(self, error=None):
         """Check the response code and body and in case of failure
 
         Try to determine if it happened due to missing TransferMethod
         """
```

### Comparing `sushy-4.8.0/sushy/resources/oem/__init__.py` & `sushy-5.0.0/sushy/resources/oem/__init__.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/oem/base.py` & `sushy-5.0.0/sushy/resources/oem/base.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/oem/common.py` & `sushy-5.0.0/sushy/resources/oem/common.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/oem/fake.py` & `sushy-5.0.0/sushy/resources/oem/fake.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/registry/attribute_registry.py` & `sushy-5.0.0/sushy/resources/registry/attribute_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 
 class AttributeRegistryEntryField(base.CompositeField):
 
     attributes = AttributeListField('Attributes')
     """List of attributes in this registry"""
 
-    # Vendors may have aditional items such as Dependencies, Menus, etc.
+    # Vendors may have additional items such as Dependencies, Menus, etc.
     # Only get the attributes.
 
 
 class AttributeRegistry(base.ResourceBase):
 
     identity = base.Field('Id', required=True)
     """The Attribute registry identity string"""
```

### Comparing `sushy-4.8.0/sushy/resources/registry/constants.py` & `sushy-5.0.0/sushy/resources/registry/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/registry/message_registry.py` & `sushy-5.0.0/sushy/resources/registry/message_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     """
 
     messages = MessageDictionaryField('Messages')
     """List of messages in this registry"""
 
 
 def parse_message(message_registries, message_field):
-    """Parse the messages in registries and substitute any parms
+    """Parse the messages in registries and substitute any params
 
     Check only registries that support messages.
 
     :param registries: dict of Message Registries
     :param message_field: settings.MessageListField to parse
 
     :returns: parsed settings.MessageListField with missing attributes filled
```

### Comparing `sushy-4.8.0/sushy/resources/registry/message_registry_file.py` & `sushy-5.0.0/sushy/resources/registry/message_registry_file.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/sessionservice/session.py` & `sushy-5.0.0/sushy/resources/sessionservice/session.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/sessionservice/sessionservice.py` & `sushy-5.0.0/sushy/resources/sessionservice/sessionservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/settings.py` & `sushy-5.0.0/sushy/resources/settings.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/system/bios.py` & `sushy-5.0.0/sushy/resources/system/bios.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/system/constants.py` & `sushy-5.0.0/sushy/resources/system/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,33 +172,33 @@
     NONE = 'None'
     """The system is not booting."""
 
     PRIMARY_PROCESSOR = 'PrimaryProcessorInitializationStarted'
     """Initialization of the Primary Processor has started."""
 
     BUS = 'BusInitializationStarted'
-    """Initalization of the buses has started."""
+    """Initialization of the buses has started."""
 
     MEMORY = 'MemoryInitializationStarted'
-    """Initalization of memory has started."""
+    """Initialization of memory has started."""
 
     SECONDARY_PROCESSOR = 'SecondaryProcessorInitializationStarted'
     """Secondary Prcessors have started initialization."""
 
     PCI_RESOURCE_CONFIG = 'PCIResourceConfigStarted'
     """Initalizatoin of PCI Resources has started."""
 
     HARDWARE_COMPLETE = 'SystemHardwareInitializationComplete'
     """Hardware Initialization is completed."""
 
     SETUP = 'SetupEntered'
     """System is in the Setup utility."""
 
     OS_BOOT_STARTED = 'OSBootStarted'
-    """Boot of the Operating Sysem has started."""
+    """Boot of the Operating System has started."""
 
     OS_RUNNING = 'OSRunning'
     """Operating System Running."""
 
     OEM = 'OEM'
     """OEM Defined Boot Progress State."""
```

### Comparing `sushy-4.8.0/sushy/resources/system/ethernet_interface.py` & `sushy-5.0.0/sushy/resources/system/ethernet_interface.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/system/network/adapter.py` & `sushy-5.0.0/sushy/resources/system/network/adapter.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/system/network/constants.py` & `sushy-5.0.0/sushy/resources/system/network/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/system/network/device_function.py` & `sushy-5.0.0/sushy/resources/system/network/device_function.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/system/network/port.py` & `sushy-5.0.0/sushy/resources/system/network/port.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/system/processor.py` & `sushy-5.0.0/sushy/resources/system/processor.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/system/secure_boot.py` & `sushy-5.0.0/sushy/resources/system/secure_boot.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/system/secure_boot_database.py` & `sushy-5.0.0/sushy/resources/system/secure_boot_database.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/system/simple_storage.py` & `sushy-5.0.0/sushy/resources/system/simple_storage.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/system/storage/constants.py` & `sushy-5.0.0/sushy/resources/system/storage/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/system/storage/controller.py` & `sushy-5.0.0/sushy/resources/system/storage/controller.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/system/storage/drive.py` & `sushy-5.0.0/sushy/resources/system/storage/drive.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/system/storage/storage.py` & `sushy-5.0.0/sushy/resources/system/storage/storage.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/system/storage/volume.py` & `sushy-5.0.0/sushy/resources/system/storage/volume.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/system/system.py` & `sushy-5.0.0/sushy/resources/system/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,15 +335,15 @@
             # is set. So we should only, and explicitly set it when we've
             # been requested to boot from UefiHTTP.
             if not http_boot_uri:
                 # This should clear out any old entries, as no URI translates
                 # to the intent of "use whatever the dhcp server says".
                 data['Boot']['HttpBootUri'] = None
             else:
-                # Explicilty set the URI.
+                # Explicitly set the URI.
                 data['Boot']['HttpBootUri'] = http_boot_uri
         elif not http_boot_uri:
             # We're not doing boot from URL, we should cleanup any setting
             # which may be from a prior step/call.
             if settings_boot_section.get('HttpBootUri'):
                 # If the setting is present, and has any value, unset it.
                 data['Boot']['HttpBootUri'] = None
```

### Comparing `sushy-4.8.0/sushy/resources/taskservice/constants.py` & `sushy-5.0.0/sushy/resources/taskservice/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/taskservice/task.py` & `sushy-5.0.0/sushy/resources/taskservice/task.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/taskservice/taskservice.py` & `sushy-5.0.0/sushy/resources/taskservice/taskservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/updateservice/constants.py` & `sushy-5.0.0/sushy/resources/updateservice/constants.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/updateservice/softwareinventory.py` & `sushy-5.0.0/sushy/resources/updateservice/softwareinventory.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/resources/updateservice/updateservice.py` & `sushy-5.0.0/sushy/resources/updateservice/updateservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/standard_registries/Base.1.0.0.json` & `sushy-5.0.0/sushy/standard_registries/Base.1.0.0.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999545454545454%*

 * *Differences: {"'Messages'": "{'AccountModified': {'Message': 'The account was successfully modified.'}}"}*

```diff
@@ -21,15 +21,15 @@
             "Message": "The account for the current session has been removed, thus the current session has been removed as well.",
             "NumberOfArgs": 0,
             "Resolution": "Attempt to connect with a valid account.",
             "Severity": "OK"
         },
         "AccountModified": {
             "Description": "Indicates that the account was successfully modified.",
-            "Message": "The account was successfully modifed.",
+            "Message": "The account was successfully modified.",
             "NumberOfArgs": 0,
             "Resolution": "No resolution is required.",
             "Severity": "OK"
         },
         "AccountNotModified": {
             "Description": "Indicates that the modification requested for the account was not successful.",
             "Message": "The account modification request failed.",
```

### Comparing `sushy-4.8.0/sushy/standard_registries/Base.1.2.0.json` & `sushy-5.0.0/sushy/standard_registries/Base.1.2.0.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/standard_registries/Base.1.3.0.json` & `sushy-5.0.0/sushy/standard_registries/Base.1.3.0.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/standard_registries/Base.1.3.1.json` & `sushy-5.0.0/sushy/standard_registries/Base.1.3.1.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/standard_registries/Base.1.4.0.json` & `sushy-5.0.0/sushy/standard_registries/Base.1.4.0.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999673458725183%*

 * *Differences: {"'Messages'": "{'ResourceTypeIncompatible': {'Description': 'Indicates that the resource type of "*

 * *               'the operation does not match that for the operation destination.  Examples of when '*

 * *               'this can happen include during a POST to a collection using the wrong resource '*

 * *               'type, an update where the @odata.types do not match or on a major version '*

 * *               "incompatibility.'}}"}*

```diff
@@ -446,15 +446,15 @@
                 "string",
                 "string"
             ],
             "Resolution": "Provide a valid resource identifier and resubmit the request.",
             "Severity": "Critical"
         },
         "ResourceTypeIncompatible": {
-            "Description": "Indicates that the resource type of the operation does not match that for the operation destination.  Examples of when this can happen include during a POST to a collection using the wrong resource type, an update where the @odata.types do not match or on a major version incompatability.",
+            "Description": "Indicates that the resource type of the operation does not match that for the operation destination.  Examples of when this can happen include during a POST to a collection using the wrong resource type, an update where the @odata.types do not match or on a major version incompatibility.",
             "Message": "The @odata.type of the request body %1 is incompatible with the @odata.type of the resource which is %2.",
             "NumberOfArgs": 2,
             "ParamTypes": [
                 "string",
                 "string"
             ],
             "Resolution": "Resubmit the request with a payload compatible with the resource's schema.",
```

### Comparing `sushy-4.8.0/sushy/taskmonitor.py` & `sushy-5.0.0/sushy/taskmonitor.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/base.py` & `sushy-5.0.0/sushy/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/TestRegistry.zip` & `sushy-5.0.0/sushy/tests/unit/json_samples/TestRegistry.zip`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/bios.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/bios.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/bios_attribute_registry.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/bios_attribute_registry.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/bios_attribute_registry_file.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/bios_attribute_registry_file.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/bios_attribute_registry_file_zthardware.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/bios_attribute_registry_file_zthardware.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/bios_attribute_registry_zthardware.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/bios_attribute_registry_zthardware.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/bios_settings.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/bios_settings.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/bios_zt.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/bios_zt.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/certificate.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/certificate.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/certificate_collection.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/certificate_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/certificate_locations.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/certificate_locations.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/certificateservice.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/certificateservice.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/chassis.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/chassis.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/chassis_collection.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/chassis_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/compositionservice.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/compositionservice.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/drive.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/drive.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/drive2.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/drive2.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/drive3.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/drive3.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/endpoint.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/endpoint.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/error.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/error.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/error_single_ext_info.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/error_single_ext_info.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/ethernet_interfaces.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/ethernet_interfaces.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/ethernet_interfaces_collection.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/ethernet_interfaces_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/eventservice.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/eventservice.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/fabric.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/fabric.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/fabric_collection.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/fabric_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/firmwareinventory_collection.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/firmwareinventory_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/manager.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/manager.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/manager_collection.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/manager_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/managerv1_18.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/managerv1_18.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/message_registry.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/message_registry.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/message_registry_file.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/message_registry_file.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/network_adapter.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/network_adapter.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/network_device_function.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/network_device_function.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/network_device_function_collection.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/network_device_function_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/network_port.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/network_port.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/network_port_collection.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/network_port_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/power.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/power.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/processor.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/processor.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/processor2.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/processor2.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/processor_collection.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/processor_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/resourceblock.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/resourceblock.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/resourcezone.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/resourcezone.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/root.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/root.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/secure_boot.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/secure_boot.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/secure_boot_database.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/secure_boot_database.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/secure_boot_database_collection.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/secure_boot_database_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/session.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/session.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/session_creation_headers.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/session_creation_headers.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/session_creation_headers_no_location.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/session_creation_headers_no_location.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/session_error.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/session_error.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/session_service.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/session_service.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/settings-body-nokia.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/settings-body-nokia.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/settings.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/settings.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/simple_storage.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/simple_storage.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/simple_storage_collection.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/simple_storage_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/softwareinventory.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/softwareinventory.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/storage.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/storage.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/storage_collection.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/storage_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/storage_controller.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/storage_controller.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/storage_controller_collection.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/storage_controller_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/system.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/system.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/system_collection.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/system_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/systemv1_20.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/systemv1_20.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/task.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/task.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/task_monitor.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/task_monitor.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/taskservice.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/taskservice.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/thermal.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/thermal.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/transfer_proto_required_error.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/transfer_proto_required_error.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/updateservice.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/updateservice.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/updateservice_no_inv.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/updateservice_no_inv.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/virtual_media.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/virtual_media.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/virtual_media_collection.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/virtual_media_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/virtual_mediav1_6.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/virtual_mediav1_6.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/volume.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/volume.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/volume2.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/volume2.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/volume3.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/volume3.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/volume4.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/volume4.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/json_samples/volume_collection.json` & `sushy-5.0.0/sushy/tests/unit/json_samples/volume_collection.json`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/certificateservice/test_certificate.py` & `sushy-5.0.0/sushy/tests/unit/resources/certificateservice/test_certificate.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/certificateservice/test_certificateservice.py` & `sushy-5.0.0/sushy/tests/unit/resources/certificateservice/test_certificateservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/chassis/test_chassis.py` & `sushy-5.0.0/sushy/tests/unit/resources/chassis/test_chassis.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/chassis/test_power.py` & `sushy-5.0.0/sushy/tests/unit/resources/chassis/test_power.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/chassis/test_thermal.py` & `sushy-5.0.0/sushy/tests/unit/resources/chassis/test_thermal.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/compositionservice/test_compositionservice.py` & `sushy-5.0.0/sushy/tests/unit/resources/compositionservice/test_compositionservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/compositionservice/test_resourceblock.py` & `sushy-5.0.0/sushy/tests/unit/resources/compositionservice/test_resourceblock.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/compositionservice/test_resourcezone.py` & `sushy-5.0.0/sushy/tests/unit/resources/compositionservice/test_resourcezone.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/eventservice/test_evendestination.py` & `sushy-5.0.0/sushy/tests/unit/resources/eventservice/test_evendestination.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/eventservice/test_eventservice.py` & `sushy-5.0.0/sushy/tests/unit/resources/eventservice/test_eventservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/fabric/test_endpoint.py` & `sushy-5.0.0/sushy/tests/unit/resources/fabric/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/fabric/test_fabric.py` & `sushy-5.0.0/sushy/tests/unit/resources/fabric/test_fabric.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/manager/test_manager.py` & `sushy-5.0.0/sushy/tests/unit/resources/manager/test_manager.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/manager/test_virtual_media.py` & `sushy-5.0.0/sushy/tests/unit/resources/manager/test_virtual_media.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,24 @@
             response_obj = json.load(f)
         response = mock.Mock(spec=['json', 'status_code'])
         response.json.return_value = response_obj
         error = exceptions.HTTPError('GET', 'VirtualMedia', response)
         retval = self.sys_virtual_media.is_transfer_protocol_required(error)
         self.assertTrue(retval)
 
+    def test_is_transfer_protocol_required_alt3(self):
+        with open('sushy/tests/unit/json_samples/'
+                  'transfer_proto_required_error3.json') as f:
+            response_obj = json.load(f)
+        response = mock.Mock(spec=['json', 'status_code'])
+        response.json.return_value = response_obj
+        error = exceptions.HTTPError('GET', 'VirtualMedia', response)
+        retval = self.sys_virtual_media.is_transfer_protocol_required(error)
+        self.assertTrue(retval)
+
     def test_is_transfer_method_required(self):
         with open('sushy/tests/unit/json_samples/'
                   'transfer_method_required_error.json') as f:
             response_obj = json.load(f)
         response = mock.Mock(spec=['json', 'status_code'])
         response.json.return_value = response_obj
         error = exceptions.HTTPError('POST', 'VirtualMedia', response)
```

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/oem/test_common.py` & `sushy-5.0.0/sushy/tests/unit/resources/oem/test_common.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/oem/test_fake.py` & `sushy-5.0.0/sushy/tests/unit/resources/oem/test_fake.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/registry/test_attribute_registry.py` & `sushy-5.0.0/sushy/tests/unit/resources/registry/test_attribute_registry.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/registry/test_message_registry.py` & `sushy-5.0.0/sushy/tests/unit/resources/registry/test_message_registry.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/registry/test_message_registry_file.py` & `sushy-5.0.0/sushy/tests/unit/resources/registry/test_message_registry_file.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/sessionservice/test_session.py` & `sushy-5.0.0/sushy/tests/unit/resources/sessionservice/test_session.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/sessionservice/test_sessionservice.py` & `sushy-5.0.0/sushy/tests/unit/resources/sessionservice/test_sessionservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/system/network/test_adapter.py` & `sushy-5.0.0/sushy/tests/unit/resources/system/network/test_adapter.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/system/network/test_device_function.py` & `sushy-5.0.0/sushy/tests/unit/resources/system/network/test_device_function.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/system/network/test_port.py` & `sushy-5.0.0/sushy/tests/unit/resources/system/network/test_port.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/system/storage/test_controller.py` & `sushy-5.0.0/sushy/tests/unit/resources/system/storage/test_controller.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/system/storage/test_drive.py` & `sushy-5.0.0/sushy/tests/unit/resources/system/storage/test_drive.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/system/storage/test_storage.py` & `sushy-5.0.0/sushy/tests/unit/resources/system/storage/test_storage.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/system/storage/test_volume.py` & `sushy-5.0.0/sushy/tests/unit/resources/system/storage/test_volume.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/system/test_bios.py` & `sushy-5.0.0/sushy/tests/unit/resources/system/test_bios.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,15 @@
             self.bios_json = json.load(f)
         # NOTE(iurygregory): ZT Hardware doesn't have Settings for Bios.
 
         self.conn.get.return_value.json.side_effect = [self.bios_json]
 
         registries = {}
         conn = mock.Mock()
-        # Note(iurygregory): re-use message registry for now.
+        # Note(iurygregory): reuse message registry for now.
         with open('sushy/tests/unit/json_samples/message_registry.json') as f:
             conn.get.return_value.json.return_value = json.load(f)
             msg_reg = message_registry.MessageRegistry(
                 conn, '/redfish/v1/Registries/Test',
                 redfish_version='1.0.2')
 
             registries['Test.1.0'] = msg_reg
```

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/system/test_ethernet_interfaces.py` & `sushy-5.0.0/sushy/tests/unit/resources/system/test_ethernet_interfaces.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/system/test_processor.py` & `sushy-5.0.0/sushy/tests/unit/resources/system/test_processor.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/system/test_secure_boot.py` & `sushy-5.0.0/sushy/tests/unit/resources/system/test_secure_boot.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/system/test_secure_boot_database.py` & `sushy-5.0.0/sushy/tests/unit/resources/system/test_secure_boot_database.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/system/test_simple_storage.py` & `sushy-5.0.0/sushy/tests/unit/resources/system/test_simple_storage.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/system/test_system.py` & `sushy-5.0.0/sushy/tests/unit/resources/system/test_system.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/taskservice/test_task.py` & `sushy-5.0.0/sushy/tests/unit/resources/taskservice/test_task.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/taskservice/test_taskservice.py` & `sushy-5.0.0/sushy/tests/unit/resources/taskservice/test_taskservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/test_base.py` & `sushy-5.0.0/sushy/tests/unit/resources/test_base.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/test_settings.py` & `sushy-5.0.0/sushy/tests/unit/resources/test_settings.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/updateservice/test_softwareinventory.py` & `sushy-5.0.0/sushy/tests/unit/resources/updateservice/test_softwareinventory.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/resources/updateservice/test_updateservice.py` & `sushy-5.0.0/sushy/tests/unit/resources/updateservice/test_updateservice.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/test_auth.py` & `sushy-5.0.0/sushy/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/test_connector.py` & `sushy-5.0.0/sushy/tests/unit/test_connector.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/test_main.py` & `sushy-5.0.0/sushy/tests/unit/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,31 +346,57 @@
 
     @mock.patch.object(main, 'LOG', autospec=True)
     def test_create_session_no_session_path_access_error(self, mock_log):
         self.root._conn._session.headers = []
         mock_res = mock.Mock()
         mock_res.status_code = 403
         mock_res.json.side_effect = ValueError('no json')
+        self.conn.post.return_value = mock_res
         mock_get_session_path = mock.Mock()
         mock_get_session_path.side_effect = exceptions.AccessError(
             'GET', 'redfish/v1', mock_res)
         self.root.get_sessions_path = mock_get_session_path
         with open('sushy/tests/unit/json_samples/'
                   'session_creation_headers_no_location.json') as f:
-            self.conn.post.return_value.headers = json.load(f)
+            mock_res.headers = json.load(f)
 
         session_key, session_uri = (
             self.root.create_session('foo', 'secret'))
         self.assertEqual('adc530e2016a0ea98c76c087f0e4b76f', session_key)
         self.assertIsNone(session_uri)
         self.conn.post.assert_called_once_with(
             '/redfish/v1/SessionService/Sessions',
             data={'UserName': 'foo', 'Password': 'secret'})
         self.assertTrue(mock_log.warning.called)
 
+    def test_create_session_recover_session_uri_from_body(self):
+        self.root._conn._session.headers = []
+        mock_res = mock.Mock()
+        mock_res.status_code = 200
+        mock_json = mock_res.json.return_value
+        mock_session_uri = mock_json.get.return_value
+
+        self.conn.post.return_value = mock_res
+        mock_get_session_path = mock.Mock()
+        mock_get_session_path.side_effect = exceptions.AccessError(
+            'GET', 'redfish/v1', mock_res)
+        self.root.get_sessions_path = mock_get_session_path
+        with open('sushy/tests/unit/json_samples/'
+                  'session_creation_headers_no_location.json') as f:
+            mock_res.headers = json.load(f)
+
+        session_key, session_uri = (
+            self.root.create_session('foo', 'secret'))
+        self.assertEqual('adc530e2016a0ea98c76c087f0e4b76f', session_key)
+        self.assertEqual(session_uri, mock_session_uri)
+        self.conn.post.assert_called_once_with(
+            '/redfish/v1/SessionService/Sessions',
+            data={'UserName': 'foo', 'Password': 'secret'})
+        mock_json.get.assert_called_with('@odata.id')
+
     def test_create_session_path_discovery(self):
         self.root._conn._session.headers = []
         with open('sushy/tests/unit/json_samples/root.json') as f:
             self.conn.get.json.return_value = json.load(f)
         with open('sushy/tests/unit/json_samples/'
                   'session_creation_headers.json') as f:
             self.conn.post.return_value.headers = json.load(f)
```

### Comparing `sushy-4.8.0/sushy/tests/unit/test_taskmonitor.py` & `sushy-5.0.0/sushy/tests/unit/test_taskmonitor.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/tests/unit/test_utils.py` & `sushy-5.0.0/sushy/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy/utils.py` & `sushy-5.0.0/sushy/utils.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/sushy.egg-info/PKG-INFO` & `sushy-5.0.0/sushy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sushy
-Version: 4.8.0
+Version: 5.0.0
 Summary: Sushy is a small Python library to communicate with Redfish based systems
 Home-page: https://docs.openstack.org/sushy/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: Overview
         ========
@@ -38,13 +38,12 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
```

### Comparing `sushy-4.8.0/sushy.egg-info/SOURCES.txt` & `sushy-5.0.0/sushy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 doc/source/conf.py
 doc/source/index.rst
 doc/source/contributor/index.rst
 doc/source/install/index.rst
 doc/source/reference/index.rst
 doc/source/reference/usage.rst
 releasenotes/notes/.placeholder
+releasenotes/notes/action-parameter-missing-7d234b96b5b1d81a.yaml
 releasenotes/notes/add-apply-time-support-to-bios-315ebad429dcab3d.yaml
 releasenotes/notes/add-bios-bf69ac56c4ae8f50.yaml
 releasenotes/notes/add-bios-update-status-cc59816c374b78e4.yaml
 releasenotes/notes/add-chassis-linkage-d8e567f9c791169d.yaml
 releasenotes/notes/add-chassis-support-5b97daffe1c61a2b.yaml
 releasenotes/notes/add-custom-connector-support-0a49c6649d5f7eaf.yaml
 releasenotes/notes/add-default-identity-10c5dd23bed0e915.yaml
@@ -357,14 +358,15 @@
 sushy/tests/unit/json_samples/task_collection.json
 sushy/tests/unit/json_samples/task_monitor.json
 sushy/tests/unit/json_samples/taskservice.json
 sushy/tests/unit/json_samples/thermal.json
 sushy/tests/unit/json_samples/transfer_method_required_error.json
 sushy/tests/unit/json_samples/transfer_proto_required_error.json
 sushy/tests/unit/json_samples/transfer_proto_required_error2.json
+sushy/tests/unit/json_samples/transfer_proto_required_error3.json
 sushy/tests/unit/json_samples/updateservice.json
 sushy/tests/unit/json_samples/updateservice_no_inv.json
 sushy/tests/unit/json_samples/virtual_media.json
 sushy/tests/unit/json_samples/virtual_media_collection.json
 sushy/tests/unit/json_samples/virtual_media_collectionv1_6.json
 sushy/tests/unit/json_samples/virtual_mediav1_6.json
 sushy/tests/unit/json_samples/volume.json
```

### Comparing `sushy-4.8.0/tools/generate-enum.py` & `sushy-5.0.0/tools/generate-enum.py`

 * *Files identical despite different names*

### Comparing `sushy-4.8.0/tox.ini` & `sushy-5.0.0/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tox]
-minversion = 3.18.0
+minversion = 4.4.0
 envlist = py3,pep8
 ignore_basepython_conflict=true
 
 [testenv]
 basepython = python3
+constrain_package_deps = true
 usedevelop = True
 setenv =
    VIRTUAL_ENV={envdir}
    PYTHONWARNINGS=default::DeprecationWarning
 deps =
   -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
   -r{toxinidir}/test-requirements.txt
@@ -16,14 +17,15 @@
 commands = stestr run --slowest {posargs}
 
 [testenv:pep8]
 deps=
     hacking~=6.0.0 # Apache-2.0
     flake8-import-order>=0.17.1 # LGPLv3
     pycodestyle>=2.0.0,<3.0.0 # MIT
+    -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
 commands = flake8 {posargs}
 
 [testenv:venv]
 setenv = PYTHONHASHSEED=0
 deps =
   -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
   -r{toxinidir}/requirements.txt
@@ -83,7 +85,16 @@
 # [H904] Delay string interpolations at logging calls.
 enable-extensions=H106,H203,H204,H205,H210,H904
 builtins = _
 exclude=.*,dist,doc,*lib/python*,*egg,build
 import-order-style = pep8
 application-import-names = sushy
 filename = *.py
+
+[testenv:codespell]
+description =
+  Run codespell to check spelling
+deps = codespell
+# note(JayF): {posargs} lets us run `tox -ecodespell -- -w` to get codespell
+#             to correct spelling issues in our code it's aware of.
+commands =
+  codespell {posargs}
```

