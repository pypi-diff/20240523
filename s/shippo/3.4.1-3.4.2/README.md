# Comparing `tmp/shippo-3.4.1.tar.gz` & `tmp/shippo-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shippo-3.4.1.tar", last modified: Mon May 13 20:46:22 2024, max compression
+gzip compressed data, was "shippo-3.4.2.tar", last modified: Thu May 23 17:39:01 2024, max compression
```

## Comparing `shippo-3.4.1.tar` & `shippo-3.4.2.tar`

### file list

```diff
@@ -1,258 +1,264 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:46:22.072456 shippo-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-13 20:46:11.000000 shippo-3.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17812 2024-05-13 20:46:22.072456 shippo-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-13 20:46:11.000000 shippo-3.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:46:22.072456 shippo-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-13 20:46:11.000000 shippo-3.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:46:22.032456 shippo-3.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:46:22.040457 shippo-3.4.1/src/shippo/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:46:22.040457 shippo-3.4.1/src/shippo/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    14213 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)    19824 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/batches.py
--rw-r--r--   0 runner    (1001) docker     (127)    28485 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/carrier_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/carrier_parcel_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/customs_declarations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/customs_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/manifests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:46:22.040457 shippo-3.4.1/src/shippo/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:46:22.060456 shippo-3.4.1/src/shippo/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/addresscompletecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/addresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/addressimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/addresspaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/addressvalidationresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/addressvalidationresultsmessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/alcohol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/batchcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/batchshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/batchshipmentbase.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/batchshipmenterrormessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/batchshipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountdpddecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountfedexcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountupscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountuspscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrieraccountwithextrainfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/carriersenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/cod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/connectexistingownaccountrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/customerreference.py
--rw-r--r--   0 runner    (1001) docker     (127)     9745 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/customsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/customsdeclarationcontentstypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/customsdeclarationcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/customsdeclarationeelpfcenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/customsdeclarationincotermenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/customsdeclarationnondeliveryoptionenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/customsdeclarationpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/customsexporteridentification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/customsinvoicedcharges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/customsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/customsitemcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/customsitempaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/customstaxidentification.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/dangerousgoodslithiumbatteries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/dangerousgoodsobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/defaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/defaultparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/departmentnumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/distanceunitenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/dryice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/fedexconnectexistingownaccountparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/instanttransactioncreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/instanttransactioncreateresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/instanttransactionrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/insurance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/invoicenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/labelfiletypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/lineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/lineitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/liverate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/liveratecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/liveratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/manifestcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/manifestpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/objectstateenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/ordercreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/orderpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/orderstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/parcelcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/parcelextra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/parcelinsurance.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/parcelpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/parcelrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/parceltemplateenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/pickupbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/ponumber.py
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/ratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/refund.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/refundpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/refundrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/responsemessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/rmanumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/servicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/servicegroupaccountandservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/servicegroupcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/servicegrouptypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/servicegroupupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/servicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)    42151 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/servicelevelenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/shipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/shipmentcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/shipmentextra.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/shipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/shippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/shippoaccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/shippoaccountupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/trackingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/trackingstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/trackingstatuslocationbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/trackingstatussubstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/tracksrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/transactioncreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/transactionpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/transactionstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/upsconnectexistingownaccountparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/userparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/userparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/components/weightunitenum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:46:22.060456 shippo-3.4.1/src/shippo/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/errors/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:46:22.060456 shippo-3.4.1/src/shippo/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:46:22.072456 shippo-3.4.1/src/shippo/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/addshipmentstobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/createaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/createbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/createcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/createcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/createcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/createliverate.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/createmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/createorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/createparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/createpickup.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/createrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/createservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/createshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/createshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/createtrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/createtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/createuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/deletedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/deleteservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/deleteuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/getaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/getbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/getcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/getcarrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/getcarrierregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/getcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/getcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/getdefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/getmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/getorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/getparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/getrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/getrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/getshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/getshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/gettrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/gettransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/getuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/listaddresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/listcarrieraccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/listcarrierparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/listcustomsdeclarations.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/listcustomsitems.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/listmanifests.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/listorders.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/listparcels.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/listrefunds.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/listservicegroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/listshipmentrates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/listshipmentratesbycurrencycode.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/listshipments.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/listshippoaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/listtransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/listuserparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/purchasebatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/registercarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/removeshipmentsfrombatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/updatecarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/updatedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/updateservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/updateshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/updateuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/models/operations/validateaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)    11426 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/pickups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15562 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/rates_at_checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/refunds.py
--rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14029 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/service_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    12041 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/shipments.py
--rw-r--r--   0 runner    (1001) docker     (127)    15058 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/shippo_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/tracking_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11272 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19025 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/user_parcel_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:46:22.072456 shippo-3.4.1/src/shippo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32651 2024-05-13 20:46:11.000000 shippo-3.4.1/src/shippo/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:46:22.040457 shippo-3.4.1/src/shippo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17812 2024-05-13 20:46:21.000000 shippo-3.4.1/src/shippo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11890 2024-05-13 20:46:21.000000 shippo-3.4.1/src/shippo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:46:21.000000 shippo-3.4.1/src/shippo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-13 20:46:21.000000 shippo-3.4.1/src/shippo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 20:46:21.000000 shippo-3.4.1/src/shippo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:01.415451 shippo-3.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-23 17:38:53.000000 shippo-3.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17812 2024-05-23 17:39:01.415451 shippo-3.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-23 17:38:53.000000 shippo-3.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 17:39:01.415451 shippo-3.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-23 17:38:53.000000 shippo-3.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:01.371451 shippo-3.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:01.375451 shippo-3.4.2/src/shippo/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:01.379451 shippo-3.4.2/src/shippo/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14213 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19824 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27210 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/carrier_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/carrier_parcel_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/customs_declarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/customs_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/manifests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:01.379451 shippo-3.4.2/src/shippo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:01.403451 shippo-3.4.2/src/shippo/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)    11696 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/addresscompletecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/addresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/addressimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/addresspaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/addressvalidationresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/addressvalidationresultsmessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/batchcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/batchshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/batchshipmentbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/batchshipmenterrormessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/batchshipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountdpddecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountfedexcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountupscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountuspscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrieraccountwithextrainfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carrierparceltemplatelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/carriersenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/cod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/connectexistingownaccountrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/customerreference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9745 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/customsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/customsdeclarationcontentstypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/customsdeclarationcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/customsdeclarationeelpfcenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/customsdeclarationincotermenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/customsdeclarationnondeliveryoptionenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/customsdeclarationpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/customsexporteridentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/customsinvoicedcharges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/customsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/customsitemcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/customsitempaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/customstaxidentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/dangerousgoodslithiumbatteries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/dangerousgoodsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/defaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/defaultparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/departmentnumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/distanceunitenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/dryice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/fedexconnectexistingownaccountparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/instanttransactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/instanttransactioncreateresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/instanttransactionrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/insurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/invoicenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/labelfiletypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/lineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/lineitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/liverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/liveratecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/liveratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/manifestcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/manifestpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/objectstateenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/ordercreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/orderpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/orderstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/parcelcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/parcelextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/parcelinsurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/parcelpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/parcelrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10534 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/parceltemplateenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/pickupbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/ponumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6504 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/ratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/refundpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/refundrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/responsemessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/rmanumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/servicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/servicegroupaccountandservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/servicegroupcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/servicegrouptypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/servicegroupupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/servicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43847 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/servicelevelenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/servicelevelwithparent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/shipmentcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17240 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/shipmentextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/shipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/shippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/shippoaccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/shippoaccountupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/trackingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/trackingstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/trackingstatuslocationbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/trackingstatussubstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/tracksrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6595 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/transactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/transactioncreateresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/transactionpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/transactionstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/upsconnectexistingownaccountparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/upsreferencefields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/userparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/userparceltemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/userparceltemplatelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/userparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/components/weightunitenum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:01.403451 shippo-3.4.2/src/shippo/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/errors/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:01.403451 shippo-3.4.2/src/shippo/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:01.415451 shippo-3.4.2/src/shippo/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/addshipmentstobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/createaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/createbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/createcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/createcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/createcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/createliverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/createmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/createorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/createparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/createpickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/createrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/createservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/createshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/createshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/createtrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/createtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/createuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/deletedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/deleteservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/deleteuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/getaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/getbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/getcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/getcarrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/getcarrierregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/getcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/getcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/getdefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/getmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/getorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/getparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/getrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/getrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/getshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/getshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/gettrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/gettransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/getuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/listaddresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/listcarrieraccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/listcarrierparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/listcustomsdeclarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/listcustomsitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/listmanifests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/listorders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/listparcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/listrefunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/listservicegroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/listshipmentrates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/listshipmentratesbycurrencycode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/listshipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/listshippoaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/listtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/listuserparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/purchasebatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/registercarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/removeshipmentsfrombatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/updatecarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/updatedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/updateservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/updateshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/updateuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/models/operations/validateaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11426 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/pickups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15429 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/rates_at_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/refunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13914 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12041 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/shipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15058 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/shippo_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/tracking_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11095 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18697 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/user_parcel_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:01.415451 shippo-3.4.2/src/shippo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32701 2024-05-23 17:38:53.000000 shippo-3.4.2/src/shippo/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:39:01.379451 shippo-3.4.2/src/shippo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17812 2024-05-23 17:39:01.000000 shippo-3.4.2/src/shippo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-05-23 17:39:01.000000 shippo-3.4.2/src/shippo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:39:01.000000 shippo-3.4.2/src/shippo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-23 17:39:01.000000 shippo-3.4.2/src/shippo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 17:39:01.000000 shippo-3.4.2/src/shippo.egg-info/top_level.txt
```

### Comparing `shippo-3.4.1/LICENSE` & `shippo-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/PKG-INFO` & `shippo-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.4.1
+Version: 3.4.2
 Summary: Shipping API Python library (USPS, FedEx, UPS and more)
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: MIT License
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
```

### Comparing `shippo-3.4.1/README.md` & `shippo-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/setup.py` & `shippo-3.4.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='shippo',
-    version='3.4.1',
+    version='3.4.2',
     author='Shippo',
     description='Shipping API Python library (USPS, FedEx, UPS and more)',
     license = 'MIT License',
     url='https://github.com/goshippo/shippo-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
```

### Comparing `shippo-3.4.1/src/shippo/_hooks/registration.py` & `shippo-3.4.2/src/shippo/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/_hooks/sdkhooks.py` & `shippo-3.4.2/src/shippo/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/_hooks/types.py` & `shippo-3.4.2/src/shippo/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/addresses.py` & `shippo-3.4.2/src/shippo/addresses.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/batches.py` & `shippo-3.4.2/src/shippo/batches.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/carrier_accounts.py` & `shippo-3.4.2/src/shippo/carrier_accounts.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
 from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
-from typing import Optional, Union
+from typing import Optional
 
 class CarrierAccounts:
     r"""Carriers are the companies who deliver your package. Shippo uses Carrier account objects as credentials to retrieve shipping rates and purchase labels from shipping Carriers.
 
     <SchemaDefinition schemaRef=\"#/components/schemas/CarrierAccount\"/>
     """
     sdk_configuration: SDKConfiguration
@@ -364,15 +364,15 @@
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def register(self, request: Union[components.CarrierAccountCanadaPostCreateRequest, components.CarrierAccountChronopostCreateRequest, components.CarrierAccountColissimoCreateRequest, components.CarrierAccountCorreosCreateRequest, components.CarrierAccountDeutschePostCreateRequest, components.CarrierAccountDHLExpressCreateRequest, components.CarrierAccountDpdDeCreateRequest, components.CarrierAccountDPDUKCreateRequest, components.CarrierAccountFedExCreateRequest, components.CarrierAccountHermesUKCreateRequest, components.CarrierAccountMondialRelayCreateRequest, components.CarrierAccountPosteItalianeCreateRequest, components.CarrierAccountUPSCreateRequest, components.CarrierAccountUSPSCreateRequest]) -> components.CarrierAccount:
+    def register(self, request: operations.RegisterCarrierAccountRequestBody) -> components.CarrierAccount:
         r"""Add a Shippo carrier account
         Adds a Shippo carrier account
         """
         hook_ctx = HookContext(operation_id='RegisterCarrierAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         _globals = operations.RegisterCarrierAccountGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
@@ -383,15 +383,15 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Union[components.CarrierAccountCanadaPostCreateRequest, components.CarrierAccountChronopostCreateRequest, components.CarrierAccountColissimoCreateRequest, components.CarrierAccountCorreosCreateRequest, components.CarrierAccountDeutschePostCreateRequest, components.CarrierAccountDHLExpressCreateRequest, components.CarrierAccountDpdDeCreateRequest, components.CarrierAccountDPDUKCreateRequest, components.CarrierAccountFedExCreateRequest, components.CarrierAccountHermesUKCreateRequest, components.CarrierAccountMondialRelayCreateRequest, components.CarrierAccountPosteItalianeCreateRequest, components.CarrierAccountUPSCreateRequest, components.CarrierAccountUSPSCreateRequest], "request", False, False, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.RegisterCarrierAccountRequestBody, "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
```

### Comparing `shippo-3.4.1/src/shippo/carrier_parcel_templates.py` & `shippo-3.4.2/src/shippo/carrier_parcel_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
 from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
-from typing import List, Optional
+from typing import Optional
 
 class CarrierParcelTemplates:
     r"""A carrier parcel template represents a package used for shipping that has preset dimensions defined by a carrier. Some examples of a carrier parcel template include USPS Flat Rate Box and Fedex Small Pak. When using a carrier parcel template, the rates returned may be limited to the carrier that provides the box. You can create user parcel templates using a carrier parcel template. Shippo takes the dimensions of the carrier parcel template but you must configure the weight.
 
     <SchemaDefinition schemaRef=\"#/components/schemas/CarrierParcelTemplate\"/>
     """
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def list(self, include: Optional[operations.Include] = None, carrier: Optional[str] = None) -> List[components.CarrierParcelTemplate]:
+    def list(self, include: Optional[operations.Include] = None, carrier: Optional[str] = None) -> components.CarrierParcelTemplateList:
         r"""List all carrier parcel templates
         List all carrier parcel template objects. <br> Use the following query string params to filter the results as needed. <br> <ul> <li>`include=all` (the default). Includes templates from all carriers </li> <li>`include=user`. Includes templates only from carriers which the user has added (whether or not they're currently enabled) </li> <li>`include=enabled`. includes templates only for carriers which the user has added and enabled </li> <li>`carrier=*token*`. filter by specific carrier, e.g. fedex, usps </li> </ul>
         """
         hook_ctx = HookContext(operation_id='ListCarrierParcelTemplates', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.ListCarrierParcelTemplatesRequest(
             include=include,
             carrier=carrier,
@@ -68,15 +68,15 @@
             
         
         
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[components.CarrierParcelTemplate]])
+                out = utils.unmarshal_json(http_res.text, Optional[components.CarrierParcelTemplateList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `shippo-3.4.1/src/shippo/customs_declarations.py` & `shippo-3.4.2/src/shippo/customs_declarations.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/customs_items.py` & `shippo-3.4.2/src/shippo/customs_items.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/debug.py` & `shippo-3.4.2/src/shippo/debug.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/manifests.py` & `shippo-3.4.2/src/shippo/manifests.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/__init__.py` & `shippo-3.4.2/src/shippo/models/components/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from .carrieraccountregistrationstatus import *
 from .carrieraccountservicelevel import *
 from .carrieraccountupscreaterequest import *
 from .carrieraccountupscreaterequestparameters import *
 from .carrieraccountuspscreaterequest import *
 from .carrieraccountwithextrainfo import *
 from .carrierparceltemplate import *
+from .carrierparceltemplatelist import *
 from .carriersenum import *
 from .cod import *
 from .connectexistingownaccountrequest import *
 from .customerreference import *
 from .customsdeclaration import *
 from .customsdeclarationb13afilingoptionenum import *
 from .customsdeclarationcontentstypeenum import *
@@ -107,14 +108,15 @@
 from .servicegroup import *
 from .servicegroupaccountandservicelevel import *
 from .servicegroupcreaterequest import *
 from .servicegrouptypeenum import *
 from .servicegroupupdaterequest import *
 from .servicelevel import *
 from .servicelevelenumset import *
+from .servicelevelwithparent import *
 from .shipment import *
 from .shipmentcreaterequest import *
 from .shipmentextra import *
 from .shipmentpaginatedlist import *
 from .shippoaccount import *
 from .shippoaccountpaginatedlist import *
 from .shippoaccountupdaterequest import *
@@ -122,17 +124,21 @@
 from .trackingstatus import *
 from .trackingstatusenum import *
 from .trackingstatuslocationbase import *
 from .trackingstatussubstatus import *
 from .tracksrequest import *
 from .transaction import *
 from .transactioncreaterequest import *
+from .transactioncreateresponse import *
 from .transactionpaginatedlist import *
 from .transactionstatusenum import *
 from .upsconnectexistingownaccountparameters import *
+from .upsreferencefields import *
 from .userparceltemplate import *
+from .userparceltemplatecreaterequest import *
+from .userparceltemplatelist import *
 from .userparceltemplateupdaterequest import *
 from .userparceltemplatewithcarriertemplatecreaterequest import *
 from .userparceltemplatewithoutcarriertemplatecreaterequest import *
 from .weightunitenum import *
 
-__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","Authentication","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentErrorMessage","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountChronopostCreateRequestParameters","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountFedExCreateRequest","CarrierAccountFedExCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountMondialRelayCreateRequest","CarrierAccountMondialRelayCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierAccountWithExtraInfo","CarrierAccountWithExtraInfoStatus","CarrierAccountWithExtraInfoType","CarrierParcelTemplate","CarriersEnum","Cod","Code","ConnectExistingOwnAccountRequest","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationB13AFilingOptionEnum","CustomsDeclarationContentsTypeEnum","CustomsDeclarationCreateRequest","CustomsDeclarationEelPfcEnum","CustomsDeclarationIncotermEnum","CustomsDeclarationNonDeliveryOptionEnum","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemCreateRequest","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnitEnum","DryIce","FedExConnectExistingOwnAccountParameters","InstantTransactionCreateRequest","InstantTransactionCreateResponse","InstantTransactionCreateResponseResponseType","InstantTransactionRate","Insurance","InvoiceNumber","LabelFileType","LabelFileTypeEnum","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","ObjectInfo","ObjectResults","ObjectState","ObjectStateEnum","Order","OrderCreateRequest","OrderPaginatedList","OrderStatusEnum","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustraliaEnum","ParcelTemplateCouriersPleaseEnum","ParcelTemplateDHLeCommerceEnum","ParcelTemplateDPDUKEnum","ParcelTemplateFedExEnum","ParcelTemplateUPSEnum","ParcelTemplateUSPSEnum","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ResponseMessage","ResponseType","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupTypeEnum","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostalEnum","ServiceLevelAPGEnum","ServiceLevelAirterraEnum","ServiceLevelAramexAustraliaEnum","ServiceLevelAsendiaEnum","ServiceLevelAustraliaPostEnum","ServiceLevelAxleHireEnum","ServiceLevelBetterTrucksEnum","ServiceLevelCDLEnum","ServiceLevelCanadaPostEnum","ServiceLevelChronopostEnum","ServiceLevelColissimoEnum","ServiceLevelCorreosEspanaEnum","ServiceLevelCouriersPleaseEnum","ServiceLevelDHLExpressEnum","ServiceLevelDHLGermanyEnum","ServiceLevelDHLeCommerceEnum","ServiceLevelDPDDEEnum","ServiceLevelDPDUKEnum","ServiceLevelDeutschePostEnum","ServiceLevelEvriUKEnum","ServiceLevelFedExEnum","ServiceLevelGLSUSEnum","ServiceLevelGlobegisticsEnum","ServiceLevelLSOEnum","ServiceLevelLasershipEnum","ServiceLevelMaergoEnum","ServiceLevelMondialRelayEnum","ServiceLevelOnTracEnum","ServiceLevelParcelforceEnum","ServiceLevelPostItalianeEnum","ServiceLevelPurolatorEnum","ServiceLevelRoyalMailEnum","ServiceLevelSendleEnum","ServiceLevelSwyftEnum","ServiceLevelUDSEnum","ServiceLevelUPSEnum","ServiceLevelUSPSEnum","ServiceLevelVehoEnum","ServiceLevelePostGlobalEnum","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnitEnum"]
+__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressFrom","AddressImporter","AddressPaginatedList","AddressReturn","AddressTo","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","Authentication","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentErrorMessage","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountBaseParameters","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountChronopostCreateRequestParameters","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountFedExCreateRequest","CarrierAccountFedExCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountMondialRelayCreateRequest","CarrierAccountMondialRelayCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountParameters","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierAccountWithExtraInfo","CarrierAccountWithExtraInfoStatus","CarrierAccountWithExtraInfoType","CarrierParcelTemplate","CarrierParcelTemplateList","CarriersEnum","Cod","Code","ConnectExistingOwnAccountRequest","ConnectExistingOwnAccountRequestParameters","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationB13AFilingOptionEnum","CustomsDeclarationContentsTypeEnum","CustomsDeclarationCreateRequest","CustomsDeclarationEelPfcEnum","CustomsDeclarationIncotermEnum","CustomsDeclarationNonDeliveryOptionEnum","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemCreateRequest","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnitEnum","DryIce","FedExConnectExistingOwnAccountParameters","InstantTransactionCreateRequest","InstantTransactionCreateResponse","InstantTransactionCreateResponseResponseType","InstantTransactionRate","Insurance","InvoiceNumber","LabelFileType","LabelFileTypeEnum","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRateCreateRequestAddressFrom","LiveRateCreateRequestAddressTo","LiveRateCreateRequestParcel","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestCreateRequestAddressFrom","ManifestPaginatedList","ManifestStatus","ObjectInfo","ObjectResults","ObjectState","ObjectStateEnum","Order","OrderCreateRequest","OrderPaginatedList","OrderStatusEnum","Parameters","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustraliaEnum","ParcelTemplateCouriersPleaseEnum","ParcelTemplateDHLeCommerceEnum","ParcelTemplateDPDUKEnum","ParcelTemplateEnumSet","ParcelTemplateFedExEnum","ParcelTemplateUPSEnum","ParcelTemplateUSPSEnum","Parcels","ParentServicelevel","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ResponseMessage","ResponseType","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupTypeEnum","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostalEnum","ServiceLevelAPGEnum","ServiceLevelAirterraEnum","ServiceLevelAramexAustraliaEnum","ServiceLevelAsendiaEnum","ServiceLevelAustraliaPostEnum","ServiceLevelAxleHireEnum","ServiceLevelBetterTrucksEnum","ServiceLevelCDLEnum","ServiceLevelCanadaPostEnum","ServiceLevelChronopostEnum","ServiceLevelColissimoEnum","ServiceLevelCorreosEspanaEnum","ServiceLevelCouriersPleaseEnum","ServiceLevelDHLExpressEnum","ServiceLevelDHLGermanyEnum","ServiceLevelDHLeCommerceEnum","ServiceLevelDPDDEEnum","ServiceLevelDPDUKEnum","ServiceLevelDeutschePostEnum","ServiceLevelEnumSet","ServiceLevelEvriUKEnum","ServiceLevelFedExEnum","ServiceLevelGLSUSEnum","ServiceLevelGlobegisticsEnum","ServiceLevelLSOEnum","ServiceLevelLasershipEnum","ServiceLevelMaergoEnum","ServiceLevelMondialRelayEnum","ServiceLevelOnTracEnum","ServiceLevelParcelforceEnum","ServiceLevelPostItalianeEnum","ServiceLevelPurolatorEnum","ServiceLevelRoyalMailEnum","ServiceLevelSendleEnum","ServiceLevelSwyftEnum","ServiceLevelUDSEnum","ServiceLevelUPSEnum","ServiceLevelUSPSEnum","ServiceLevelVehoEnum","ServiceLevelWithParent","ServiceLevelePostGlobalEnum","Shipment","ShipmentCreateRequest","ShipmentCreateRequestCustomsDeclaration","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionCreateResponse","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UPSReferenceFields","UserParcelTemplate","UserParcelTemplateCreateRequest","UserParcelTemplateList","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnitEnum"]
```

### Comparing `shippo-3.4.1/src/shippo/models/components/address.py` & `shippo-3.4.2/src/shippo/models/components/address.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,23 +63,23 @@
     email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     r"""E-mail address of the contact person, RFC3696/5321-compliant."""
     is_residential: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_residential'), 'exclude': lambda f: f is None }})
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""A string of up to 100 characters that can be filled with any additional information you want
     to attach to the object.
     """
-    latitude: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('latitude'), 'exclude': lambda f: f is None }})
-    r"""Latitude of address"""
-    longitude: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('longitude'), 'exclude': lambda f: f is None }})
-    r"""Longitude of address"""
     is_complete: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_complete'), 'exclude': lambda f: f is None }})
     r"""Complete addresses contain all required values.<br><br>Incomplete addresses have failed one or multiple
     validations.<br>Incomplete Addresses are eligible for requesting rates but lack at least one required 
     value for purchasing labels.
     """
+    latitude: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('latitude'), 'exclude': lambda f: f is None }})
+    r"""Latitude of address"""
+    longitude: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('longitude'), 'exclude': lambda f: f is None }})
+    r"""Longitude of address"""
     object_created: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_created'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""Date and time of Address creation."""
     object_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the given Address object.
     This ID is required to create a Shipment object.
     """
     object_owner: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_owner'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.4.1/src/shippo/models/components/addresscompletecreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/addresscompletecreaterequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,14 +60,10 @@
     email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     r"""E-mail address of the contact person, RFC3696/5321-compliant."""
     is_residential: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_residential'), 'exclude': lambda f: f is None }})
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""A string of up to 100 characters that can be filled with any additional information you want
     to attach to the object.
     """
-    latitude: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('latitude'), 'exclude': lambda f: f is None }})
-    r"""Latitude of address"""
-    longitude: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('longitude'), 'exclude': lambda f: f is None }})
-    r"""Longitude of address"""
     validate: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validate'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.4.1/src/shippo/models/components/addresscreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/addresscreaterequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,11 @@
     email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email'), 'exclude': lambda f: f is None }})
     r"""E-mail address of the contact person, RFC3696/5321-compliant."""
     is_residential: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_residential'), 'exclude': lambda f: f is None }})
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""A string of up to 100 characters that can be filled with any additional information you want
     to attach to the object.
     """
-    latitude: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('latitude'), 'exclude': lambda f: f is None }})
-    r"""Latitude of address"""
-    longitude: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('longitude'), 'exclude': lambda f: f is None }})
-    r"""Longitude of address"""
     validate: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validate'), 'exclude': lambda f: f is None }})
     r"""Set to true to validate Address object."""
```

### Comparing `shippo-3.4.1/src/shippo/models/components/addressimporter.py` & `shippo-3.4.2/src/shippo/models/components/addressimporter.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/addresspaginatedlist.py` & `shippo-3.4.2/src/shippo/models/components/addresspaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/addressvalidationresults.py` & `shippo-3.4.2/src/shippo/models/components/addressvalidationresults.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/addressvalidationresultsmessage.py` & `shippo-3.4.2/src/shippo/models/components/addressvalidationresultsmessage.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
 from typing import Optional
 
+
 class Code(str, Enum):
     VERIFICATION_ERROR = 'verification_error'
     UNKNOWN_STREET_LOWER = 'unknown_street'
     COMPONENT_MISMATCH_ERROR = 'component_mismatch_error'
     MULTIPLE_MATCH = 'multiple_match'
     SUB_PREMISE_NUMBER_INVALID = 'sub_premise_number_invalid'
     SUB_PREMISE_NUMBER_MISSING = 'sub_premise_number_missing'
@@ -65,14 +66,15 @@
     NON_DELIVERABLE_ZIP4 = 'Non-Deliverable ZIP4'
     MULTIPLE_RESPONSES = 'Multiple Responses'
     INVALID_DUAL_ADDRESS = 'Invalid Dual Address'
     INVALID_STATE = 'Invalid State'
     INVALID_CITY = 'Invalid City'
     AMBIGUOUS_ADDRESS = 'Ambiguous Address'
 
+
 class Source(str, Enum):
     SHIPPO_ADDRESS_VALIDATOR = 'Shippo Address Validator'
     UPS = 'UPS'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `shippo-3.4.1/src/shippo/models/components/alcohol.py` & `shippo-3.4.2/src/shippo/models/components/alcohol.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
 from typing import Optional
 
+
 class RecipientType(str, Enum):
     r"""Mandatory for Fedex only. License type of the recipient of the Alcohol Package."""
     LICENSEE = 'licensee'
     CONSUMER = 'consumer'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `shippo-3.4.1/src/shippo/models/components/batch.py` & `shippo-3.4.2/src/shippo/models/components/batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     creation_failed: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creation_failed') }})
     creation_succeeded: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('creation_succeeded') }})
     purchase_failed: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('purchase_failed') }})
     purchase_succeeded: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('purchase_succeeded') }})
     
 
 
+
 class BatchStatus(str, Enum):
     r"""Batches that are `VALIDATING` are being created and validated<br>
     `VALID` batches can be purchased<br>
     `INVALID` batches cannot be purchased, `INVALID` BatchShipments must be removed<br>
     Batches that are in the `PURCHASING` state are being purchased<br>
     `PURCHASED` batches are finished purchasing.
     """
```

### Comparing `shippo-3.4.1/src/shippo/models/components/batchcreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/batchcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/batchshipment.py` & `shippo-3.4.2/src/shippo/models/components/batchshipment.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .batchshipmenterrormessage import BatchShipmentErrorMessage
 from .shipmentcreaterequest import ShipmentCreateRequest
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
+
 class Status(str, Enum):
     r"""`INVALID` batch shipments cannot be purchased and will have to be removed, fixed, and added to the batch again.<br>
     `VALID` batch shipments can be purchased. <br>
     Batch shipments with the status `TRANSACTION_FAILED` were not able to be purchased and the error will be displayed on the message field<br> 
     `INCOMPLETE` batch shipments have an issue with the Address and will need to be removed, fixed, and added to the batch again.
     """
     INVALID = 'INVALID'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/batchshipmentbase.py` & `shippo-3.4.2/src/shippo/models/components/batchshipmentbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/batchshipmenterrormessage.py` & `shippo-3.4.2/src/shippo/models/components/batchshipmenterrormessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/batchshipmentpaginatedlist.py` & `shippo-3.4.2/src/shippo/models/components/batchshipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/billing.py` & `shippo-3.4.2/src/shippo/models/components/billing.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
 from typing import Optional
 
+
 class Type(str, Enum):
     r"""Party to be billed. (Leave blank for DHL Germany.)"""
     SENDER = 'SENDER'
     RECIPIENT = 'RECIPIENT'
     THIRD_PARTY = 'THIRD_PARTY'
     THIRD_PARTY_CONSIGNEE = 'THIRD_PARTY_CONSIGNEE'
     COLLECT = 'COLLECT'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccount.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccount.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from .carrieraccountservicelevel import CarrierAccountServiceLevel
 from .fedexconnectexistingownaccountparameters import FedExConnectExistingOwnAccountParameters
 from .upsconnectexistingownaccountparameters import UPSConnectExistingOwnAccountParameters
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Any, Dict, List, Optional, Union
 
+CarrierAccountParameters = Union[Dict[str, Any], FedExConnectExistingOwnAccountParameters, UPSConnectExistingOwnAccountParameters]
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CarrierAccount:
     account_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_id') }})
     r"""Unique identifier of the account. Please check the <a href=\\"https://docs.goshippo.com/docs/carriers/carrieraccounts/\\">carrier accounts tutorial</a>
     page for the `account_id` per carrier.<br> 
@@ -22,15 +24,15 @@
     r"""Carrier token, see <a href=\\"#tag/Carriers\\">Carriers</a><br>
     Please check the <a href=\"https://docs.goshippo.com/docs/carriers/carrieraccounts/\">carrier accounts tutorial</a> page for all supported carriers.
     """
     active: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('active'), 'exclude': lambda f: f is None }})
     r"""Determines whether the account is active. When creating a shipment, if no `carrier_accounts` are explicitly
     passed Shippo will query all carrier accounts that have this field set. By default, this is set to True.
     """
-    parameters: Optional[Union[Dict[str, Any], FedExConnectExistingOwnAccountParameters, UPSConnectExistingOwnAccountParameters]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
+    parameters: Optional[CarrierAccountParameters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
     carrier_name: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier_name'), 'exclude': lambda f: f is None }})
     r"""Carrier name, see <a href=\\"#tag/Carriers\\">Carriers</a><br>"""
     is_shippo_account: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_shippo_account'), 'exclude': lambda f: f is None }})
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     object_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the carrier account object."""
     object_owner: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_owner'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountbase.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountbase.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import dataclasses
 from .fedexconnectexistingownaccountparameters import FedExConnectExistingOwnAccountParameters
 from .upsconnectexistingownaccountparameters import UPSConnectExistingOwnAccountParameters
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Any, Dict, Optional, Union
 
+CarrierAccountBaseParameters = Union[Dict[str, Any], FedExConnectExistingOwnAccountParameters, UPSConnectExistingOwnAccountParameters]
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CarrierAccountBase:
     account_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_id') }})
     r"""Unique identifier of the account. Please check the <a href=\\"https://docs.goshippo.com/docs/carriers/carrieraccounts/\\">carrier accounts tutorial</a>
     page for the `account_id` per carrier.<br> 
@@ -21,10 +23,10 @@
     r"""Carrier token, see <a href=\\"#tag/Carriers\\">Carriers</a><br>
     Please check the <a href=\"https://docs.goshippo.com/docs/carriers/carrieraccounts/\">carrier accounts tutorial</a> page for all supported carriers.
     """
     active: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('active'), 'exclude': lambda f: f is None }})
     r"""Determines whether the account is active. When creating a shipment, if no `carrier_accounts` are explicitly
     passed Shippo will query all carrier accounts that have this field set. By default, this is set to True.
     """
-    parameters: Optional[Union[Dict[str, Any], FedExConnectExistingOwnAccountParameters, UPSConnectExistingOwnAccountParameters]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
+    parameters: Optional[CarrierAccountBaseParameters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountchronopostcreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountchronopostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountcolissimocreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountcolissimocreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountcorreoscreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountcorreoscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountdpddecreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountdpddecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountdpdukcreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountdpdukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountfedexcreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountfedexcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccounthermesukcreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccounthermesukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountpaginatedlist.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountregistrationstatus.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountservicelevel.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountupscreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountupscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountupscreaterequestparameters.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountupscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountuspscreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountuspscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carrieraccountwithextrainfo.py` & `shippo-3.4.2/src/shippo/models/components/carrieraccountwithextrainfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,23 @@
 from .fedexconnectexistingownaccountparameters import FedExConnectExistingOwnAccountParameters
 from .upsconnectexistingownaccountparameters import UPSConnectExistingOwnAccountParameters
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
 from typing import Any, Dict, List, Optional, Union
 
+Parameters = Union[Dict[str, Any], FedExConnectExistingOwnAccountParameters, UPSConnectExistingOwnAccountParameters]
+
+
 class CarrierAccountWithExtraInfoType(str, Enum):
     r"""Authentication method used by this account."""
     DEFAULT = 'default'
     OAUTH = 'oauth'
 
+
 class CarrierAccountWithExtraInfoStatus(str, Enum):
     r"""Current authentication status. Possible values: 'disconnected' (authorization lost, reconnect needed), 'connected' (authorized and active), 'authorization_pending' (awaiting initial authorization flow)."""
     DISCONNECTED = 'disconnected'
     CONNECTED = 'connected'
     AUTHORIZATION_PENDING = 'authorization_pending'
 
 
@@ -54,15 +58,15 @@
     r"""Carrier token, see <a href=\\"#tag/Carriers\\">Carriers</a><br>
     Please check the <a href=\"https://docs.goshippo.com/docs/carriers/carrieraccounts/\">carrier accounts tutorial</a> page for all supported carriers.
     """
     active: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('active'), 'exclude': lambda f: f is None }})
     r"""Determines whether the account is active. When creating a shipment, if no `carrier_accounts` are explicitly
     passed Shippo will query all carrier accounts that have this field set. By default, this is set to True.
     """
-    parameters: Optional[Union[Dict[str, Any], FedExConnectExistingOwnAccountParameters, UPSConnectExistingOwnAccountParameters]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
+    parameters: Optional[Parameters] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters'), 'exclude': lambda f: f is None }})
     carrier_name: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier_name'), 'exclude': lambda f: f is None }})
     r"""Carrier name, see <a href=\\"#tag/Carriers\\">Carriers</a><br>"""
     is_shippo_account: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_shippo_account'), 'exclude': lambda f: f is None }})
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     object_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id'), 'exclude': lambda f: f is None }})
     r"""Unique identifier of the carrier account object."""
     object_owner: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_owner'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.4.1/src/shippo/models/components/carrierparceltemplate.py` & `shippo-3.4.2/src/shippo/models/components/carrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/carriersenum.py` & `shippo-3.4.2/src/shippo/models/components/carriersenum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
+
 class CarriersEnum(str, Enum):
     r"""|Token | Carrier name|
     |:---|:---|
     | airterra | Airterra |
     | apc_postal | APC Postal|
     | apg | APG|
     | aramex | Aramex|
```

### Comparing `shippo-3.4.1/src/shippo/models/components/cod.py` & `shippo-3.4.2/src/shippo/models/components/cod.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
 from typing import Optional
 
+
 class PaymentMethod(str, Enum):
     r"""Secured funds include money orders, certified cheques and others (see
     <a href=\"https://www.ups.com/content/us/en/shipping/time/service/value_added/cod.html\">UPS</a> for details). 
     If no payment_method inputted the value defaults to \"ANY\".)
     """
     SECURED_FUNDS = 'SECURED_FUNDS'
     CASH = 'CASH'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/connectexistingownaccountrequest.py` & `shippo-3.4.2/src/shippo/models/components/connectexistingownaccountrequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 import dataclasses
 from .fedexconnectexistingownaccountparameters import FedExConnectExistingOwnAccountParameters
 from .upsconnectexistingownaccountparameters import UPSConnectExistingOwnAccountParameters
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Any, Dict, Optional, Union
 
+ConnectExistingOwnAccountRequestParameters = Union[Dict[str, Any], FedExConnectExistingOwnAccountParameters, UPSConnectExistingOwnAccountParameters]
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ConnectExistingOwnAccountRequest:
     account_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_id') }})
     carrier: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier') }})
-    parameters: Union[Dict[str, Any], FedExConnectExistingOwnAccountParameters, UPSConnectExistingOwnAccountParameters] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters') }})
+    parameters: ConnectExistingOwnAccountRequestParameters = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parameters') }})
     active: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('active'), 'exclude': lambda f: f is None }})
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     test: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('test'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.4.1/src/shippo/models/components/customerreference.py` & `shippo-3.4.2/src/shippo/models/components/customerreference.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CustomerReference:
-    r"""Specify the reference field on the label (FedEx only)."""
+    r"""Specify the reference field on the label (FedEx and UPS only)."""
     prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prefix'), 'exclude': lambda f: f is None }})
     r"""Custom prefix for customer reference field (ZPL labels only). Up to 11 characters, including trailing
     spaces. Empty string indicates removal of default prefix. To use the default prefix, do not include
     this property.
     """
     value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value'), 'exclude': lambda f: f is None }})
     r"""Optional text to be printed on the shipping label for customer reference. Up to 40 characters. If
     this is provided, reference_1 will be ignored.
     """
+    ref_sort: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ref_sort'), 'exclude': lambda f: f is None }})
+    r"""Order UPS reference fields are printed on ZPL labels. For UPS shipments, if you choose to set `ref_sort` for one reference, you must set `ref_sort` for all other supported UPS references using unique integers."""
```

### Comparing `shippo-3.4.1/src/shippo/models/components/customsdeclaration.py` & `shippo-3.4.2/src/shippo/models/components/customsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py` & `shippo-3.4.2/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
+
 class CustomsDeclarationB13AFilingOptionEnum(str, Enum):
     r"""B13A Option details are obtained by filing a B13A Canada Export Declaration via the Canadian Export Reporting System (CERS).
     <a href=\"https://www.cbsa-asfc.gc.ca/services/export/guide-eng.html\" target=\"_blank\" rel=\"noopener noreferrer\"> More information on reporting commercial exports from Canada. </a>
     Allowed values available <a href=\"#tag/Customs-Declaration-B13A-Filing-Option\">here</a>
     """
     FILED_ELECTRONICALLY = 'FILED_ELECTRONICALLY'
     SUMMARY_REPORTING = 'SUMMARY_REPORTING'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/customsdeclarationcontentstypeenum.py` & `shippo-3.4.2/src/shippo/models/components/customsdeclarationcontentstypeenum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
+
 class CustomsDeclarationContentsTypeEnum(str, Enum):
     r"""Type of goods of the shipment.
     Allowed values available <a href=\"#tag/Customs-Declaration-Contents-Type\">here</a>
     """
     DOCUMENTS = 'DOCUMENTS'
     GIFT = 'GIFT'
     SAMPLE = 'SAMPLE'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/customsdeclarationcreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/customsdeclarationcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/customsdeclarationeelpfcenum.py` & `shippo-3.4.2/src/shippo/models/components/customsdeclarationeelpfcenum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
+
 class CustomsDeclarationEelPfcEnum(str, Enum):
     r"""EEL / PFC type of the shipment. For most shipments from the US to CA, `NOEEI_30_36` is applicable; for most
     other shipments from the US, `NOEEI_30_37_a` is applicable.
     Allowed values available <a href=\"#tag/Customs-Declaration-EELPFC\">here</a>
     """
     NOEEI_30_37_A = 'NOEEI_30_37_a'
     NOEEI_30_37_H = 'NOEEI_30_37_h'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/customsdeclarationincotermenum.py` & `shippo-3.4.2/src/shippo/models/components/customsdeclarationincotermenum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
+
 class CustomsDeclarationIncotermEnum(str, Enum):
     r"""The incoterm reference of the shipment. FCA is available for DHL Express and FedEx only.
     eDAP is available for DPD UK only. DAP is available for DHL Express and DPD UK.
     If expecting DAP for other carriers, please use DDU.
     Allowed values available <a href=\"#tag/Customs-Declaration-Incoterm\">here</a>
     """
     DDP = 'DDP'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/customsdeclarationpaginatedlist.py` & `shippo-3.4.2/src/shippo/models/components/customsdeclarationpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/customsexporteridentification.py` & `shippo-3.4.2/src/shippo/models/components/customsexporteridentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/customsinvoicedcharges.py` & `shippo-3.4.2/src/shippo/models/components/customsinvoicedcharges.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/customsitem.py` & `shippo-3.4.2/src/shippo/models/components/customsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/customsitemcreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/customsitemcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/customsitempaginatedlist.py` & `shippo-3.4.2/src/shippo/models/components/customsitempaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/customstaxidentification.py` & `shippo-3.4.2/src/shippo/models/components/customstaxidentification.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
 from typing import Optional
 
+
 class CustomsTaxIdentificationType(str, Enum):
     r"""Type of tax identification.
     * `EIN` - Employer Identification Number, also known as a Federal Tax Identification Number.
     * `VAT` - Value Added Tax identification number.
     * `IOSS` - Import One-Stop Shop
     * `ARN` - Australian Taxation Office Reference Number
     """
```

### Comparing `shippo-3.4.1/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py` & `shippo-3.4.2/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/dangerousgoodslithiumbatteries.py` & `shippo-3.4.2/src/shippo/models/components/dangerousgoodslithiumbatteries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/dangerousgoodsobject.py` & `shippo-3.4.2/src/shippo/models/components/dangerousgoodsobject.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/defaultparceltemplate.py` & `shippo-3.4.2/src/shippo/models/components/defaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/defaultparceltemplateupdaterequest.py` & `shippo-3.4.2/src/shippo/models/components/defaultparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/departmentnumber.py` & `shippo-3.4.2/src/shippo/models/components/upsreferencefields.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DepartmentNumber:
-    r"""Specify the department number field on the label (FedEx only)."""
+class UPSReferenceFields:
     prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prefix'), 'exclude': lambda f: f is None }})
-    r"""Custom prefix for department number field (ZPL labels only). Up to 11 characters, including trailing
-    spaces. Empty string indicates removal of default prefix. To use the default prefix, do not include
-    this property.
-    """
+    r"""Custom prefix text."""
     value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value'), 'exclude': lambda f: f is None }})
-    r"""Optional text to be printed on the shipping label for department number. Up to 40 characters."""
+    r"""Label reference text. 35 character limit."""
+    ref_sort: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ref_sort'), 'exclude': lambda f: f is None }})
+    r"""Order UPS reference fields are printed on ZPL labels. For UPS shipments, if you choose to set `ref_sort` for one reference, you must set `ref_sort` for all other supported UPS references using unique integers."""
```

### Comparing `shippo-3.4.1/src/shippo/models/components/dryice.py` & `shippo-3.4.2/src/shippo/models/components/dryice.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/fedexconnectexistingownaccountparameters.py` & `shippo-3.4.2/src/shippo/models/components/fedexconnectexistingownaccountparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/instanttransactioncreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/instanttransactioncreaterequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import dataclasses
 from .shipmentcreaterequest import ShipmentCreateRequest
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
 from typing import Optional
 
+
 class LabelFileType(str, Enum):
     PNG = 'PNG'
     PNG_2_3X7_5 = 'PNG_2.3x7.5'
     PDF = 'PDF'
     PDF_2_3X7_5 = 'PDF_2.3x7.5'
     PDF_4X6 = 'PDF_4x6'
     PDF_4X8 = 'PDF_4x8'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/instanttransactioncreateresponse.py` & `shippo-3.4.2/src/shippo/models/components/instanttransactioncreateresponse.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .transactionstatusenum import TransactionStatusEnum
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
+
 class InstantTransactionCreateResponseResponseType(str, Enum):
     INSTANT = 'instant'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class InstantTransactionCreateResponse:
```

### Comparing `shippo-3.4.1/src/shippo/models/components/instanttransactionrate.py` & `shippo-3.4.2/src/shippo/models/components/instanttransactionrate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/insurance.py` & `shippo-3.4.2/src/shippo/models/components/insurance.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
 from typing import Optional
 
+
 class Provider(str, Enum):
     r"""To have insurance cover provided by a carrier directly instead of Shippo's provider (XCover), set `provider` to `FEDEX`, `UPS`, or `ONTRAC`."""
     FEDEX = 'FEDEX'
     UPS = 'UPS'
     ONTRAC = 'ONTRAC'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/invoicenumber.py` & `shippo-3.4.2/src/shippo/models/components/invoicenumber.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class InvoiceNumber:
-    r"""Specify the invoice number field on the label (FedEx only)."""
+    r"""Specify the invoice number field on the label (FedEx and UPS only)."""
     prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prefix'), 'exclude': lambda f: f is None }})
     r"""Custom prefix for invoice number field (ZPL labels only). Up to 11 characters, including trailing
     spaces. Empty string indicates removal of default prefix. To use the default prefix, do not include
     this property.
     """
     value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value'), 'exclude': lambda f: f is None }})
     r"""Optional text to be printed on the shipping label for invoice number. Up to 40 characters. If
     provided, this will be used on the label instead of shipment.customs_declaration.invoice.
     """
+    ref_sort: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ref_sort'), 'exclude': lambda f: f is None }})
+    r"""Order UPS reference fields are printed on ZPL labels. For UPS shipments, if you choose to set `ref_sort` for one reference, you must set `ref_sort` for all other supported UPS references using unique integers."""
```

### Comparing `shippo-3.4.1/src/shippo/models/components/labelfiletypeenum.py` & `shippo-3.4.2/src/shippo/models/components/labelfiletypeenum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
+
 class LabelFileTypeEnum(str, Enum):
     r"""Print format of the <a href=\\"https://docs.goshippo.com/docs/shipments/shippinglabelsizes/\\">label</a>. If empty, will use the default format set from
     <a href=\"https://apps.goshippo.com/settings/labels\">the Shippo dashboard.</a>
     """
     PNG = 'PNG'
     PNG_2_3X7_5 = 'PNG_2.3x7.5'
     PDF = 'PDF'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/lineitem.py` & `shippo-3.4.2/src/shippo/models/components/lineitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/lineitembase.py` & `shippo-3.4.2/src/shippo/models/components/lineitembase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/liverate.py` & `shippo-3.4.2/src/shippo/models/components/liverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/liveratecreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/liveratecreaterequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,33 @@
 from .addresscompletecreaterequest import AddressCompleteCreateRequest
 from .lineitem import LineItem
 from .parcel import Parcel
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import List, Optional, Union
 
+LiveRateCreateRequestAddressFrom = Union[str, AddressCompleteCreateRequest]
+
+LiveRateCreateRequestAddressTo = Union[str, AddressCompleteCreateRequest]
+
+LiveRateCreateRequestParcel = Union[str, Parcel]
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class LiveRateCreateRequest:
-    address_to: Union[str, AddressCompleteCreateRequest] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_to') }})
+    address_to: LiveRateCreateRequestAddressTo = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_to') }})
     r"""The recipient address, which includes the recipient's name, company name, street address, city, state, zip code,
     country, phone number, and email address (strings). Special characters should not be included in 
     any address element, especially name, company, and email.
     """
     line_items: List[LineItem] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line_items') }})
     r"""Array of Line Item objects"""
-    address_from: Optional[Union[str, AddressCompleteCreateRequest]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_from'), 'exclude': lambda f: f is None }})
+    address_from: Optional[LiveRateCreateRequestAddressFrom] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_from'), 'exclude': lambda f: f is None }})
     r"""The sender address, which includes your name, company name, street address, city, state, zip code,
     country, phone number, and email address (strings). Special characters should not be included in 
     any address element, especially name, company, and email.
     """
-    parcel: Optional[Union[str, Parcel]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parcel'), 'exclude': lambda f: f is None }})
+    parcel: Optional[LiveRateCreateRequestParcel] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parcel'), 'exclude': lambda f: f is None }})
     r"""Object ID for an existing User Parcel Template OR a fully formed Parcel object."""
```

### Comparing `shippo-3.4.1/src/shippo/models/components/liveratepaginatedlist.py` & `shippo-3.4.2/src/shippo/models/components/liveratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/location.py` & `shippo-3.4.2/src/shippo/models/components/location.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import dataclasses
 from .addresscompletecreaterequest import AddressCompleteCreateRequest
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
 from typing import Optional
 
+
 class BuildingLocationType(str, Enum):
     r"""Where your parcels will be available for pickup. \\"Security Deck\\" and \\"Shipping Dock\\" are only
     supported for DHL Express.
     """
     BACK_DOOR = 'Back Door'
     RING_BELL = 'Ring Bell'
     SECURITY_DECK = 'Security Deck'
@@ -21,14 +22,15 @@
     IN_AT_MAILBOX = 'In/At Mailbox'
     MAIL_ROOM = 'Mail Room'
     OFFICE = 'Office'
     OTHER = 'Other'
     RECEPTION = 'Reception'
     SIDE_DOOR = 'Side Door'
 
+
 class BuildingType(str, Enum):
     r"""The type of building where the pickup is located."""
     APARTMENT = 'apartment'
     BUILDING = 'building'
     DEPARTMENT = 'department'
     FLOOR = 'floor'
     ROOM = 'room'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/manifest.py` & `shippo-3.4.2/src/shippo/models/components/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
+
 class ManifestStatus(str, Enum):
     r"""Indicates the status of the manifest."""
     QUEUED = 'QUEUED'
     SUCCESS = 'SUCCESS'
     ERROR = 'ERROR'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/manifestcreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/manifestcreaterequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 from __future__ import annotations
 import dataclasses
 from .addresscreaterequest import AddressCreateRequest
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import List, Optional, Union
 
+ManifestCreateRequestAddressFrom = Union[AddressCreateRequest, str]
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ManifestCreateRequest:
     carrier_account: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier_account') }})
     r"""ID of carrier account"""
     shipment_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shipment_date') }})
     r"""All shipments to be submitted on this day will be closed out.
     Must be in the format `2014-01-18T00:35:03.463Z` (ISO 8601 date).
     """
-    address_from: Union[AddressCreateRequest, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_from') }})
+    address_from: ManifestCreateRequestAddressFrom = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_from') }})
     transactions: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transactions'), 'exclude': lambda f: f is None }})
     r"""IDs transactions to use. If you set this to null or not send this parameter,
     Shippo will automatically assign all applicable transactions.
     """
     async_: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('async'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.4.1/src/shippo/models/components/manifestpaginatedlist.py` & `shippo-3.4.2/src/shippo/models/components/manifestpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/order.py` & `shippo-3.4.2/src/shippo/models/components/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .orderstatusenum import OrderStatusEnum
 from .weightunitenum import WeightUnitEnum
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
+
 class ShopApp(str, Enum):
     r"""Platform the order was created on and, if applicable, imported from.
     Orders created via the Shippo API or dashboard will have the value \"Shippo\".
     """
     AMAZON = 'Amazon'
     BIGCOMMERCE = 'Bigcommerce'
     CSV_IMPORT = 'CSV_Import'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/ordercreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/ordercreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/orderpaginatedlist.py` & `shippo-3.4.2/src/shippo/models/components/orderpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/orderstatusenum.py` & `shippo-3.4.2/src/shippo/models/components/orderstatusenum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
+
 class OrderStatusEnum(str, Enum):
     r"""Current state of the order. See the <a href=\\"https://docs.goshippo.com/docs/orders/orders/\\">orders tutorial</a>
     for the logic of how the status is handled.
     """
     UNKNOWN = 'UNKNOWN'
     AWAITPAY = 'AWAITPAY'
     PAID = 'PAID'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/parcel.py` & `shippo-3.4.2/src/shippo/models/components/parcel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from .distanceunitenum import DistanceUnitEnum
 from .parcelextra import ParcelExtra
-from .parceltemplateenumset import ParcelTemplateAramexAustraliaEnum, ParcelTemplateCouriersPleaseEnum, ParcelTemplateDHLeCommerceEnum, ParcelTemplateDPDUKEnum, ParcelTemplateFedExEnum, ParcelTemplateUPSEnum, ParcelTemplateUSPSEnum
+from .parceltemplateenumset import ParcelTemplateEnumSet
 from .weightunitenum import WeightUnitEnum
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from shippo import utils
-from typing import Optional, Union
+from typing import Optional
+
 
 class ObjectState(str, Enum):
     r"""A Parcel will only be valid when all required values have been sent and validated successfully."""
     VALID = 'VALID'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
@@ -51,13 +52,13 @@
     r"""Unique identifier of the given Parcel object. This ID is required to create a Shipment object."""
     object_owner: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_owner'), 'exclude': lambda f: f is None }})
     r"""Username of the user who created the Parcel object."""
     object_state: Optional[ObjectState] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_state'), 'exclude': lambda f: f is None }})
     r"""A Parcel will only be valid when all required values have been sent and validated successfully."""
     object_updated: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_updated'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""Date and time of last Parcel update. Since you cannot update Parcels after they were created, this time stamp reflects the time when the Parcel was changed by Shippo's systems for the last time, e.g., during sorting the dimensions given."""
-    template: Optional[Union[ParcelTemplateFedExEnum, ParcelTemplateUPSEnum, ParcelTemplateUSPSEnum, ParcelTemplateDHLeCommerceEnum, ParcelTemplateDPDUKEnum, ParcelTemplateCouriersPleaseEnum, ParcelTemplateAramexAustraliaEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('template'), 'exclude': lambda f: f is None }})
+    template: Optional[ParcelTemplateEnumSet] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('template'), 'exclude': lambda f: f is None }})
     r"""If template is passed, `length`, `width`, `height`, and `distance_unit` are not required"""
     test: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('test'), 'exclude': lambda f: f is None }})
     r"""Indicates whether the object has been created in test mode."""
```

### Comparing `shippo-3.4.1/src/shippo/models/components/parcelcreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/parcelcreaterequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from .distanceunitenum import DistanceUnitEnum
-from .parceltemplateenumset import ParcelTemplateAramexAustraliaEnum, ParcelTemplateCouriersPleaseEnum, ParcelTemplateDHLeCommerceEnum, ParcelTemplateDPDUKEnum, ParcelTemplateFedExEnum, ParcelTemplateUPSEnum, ParcelTemplateUSPSEnum
+from .parceltemplateenumset import ParcelTemplateEnumSet
 from .weightunitenum import WeightUnitEnum
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
-from typing import Optional, Union
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ParcelCreateRequest:
     distance_unit: DistanceUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
     r"""The measure unit used for length, width and height."""
@@ -27,12 +27,12 @@
     r"""The unit used for weight."""
     weight: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight') }})
     r"""Weight of the parcel. Up to six digits in front and four digits after the decimal separator are accepted."""
     width: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width') }})
     r"""**Required if template is not specified**<br>
     Width of the Parcel. Up to six digits in front and four digits after the decimal separator are accepted.
     """
-    template: Optional[Union[ParcelTemplateFedExEnum, ParcelTemplateUPSEnum, ParcelTemplateUSPSEnum, ParcelTemplateDHLeCommerceEnum, ParcelTemplateDPDUKEnum, ParcelTemplateCouriersPleaseEnum, ParcelTemplateAramexAustraliaEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('template'), 'exclude': lambda f: f is None }})
+    template: Optional[ParcelTemplateEnumSet] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('template'), 'exclude': lambda f: f is None }})
     r"""If template is passed, `length`, `width`, `height`, and `distance_unit` are not required"""
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.4.1/src/shippo/models/components/parcelextra.py` & `shippo-3.4.2/src/shippo/models/components/parcelextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/parcelinsurance.py` & `shippo-3.4.2/src/shippo/models/components/parcelinsurance.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
 from typing import Optional
 
+
 class ParcelInsuranceProvider(str, Enum):
     r"""To have insurance cover provided by a carrier directly instead of Shippo's provider (XCover), set provider to `FEDEX`, `UPS`, or `ONTRAC`."""
     FEDEX = 'FEDEX'
     UPS = 'UPS'
     ONTRAC = 'ONTRAC'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/parcelpaginatedlist.py` & `shippo-3.4.2/src/shippo/models/components/parcelpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/parcelrequest.py` & `shippo-3.4.2/src/shippo/models/components/parcelrequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from .distanceunitenum import DistanceUnitEnum
 from .parcelextra import ParcelExtra
-from .parceltemplateenumset import ParcelTemplateAramexAustraliaEnum, ParcelTemplateCouriersPleaseEnum, ParcelTemplateDHLeCommerceEnum, ParcelTemplateDPDUKEnum, ParcelTemplateFedExEnum, ParcelTemplateUPSEnum, ParcelTemplateUSPSEnum
+from .parceltemplateenumset import ParcelTemplateEnumSet
 from .weightunitenum import WeightUnitEnum
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
-from typing import Optional, Union
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ParcelRequest:
     distance_unit: DistanceUnitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
     r"""The measure unit used for length, width and height."""
@@ -28,13 +28,13 @@
     r"""Required if template is not specified. Width of the Parcel. Up to six digits in front and four digits after the decimal separator are accepted."""
     extra: Optional[ParcelExtra] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extra'), 'exclude': lambda f: f is None }})
     r"""An object holding optional extra services to be requested for each parcel in a multi-piece shipment.
     See the <a href=\"#section/Parcel-Extras\">Parcel Extra table below</a> for all available services.
     """
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""A string of up to 100 characters that can be filled with any additional information you want to attach to the object."""
-    template: Optional[Union[ParcelTemplateFedExEnum, ParcelTemplateUPSEnum, ParcelTemplateUSPSEnum, ParcelTemplateDHLeCommerceEnum, ParcelTemplateDPDUKEnum, ParcelTemplateCouriersPleaseEnum, ParcelTemplateAramexAustraliaEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('template'), 'exclude': lambda f: f is None }})
+    template: Optional[ParcelTemplateEnumSet] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('template'), 'exclude': lambda f: f is None }})
     r"""If template is passed, `length`, `width`, `height`, and `distance_unit` are not required"""
     test: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('test'), 'exclude': lambda f: f is None }})
     r"""Indicates whether the object has been created in test mode."""
```

### Comparing `shippo-3.4.1/src/shippo/models/components/parceltemplateenumset.py` & `shippo-3.4.2/src/shippo/models/components/parceltemplateenumset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,54 +1,60 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
+from typing import Union
+
 
 class ParcelTemplateAramexAustraliaEnum(str, Enum):
     r"""|Token | Name | Dimensions|
     |:---|:---|:---|
     | Fastway_Australia_Satchel_A2 | Satchel A2 | 594.00 x 420.00 x 48.00 mm|
     | Fastway_Australia_Satchel_A3 | Satchel A3 | 420.00 x 297.00 x 64.00 mm|
     | Fastway_Australia_Satchel_A4 | Satchel A4 | 297.00 x 210.00 x 64.00 mm|
     | Fastway_Australia_Satchel_A5 | Satchel A5 | 210.00 x 148.00 x 64.00 mm|
     """
     FASTWAY_AUSTRALIA_SATCHEL_A2 = 'Fastway_Australia_Satchel_A2'
     FASTWAY_AUSTRALIA_SATCHEL_A3 = 'Fastway_Australia_Satchel_A3'
     FASTWAY_AUSTRALIA_SATCHEL_A4 = 'Fastway_Australia_Satchel_A4'
     FASTWAY_AUSTRALIA_SATCHEL_A5 = 'Fastway_Australia_Satchel_A5'
 
+
 class ParcelTemplateCouriersPleaseEnum(str, Enum):
     r"""|Token | Name | Dimensions|
     |:---|:---|:---|
     | couriersplease_500g_satchel | 500g Satchel | 22.00 x 33.50 x 0.10 cm|
     | couriersplease_1kg_satchel | 1kg Satchel | 28.00 x 35.00 x 0.10 cm|
     | couriersplease_3kg_satchel | 3kg Satchel | 34.00 x 42.00 x 0.10 cm|
     | couriersplease_5kg_satchel | 5kg Satchel | 43.70 x 59.70 x 0.10 cm|
     """
     COURIERSPLEASE_500G_SATCHEL = 'couriersplease_500g_satchel'
     COURIERSPLEASE_1KG_SATCHEL = 'couriersplease_1kg_satchel'
     COURIERSPLEASE_3KG_SATCHEL = 'couriersplease_3kg_satchel'
     COURIERSPLEASE_5KG_SATCHEL = 'couriersplease_5kg_satchel'
 
+
 class ParcelTemplateDPDUKEnum(str, Enum):
     r"""|Token | Name | Dimensions|
     |:---|:---|:---|
     | DPD_UK_Express_Pak| DPD UK Express Pak | 530.00 x 400.00 x 100.00 mm|
     """
     DPD_UK_EXPRESS_PAK = 'DPD_UK_Express_Pak'
 
+
 class ParcelTemplateDHLeCommerceEnum(str, Enum):
     r"""|Token | Name | Dimensions|
     |:---|:---|:---|
     | DHLeC_Irregular | Irregular Shipment | 10.00 x 10.00 x 10.00 in|
     | DHLeC_SM_Flats | Flats | 27.00 x 17.00 x 17.00 in|
     """
     DH_LE_C_IRREGULAR = 'DHLeC_Irregular'
     DH_LE_C_SM_FLATS = 'DHLeC_SM_Flats'
 
+
 class ParcelTemplateUSPSEnum(str, Enum):
     r"""|Token | Name | Dimensions|
     |:---|:---|:---|
     | USPS_FlatRateCardboardEnvelope | Flat Rate Cardboard Envelope |  12.50 x 9.50 x 0.75 in |
     | USPS_FlatRateEnvelope | Flat Rate Envelope |  12.50 x 9.50 x 0.75 in |
     | USPS_FlatRateGiftCardEnvelope | Flat Rate Gift Card Envelope |  10.00 x 7.00 x 0.75 in |
     | USPS_FlatRateLegalEnvelope | Flat Rate Legal Envelope |  15.00 x 9.50 x 0.75 in |
@@ -86,14 +92,15 @@
     USPS_REGIONAL_RATE_BOX_A2 = 'USPS_RegionalRateBoxA2'
     USPS_REGIONAL_RATE_BOX_B1 = 'USPS_RegionalRateBoxB1'
     USPS_REGIONAL_RATE_BOX_B2 = 'USPS_RegionalRateBoxB2'
     USPS_SMALL_FLAT_RATE_BOX = 'USPS_SmallFlatRateBox'
     USPS_SMALL_FLAT_RATE_ENVELOPE = 'USPS_SmallFlatRateEnvelope'
     USPS_SOFT_PACK = 'USPS_SoftPack'
 
+
 class ParcelTemplateUPSEnum(str, Enum):
     r"""|Token | Name | Dimensions|
     |:---|:---|:---|
     | UPS_Box_10kg | Box 10kg | 410.00 x 335.00 x 265.00 mm|
     | UPS_Box_25kg | Box 25kg | 484.00 x 433.00 x 350.00 mm|
     | UPS_Express_Box | Express Box | 460.00 x 315.00 x 95.00 mm|
     | UPS_Express_Box_Large | Express Box Large | 18.00 x 13.00 x 3.00 in|
@@ -141,14 +148,15 @@
     UPS_MI_MEDIA_MAIL = 'UPS_MI_MEDIA_MAIL'
     UPS_MI_PARCEL_POST = 'UPS_MI_Parcel_Post'
     UPS_MI_PRIORITY = 'UPS_MI_Priority'
     UPS_MI_STANDARD_FLAT = 'UPS_MI_Standard_Flat'
     UPS_PAD_PAK = 'UPS_Pad_Pak'
     UPS_PALLET = 'UPS_Pallet'
 
+
 class ParcelTemplateFedExEnum(str, Enum):
     r"""|Token | Name | Dimensions|
     |:---|:---|:---|
     | FedEx_Box_10kg | FedEx® 10kg Box | 15.81 x 12.94 x 10.19 in|
     | FedEx_Box_25kg | FedEx® 25kg Box | 54.80 x 42.10 x 33.50 in|
     | FedEx_Box_Extra_Large_1 | FedEx® Extra Large Box (X1) | 11.88 x 11.00 x 10.75 in|
     | FedEx_Box_Extra_Large_2 | FedEx® Extra Large Box (X2) | 15.75 x 14.13 x 6.00 in|
@@ -177,7 +185,9 @@
     FED_EX_BOX_SMALL_2 = 'FedEx_Box_Small_2'
     FED_EX_ENVELOPE = 'FedEx_Envelope'
     FED_EX_PADDED_PAK = 'FedEx_Padded_Pak'
     FED_EX_PAK_1 = 'FedEx_Pak_1'
     FED_EX_PAK_2 = 'FedEx_Pak_2'
     FED_EX_TUBE = 'FedEx_Tube'
     FED_EX_XL_PAK = 'FedEx_XL_Pak'
+
+ParcelTemplateEnumSet = Union['ParcelTemplateFedExEnum', 'ParcelTemplateUPSEnum', 'ParcelTemplateUSPSEnum', 'ParcelTemplateDHLeCommerceEnum', 'ParcelTemplateDPDUKEnum', 'ParcelTemplateCouriersPleaseEnum', 'ParcelTemplateAramexAustraliaEnum']
```

### Comparing `shippo-3.4.1/src/shippo/models/components/pickup.py` & `shippo-3.4.2/src/shippo/models/components/pickup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .location import Location
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
+
 class PickupStatus(str, Enum):
     r"""Indicates the status of the pickup."""
     PENDING = 'PENDING'
     CONFIRMED = 'CONFIRMED'
     ERROR = 'ERROR'
     CANCELLED = 'CANCELLED'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/pickupbase.py` & `shippo-3.4.2/src/shippo/models/components/pickupbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/ponumber.py` & `shippo-3.4.2/src/shippo/models/components/ponumber.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class PoNumber:
-    r"""Specify the PO number field on the label (FedEx only)."""
+    r"""Specify the PO number field on the label (FedEx and UPS only)."""
     prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prefix'), 'exclude': lambda f: f is None }})
     r"""Custom prefix for PO number field (ZPL labels only). Up to 11 characters, including trailing
     spaces. Empty string indicates removal of default prefix. To use the default prefix, do not include
     this property.
     """
     value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value'), 'exclude': lambda f: f is None }})
     r"""Optional text to be printed on the shipping label for PO number. Up to 40 characters. If
     this is provided, reference_2 will be ignored.
     """
+    ref_sort: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ref_sort'), 'exclude': lambda f: f is None }})
+    r"""Order UPS reference fields are printed on ZPL labels. For UPS shipments, if you choose to set `ref_sort` for one reference, you must set `ref_sort` for all other supported UPS references using unique integers."""
```

### Comparing `shippo-3.4.1/src/shippo/models/components/rate.py` & `shippo-3.4.2/src/shippo/models/components/rate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from .responsemessage import ResponseMessage
-from .servicelevel import ServiceLevel
+from .servicelevelwithparent import ServiceLevelWithParent
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
+
 class Attributes(str, Enum):
     BESTVALUE = 'BESTVALUE'
     CHEAPEST = 'CHEAPEST'
     FASTEST = 'FASTEST'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
@@ -42,16 +43,15 @@
     r"""Date and time of Rate creation."""
     object_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id') }})
     r"""Unique identifier of the given Rate object."""
     object_owner: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_owner') }})
     r"""Username of the user who created the rate object."""
     provider: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('provider') }})
     r"""Carrier offering the rate, e.g., `FedEx` or `Deutsche Post DHL`."""
-    servicelevel: ServiceLevel = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('servicelevel') }})
-    r"""Contains details regarding the service level for the given rate."""
+    servicelevel: ServiceLevelWithParent = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('servicelevel') }})
     shipment: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shipment') }})
     arrives_by: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('arrives_by'), 'exclude': lambda f: f is None }})
     r"""Predicted time the carrier will deliver the package in the destination's local time zone. In the format `HH:MM:SS`."""
     duration_terms: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration_terms'), 'exclude': lambda f: f is None }})
     r"""Further clarification of the transit times.
     Often, this includes notes that the transit time as given in \"days\" is only an average, not a guaranteed time.
     """
```

### Comparing `shippo-3.4.1/src/shippo/models/components/ratepaginatedlist.py` & `shippo-3.4.2/src/shippo/models/components/ratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/refund.py` & `shippo-3.4.2/src/shippo/models/components/refund.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import dateutil.parser
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from shippo import utils
 from typing import Optional
 
+
 class RefundStatus(str, Enum):
     r"""Indicates the status of the Refund."""
     QUEUED = 'QUEUED'
     PENDING = 'PENDING'
     SUCCESS = 'SUCCESS'
     ERROR = 'ERROR'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/refundpaginatedlist.py` & `shippo-3.4.2/src/shippo/models/components/refundpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/refundrequestbody.py` & `shippo-3.4.2/src/shippo/models/components/refundrequestbody.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/responsemessage.py` & `shippo-3.4.2/src/shippo/models/components/responsemessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/rmanumber.py` & `shippo-3.4.2/src/shippo/models/components/servicelevel.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,18 +5,26 @@
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class RmaNumber:
-    r"""Specify the RMA number field on the label (FedEx only)."""
-    prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prefix'), 'exclude': lambda f: f is None }})
-    r"""Custom prefix for RMA number field (ZPL labels only). Up to 11 characters, including trailing
-    spaces. Empty string indicates removal of default prefix. To use the default prefix, do not include
-    this property.
+class ServiceLevel:
+    r"""Contains details regarding the service level for the given rate."""
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    r"""Name of the Rate's servicelevel, e.g. `International Priority` or `Standard Post`.
+    A servicelevel commonly defines the transit time of a Shipment (e.g., Express vs. Standard), along with other properties. 
+    These names vary depending on the provider.
+    """
+    terms: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terms'), 'exclude': lambda f: f is None }})
+    r"""Further clarification of the service."""
+    token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token'), 'exclude': lambda f: f is None }})
+    r"""Token of the Rate's servicelevel, e.g. `usps_priority` or `fedex_ground`.
+    See <a href=\"#tag/Service-Levels\">servicelevels</a>.
+    """
+    extended_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extended_token'), 'exclude': lambda f: f is None }})
+    r"""Unique, extended version of the Service Level \\"token\\".
+    Guaranteed to be unique across all Service Levels, and may help offer insight into the specific Service Level it describes.
     """
-    value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value'), 'exclude': lambda f: f is None }})
-    r"""Optional text to be printed on the shipping label for RMA number. Up to 40 characters."""
```

### Comparing `shippo-3.4.1/src/shippo/models/components/servicegroup.py` & `shippo-3.4.2/src/shippo/models/components/servicegroup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from .servicegrouptypeenum import ServiceGroupTypeEnum
-from .servicelevel import ServiceLevel
+from .servicelevelwithparent import ServiceLevelWithParent
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
@@ -16,15 +16,15 @@
     r"""Description for the service group"""
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     r"""Name for the service group that will be shown to customers in the response"""
     type: ServiceGroupTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
     r"""The type of the service group.<br> `LIVE_RATE` - Shippo will make a rating request and return real-time rates for the shipping group, only falling back to the specified flat rate amount if no rates match a service level in the service group.<br> `FLAT_RATE` - Returns a shipping option with the specified flat rate amount.<br> `FREE_SHIPPING` - Returns a shipping option with a price of $0 only if the total cost of items exceeds the amount defined by `free_shipping_threshold_min`"""
     object_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id') }})
     r"""The unique identifier of the given Service Group object."""
-    service_levels: List[ServiceLevel] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service_levels') }})
+    service_levels: List[ServiceLevelWithParent] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service_levels') }})
     flat_rate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('flat_rate'), 'exclude': lambda f: f is None }})
     r"""String representation of an amount to be returned as the flat rate
     if 1. The service group is of type `LIVE_RATE` and no matching rates
     were found; or 2. The service group is of type `FLAT_RATE`. Either
     integers or decimals are accepted. Required unless type is
     `FREE_SHIPPING`
     """
```

### Comparing `shippo-3.4.1/src/shippo/models/components/servicegroupaccountandservicelevel.py` & `shippo-3.4.2/src/shippo/models/components/servicegroupaccountandservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/servicegroupcreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/servicegroupcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/servicegrouptypeenum.py` & `shippo-3.4.2/src/shippo/models/components/servicegrouptypeenum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
+
 class ServiceGroupTypeEnum(str, Enum):
     r"""The type of the service group.<br> `LIVE_RATE` - Shippo will make a rating request and return real-time rates for the shipping group, only falling back to the specified flat rate amount if no rates match a service level in the service group.<br> `FLAT_RATE` - Returns a shipping option with the specified flat rate amount.<br> `FREE_SHIPPING` - Returns a shipping option with a price of $0 only if the total cost of items exceeds the amount defined by `free_shipping_threshold_min`"""
     LIVE_RATE = 'LIVE_RATE'
     FLAT_RATE = 'FLAT_RATE'
     FREE_SHIPPING = 'FREE_SHIPPING'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/servicegroupupdaterequest.py` & `shippo-3.4.2/src/shippo/models/components/servicegroupupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/servicelevel.py` & `shippo-3.4.2/src/shippo/models/components/servicelevelwithparent.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,20 @@
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ServiceLevel:
-    r"""Contains details regarding the service level for the given rate."""
+class ParentServicelevel:
+    r"""Used for some Service Levels to link to the more \\"generic\\" version of this Service Level - for example,
+    if this Service Level is a variation specific to shipments to Europe(\"ups_saver_eu\"), the \"parent\" is 
+    the fully generic version (\"ups_saver\"). Helpful when displaying Service Levels to users. Has the same 
+    structure of the servicelevel - \"name\", \"token\", \"terms\", and \"extended_token\", or it is otherwise null.
+    """
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     r"""Name of the Rate's servicelevel, e.g. `International Priority` or `Standard Post`.
     A servicelevel commonly defines the transit time of a Shipment (e.g., Express vs. Standard), along with other properties. 
     These names vary depending on the provider.
     """
     terms: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terms'), 'exclude': lambda f: f is None }})
     r"""Further clarification of the service."""
@@ -22,15 +26,33 @@
     r"""Token of the Rate's servicelevel, e.g. `usps_priority` or `fedex_ground`.
     See <a href=\"#tag/Service-Levels\">servicelevels</a>.
     """
     extended_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extended_token'), 'exclude': lambda f: f is None }})
     r"""Unique, extended version of the Service Level \\"token\\".
     Guaranteed to be unique across all Service Levels, and may help offer insight into the specific Service Level it describes.
     """
-    parent_servicelevel: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parent_servicelevel'), 'exclude': lambda f: f is None }})
-    r"""Used for some Service Levels to link to the more \\"generic\\" version of this Service Level - for example,
-    if this Service Level is a variation specific to shipments to Europe(\"ups_saver_eu\"), the \"parent\" is 
-    the fully generic version (\"ups_saver\"). Helpful when displaying Service Levels to users. Has the same 
-    structure of the servicelevel - \"name\", \"token\", \"terms\", and \"extended_token\", or it is otherwise null.
+    
+
+
+
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class ServiceLevelWithParent:
+    r"""Contains details regarding the service level for the given rate."""
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    r"""Name of the Rate's servicelevel, e.g. `International Priority` or `Standard Post`.
+    A servicelevel commonly defines the transit time of a Shipment (e.g., Express vs. Standard), along with other properties. 
+    These names vary depending on the provider.
+    """
+    terms: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terms'), 'exclude': lambda f: f is None }})
+    r"""Further clarification of the service."""
+    token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token'), 'exclude': lambda f: f is None }})
+    r"""Token of the Rate's servicelevel, e.g. `usps_priority` or `fedex_ground`.
+    See <a href=\"#tag/Service-Levels\">servicelevels</a>.
+    """
+    extended_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extended_token'), 'exclude': lambda f: f is None }})
+    r"""Unique, extended version of the Service Level \\"token\\".
+    Guaranteed to be unique across all Service Levels, and may help offer insight into the specific Service Level it describes.
     """
+    parent_servicelevel: Optional[ParentServicelevel] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parent_servicelevel'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.4.1/src/shippo/models/components/servicelevelenumset.py` & `shippo-3.4.2/src/shippo/models/components/servicelevelenumset.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
+from typing import Union
+
 
 class ServiceLevelSwyftEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | same_day | Next Day|
     | next_day | Next Day|
     """
     SAME_DAY = 'same_day'
     NEXT_DAY = 'next_day'
 
+
 class ServiceLevelVehoEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | veho_next_day | Veho Next Day |
     """
     VEHO_NEXT_DAY = 'veho_next_day'
 
+
 class ServiceLevelUDSEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | uds_next_day | Next Day|
     """
     UDS_NEXT_DAY = 'uds_next_day'
 
+
 class ServiceLevelEvriUKEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | hermes_uk_courier_service | Courier Collection|
     | hermes_uk_parcelshop_dropoff | ParcelShop Drop-Off|
     | hermes_uk_parcelshop_dropoff_nextday | ParcelShop Drop-Off Next Day|
     | hermes_uk_postable | Postable|
@@ -37,39 +42,43 @@
     """
     HERMES_UK_COURIER_SERVICE = 'hermes_uk_courier_service'
     HERMES_UK_PARCELSHOP_DROPOFF = 'hermes_uk_parcelshop_dropoff'
     HERMES_UK_PARCELSHOP_DROPOFF_NEXTDAY = 'hermes_uk_parcelshop_dropoff_nextday'
     HERMES_UK_POSTABLE = 'hermes_uk_postable'
     HERMES_UK_POSTABLE_NEXTDAY = 'hermes_uk_postable_nextday'
 
+
 class ServiceLevelLasershipEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | lasership_routed_delivery | Routed Delivery|
     """
     LASERSHIP_ROUTED_DELIVERY = 'lasership_routed_delivery'
 
+
 class ServiceLevelOnTracEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | ontrac_ground | Ground|
     | ontrac_sunrise_gold | Sunrise Gold|
     | ontrac_sunrise | Sunrise|
     """
     ONTRAC_GROUND = 'ontrac_ground'
     ONTRAC_SUNRISE_GOLD = 'ontrac_sunrise_gold'
     ONTRAC_SUNRISE = 'ontrac_sunrise'
 
+
 class ServiceLevelSendleEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | sendle_parcel | Sendle Parcel|
     """
     SENDLE_PARCEL = 'sendle_parcel'
 
+
 class ServiceLevelRoyalMailEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | royal_mail_tracked_letter_boxable_24_no_signature | Royal Mail Tracked Letter-Boxable 24 No Signature|
     | royal_mail_tracked_letter_boxable_48_no_signature | Royal Mail Tracked Letter-Boxable 48 No Signature|
     | royal_mail_tracked_24_returns | Royal Mail Tracked Returns 24|
     | royal_mail_tracked_48_returns | Royal Mail Tracked Returns 48|
@@ -107,14 +116,15 @@
     ROYAL_MAIL_INTL_BUS_MAIL_LRG_LTR_ZONE_SORT_PRI = 'royal_mail_intl_bus_mail_lrg_ltr_zone_sort_pri'
     ROYAL_MAIL_INTL_BUS_PARCELS_TRACKED_ZONE_SORT = 'royal_mail_intl_bus_parcels_tracked_zone_sort'
     ROYAL_MAIL_INTL_BUS_PARCELS_TRACKED_COUNTRY_PRICED = 'royal_mail_intl_bus_parcels_tracked_country_priced'
     ROYAL_MAIL_INTL_BUS_PARCELS_TRACKED_SIGNED_ZONE_SRT = 'royal_mail_intl_bus_parcels_tracked_signed_zone_srt'
     ROYAL_MAIL_24_FLAT_RATE = 'royal_mail_24_flat_rate'
     ROYAL_MAIL_48_FLAT_RATE = 'royal_mail_48_flat_rate'
 
+
 class ServiceLevelePostGlobalEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | rr_donnelley_domestic_economy_parcel | Domestic Economy Parcel|
     | rr_donnelley_domestic_priority_parcel | Domestic Priority Parcel |
     | rr_donnelley_domestic_parcel_bpm | Domestic Parcel BPM|
     | rr_donnelley_priority_domestic_priority_parcel_bpm | Domestic Priority Parcel BPM|
@@ -138,46 +148,51 @@
     RR_DONNELLEY_IPA = 'rr_donnelley_ipa'
     RR_DONNELLEY_COURIER = 'rr_donnelley_courier'
     RR_DONNELLEY_ISAL = 'rr_donnelley_isal'
     RR_DONNELLEY_EPACKET = 'rr_donnelley_epacket'
     RR_DONNELLEY_PMI = 'rr_donnelley_pmi'
     RR_DONNELLEY_EMI = 'rr_donnelley_emi'
 
+
 class ServiceLevelPostItalianeEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | poste_italiane_delivery_business_express | Poste Delivery Business Express|
     """
     POSTE_ITALIANE_DELIVERY_BUSINESS_EXPRESS = 'poste_italiane_delivery_business_express'
 
+
 class ServiceLevelParcelforceEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | parcelforce_express48 | Express 48|
     | parcelforce_express24 | Express 24|
     | parcelforce_expressam | Express AM|
     """
     PARCELFORCE_EXPRESS48 = 'parcelforce_express48'
     PARCELFORCE_EXPRESS24 = 'parcelforce_express24'
     PARCELFORCE_EXPRESSAM = 'parcelforce_expressam'
 
+
 class ServiceLevelMaergoEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | x_delivery_expedited | Expedited|
     """
     X_DELIVERY_EXPEDITED = 'x_delivery_expedited'
 
+
 class ServiceLevelMondialRelayEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | mondial_relay_pointrelais | Point Relais|
     """
     MONDIAL_RELAY_POINTRELAIS = 'mondial_relay_pointrelais'
 
+
 class ServiceLevelLSOEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | lso_ground | Ground|
     | lso_economy_next_day | Economy Next Day|
     | lso_saturday_delivery | Saturday Delivery|
     | lso_2nd_day | 2nd Day|
@@ -187,14 +202,15 @@
     LSO_GROUND = 'lso_ground'
     LSO_ECONOMY_NEXT_DAY = 'lso_economy_next_day'
     LSO_SATURDAY_DELIVERY = 'lso_saturday_delivery'
     LSO_2ND_DAY = 'lso_2nd_day'
     LSO_PRIORITY_NEXT_DAY = 'lso_priority_next_day'
     LSO_EARLY_OVERNIGHT = 'lso_early_overnight'
 
+
 class ServiceLevelGLSUSEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | gls_us_cps | GSO Ground|
     | gls_us_eps | Early Priority Overnight|
     | gls_us_ess | Early Saturday Delivery|
     | gls_us_nps | Noon Priority Overnight|
@@ -204,14 +220,15 @@
     GLS_US_CPS = 'gls_us_cps'
     GLS_US_EPS = 'gls_us_eps'
     GLS_US_ESS = 'gls_us_ess'
     GLS_US_NPS = 'gls_us_nps'
     GLS_US_PDS = 'gls_us_pds'
     GLS_US_SDS = 'gls_us_sds'
 
+
 class ServiceLevelGlobegisticsEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | globegistics_priority_mail_express_international | Globegistics Priority Mail Express International|
     | globegistics_priority_mail_international | Globegistics Priority Mail International|
     | globegistics_priority_mail_express_international_pds | Globegistics Priority Mail Express International PreSort Drop Ship|
     | globegistics_priority_mail_international_pds | Globegistics Priority Mail International PreSort Drop Ship|
@@ -233,14 +250,15 @@
     GLOBEGISTICS_ECOM_PACKET_DDP = 'globegistics_ecom_packet_ddp'
     GLOBEGISTICS_ECOM_PRIORITY_MAIL_INTERNATIONAL_DDP = 'globegistics_ecom_priority_mail_international_ddp'
     GLOBEGISTICS_ECOM_PRIORITY_MAIL_EXPRESS_INTERNATIONAL_DDP = 'globegistics_ecom_priority_mail_express_international_ddp'
     GLOBEGISTICS_ECOM_EXTRA = 'globegistics_ecom_extra'
     GLOBEGISTICS_ECOM_INTERNATIONAL_PRIORITY_AIRMAIL = 'globegistics_ecom_international_priority_airmail'
     GLOBEGISTICS_ECOM_INTERNATIONAL_SURFACE_AIRLIFT = 'globegistics_ecom_international_surface_airlift'
 
+
 class ServiceLevelAramexAustraliaEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | fastway_australia_parcel | Parcel|
     | fastway_australia_satchel | Satchel|
     | fastway_australia_box_small | Box Small|
     | fastway_australia_box_medium | Box Medium|
@@ -248,14 +266,15 @@
     """
     FASTWAY_AUSTRALIA_PARCEL = 'fastway_australia_parcel'
     FASTWAY_AUSTRALIA_SATCHEL = 'fastway_australia_satchel'
     FASTWAY_AUSTRALIA_BOX_SMALL = 'fastway_australia_box_small'
     FASTWAY_AUSTRALIA_BOX_MEDIUM = 'fastway_australia_box_medium'
     FASTWAY_AUSTRALIA_BOX_LARGE = 'fastway_australia_box_large'
 
+
 class ServiceLevelDeutschePostEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | deutsche_post_postkarte | Postkarte|
     | deutsche_post_standardbrief | Standardbrief|
     | deutsche_post_kompaktbrief | Kompaktbrief|
     | deutsche_post_grossbrief | Grossbrief|
@@ -273,14 +292,15 @@
     DEUTSCHE_POST_MAXIBRIEF = 'deutsche_post_maxibrief'
     DEUTSCHE_POST_MAXIBRIEF_PLUS = 'deutsche_post_maxibrief_plus'
     DEUTSCHE_POST_WARENPOST_INTERNATIONAL_XS = 'deutsche_post_warenpost_international_xs'
     DEUTSCHE_POST_WARENPOST_INTERNATIONAL_S = 'deutsche_post_warenpost_international_s'
     DEUTSCHE_POST_WARENPOST_INTERNATIONAL_M = 'deutsche_post_warenpost_international_m'
     DEUTSCHE_POST_WARENPOST_INTERNATIONAL_L = 'deutsche_post_warenpost_international_l'
 
+
 class ServiceLevelDPDUKEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | dpd_uk_ship_to_shop | Ship to shop|
     | dpd_uk_1030 | Door to door 10.30 next day|
     | dpd_uk_1200 | Door to door 12.00 next day|
     | dpd_uk_saturday | Saturday Delivery|
@@ -312,21 +332,23 @@
     DPD_UK_CLASSIC = 'dpd_uk_classic'
     DPD_UK_AIR_CLASSIC = 'dpd_uk_air_classic'
     DPD_UK_AIR_EXPRESS = 'dpd_uk_air_express'
     DPD_UK_DIRECT = 'dpd_uk_direct'
     DPD_UK_DIRECT_TRACKED_MAIL = 'dpd_uk_direct_tracked_mail'
     DPD_UK_PICKUP_RETURNS = 'dpd_uk_pickup_returns'
 
+
 class ServiceLevelDPDDEEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | dpd_de_classic | DPD Classic|
     """
     DPD_DE_CLASSIC = 'dpd_de_classic'
 
+
 class ServiceLevelDHLGermanyEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | dhl_germany_europaket | DHL Germany Europaket|
     | dhl_germany_paket | DHL Germany Paket|
     | dhl_germany_paket_connect | DHL Germany Paket Connect|
     | dhl_germany_paket_international | DHL Germany Paket International|
@@ -336,14 +358,15 @@
     DHL_GERMANY_EUROPAKET = 'dhl_germany_europaket'
     DHL_GERMANY_PAKET = 'dhl_germany_paket'
     DHL_GERMANY_PAKET_CONNECT = 'dhl_germany_paket_connect'
     DHL_GERMANY_PAKET_INTERNATIONAL = 'dhl_germany_paket_international'
     DHL_GERMANY_PAKET_PRIORITY = 'dhl_germany_paket_priority'
     DHL_GERMANY_PAKET_SAMEDAY = 'dhl_germany_paket_sameday'
 
+
 class ServiceLevelDHLeCommerceEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | dhl_ecommerce_marketing_parcel_expedited | Marketing Parcel Expedited|
     | dhl_ecommerce_globalmail_business_ipa | GlobalMail Business IPA|
     | dhl_ecommerce_parcel_international_direct | Parcel International Direct|
     | dhl_ecommerce_parcels_expedited_max | Parcels Expedited Max|
@@ -397,14 +420,15 @@
     DHL_ECOMMERCE_GLOBALMAIL_PACKET_PRIORITY = 'dhl_ecommerce_globalmail_packet_priority'
     DHL_ECOMMERCE_EASY_RETURN_LIGHT = 'dhl_ecommerce_easy_return_light'
     DHL_ECOMMERCE_PARCEL_PLUS_EXPEDITED = 'dhl_ecommerce_parcel_plus_expedited'
     DHL_ECOMMERCE_GLOBALMAIL_BUSINESS_STANDARD = 'dhl_ecommerce_globalmail_business_standard'
     DHL_ECOMMERCE_GROUND = 'dhl_ecommerce_ground'
     DHL_ECOMMERCE_GLOBALMAIL_PACKET_STANDARD = 'dhl_ecommerce_globalmail_packet_standard'
 
+
 class ServiceLevelDHLExpressEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | dhl_express_domestic_express_doc | Domestic Express Doc|
     | dhl_express_economy_select_doc | Economy Select Doc|
     | dhl_express_worldwide_nondoc | Express Worldwide Nondoc|
     | dhl_express_worldwide_doc | Express Worldwide Doc|
@@ -446,14 +470,15 @@
     DHL_EXPRESS_EXPRESS_12_00_NONDOC = 'dhl_express_express_12_00_nondoc'
     DHL_EXPRESS_EXPRESS_12_DOC = 'dhl_express_express_12_doc'
     DHL_EXPRESS_WORLDWIDE_B2C_DOC = 'dhl_express_worldwide_b2c_doc'
     DHL_EXPRESS_WORLDWIDE_B2C_NONDOC = 'dhl_express_worldwide_b2c_nondoc'
     DHL_EXPRESS_MEDICAL_EXPRESS = 'dhl_express_medical_express'
     DHL_EXPRESS_EXPRESS_EASY_NONDOC = 'dhl_express_express_easy_nondoc'
 
+
 class ServiceLevelPurolatorEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | purolator_ground | Ground|
     | purolator_ground9_am | Ground 9am|
     | purolator_ground1030_am | Ground 10:30am|
     | purolator_ground_distribution | Ground Distribution|
@@ -487,34 +512,37 @@
     PUROLATOR_EXPRESS_US1030_AM = 'purolator_express_us1030_am'
     PUROLATOR_EXPRESS_US1200 = 'purolator_express_us1200'
     PUROLATOR_EXPRESS_INTERNATIONAL = 'purolator_express_international'
     PUROLATOR_EXPRESS_INTERNATIONAL9_AM = 'purolator_express_international9_am'
     PUROLATOR_EXPRESS_INTERNATIONAL1030_AM = 'purolator_express_international1030_am'
     PUROLATOR_EXPRESS_INTERNATIONAL1200 = 'purolator_express_international1200'
 
+
 class ServiceLevelColissimoEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | colissimo_home | Domicile|
     | colissimo_pick_up_point | Point Retrait|
     | colissimo_return_mainland_france | Retour France|
     """
     COLISSIMO_HOME = 'colissimo_home'
     COLISSIMO_PICK_UP_POINT = 'colissimo_pick_up_point'
     COLISSIMO_RETURN_MAINLAND_FRANCE = 'colissimo_return_mainland_france'
 
+
 class ServiceLevelCorreosEspanaEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | correos_standard_home| Paquete Estándar|
     | correos_premium_home | Paquete Premium|
     """
     CORREOS_STANDARD_HOME = 'correos_standard_home'
     CORREOS_PREMIUM_HOME = 'correos_premium_home'
 
+
 class ServiceLevelCouriersPleaseEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | couriersplease_domestic_priority_auth_to_leave | Domestic Priority - Authority To Leave/POPPoints|
     | couriersplease_domestic_priority_sign_required | Domestic Priority - Signature Required|
     | couriersplease_gold_domestic_auth_to_leave | Gold Domestic - Authority To Leave/POPPoints|
     | couriersplease_gold_domestic_sign_required | Gold Domestic - Signature Required|
@@ -534,14 +562,15 @@
     COURIERSPLEASE_OFF_PEAK_SIGN_REQUIRED = 'couriersplease_off_peak_sign_required'
     COURIERSPLEASE_PARCEL_AUTH_TO_LEAVE = 'couriersplease_parcel_auth_to_leave'
     COURIERSPLEASE_PARCEL_SIGN_REQUIRED = 'couriersplease_parcel_sign_required'
     COURIERSPLEASE_ROAD_EXPRESS = 'couriersplease_road_express'
     COURIERSPLEASE_SATCHEL_AUTH_TO_LEAVE = 'couriersplease_satchel_auth_to_leave'
     COURIERSPLEASE_SATCHEL_SIGN_REQUIRED = 'couriersplease_satchel_sign_required'
 
+
 class ServiceLevelChronopostEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | chronopost_13 | Chrono 13|
     | chronopost_10 | Chrono 10|
     | chronopost_18| Chrono 18|
     | chronopost_relais_fr | Chrono Point Relais|
@@ -551,21 +580,23 @@
     CHRONOPOST_13 = 'chronopost_13'
     CHRONOPOST_10 = 'chronopost_10'
     CHRONOPOST_18 = 'chronopost_18'
     CHRONOPOST_RELAIS_FR = 'chronopost_relais_fr'
     CHRONOPOST_CLASSIC = 'chronopost_classic'
     CHRONOPOST_EXPRESS = 'chronopost_express'
 
+
 class ServiceLevelCDLEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | cdl_next_day | Next Day|
     """
     CDL_NEXT_DAY = 'cdl_next_day'
 
+
 class ServiceLevelCanadaPostEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | canada_post_regular_parcel | Regular Parcel|
     | canada_post_expedited_parcel | Expedited Parcel|
     | canada_post_priority | Priority|
     | canada_post_xpresspost | Xpresspost|
@@ -585,45 +616,49 @@
     CANADA_POST_XPRESSPOST_USA = 'canada_post_xpresspost_usa'
     CANADA_POST_EXPEDITED_PARCEL_USA = 'canada_post_expedited_parcel_usa'
     CANADA_POST_TRACKED_PACKET_USA = 'canada_post_tracked_packet_usa'
     CANADA_POST_SMALL_PACKET_USA_AIR = 'canada_post_small_packet_usa_air'
     CANADA_POST_TRACKED_PACKET_INTERNATIONAL = 'canada_post_tracked_packet_international'
     CANADA_POST_SMALL_PACKET_INTERNATIONAL_AIR = 'canada_post_small_packet_international_air'
 
+
 class ServiceLevelBetterTrucksEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | better_trucks_same_day | Same Day|
     | better_trucks_next_day | Next Day|
     """
     BETTER_TRUCKS_SAME_DAY = 'better_trucks_same_day'
     BETTER_TRUCKS_NEXT_DAY = 'better_trucks_next_day'
 
+
 class ServiceLevelAPGEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | epacket | ePacket|
     | epacket_plus | ePacket Plus|
     | eparcel_premium | eParcel premium|
     | apg_eparcel_expedited | eParcel Expedited|
     """
     EPACKET = 'epacket'
     EPACKET_PLUS = 'epacket_plus'
     EPARCEL_PREMIUM = 'eparcel_premium'
     APG_EPARCEL_EXPEDITED = 'apg_eparcel_expedited'
 
+
 class ServiceLevelAxleHireEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | axlehire_same_day | Same Day|
     | axlehire_next_day | Next Day|
     """
     AXLEHIRE_SAME_DAY = 'axlehire_same_day'
     AXLEHIRE_NEXT_DAY = 'axlehire_next_day'
 
+
 class ServiceLevelAustraliaPostEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | australia_post_express_post | Express Post|
     | australia_post_parcel_post | Parcel Post|
     | australia_post_pack_and_track_international | Pack and Track International|
     | australia_post_international_airmail | International Airmail|
@@ -641,14 +676,15 @@
     AUSTRALIA_POST_EXPRESS_POST_INTERNATIONAL = 'australia_post_express_post_international'
     AUSTRALIA_POST_EXPRESS_COURIER_INTERNATIONAL = 'australia_post_express_courier_international'
     AUSTRALIA_POST_INTERNATIONAL_EXPRESS = 'australia_post_international_express'
     AUSTRALIA_POST_INTERNATIONAL_STANDARD = 'australia_post_international_standard'
     AUSTRALIA_POST_INTERNATIONAL_ECONOMY = 'australia_post_international_economy'
     AUSTRALIA_POST_PARCEL_POST_RETURN = 'australia_post_parcel_post_return'
 
+
 class ServiceLevelAsendiaEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | asendia_us_priority_tracked | Asendia USA Priority Tracked|
     | asendia_us_international_express | Asendia USA International Express|
     | asendia_us_international_priority_airmail | Asendia USA International Priority Airmail|
     | asendia_us_international_surface_airlift | Asendia USA International Surface Air Lift|
@@ -662,14 +698,15 @@
     ASENDIA_US_INTERNATIONAL_PRIORITY_AIRMAIL = 'asendia_us_international_priority_airmail'
     ASENDIA_US_INTERNATIONAL_SURFACE_AIRLIFT = 'asendia_us_international_surface_airlift'
     ASENDIA_US_PRIORITY_MAIL_INTERNATIONAL = 'asendia_us_priority_mail_international'
     ASENDIA_US_PRIORITY_MAIL_EXPRESS_INTERNATIONAL = 'asendia_us_priority_mail_express_international'
     ASENDIA_US_EPACKET = 'asendia_us_epacket'
     ASENDIA_US_OTHER = 'asendia_us_other'
 
+
 class ServiceLevelAPCPostalEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | apc_postal_parcelconnect_expedited | parcelConnect Expedited|
     | apc_postal_parcelconnect_priority | parcelConnect Priority|
     | apc_postal_parcelconnect_priority_delcon | parcelConnect Priority Delcon|
     | apc_postal_parcelconnect_priority_pqw | parcelConnect Priority PQW|
@@ -685,23 +722,25 @@
     APC_POSTAL_PARCELCONNECT_PRIORITY_PQW = 'apc_postal_parcelconnect_priority_pqw'
     APC_POSTAL_PARCELCONNECT_BOOK_SERVICE = 'apc_postal_parcelconnect_book_service'
     APC_POSTAL_PARCELCONNECT_STANDARD = 'apc_postal_parcelconnect_standard'
     APC_POSTAL_PARCELCONNECT_EPMI = 'apc_postal_parcelconnect_epmi'
     APC_POSTAL_PARCELCONNECT_EPACKET = 'apc_postal_parcelconnect_epacket'
     APC_POSTAL_PARCELCONNECT_EPMEI = 'apc_postal_parcelconnect_epmei'
 
+
 class ServiceLevelAirterraEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | airterra_ground | GroundXC|
     | airterra_postal | FastPost|
     """
     AIRTERRA_GROUND = 'airterra_ground'
     AIRTERRA_POSTAL = 'airterra_postal'
 
+
 class ServiceLevelUPSEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | ups_standard | Standard℠|
     | ups_ground | Ground|
     | ups_saver | Saver®|
     | ups_3_day_select | 3 Day Select®|
@@ -749,59 +788,69 @@
     UPS_EXPRESS = 'ups_express'
     UPS_EXPRESS_1200 = 'ups_express_1200'
     UPS_EXPRESS_PLUS = 'ups_express_plus'
     UPS_EXPEDITED = 'ups_expedited'
     UPS_EXPRESS_EARLY = 'ups_express_early'
     UPS_ACCESS_POINT_ECONOMY = 'ups_access_point_economy'
 
+
 class ServiceLevelFedExEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | fedex_ground | FedEx Ground®|
     | fedex_home_delivery | FedEx Home Delivery®|
     | fedex_ground_economy | FedEx Ground® Economy|
     | fedex_2_day | FedEx 2Day®|
     | fedex_2_day_am | FedEx 2Day® A.M.|
     | fedex_express_saver | FedEx Express Saver®|
     | fedex_standard_overnight | FedEx Standard Overnight®|
     | fedex_priority_overnight | FedEx Priority Overnight®|
     | fedex_first_overnight | FedEx First Overnight®|
-    | fedex_freight_priority | FedEx Freight® Priority|
-    | fedex_next_day_freight | FedEx Next Day Freight|
-    | fedex_freight_economy | FedEx Freight® Economy|
-    | fedex_first_freight | FedEx First Freight|
     | fedex_international_economy | FedEx International Economy®|
     | fedex_international_priority | FedEx International Priority®|
     | fedex_international_first | FedEx International First®|
     | fedex_europe_first_international_priority | FedEx International First®|
     | fedex_international_connect_plus | FedEx International Connect Plus|
-    | international_economy_freight | FedEx International Economy® Freight|
-    | international_priority_freight | FedEx International Priority® Freight|
+    | fedex_first | FedEx First |
+    | fedex_priority | FedEx Priority |
+    | fedex_priority_express | FedEx Priority Express|
+    | fedex_economy_select | FedEx® Economy |
+    | fedex_regional_economy | FedEx® Regional Economy |
+    | fedex_first_overnight_extra_hours | First Overnight® EH |
+    | fedex_international_priority_express | International Priority® Express |
+    | fedex_next_day_mid_morning | Next Day Mid Morning |
+    | fedex_priority_overnight_extra_hours | Priority Overnight® EH |
+    | fedex_standard_overnight_extra_hours | Standard Overnight® EH |
     """
     FEDEX_GROUND = 'fedex_ground'
     FEDEX_HOME_DELIVERY = 'fedex_home_delivery'
     FEDEX_SMART_POST = 'fedex_smart_post'
     FEDEX_GROUND_ECONOMY = 'fedex_ground_economy'
     FEDEX_2_DAY = 'fedex_2_day'
     FEDEX_2_DAY_AM = 'fedex_2_day_am'
     FEDEX_EXPRESS_SAVER = 'fedex_express_saver'
     FEDEX_STANDARD_OVERNIGHT = 'fedex_standard_overnight'
     FEDEX_PRIORITY_OVERNIGHT = 'fedex_priority_overnight'
     FEDEX_FIRST_OVERNIGHT = 'fedex_first_overnight'
-    FEDEX_FREIGHT_PRIORITY = 'fedex_freight_priority'
-    FEDEX_NEXT_DAY_FREIGHT = 'fedex_next_day_freight'
-    FEDEX_FREIGHT_ECONOMY = 'fedex_freight_economy'
-    FEDEX_FIRST_FREIGHT = 'fedex_first_freight'
     FEDEX_INTERNATIONAL_ECONOMY = 'fedex_international_economy'
     FEDEX_INTERNATIONAL_PRIORITY = 'fedex_international_priority'
     FEDEX_INTERNATIONAL_FIRST = 'fedex_international_first'
     FEDEX_EUROPE_FIRST_INTERNATIONAL_PRIORITY = 'fedex_europe_first_international_priority'
     FEDEX_INTERNATIONAL_CONNECT_PLUS = 'fedex_international_connect_plus'
-    INTERNATIONAL_ECONOMY_FREIGHT = 'international_economy_freight'
-    INTERNATIONAL_PRIORITY_FREIGHT = 'international_priority_freight'
+    FEDEX_FIRST = 'fedex_first'
+    FEDEX_PRIORITY = 'fedex_priority'
+    FEDEX_PRIORITY_EXPRESS = 'fedex_priority_express'
+    FEDEX_ECONOMY_SELECT = 'fedex_economy_select'
+    FEDEX_REGIONAL_ECONOMY = 'fedex_regional_economy'
+    FEDEX_FIRST_OVERNIGHT_EXTRA_HOURS = 'fedex_first_overnight_extra_hours'
+    FEDEX_INTERNATIONAL_PRIORITY_EXPRESS = 'fedex_international_priority_express'
+    FEDEX_NEXT_DAY_MID_MORNING = 'fedex_next_day_mid_morning'
+    FEDEX_PRIORITY_OVERNIGHT_EXTRA_HOURS = 'fedex_priority_overnight_extra_hours'
+    FEDEX_STANDARD_OVERNIGHT_EXTRA_HOURS = 'fedex_standard_overnight_extra_hours'
+
 
 class ServiceLevelUSPSEnum(str, Enum):
     r"""|Token | Service name|
     |:---|:---|
     | usps_priority | Priority Mail|
     | usps_priority_express | Priority Mail Express|
     | usps_media_mail | Media Mail, only for existing Shippo customers with grandfathered Media Mail option.|
@@ -813,7 +862,9 @@
     USPS_PRIORITY = 'usps_priority'
     USPS_PRIORITY_EXPRESS = 'usps_priority_express'
     USPS_MEDIA_MAIL = 'usps_media_mail'
     USPS_PRIORITY_MAIL_INTERNATIONAL = 'usps_priority_mail_international'
     USPS_PRIORITY_MAIL_EXPRESS_INTERNATIONAL = 'usps_priority_mail_express_international'
     USPS_FIRST_CLASS_PACKAGE_INTERNATIONAL_SERVICE = 'usps_first_class_package_international_service'
     USPS_GROUND_ADVANTAGE = 'usps_ground_advantage'
+
+ServiceLevelEnumSet = Union['ServiceLevelUSPSEnum', 'ServiceLevelFedExEnum', 'ServiceLevelUPSEnum', 'ServiceLevelAirterraEnum', 'ServiceLevelAPCPostalEnum', 'ServiceLevelAsendiaEnum', 'ServiceLevelAustraliaPostEnum', 'ServiceLevelAxleHireEnum', 'ServiceLevelAPGEnum', 'ServiceLevelBetterTrucksEnum', 'ServiceLevelCanadaPostEnum', 'ServiceLevelCDLEnum', 'ServiceLevelChronopostEnum', 'ServiceLevelCouriersPleaseEnum', 'ServiceLevelCorreosEspanaEnum', 'ServiceLevelColissimoEnum', 'ServiceLevelPurolatorEnum', 'ServiceLevelDHLExpressEnum', 'ServiceLevelDHLeCommerceEnum', 'ServiceLevelDHLGermanyEnum', 'ServiceLevelDPDDEEnum', 'ServiceLevelDPDUKEnum', 'ServiceLevelDeutschePostEnum', 'ServiceLevelAramexAustraliaEnum', 'ServiceLevelGlobegisticsEnum', 'ServiceLevelGLSUSEnum', 'ServiceLevelLSOEnum', 'ServiceLevelMondialRelayEnum', 'ServiceLevelMaergoEnum', 'ServiceLevelParcelforceEnum', 'ServiceLevelPostItalianeEnum', 'ServiceLevelePostGlobalEnum', 'ServiceLevelRoyalMailEnum', 'ServiceLevelSendleEnum', 'ServiceLevelOnTracEnum', 'ServiceLevelLasershipEnum', 'ServiceLevelEvriUKEnum', 'ServiceLevelUDSEnum', 'ServiceLevelVehoEnum', 'ServiceLevelSwyftEnum']
```

### Comparing `shippo-3.4.1/src/shippo/models/components/shipment.py` & `shippo-3.4.2/src/shippo/models/components/shipment.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .shipmentextra import ShipmentExtra
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
+
 class ShipmentStatus(str, Enum):
     r"""`Waiting` shipments have been successfully submitted but not yet been processed.
     `Queued` shipments are currently being processed. 
     `Success` shipments have been processed successfully, meaning that rate generation has concluded. 
     `Error` does not occur currently and is reserved for future use.
     """
     ERROR = 'ERROR'
```

### Comparing `shippo-3.4.1/src/shippo/models/components/shipmentcreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/shipmentcreaterequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,32 +6,42 @@
 from .customsdeclarationcreaterequest import CustomsDeclarationCreateRequest
 from .parcelcreaterequest import ParcelCreateRequest
 from .shipmentextra import ShipmentExtra
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import List, Optional, Union
 
+AddressFrom = Union[AddressCreateRequest, str]
+
+AddressReturn = Union[AddressCreateRequest, str]
+
+AddressTo = Union[AddressCreateRequest, str]
+
+ShipmentCreateRequestCustomsDeclaration = Union[CustomsDeclarationCreateRequest, str]
+
+Parcels = Union[ParcelCreateRequest, str]
+
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ShipmentCreateRequest:
-    address_from: Union[AddressCreateRequest, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_from') }})
-    address_to: Union[AddressCreateRequest, str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_to') }})
-    parcels: List[Union[ParcelCreateRequest, str]] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parcels') }})
+    address_from: AddressFrom = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_from') }})
+    address_to: AddressTo = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_to') }})
+    parcels: List[Parcels] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parcels') }})
     extra: Optional[ShipmentExtra] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extra'), 'exclude': lambda f: f is None }})
     r"""An object holding optional extra services to be requested."""
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""A string of up to 100 characters that can be filled with any additional information you want to attach to the object."""
     shipment_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shipment_date'), 'exclude': lambda f: f is None }})
     r"""Date the shipment will be tendered to the carrier. Must be in the format `2014-01-18T00:35:03.463Z`.
     Defaults to current date and time if no value is provided. Please note that some carriers require this value to
     be in the future, on a working day, or similar.
     """
-    address_return: Optional[Union[AddressCreateRequest, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_return'), 'exclude': lambda f: f is None }})
-    customs_declaration: Optional[Union[CustomsDeclarationCreateRequest, str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customs_declaration'), 'exclude': lambda f: f is None }})
+    address_return: Optional[AddressReturn] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_return'), 'exclude': lambda f: f is None }})
+    customs_declaration: Optional[ShipmentCreateRequestCustomsDeclaration] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customs_declaration'), 'exclude': lambda f: f is None }})
     async_: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('async'), 'exclude': lambda f: f is None }})
     carrier_accounts: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier_accounts'), 'exclude': lambda f: f is None }})
     r"""List of <a href=\\"#tag/Carrier-Accounts/\\">Carrier Accounts</a> `object_id`s used to filter
     the returned rates.  If set, only rates from these carriers will be returned.
     """
```

### Comparing `shippo-3.4.1/src/shippo/models/components/shipmentextra.py` & `shippo-3.4.2/src/shippo/models/components/shipmentextra.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,64 +9,71 @@
 from .dangerousgoodsobject import DangerousGoodsObject
 from .departmentnumber import DepartmentNumber
 from .dryice import DryIce
 from .insurance import Insurance
 from .invoicenumber import InvoiceNumber
 from .ponumber import PoNumber
 from .rmanumber import RmaNumber
+from .upsreferencefields import UPSReferenceFields
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from shippo import utils
 from typing import Optional
 
+
 class AncillaryEndorsement(str, Enum):
     r"""Specify an ancillary service endorsement to provide the USPS with instructions on how to handle undeliverable-as-addressed pieces (DHL eCommerce only)."""
     FORWARDING_SERVICE_REQUESTED = 'FORWARDING_SERVICE_REQUESTED'
     RETURN_SERVICE_REQUESTED = 'RETURN_SERVICE_REQUESTED'
 
+
 class DangerousGoodsCode(str, Enum):
     r"""Dangerous Goods Code (DHL eCommerce only). See <a href=\\"https://api-legacy.dhlecs.com/docs/v2/appendix.html#dangerous-goods\\">Category Codes</a>"""
     ONE = '01'
     TWO = '02'
     THREE = '03'
     FOUR = '04'
     FIVE = '05'
     SIX = '06'
     SEVEN = '07'
     EIGHT = '08'
     NINE = '09'
 
+
 class LasershipAttrs(str, Enum):
     r"""Specify Lasership Attributes (Lasership only). Multiple options accepted."""
     TWO_PERSON_DELIVERY = 'TwoPersonDelivery'
     EXPLOSIVE = 'Explosive'
     ALCOHOL = 'Alcohol'
     HAZMAT = 'Hazmat'
     CONTROLLED_SUBSTANCE = 'ControlledSubstance'
     REFRIGERATED = 'Refrigerated'
     DRY_ICE = 'DryIce'
     PERISHABLE = 'Perishable'
     NO_RTS = 'NoRTS'
 
+
 class PreferredDeliveryTimeframe(str, Enum):
     r"""Required for DHL Germany Paket Sameday. Designates a desired timeframe for delivery. Format is `HHMMHHMM`"""
     TEN_MILLION_ONE_THOUSAND_TWO_HUNDRED = '10001200'
     TWELVE_MILLION_ONE_THOUSAND_FOUR_HUNDRED = '12001400'
     FOURTEEN_MILLION_ONE_THOUSAND_SIX_HUNDRED = '14001600'
     SIXTEEN_MILLION_ONE_THOUSAND_EIGHT_HUNDRED = '16001800'
     EIGHTEEN_MILLION_TWO_THOUSAND = '18002000'
     NINETEEN_MILLION_TWO_THOUSAND_ONE_HUNDRED = '19002100'
 
+
 class ReturnServiceType(str, Enum):
     r"""Request additional return option for return shipments (UPS only)."""
     PRINT_AND_MAIL = 'PRINT_AND_MAIL'
     ATTEMPT_1 = 'ATTEMPT_1'
     ATTEMPT_3 = 'ATTEMPT_3'
     ELECTRONIC_LABEL = 'ELECTRONIC_LABEL'
 
+
 class SignatureConfirmation(str, Enum):
     r"""Request standard or adult signature confirmation. You can alternatively request Certified Mail (USPS only)
     or Indirect signature (FedEx only) or Carrier Confirmation (Deutsche Post only).
     """
     STANDARD = 'STANDARD'
     ADULT = 'ADULT'
     CERTIFIED = 'CERTIFIED'
@@ -74,89 +81,104 @@
     CARRIER_CONFIRMATION = 'CARRIER_CONFIRMATION'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ShipmentExtra:
     r"""An object holding optional extra services to be requested."""
+    accounts_receivable_customer_account: Optional[UPSReferenceFields] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accounts_receivable_customer_account'), 'exclude': lambda f: f is None }})
+    alcohol: Optional[Alcohol] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('alcohol'), 'exclude': lambda f: f is None }})
+    r"""Indicates that a shipment contains Alcohol (Fedex and UPS only)."""
     ancillary_endorsement: Optional[AncillaryEndorsement] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ancillary_endorsement'), 'exclude': lambda f: f is None }})
     r"""Specify an ancillary service endorsement to provide the USPS with instructions on how to handle undeliverable-as-addressed pieces (DHL eCommerce only)."""
+    appropriation_number: Optional[UPSReferenceFields] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('appropriation_number'), 'exclude': lambda f: f is None }})
     authority_to_leave: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('authority_to_leave'), 'exclude': lambda f: f is None }})
     r"""Request `true` to give carrier permission to leave the parcel in a safe place if no one answers the
     door (where supported). When set to `false`, if no one is available to receive the item, the parcel 
     will not be left (*surcharges may be applicable).
     """
-    alcohol: Optional[Alcohol] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('alcohol'), 'exclude': lambda f: f is None }})
-    r"""Indicates that a shipment contains Alcohol (Fedex and UPS only)."""
+    bill_of_lading_number: Optional[UPSReferenceFields] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bill_of_lading_number'), 'exclude': lambda f: f is None }})
     billing: Optional[Billing] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('billing'), 'exclude': lambda f: f is None }})
     r"""Specify billing details (UPS, FedEx, and DHL Germany only)."""
     bypass_address_validation: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bypass_address_validation'), 'exclude': lambda f: f is None }})
     r"""Bypasses address validation (USPS, UPS, & LaserShip only)."""
     carbon_neutral: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carbon_neutral'), 'exclude': lambda f: f is None }})
     r"""Request carbon offsets by passing true (UPS only)."""
     carrier_hub_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier_hub_id'), 'exclude': lambda f: f is None }})
     r"""Identifies the carrier injection site."""
     carrier_hub_travel_time: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier_hub_travel_time'), 'exclude': lambda f: f is None }})
     r"""Travel time in hours from fulfillment center to carrier injection site."""
     cod: Optional[Cod] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('COD'), 'exclude': lambda f: f is None }})
     r"""Specify collection on delivery details (UPS only)."""
+    cod_number: Optional[UPSReferenceFields] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cod_number'), 'exclude': lambda f: f is None }})
     container_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('container_type'), 'exclude': lambda f: f is None }})
     r"""Specify container type."""
     critical_pull_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('critical_pull_time'), 'exclude': lambda f: f is None }})
     r"""Carrier arrival time to pickup packages from the fulfillment center.
     UTC format: `%Y-%m-%dT%H:%M:%SZ`
     """
     customer_branch: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer_branch'), 'exclude': lambda f: f is None }})
     r"""Specify customer branch (Lasership only)."""
     customer_reference: Optional[CustomerReference] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer_reference'), 'exclude': lambda f: f is None }})
-    r"""Specify the reference field on the label (FedEx only)."""
-    dangerous_goods_code: Optional[DangerousGoodsCode] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dangerous_goods_code'), 'exclude': lambda f: f is None }})
-    r"""Dangerous Goods Code (DHL eCommerce only). See <a href=\\"https://api-legacy.dhlecs.com/docs/v2/appendix.html#dangerous-goods\\">Category Codes</a>"""
+    r"""Specify the reference field on the label (FedEx and UPS only)."""
     dangerous_goods: Optional[DangerousGoodsObject] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dangerous_goods'), 'exclude': lambda f: f is None }})
     r"""Container for specifying the presence of dangerous materials. This is specific to USPS, and if any contents
     are provided, only certain USPS service levels will be eligible. For more information, see our
     <a href=\"https://docs.goshippo.com/docs/shipments/hazmat/\">guide on hazardous or dangerous materials shipping</a>.
     """
+    dangerous_goods_code: Optional[DangerousGoodsCode] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dangerous_goods_code'), 'exclude': lambda f: f is None }})
+    r"""Dangerous Goods Code (DHL eCommerce only). See <a href=\\"https://api-legacy.dhlecs.com/docs/v2/appendix.html#dangerous-goods\\">Category Codes</a>"""
+    dealer_order_number: Optional[UPSReferenceFields] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dealer_order_number'), 'exclude': lambda f: f is None }})
     delivery_instructions: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('delivery_instructions'), 'exclude': lambda f: f is None }})
     r"""Specify delivery instructions. Up to 500 characters. (FedEx and OnTrac only)."""
     dept_number: Optional[DepartmentNumber] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dept_number'), 'exclude': lambda f: f is None }})
-    r"""Specify the department number field on the label (FedEx only)."""
+    r"""Specify the department number field on the label (FedEx and UPS only)."""
     dry_ice: Optional[DryIce] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dry_ice'), 'exclude': lambda f: f is None }})
     r"""Specify that the package contains Dry Ice (FedEx, Veho, and UPS only)."""
+    fda_product_code: Optional[UPSReferenceFields] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fda_product_code'), 'exclude': lambda f: f is None }})
     fulfillment_center: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fulfillment_center'), 'exclude': lambda f: f is None }})
     r"""The fulfilment center where the package originates from."""
     insurance: Optional[Insurance] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('insurance'), 'exclude': lambda f: f is None }})
     r"""To add 3rd party insurance powered by <a href=\\"https://docs.goshippo.com/docs/shipments/shippinginsurance/\\">XCover</a>, specify <br> `amount`, `content`, and `currency`. <br> Alternatively, you can choose carrier provided insurance by additionally specifying `provider` (UPS, FedEx and OnTrac only). <br><br> If you do not want to add insurance to you shipment, do not set these parameters."""
     invoice_number: Optional[InvoiceNumber] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('invoice_number'), 'exclude': lambda f: f is None }})
-    r"""Specify the invoice number field on the label (FedEx only)."""
+    r"""Specify the invoice number field on the label (FedEx and UPS only)."""
     is_return: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_return'), 'exclude': lambda f: f is None }})
     r"""This field specifies if it is a scan-based return shipment. See the <a href=\\"https://docs.goshippo.com/docs/shipments/returns/\\">Create a return shipment</a> section for more details."""
     lasership_attrs: Optional[LasershipAttrs] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lasership_attrs'), 'exclude': lambda f: f is None }})
     r"""Specify Lasership Attributes (Lasership only). Multiple options accepted."""
     lasership_declared_value: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lasership_declared_value'), 'exclude': lambda f: f is None }})
     r"""Declared value (Lasership only). Defaults to `50.00`."""
+    manifest_number: Optional[UPSReferenceFields] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('manifest_number'), 'exclude': lambda f: f is None }})
+    model_number: Optional[UPSReferenceFields] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('model_number'), 'exclude': lambda f: f is None }})
+    part_number: Optional[UPSReferenceFields] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('part_number'), 'exclude': lambda f: f is None }})
     po_number: Optional[PoNumber] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('po_number'), 'exclude': lambda f: f is None }})
-    r"""Specify the PO number field on the label (FedEx only)."""
+    r"""Specify the PO number field on the label (FedEx and UPS only)."""
     preferred_delivery_timeframe: Optional[PreferredDeliveryTimeframe] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('preferred_delivery_timeframe'), 'exclude': lambda f: f is None }})
     r"""Required for DHL Germany Paket Sameday. Designates a desired timeframe for delivery. Format is `HHMMHHMM`"""
     premium: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('premium'), 'exclude': lambda f: f is None }})
     r"""Add premium service to a shipment (DHL Germany international shipments only)."""
+    production_code: Optional[UPSReferenceFields] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('production_code'), 'exclude': lambda f: f is None }})
+    purchase_request_number: Optional[UPSReferenceFields] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('purchase_request_number'), 'exclude': lambda f: f is None }})
     qr_code_requested: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('qr_code_requested'), 'exclude': lambda f: f is None }})
     r"""Request a QR code for a given transaction when creating a shipping label (USPS domestic and Evri UK only)."""
     reference_1: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference_1'), 'exclude': lambda f: f is None }})
     r"""Optional text to be printed on the shipping label if supported by carrier. Up to 50 characters."""
     reference_2: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reference_2'), 'exclude': lambda f: f is None }})
     r"""Optional text to be printed on the shipping label if supported by carrier. Up to 50 characters. For DHL eCommerce, this field can be used for billing reference."""
     request_retail_rates: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('request_retail_rates'), 'exclude': lambda f: f is None }})
     r"""Returns retail rates instead of account-based rates (UPS and FedEx only)."""
     return_service_type: Optional[ReturnServiceType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('return_service_type'), 'exclude': lambda f: f is None }})
     r"""Request additional return option for return shipments (UPS only)."""
     rma_number: Optional[RmaNumber] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rma_number'), 'exclude': lambda f: f is None }})
-    r"""Specify the RMA number field on the label (FedEx only)."""
+    r"""Specify the RMA number field on the label (FedEx and UPS only)."""
     saturday_delivery: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('saturday_delivery'), 'exclude': lambda f: f is None }})
     r"""Marks shipment as to be delivered on a Saturday."""
+    salesperson_number: Optional[UPSReferenceFields] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('salesperson_number'), 'exclude': lambda f: f is None }})
+    serial_number: Optional[UPSReferenceFields] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('serial_number'), 'exclude': lambda f: f is None }})
     signature_confirmation: Optional[SignatureConfirmation] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('signature_confirmation'), 'exclude': lambda f: f is None }})
     r"""Request standard or adult signature confirmation. You can alternatively request Certified Mail (USPS only)
     or Indirect signature (FedEx only) or Carrier Confirmation (Deutsche Post only).
     """
+    store_number: Optional[UPSReferenceFields] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('store_number'), 'exclude': lambda f: f is None }})
+    transaction_reference_number: Optional[UPSReferenceFields] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transaction_reference_number'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.4.1/src/shippo/models/components/shipmentpaginatedlist.py` & `shippo-3.4.2/src/shippo/models/components/shipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/shippoaccount.py` & `shippo-3.4.2/src/shippo/models/components/shippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/shippoaccountpaginatedlist.py` & `shippo-3.4.2/src/shippo/models/components/shippoaccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/shippoaccountupdaterequest.py` & `shippo-3.4.2/src/shippo/models/components/shippoaccountupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/track.py` & `shippo-3.4.2/src/shippo/models/components/track.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from .servicelevel import ServiceLevel
+from .servicelevelwithparent import ServiceLevelWithParent
 from .trackingstatus import TrackingStatus
 from .trackingstatuslocationbase import TrackingStatusLocationBase
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from shippo import utils
 from typing import List, Optional
 
@@ -30,16 +30,15 @@
     r"""The recipient address with city, state, zip and country information."""
     eta: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eta'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""The estimated time of arrival according to the carrier, this might be updated by carriers during the life of the shipment."""
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""A string of up to 100 characters that can be filled with any additional information you want to attach to the object."""
     original_eta: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('original_eta'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""The estimated time of arrival according to the carrier at the time the shipment first entered the system."""
-    servicelevel: Optional[ServiceLevel] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('servicelevel'), 'exclude': lambda f: f is None }})
-    r"""Contains details regarding the service level for the given rate."""
+    servicelevel: Optional[ServiceLevelWithParent] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('servicelevel'), 'exclude': lambda f: f is None }})
     tracking_status: Optional[TrackingStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_status'), 'exclude': lambda f: f is None }})
     r"""The latest tracking information of this shipment."""
     transaction: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transaction'), 'exclude': lambda f: f is None }})
     r"""The <code>object_id</code> of the transaction associated with this tracking object.
     This field is visible only to the object owner of the transaction.
     """
```

### Comparing `shippo-3.4.1/src/shippo/models/components/trackingstatus.py` & `shippo-3.4.2/src/shippo/models/components/trackingstatus.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 class TrackingStatus:
     r"""The latest tracking information of this shipment."""
     object_created: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_created'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
     object_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id') }})
     object_updated: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_updated'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
     status: TrackingStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
     r"""Indicates the high level status of the shipment."""
-    status_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
-    r"""Date and time when the carrier scanned this tracking event. This is displayed in UTC."""
     status_details: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status_details') }})
     r"""The human-readable description of the status."""
     location: Optional[TrackingStatusLocationBase] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location'), 'exclude': lambda f: f is None }})
     r"""An object containing zip, city, state and country information of the tracking event."""
     substatus: Optional[TrackingStatusSubstatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('substatus'), 'exclude': lambda f: f is None }})
     r"""A finer-grained classification of the tracking event."""
+    status_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
+    r"""Date and time when the carrier scanned this tracking event. This is displayed in UTC."""
```

### Comparing `shippo-3.4.1/src/shippo/models/components/trackingstatuslocationbase.py` & `shippo-3.4.2/src/shippo/models/components/trackingstatuslocationbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/trackingstatussubstatus.py` & `shippo-3.4.2/src/shippo/models/components/trackingstatussubstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/tracksrequest.py` & `shippo-3.4.2/src/shippo/models/components/tracksrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/transaction.py` & `shippo-3.4.2/src/shippo/models/components/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .transactionstatusenum import TransactionStatusEnum
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
+
 class ResponseType(str, Enum):
     STANDARD = 'standard'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Transaction:
```

### Comparing `shippo-3.4.1/src/shippo/models/components/transactioncreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/transactioncreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/transactionpaginatedlist.py` & `shippo-3.4.2/src/shippo/models/components/transactionpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/upsconnectexistingownaccountparameters.py` & `shippo-3.4.2/src/shippo/models/components/upsconnectexistingownaccountparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/userparceltemplate.py` & `shippo-3.4.2/src/shippo/models/components/userparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/userparceltemplateupdaterequest.py` & `shippo-3.4.2/src/shippo/models/components/userparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py` & `shippo-3.4.2/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/errors/initiateoauth2signin.py` & `shippo-3.4.2/src/shippo/models/errors/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/errors/sdkerror.py` & `shippo-3.4.2/src/shippo/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/__init__.py` & `shippo-3.4.2/src/shippo/models/operations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,8 +62,8 @@
 from .updatecarrieraccount import *
 from .updatedefaultparceltemplate import *
 from .updateservicegroup import *
 from .updateshippoaccount import *
 from .updateuserparceltemplate import *
 from .validateaddress import *
 
-__all__ = ["AddShipmentsToBatchGlobals","AddShipmentsToBatchRequest","Carrier","CreateAddressGlobals","CreateBatchGlobals","CreateCarrierAccountGlobals","CreateCustomsDeclarationGlobals","CreateCustomsItemGlobals","CreateLiveRateGlobals","CreateManifestGlobals","CreateOrderGlobals","CreateParcelGlobals","CreatePickupGlobals","CreateRefundGlobals","CreateServiceGroupGlobals","CreateShipmentGlobals","CreateShippoAccountGlobals","CreateTrackGlobals","CreateTransactionGlobals","CreateUserParcelTemplateGlobals","DeleteDefaultParcelTemplateGlobals","DeleteDefaultParcelTemplateRequest","DeleteDefaultParcelTemplateResponse","DeleteServiceGroupGlobals","DeleteServiceGroupRequest","DeleteServiceGroupResponse","DeleteUserParcelTemplateGlobals","DeleteUserParcelTemplateRequest","DeleteUserParcelTemplateResponse","GetAddressGlobals","GetAddressRequest","GetBatchGlobals","GetBatchRequest","GetCarrierAccountGlobals","GetCarrierAccountRequest","GetCarrierParcelTemplateGlobals","GetCarrierParcelTemplateRequest","GetCarrierRegistrationStatusGlobals","GetCarrierRegistrationStatusRequest","GetCustomsDeclarationGlobals","GetCustomsDeclarationRequest","GetCustomsItemGlobals","GetCustomsItemRequest","GetDefaultParcelTemplateGlobals","GetDefaultParcelTemplateRequest","GetManifestGlobals","GetManifestRequest","GetOrderGlobals","GetOrderRequest","GetParcelGlobals","GetParcelRequest","GetRateGlobals","GetRateRequest","GetRefundGlobals","GetRefundRequest","GetShipmentGlobals","GetShipmentRequest","GetShippoAccountGlobals","GetShippoAccountRequest","GetTrackGlobals","GetTrackRequest","GetTransactionGlobals","GetTransactionRequest","GetUserParcelTemplateGlobals","GetUserParcelTemplateRequest","Include","InitiateOauth2SigninGlobals","InitiateOauth2SigninRequest","InitiateOauth2SigninResponse","ListAddressesGlobals","ListAddressesRequest","ListCarrierAccountsGlobals","ListCarrierAccountsRequest","ListCarrierParcelTemplatesGlobals","ListCarrierParcelTemplatesRequest","ListCustomsDeclarationsGlobals","ListCustomsDeclarationsRequest","ListCustomsItemsGlobals","ListCustomsItemsRequest","ListManifestsGlobals","ListManifestsRequest","ListOrdersGlobals","ListOrdersRequest","ListParcelsGlobals","ListParcelsRequest","ListRefundsGlobals","ListRefundsRequest","ListServiceGroupsGlobals","ListServiceGroupsRequest","ListShipmentRatesByCurrencyCodeGlobals","ListShipmentRatesByCurrencyCodeRequest","ListShipmentRatesGlobals","ListShipmentRatesRequest","ListShipmentsGlobals","ListShipmentsRequest","ListShippoAccountsGlobals","ListShippoAccountsRequest","ListTransactionsGlobals","ListTransactionsRequest","ListUserParcelTemplatesGlobals","ListUserParcelTemplatesRequest","PurchaseBatchGlobals","PurchaseBatchRequest","RegisterCarrierAccountGlobals","RemoveShipmentsFromBatchGlobals","RemoveShipmentsFromBatchRequest","UpdateCarrierAccountGlobals","UpdateCarrierAccountRequest","UpdateDefaultParcelTemplateGlobals","UpdateServiceGroupGlobals","UpdateShippoAccountGlobals","UpdateShippoAccountRequest","UpdateUserParcelTemplateGlobals","UpdateUserParcelTemplateRequest","ValidateAddressGlobals","ValidateAddressRequest"]
+__all__ = ["AddShipmentsToBatchGlobals","AddShipmentsToBatchRequest","Carrier","CreateAddressGlobals","CreateBatchGlobals","CreateCarrierAccountGlobals","CreateCustomsDeclarationGlobals","CreateCustomsItemGlobals","CreateLiveRateGlobals","CreateManifestGlobals","CreateOrderGlobals","CreateParcelGlobals","CreatePickupGlobals","CreateRefundGlobals","CreateServiceGroupGlobals","CreateShipmentGlobals","CreateShippoAccountGlobals","CreateTrackGlobals","CreateTransactionGlobals","CreateTransactionRequestBody","CreateUserParcelTemplateGlobals","DeleteDefaultParcelTemplateGlobals","DeleteDefaultParcelTemplateRequest","DeleteServiceGroupGlobals","DeleteServiceGroupRequest","DeleteUserParcelTemplateGlobals","DeleteUserParcelTemplateRequest","GetAddressGlobals","GetAddressRequest","GetBatchGlobals","GetBatchRequest","GetCarrierAccountGlobals","GetCarrierAccountRequest","GetCarrierParcelTemplateGlobals","GetCarrierParcelTemplateRequest","GetCarrierRegistrationStatusGlobals","GetCarrierRegistrationStatusRequest","GetCustomsDeclarationGlobals","GetCustomsDeclarationRequest","GetCustomsItemGlobals","GetCustomsItemRequest","GetDefaultParcelTemplateGlobals","GetDefaultParcelTemplateRequest","GetManifestGlobals","GetManifestRequest","GetOrderGlobals","GetOrderRequest","GetParcelGlobals","GetParcelRequest","GetRateGlobals","GetRateRequest","GetRefundGlobals","GetRefundRequest","GetShipmentGlobals","GetShipmentRequest","GetShippoAccountGlobals","GetShippoAccountRequest","GetTrackGlobals","GetTrackRequest","GetTransactionGlobals","GetTransactionRequest","GetUserParcelTemplateGlobals","GetUserParcelTemplateRequest","Include","InitiateOauth2SigninGlobals","InitiateOauth2SigninRequest","InitiateOauth2SigninResponse","ListAddressesGlobals","ListAddressesRequest","ListCarrierAccountsGlobals","ListCarrierAccountsRequest","ListCarrierParcelTemplatesGlobals","ListCarrierParcelTemplatesRequest","ListCustomsDeclarationsGlobals","ListCustomsDeclarationsRequest","ListCustomsItemsGlobals","ListCustomsItemsRequest","ListManifestsGlobals","ListManifestsRequest","ListOrdersGlobals","ListOrdersRequest","ListParcelsGlobals","ListParcelsRequest","ListRefundsGlobals","ListRefundsRequest","ListServiceGroupsGlobals","ListServiceGroupsRequest","ListShipmentRatesByCurrencyCodeGlobals","ListShipmentRatesByCurrencyCodeRequest","ListShipmentRatesGlobals","ListShipmentRatesRequest","ListShipmentsGlobals","ListShipmentsRequest","ListShippoAccountsGlobals","ListShippoAccountsRequest","ListTransactionsGlobals","ListTransactionsRequest","ListUserParcelTemplatesGlobals","ListUserParcelTemplatesRequest","PurchaseBatchGlobals","PurchaseBatchRequest","RegisterCarrierAccountGlobals","RegisterCarrierAccountRequestBody","RemoveShipmentsFromBatchGlobals","RemoveShipmentsFromBatchRequest","UpdateCarrierAccountGlobals","UpdateCarrierAccountRequest","UpdateDefaultParcelTemplateGlobals","UpdateServiceGroupGlobals","UpdateShippoAccountGlobals","UpdateShippoAccountRequest","UpdateUserParcelTemplateGlobals","UpdateUserParcelTemplateRequest","ValidateAddressGlobals","ValidateAddressRequest"]
```

### Comparing `shippo-3.4.1/src/shippo/models/operations/addshipmentstobatch.py` & `shippo-3.4.2/src/shippo/models/operations/addshipmentstobatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/deletedefaultparceltemplate.py` & `shippo-3.4.2/src/shippo/models/operations/deletedefaultparceltemplate.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,12 +12,7 @@
     
 
 
 
 @dataclasses.dataclass
 class DeleteDefaultParcelTemplateRequest:
     pass
-
-
-@dataclasses.dataclass
-class DeleteDefaultParcelTemplateResponse:
-    pass
```

### Comparing `shippo-3.4.1/src/shippo/models/operations/deleteservicegroup.py` & `shippo-3.4.2/src/shippo/models/operations/deleteservicegroup.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,12 +15,7 @@
 
 @dataclasses.dataclass
 class DeleteServiceGroupRequest:
     service_group_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ServiceGroupId', 'style': 'simple', 'explode': False }})
     r"""Object ID of the service group"""
     
 
-
-
-@dataclasses.dataclass
-class DeleteServiceGroupResponse:
-    pass
```

### Comparing `shippo-3.4.1/src/shippo/models/operations/deleteuserparceltemplate.py` & `shippo-3.4.2/src/shippo/models/operations/deleteuserparceltemplate.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,12 +15,7 @@
 
 @dataclasses.dataclass
 class DeleteUserParcelTemplateRequest:
     user_parcel_template_object_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'UserParcelTemplateObjectId', 'style': 'simple', 'explode': False }})
     r"""Object ID of the user parcel template"""
     
 
-
-
-@dataclasses.dataclass
-class DeleteUserParcelTemplateResponse:
-    pass
```

### Comparing `shippo-3.4.1/src/shippo/models/operations/getaddress.py` & `shippo-3.4.2/src/shippo/models/operations/getaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/getbatch.py` & `shippo-3.4.2/src/shippo/models/operations/getbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/getcarrieraccount.py` & `shippo-3.4.2/src/shippo/models/operations/getcarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/getcarrierparceltemplate.py` & `shippo-3.4.2/src/shippo/models/operations/getcarrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/getcarrierregistrationstatus.py` & `shippo-3.4.2/src/shippo/models/operations/getcarrierregistrationstatus.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 @dataclasses.dataclass
 class GetCarrierRegistrationStatusGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
+
 class Carrier(str, Enum):
     r"""filter by specific carrier"""
     UPS = 'ups'
     USPS = 'usps'
     CANADA_POST = 'canada_post'
```

### Comparing `shippo-3.4.1/src/shippo/models/operations/getcustomsdeclaration.py` & `shippo-3.4.2/src/shippo/models/operations/getcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/getcustomsitem.py` & `shippo-3.4.2/src/shippo/models/operations/getcustomsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/getdefaultparceltemplate.py` & `shippo-3.4.2/src/shippo/models/operations/getdefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/getmanifest.py` & `shippo-3.4.2/src/shippo/models/operations/getmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/getorder.py` & `shippo-3.4.2/src/shippo/models/operations/getorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/getparcel.py` & `shippo-3.4.2/src/shippo/models/operations/getparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/getrate.py` & `shippo-3.4.2/src/shippo/models/operations/getrate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/getrefund.py` & `shippo-3.4.2/src/shippo/models/operations/getrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/getshipment.py` & `shippo-3.4.2/src/shippo/models/operations/getshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/getshippoaccount.py` & `shippo-3.4.2/src/shippo/models/operations/getshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/gettrack.py` & `shippo-3.4.2/src/shippo/models/operations/gettrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/gettransaction.py` & `shippo-3.4.2/src/shippo/models/operations/gettransaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/getuserparceltemplate.py` & `shippo-3.4.2/src/shippo/models/operations/getuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/initiateoauth2signin.py` & `shippo-3.4.2/src/shippo/models/operations/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/listaddresses.py` & `shippo-3.4.2/src/shippo/models/operations/listaddresses.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/listcarrieraccounts.py` & `shippo-3.4.2/src/shippo/models/operations/listcarrieraccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/listcarrierparceltemplates.py` & `shippo-3.4.2/src/shippo/models/operations/listcarrierparceltemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 @dataclasses.dataclass
 class ListCarrierParcelTemplatesGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
+
 class Include(str, Enum):
     r"""filter by user or enabled"""
     ALL = 'all'
     USER = 'user'
     ENABLED = 'enabled'
```

### Comparing `shippo-3.4.1/src/shippo/models/operations/listcustomsdeclarations.py` & `shippo-3.4.2/src/shippo/models/operations/listcustomsdeclarations.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/listcustomsitems.py` & `shippo-3.4.2/src/shippo/models/operations/listcustomsitems.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/listmanifests.py` & `shippo-3.4.2/src/shippo/models/operations/listmanifests.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/listorders.py` & `shippo-3.4.2/src/shippo/models/operations/listorders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/listparcels.py` & `shippo-3.4.2/src/shippo/models/operations/listparcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/listservicegroups.py` & `shippo-3.4.2/src/shippo/models/operations/listservicegroups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/listshipmentrates.py` & `shippo-3.4.2/src/shippo/models/operations/listshipmentrates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/listshipmentratesbycurrencycode.py` & `shippo-3.4.2/src/shippo/models/operations/listshipmentratesbycurrencycode.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/listshipments.py` & `shippo-3.4.2/src/shippo/models/operations/listshipments.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/listshippoaccounts.py` & `shippo-3.4.2/src/shippo/models/operations/listshippoaccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/listtransactions.py` & `shippo-3.4.2/src/shippo/models/operations/listtransactions.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/listuserparceltemplates.py` & `shippo-3.4.2/src/shippo/models/operations/listuserparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/purchasebatch.py` & `shippo-3.4.2/src/shippo/models/operations/purchasebatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/removeshipmentsfrombatch.py` & `shippo-3.4.2/src/shippo/models/operations/removeshipmentsfrombatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/updatecarrieraccount.py` & `shippo-3.4.2/src/shippo/models/operations/updatecarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/updateshippoaccount.py` & `shippo-3.4.2/src/shippo/models/operations/updateshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/updateuserparceltemplate.py` & `shippo-3.4.2/src/shippo/models/operations/updateuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/models/operations/validateaddress.py` & `shippo-3.4.2/src/shippo/models/operations/validateaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/orders.py` & `shippo-3.4.2/src/shippo/orders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/parcels.py` & `shippo-3.4.2/src/shippo/parcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/pickups.py` & `shippo-3.4.2/src/shippo/pickups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/rates.py` & `shippo-3.4.2/src/shippo/rates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/rates_at_checkout.py` & `shippo-3.4.2/src/shippo/rates_at_checkout.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def delete_default_parcel_template(self) -> operations.DeleteDefaultParcelTemplateResponse:
+    def delete_default_parcel_template(self):
         r"""Clear current default parcel template
         Clears the currently configured default parcel template for live rates.
         """
         hook_ctx = HookContext(operation_id='DeleteDefaultParcelTemplate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.DeleteDefaultParcelTemplateRequest(
         )
         
@@ -266,20 +266,17 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.DeleteDefaultParcelTemplateResponse()
         
         if http_res.status_code == 204:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-        return res
-
```

### Comparing `shippo-3.4.1/src/shippo/refunds.py` & `shippo-3.4.2/src/shippo/refunds.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
     
     def create(self, transaction: str, async_: Optional[bool] = None) -> components.Refund:
         r"""Create a refund
         Creates a new refund object.
         """
         hook_ctx = HookContext(operation_id='CreateRefund', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = components.RefundRequestBody(
-            transaction=transaction,
             async_=async_,
+            transaction=transaction,
         )
         
         _globals = operations.CreateRefundGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
```

### Comparing `shippo-3.4.1/src/shippo/sdk.py` & `shippo-3.4.2/src/shippo/sdk.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/sdkconfiguration.py` & `shippo-3.4.2/src/shippo/sdkconfiguration.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '2018-02-08'
-    sdk_version: str = '3.4.1'
-    gen_version: str = '2.329.0'
-    user_agent: str = 'speakeasy-sdk/python 3.4.1 2.329.0 2018-02-08 shippo'
+    sdk_version: str = '3.4.2'
+    gen_version: str = '2.335.5'
+    user_agent: str = 'speakeasy-sdk/python 3.4.2 2.335.5 2018-02-08 shippo'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `shippo-3.4.1/src/shippo/service_groups.py` & `shippo-3.4.2/src/shippo/service_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def delete(self, service_group_id: str) -> operations.DeleteServiceGroupResponse:
+    def delete(self, service_group_id: str):
         r"""Delete a service group
         Deletes an existing service group using an object ID.
         """
         hook_ctx = HookContext(operation_id='DeleteServiceGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.DeleteServiceGroupRequest(
             service_group_id=service_group_id,
         )
@@ -254,20 +254,17 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.DeleteServiceGroupResponse()
         
         if http_res.status_code == 204:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-        return res
-
```

### Comparing `shippo-3.4.1/src/shippo/shipments.py` & `shippo-3.4.2/src/shippo/shipments.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/shippo_accounts.py` & `shippo-3.4.2/src/shippo/shippo_accounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/tracking_status.py` & `shippo-3.4.2/src/shippo/tracking_status.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     def create(self, carrier: str, tracking_number: str, metadata: Optional[str] = None) -> components.Track:
         r"""Register a tracking webhook
         Registers a webhook that will send HTTP notifications to you when the status of your tracked package changes. For more details on creating a webhook, see our guides on <a href=\"https://docs.goshippo.com/docs/tracking/webhooks/\">Webhooks</a> and <a href=\"https://docs.goshippo.com/docs/tracking/tracking/\">Tracking</a>.
         """
         hook_ctx = HookContext(operation_id='CreateTrack', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = components.TracksRequest(
             carrier=carrier,
-            tracking_number=tracking_number,
             metadata=metadata,
+            tracking_number=tracking_number,
         )
         
         _globals = operations.CreateTrackGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
```

### Comparing `shippo-3.4.1/src/shippo/transactions.py` & `shippo-3.4.2/src/shippo/transactions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
 from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
-from typing import Optional, Union
+from typing import Optional
 
 class Transactions:
     r"""A transaction is the purchase of a shipping label from a shipping provider for a specific service. You can print purchased labels and used them to ship a parcel with a carrier, such as USPS or FedEx.
     <SchemaDefinition schemaRef=\"#/components/schemas/Transaction\"/>
     """
     sdk_configuration: SDKConfiguration
 
@@ -74,15 +74,15 @@
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, request: Union[components.TransactionCreateRequest, components.InstantTransactionCreateRequest]) -> Union[components.Transaction, components.InstantTransactionCreateResponse]:
+    def create(self, request: operations.CreateTransactionRequestBody) -> components.TransactionCreateResponse:
         r"""Create a shipping label
         Creates a new transaction object and purchases the shipping label using a rate object that has previously been created. <br> OR <br> Creates a new transaction object and purchases the shipping label instantly using shipment details, an existing carrier account, and an existing service level token.
         """
         hook_ctx = HookContext(operation_id='CreateTransaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         _globals = operations.CreateTransactionGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
@@ -93,15 +93,15 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Union[components.TransactionCreateRequest, components.InstantTransactionCreateRequest], "request", False, False, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateTransactionRequestBody, "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
@@ -127,15 +127,15 @@
             
         
         
         
         if http_res.status_code == 201:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[Union[components.Transaction, components.InstantTransactionCreateResponse]])
+                out = utils.unmarshal_json(http_res.text, Optional[components.TransactionCreateResponse])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `shippo-3.4.1/src/shippo/user_parcel_templates.py` & `shippo-3.4.2/src/shippo/user_parcel_templates.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
 from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
-from typing import List, Optional, Union
+from typing import Optional
 
 class UserParcelTemplates:
     r"""A user parcel template represents a package used for shipping that has preset dimensions and attributes defined
     by you. They are useful for capturing attributes of parcel-types you frequently use for shipping, allowing 
     them to be defined once and then used for many shipments. These parcel templates can also be used for live rates.
 
     User parcel templates can also be created using a carrier parcel template, where the dimensions will be copied from 
@@ -19,15 +19,15 @@
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def list(self) -> List[components.UserParcelTemplate]:
+    def list(self) -> components.UserParcelTemplateList:
         r"""List all user parcel templates
         Returns a list all of all user parcel template objects.
         """
         hook_ctx = HookContext(operation_id='ListUserParcelTemplates', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.ListUserParcelTemplatesRequest(
         )
         
@@ -70,27 +70,27 @@
             
         
         
         
         if http_res.status_code == 200:
             # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[List[components.UserParcelTemplate]])
+                out = utils.unmarshal_json(http_res.text, Optional[components.UserParcelTemplateList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, request: Union[components.UserParcelTemplateWithCarrierTemplateCreateRequest, components.UserParcelTemplateWithoutCarrierTemplateCreateRequest]) -> components.UserParcelTemplate:
+    def create(self, request: components.UserParcelTemplateCreateRequest) -> components.UserParcelTemplate:
         r"""Create a new user parcel template
         Creates a new user parcel template. <br>You can choose to create a
         parcel template using a preset carrier template as a starting point, or
         you can create an entirely custom one. To use a preset carrier template,
         pass in a unique template token from <a href=\"#tag/Parcel-Templates\">this list</a>
         plus the weight fields (**weight** and **weight_unit**). Otherwise, omit
         the template field and pass the other fields, for the weight, length, height,
@@ -107,15 +107,15 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Union[components.UserParcelTemplateWithCarrierTemplateCreateRequest, components.UserParcelTemplateWithoutCarrierTemplateCreateRequest], "request", False, False, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, components.UserParcelTemplateCreateRequest, "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         if data is None and form is None:
             raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
@@ -153,15 +153,15 @@
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def delete(self, user_parcel_template_object_id: str) -> operations.DeleteUserParcelTemplateResponse:
+    def delete(self, user_parcel_template_object_id: str):
         r"""Delete a user parcel template
         Deletes a user parcel template using an object ID.
         """
         hook_ctx = HookContext(operation_id='DeleteUserParcelTemplate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.DeleteUserParcelTemplateRequest(
             user_parcel_template_object_id=user_parcel_template_object_id,
         )
@@ -201,25 +201,22 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.DeleteUserParcelTemplateResponse()
         
         if http_res.status_code == 204:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-        return res
-
     
     
     def get(self, user_parcel_template_object_id: str) -> components.UserParcelTemplate:
         r"""Retrieves a user parcel template
         Returns the parcel template information for a specific user parcel
         template, identified by the object ID.
         """
```

### Comparing `shippo-3.4.1/src/shippo/utils/retries.py` & `shippo-3.4.2/src/shippo/utils/retries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.4.1/src/shippo/utils/utils.py` & `shippo-3.4.2/src/shippo/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -814,19 +814,19 @@
             return ",".join(items)
     else:
         return f"{_val_to_string(obj)}"
 
     return ""
 
 
-def unmarshal_json(data, typ, decoder=None):
+def unmarshal_json(data, typ, decoder=None, infer_missing=False):
     unmarshal = make_dataclass("Unmarshal", [("res", typ)], bases=(DataClassJsonMixin,))
     json_dict = json.loads(data)
     try:
-        out = unmarshal.from_dict({"res": json_dict})
+        out = unmarshal.from_dict({"res": json_dict}, infer_missing=infer_missing)
     except AttributeError as attr_err:
         raise AttributeError(
             f"unable to unmarshal {data} as {typ} - {attr_err}"
         ) from attr_err
 
     return out.res if decoder is None else decoder(out.res)
```

### Comparing `shippo-3.4.1/src/shippo.egg-info/PKG-INFO` & `shippo-3.4.2/src/shippo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.4.1
+Version: 3.4.2
 Summary: Shipping API Python library (USPS, FedEx, UPS and more)
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: MIT License
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
```

### Comparing `shippo-3.4.1/src/shippo.egg-info/SOURCES.txt` & `shippo-3.4.2/src/shippo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 src/shippo/models/components/carrieraccountregistrationstatus.py
 src/shippo/models/components/carrieraccountservicelevel.py
 src/shippo/models/components/carrieraccountupscreaterequest.py
 src/shippo/models/components/carrieraccountupscreaterequestparameters.py
 src/shippo/models/components/carrieraccountuspscreaterequest.py
 src/shippo/models/components/carrieraccountwithextrainfo.py
 src/shippo/models/components/carrierparceltemplate.py
+src/shippo/models/components/carrierparceltemplatelist.py
 src/shippo/models/components/carriersenum.py
 src/shippo/models/components/cod.py
 src/shippo/models/components/connectexistingownaccountrequest.py
 src/shippo/models/components/customerreference.py
 src/shippo/models/components/customsdeclaration.py
 src/shippo/models/components/customsdeclarationb13afilingoptionenum.py
 src/shippo/models/components/customsdeclarationcontentstypeenum.py
@@ -142,14 +143,15 @@
 src/shippo/models/components/servicegroup.py
 src/shippo/models/components/servicegroupaccountandservicelevel.py
 src/shippo/models/components/servicegroupcreaterequest.py
 src/shippo/models/components/servicegrouptypeenum.py
 src/shippo/models/components/servicegroupupdaterequest.py
 src/shippo/models/components/servicelevel.py
 src/shippo/models/components/servicelevelenumset.py
+src/shippo/models/components/servicelevelwithparent.py
 src/shippo/models/components/shipment.py
 src/shippo/models/components/shipmentcreaterequest.py
 src/shippo/models/components/shipmentextra.py
 src/shippo/models/components/shipmentpaginatedlist.py
 src/shippo/models/components/shippoaccount.py
 src/shippo/models/components/shippoaccountpaginatedlist.py
 src/shippo/models/components/shippoaccountupdaterequest.py
@@ -157,18 +159,22 @@
 src/shippo/models/components/trackingstatus.py
 src/shippo/models/components/trackingstatusenum.py
 src/shippo/models/components/trackingstatuslocationbase.py
 src/shippo/models/components/trackingstatussubstatus.py
 src/shippo/models/components/tracksrequest.py
 src/shippo/models/components/transaction.py
 src/shippo/models/components/transactioncreaterequest.py
+src/shippo/models/components/transactioncreateresponse.py
 src/shippo/models/components/transactionpaginatedlist.py
 src/shippo/models/components/transactionstatusenum.py
 src/shippo/models/components/upsconnectexistingownaccountparameters.py
+src/shippo/models/components/upsreferencefields.py
 src/shippo/models/components/userparceltemplate.py
+src/shippo/models/components/userparceltemplatecreaterequest.py
+src/shippo/models/components/userparceltemplatelist.py
 src/shippo/models/components/userparceltemplateupdaterequest.py
 src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
 src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
 src/shippo/models/components/weightunitenum.py
 src/shippo/models/errors/__init__.py
 src/shippo/models/errors/initiateoauth2signin.py
 src/shippo/models/errors/sdkerror.py
```

