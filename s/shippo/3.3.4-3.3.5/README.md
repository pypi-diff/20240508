# Comparing `tmp/shippo-3.3.4.tar.gz` & `tmp/shippo-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shippo-3.3.4.tar", last modified: Fri May  3 17:39:53 2024, max compression
+gzip compressed data, was "shippo-3.3.5.tar", last modified: Wed May  8 01:22:00 2024, max compression
```

## Comparing `shippo-3.3.4.tar` & `shippo-3.3.5.tar`

### file list

```diff
@@ -1,257 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.217130 shippo-3.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    17793 2024-05-03 17:39:53.217130 shippo-3.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-03 17:39:44.000000 shippo-3.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 17:39:53.217130 shippo-3.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-03 17:39:44.000000 shippo-3.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.177130 shippo-3.3.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.181130 shippo-3.3.4/src/shippo/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.181130 shippo-3.3.4/src/shippo/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)    19356 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/batches.py
--rw-r--r--   0 runner    (1001) docker     (127)    27922 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/carrier_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/carrier_parcel_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/customs_declarations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/customs_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    10900 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/manifests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.181130 shippo-3.3.4/src/shippo/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.205130 shippo-3.3.4/src/shippo/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/addresscompletecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/addresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/addressimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/addresspaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/addressvalidationresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/addressvalidationresultsmessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/alcohol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/batchcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/batchshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/batchshipmentbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/batchshipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountdpddecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountfedexcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountupscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountuspscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrieraccountwithextrainfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/carriersenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/cod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/connectexistingownaccountrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customerreference.py
--rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsdeclarationcontentstypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsdeclarationcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsdeclarationeelpfcenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsdeclarationincotermenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsdeclarationnondeliveryoptionenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsdeclarationpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsexporteridentification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsinvoicedcharges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsitemcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customsitempaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/customstaxidentification.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/dangerousgoodslithiumbatteries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/dangerousgoodsobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/defaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/defaultparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/departmentnumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/distanceunitenum.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/dryice.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/errormessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/fedexconnectexistingownaccountparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/instanttransactioncreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/instanttransactioncreateresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/instanttransactionrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/insurance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/invoicenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/labelfiletypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/lineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/lineitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/liverate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/liveratecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/liveratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/manifestcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/manifestpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/objectstateenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/ordercreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/orderpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/orderstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/parcelcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/parcelextra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/parcelinsurance.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/parcelpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/parcelrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/parceltemplateenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/pickupbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/ponumber.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/ratemessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/ratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/refund.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/refundpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/refundrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/rmanumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/servicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/servicegroupaccountandservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/servicegroupcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/servicegrouptypeenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/servicegroupupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/servicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)    42151 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/servicelevelenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/shipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/shipmentcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/shipmentextra.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/shipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/shippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/shippoaccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/shippoaccountupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/trackingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/trackingstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/trackingstatuslocationbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/trackingstatussubstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/tracksrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/transactioncreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/transactionpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/transactionstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/upsconnectexistingownaccountparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/userparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/userparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/components/weightunitenum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.205130 shippo-3.3.4/src/shippo/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/errors/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.205130 shippo-3.3.4/src/shippo/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.213130 shippo-3.3.4/src/shippo/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/addshipmentstobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createliverate.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createpickup.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createtrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/createuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/deletedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/deleteservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/deleteuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getcarrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getcarrierregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getdefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/gettrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/gettransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/getuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/initiateoauth2signin.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listaddresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listcarrieraccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listcarrierparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listcustomsdeclarations.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listcustomsitems.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listmanifests.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listorders.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listparcels.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listrefunds.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listservicegroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listshipmentrates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listshipmentratesbycurrencycode.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listshipments.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listshippoaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listtransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/listuserparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/purchasebatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/registercarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/removeshipmentsfrombatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/updatecarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/updatedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/updateservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/updateshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/updateuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/models/operations/validateaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10829 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/pickups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15348 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/rates_at_checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/refunds.py
--rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/service_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11827 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/shipments.py
--rw-r--r--   0 runner    (1001) docker     (127)    14799 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/shippo_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8656 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/tracking_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    11058 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18766 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/user_parcel_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.213130 shippo-3.3.4/src/shippo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32651 2024-05-03 17:39:44.000000 shippo-3.3.4/src/shippo/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 17:39:53.181130 shippo-3.3.4/src/shippo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17793 2024-05-03 17:39:52.000000 shippo-3.3.4/src/shippo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-03 17:39:53.000000 shippo-3.3.4/src/shippo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 17:39:52.000000 shippo-3.3.4/src/shippo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-03 17:39:52.000000 shippo-3.3.4/src/shippo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 17:39:52.000000 shippo-3.3.4/src/shippo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.455736 shippo-3.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-05-08 01:22:00.455736 shippo-3.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-05-08 01:21:51.000000 shippo-3.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 01:22:00.455736 shippo-3.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-08 01:21:51.000000 shippo-3.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.415736 shippo-3.3.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.419736 shippo-3.3.5/src/shippo/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.423736 shippo-3.3.5/src/shippo/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14213 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19824 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28485 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/carrier_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/carrier_parcel_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/customs_declarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/customs_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11114 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/manifests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.423736 shippo-3.3.5/src/shippo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.443736 shippo-3.3.5/src/shippo/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)    10928 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/addresscompletecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/addresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/addressimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/addresspaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/addressvalidationresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/addressvalidationresultsmessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/batchcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/batchshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/batchshipmentbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/batchshipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountdpddecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountfedexcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountupscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountuspscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrieraccountwithextrainfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/carriersenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/cod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/connectexistingownaccountrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customerreference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9857 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsdeclarationcontentstypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsdeclarationcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsdeclarationeelpfcenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsdeclarationincotermenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsdeclarationnondeliveryoptionenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsdeclarationpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsexporteridentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsinvoicedcharges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsitemcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customsitempaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/customstaxidentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/dangerousgoodslithiumbatteries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/dangerousgoodsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/defaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/defaultparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/departmentnumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/distanceunitenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/dryice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/errormessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/fedexconnectexistingownaccountparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/instanttransactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/instanttransactioncreateresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/instanttransactionrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/insurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/invoicenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/labelfiletypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/lineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/lineitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/liverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/liveratecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/liveratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/manifestcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/manifestpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/objectstateenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/ordercreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/orderpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/orderstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/parcelcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/parcelextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/parcelinsurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/parcelpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/parcelrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/parceltemplateenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/pickupbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/ponumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/ratemessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/ratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/refundpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/refundrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/rmanumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/servicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/servicegroupaccountandservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/servicegroupcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/servicegrouptypeenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/servicegroupupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/servicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42151 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/servicelevelenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/shipmentcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/shipmentextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/shipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/shippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/shippoaccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/shippoaccountupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/trackingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/trackingstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/trackingstatuslocationbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/trackingstatussubstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/tracksrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/transactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/transactionpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/transactionstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/upsconnectexistingownaccountparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/userparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/userparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/components/weightunitenum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.443736 shippo-3.3.5/src/shippo/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/errors/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.443736 shippo-3.3.5/src/shippo/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.451736 shippo-3.3.5/src/shippo/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/addshipmentstobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createliverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createpickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createtrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/createuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/deletedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/deleteservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/deleteuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getcarrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getcarrierregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getdefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/gettrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/gettransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/getuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listaddresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listcarrieraccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listcarrierparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listcustomsdeclarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listcustomsitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listmanifests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listorders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listparcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listrefunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listservicegroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listshipmentrates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listshipmentratesbycurrencycode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listshipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listshippoaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/listuserparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/purchasebatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/registercarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/removeshipmentsfrombatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/updatecarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/updatedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/updateservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/updateshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/updateuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/models/operations/validateaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11426 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/pickups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11708 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15562 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/rates_at_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/refunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14022 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12041 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/shipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15058 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/shippo_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/tracking_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11272 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19025 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/user_parcel_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.455736 shippo-3.3.5/src/shippo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32651 2024-05-08 01:21:51.000000 shippo-3.3.5/src/shippo/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 01:22:00.423736 shippo-3.3.5/src/shippo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17808 2024-05-08 01:22:00.000000 shippo-3.3.5/src/shippo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-05-08 01:22:00.000000 shippo-3.3.5/src/shippo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 01:22:00.000000 shippo-3.3.5/src/shippo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-08 01:22:00.000000 shippo-3.3.5/src/shippo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 01:22:00.000000 shippo-3.3.5/src/shippo.egg-info/top_level.txt
```

### Comparing `shippo-3.3.4/PKG-INFO` & `shippo-3.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.3.4
-Summary: Python Client SDK Generated by Speakeasy
+Version: 3.3.5
+Summary: Shipping API Python library (USPS, FedEx, UPS and more)
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
```

### Comparing `shippo-3.3.4/README.md` & `shippo-3.3.5/README.md`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/setup.py` & `shippo-3.3.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,17 +15,17 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='shippo',
-    version='3.3.4',
+    version='3.3.5',
     author='Shippo',
-    description='Python Client SDK Generated by Speakeasy',
+    description='Shipping API Python library (USPS, FedEx, UPS and more)',
     url='https://github.com/goshippo/shippo-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
         "certifi>=2023.7.22",
         "charset-normalizer>=3.2.0",
```

### Comparing `shippo-3.3.4/src/shippo/_hooks/registration.py` & `shippo-3.3.5/src/shippo/_hooks/registration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Union, Tuple
+from typing import Union
 
 import json
 import requests
 
-from .types import Hooks, BeforeRequestHook, BeforeRequestContext, SDKInitHook, AfterSuccessHook, AfterSuccessContext
+from .types import Hooks, BeforeRequestHook, BeforeRequestContext, AfterSuccessHook, AfterSuccessContext
 
 
 # This file is only ever generated once on the first generation and then is free to be modified.
 # Any hooks you wish to add should be registered in the init_hooks function. Feel free to define them
 # in this file or in separate files in the hooks folder.
```

### Comparing `shippo-3.3.4/src/shippo/_hooks/sdkhooks.py` & `shippo-3.3.5/src/shippo/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/_hooks/types.py` & `shippo-3.3.5/src/shippo/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/addresses.py` & `shippo-3.3.5/src/shippo/addresses.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,28 +65,29 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.AddressPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, request: Optional[components.AddressCreateRequest]) -> components.Address:
+    def create(self, request: components.AddressCreateRequest) -> components.Address:
         r"""Create a new address
         Creates a new address object. You can use address objects to create new shipments, calculate rates, and to create orders.
         """
         hook_ctx = HookContext(operation_id='CreateAddress', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         _globals = operations.CreateAddressGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
@@ -97,17 +98,19 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[components.AddressCreateRequest], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, components.AddressCreateRequest, "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -127,14 +130,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Address])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -190,14 +194,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Address])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -253,14 +258,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Address])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `shippo-3.3.4/src/shippo/batches.py` & `shippo-3.3.5/src/shippo/batches.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, request: Optional[components.BatchCreateRequest]) -> components.Batch:
+    def create(self, request: components.BatchCreateRequest) -> components.Batch:
         r"""Create a batch
         Creates a new batch object for purchasing shipping labels for many shipments at once. Batches are created asynchronously. This means that the API response won't include your batch shipments yet. You need to retrieve the batch later to verify that all batch shipments are valid.
         """
         hook_ctx = HookContext(operation_id='CreateBatch', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         _globals = operations.CreateBatchGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
@@ -41,17 +41,19 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[components.BatchCreateRequest], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, components.BatchCreateRequest, "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -71,14 +73,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Batch])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -137,28 +140,29 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Batch])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def add_shipments(self, batch_id: str, request_body: Optional[List[components.BatchShipmentBase]] = None) -> components.Batch:
+    def add_shipments(self, batch_id: str, request_body: List[components.BatchShipmentBase]) -> components.Batch:
         r"""Add shipments to a batch
         Adds batch shipments to an existing batch.
         """
         hook_ctx = HookContext(operation_id='AddShipmentsToBatch', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.AddShipmentsToBatchRequest(
             batch_id=batch_id,
             request_body=request_body,
@@ -174,17 +178,19 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, operations.AddShipmentsToBatchRequest, "request_body", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.AddShipmentsToBatchRequest, "request_body", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -204,14 +210,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Batch])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -270,28 +277,29 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Batch])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def remove_shipments(self, batch_id: str, request_body: Optional[List[str]] = None) -> components.Batch:
+    def remove_shipments(self, batch_id: str, request_body: List[str]) -> components.Batch:
         r"""Remove shipments from a batch
         Removes shipments from an existing batch shipment.
         """
         hook_ctx = HookContext(operation_id='RemoveShipmentsFromBatch', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.RemoveShipmentsFromBatchRequest(
             batch_id=batch_id,
             request_body=request_body,
@@ -307,17 +315,19 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, operations.RemoveShipmentsFromBatchRequest, "request_body", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.RemoveShipmentsFromBatchRequest, "request_body", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -337,14 +347,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Batch])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `shippo-3.3.4/src/shippo/carrier_accounts.py` & `shippo-3.3.5/src/shippo/carrier_accounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,28 +65,29 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CarrierAccountPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, request: Optional[components.ConnectExistingOwnAccountRequest]) -> components.CarrierAccount:
+    def create(self, request: components.ConnectExistingOwnAccountRequest) -> components.CarrierAccount:
         r"""Create a new carrier account
         Creates a new carrier account or connects an existing carrier account to the Shippo account.
         """
         hook_ctx = HookContext(operation_id='CreateCarrierAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         _globals = operations.CreateCarrierAccountGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
@@ -97,17 +98,19 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[components.ConnectExistingOwnAccountRequest], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, components.ConnectExistingOwnAccountRequest, "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -127,14 +130,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CarrierAccount])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -190,14 +194,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CarrierAccount])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -257,14 +262,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CarrierAccount])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -326,28 +332,31 @@
         
         res = operations.InitiateOauth2SigninResponse(headers=None)
         
         if http_res.status_code == 302:
             res.headers = http_res.headers
             
         elif http_res.status_code == 400:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.InitiateOauth2SigninResponseBody)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 401:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.InitiateOauth2SigninCarrierAccountsResponseBody)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 404:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.InitiateOauth2SigninCarrierAccountsResponseResponseBody)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -355,15 +364,15 @@
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
     
-    def register(self, request: Optional[Union[components.CarrierAccountCanadaPostCreateRequest, components.CarrierAccountChronopostCreateRequest, components.CarrierAccountColissimoCreateRequest, components.CarrierAccountCorreosCreateRequest, components.CarrierAccountDeutschePostCreateRequest, components.CarrierAccountDHLExpressCreateRequest, components.CarrierAccountDpdDeCreateRequest, components.CarrierAccountDPDUKCreateRequest, components.CarrierAccountFedExCreateRequest, components.CarrierAccountHermesUKCreateRequest, components.CarrierAccountMondialRelayCreateRequest, components.CarrierAccountPosteItalianeCreateRequest, components.CarrierAccountUPSCreateRequest, components.CarrierAccountUSPSCreateRequest]]) -> components.CarrierAccount:
+    def register(self, request: Union[components.CarrierAccountCanadaPostCreateRequest, components.CarrierAccountChronopostCreateRequest, components.CarrierAccountColissimoCreateRequest, components.CarrierAccountCorreosCreateRequest, components.CarrierAccountDeutschePostCreateRequest, components.CarrierAccountDHLExpressCreateRequest, components.CarrierAccountDpdDeCreateRequest, components.CarrierAccountDPDUKCreateRequest, components.CarrierAccountFedExCreateRequest, components.CarrierAccountHermesUKCreateRequest, components.CarrierAccountMondialRelayCreateRequest, components.CarrierAccountPosteItalianeCreateRequest, components.CarrierAccountUPSCreateRequest, components.CarrierAccountUSPSCreateRequest]) -> components.CarrierAccount:
         r"""Add a Shippo carrier account
         Adds a Shippo carrier account
         """
         hook_ctx = HookContext(operation_id='RegisterCarrierAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         _globals = operations.RegisterCarrierAccountGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
@@ -374,17 +383,19 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[Union[components.CarrierAccountCanadaPostCreateRequest, components.CarrierAccountChronopostCreateRequest, components.CarrierAccountColissimoCreateRequest, components.CarrierAccountCorreosCreateRequest, components.CarrierAccountDeutschePostCreateRequest, components.CarrierAccountDHLExpressCreateRequest, components.CarrierAccountDpdDeCreateRequest, components.CarrierAccountDPDUKCreateRequest, components.CarrierAccountFedExCreateRequest, components.CarrierAccountHermesUKCreateRequest, components.CarrierAccountMondialRelayCreateRequest, components.CarrierAccountPosteItalianeCreateRequest, components.CarrierAccountUPSCreateRequest, components.CarrierAccountUSPSCreateRequest]], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, Union[components.CarrierAccountCanadaPostCreateRequest, components.CarrierAccountChronopostCreateRequest, components.CarrierAccountColissimoCreateRequest, components.CarrierAccountCorreosCreateRequest, components.CarrierAccountDeutschePostCreateRequest, components.CarrierAccountDHLExpressCreateRequest, components.CarrierAccountDpdDeCreateRequest, components.CarrierAccountDPDUKCreateRequest, components.CarrierAccountFedExCreateRequest, components.CarrierAccountHermesUKCreateRequest, components.CarrierAccountMondialRelayCreateRequest, components.CarrierAccountPosteItalianeCreateRequest, components.CarrierAccountUPSCreateRequest, components.CarrierAccountUSPSCreateRequest], "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -404,14 +415,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CarrierAccount])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -467,14 +479,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CarrierAccountRegistrationStatus])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `shippo-3.3.4/src/shippo/carrier_parcel_templates.py` & `shippo-3.3.5/src/shippo/carrier_parcel_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[components.CarrierParcelTemplate]])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -129,14 +130,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CarrierParcelTemplate])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `shippo-3.3.4/src/shippo/customs_declarations.py` & `shippo-3.3.5/src/shippo/customs_declarations.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,28 +66,29 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CustomsDeclarationPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, request: Optional[components.CustomsDeclarationCreateRequest]) -> components.CustomsDeclaration:
+    def create(self, request: components.CustomsDeclarationCreateRequest) -> components.CustomsDeclaration:
         r"""Create a new customs declaration
         Creates a new customs declaration object
         """
         hook_ctx = HookContext(operation_id='CreateCustomsDeclaration', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         _globals = operations.CreateCustomsDeclarationGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
@@ -98,17 +99,19 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[components.CustomsDeclarationCreateRequest], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, components.CustomsDeclarationCreateRequest, "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -128,14 +131,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CustomsDeclaration])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -192,14 +196,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CustomsDeclaration])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `shippo-3.3.4/src/shippo/customs_items.py` & `shippo-3.3.5/src/shippo/parcels.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,42 +3,46 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
 from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
-class CustomsItems:
-    r"""Customs declarations are relevant information, including one or multiple customs items, you need to provide for customs clearance for your international shipments.
-    <SchemaDefinition schemaRef=\"#/components/schemas/CustomsItem\"/>
+class Parcels:
+    r"""A parcel is an item you are shipping. The parcel object includes details about its physical make-up of the parcel. It includes dimensions and weight that Shippo uses to calculate rates.
+    <SchemaDefinition schemaRef=\"#/components/schemas/Parcel\"/>
+
+    # Parcel Extras
+    The following values are supported for the `extra` field of the parcel object.
+    <SchemaDefinition schemaRef=\"#/components/schemas/ParcelExtra\"/>
     """
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def list(self, page: Optional[int] = None, results: Optional[int] = None) -> components.CustomsItemPaginatedList:
-        r"""List all customs items
-        Returns a list all customs items objects.
+    def list(self, page: Optional[int] = None, results: Optional[int] = None) -> components.ParcelPaginatedList:
+        r"""List all parcels
+        Returns a list of all parcel objects.
         """
-        hook_ctx = HookContext(operation_id='ListCustomsItems', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.ListCustomsItemsRequest(
+        hook_ctx = HookContext(operation_id='ListParcels', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.ListParcelsRequest(
             page=page,
             results=results,
         )
         
-        _globals = operations.ListCustomsItemsGlobals(
+        _globals = operations.ListParcelsGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/customs/items', request, _globals)
+        url = utils.generate_url(base_url, '/parcels', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -65,49 +69,52 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsItemPaginatedList])
+                out = utils.unmarshal_json(http_res.text, Optional[components.ParcelPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, request: Optional[components.CustomsItemCreateRequest]) -> components.CustomsItem:
-        r"""Create a new customs item
-        Creates a new customs item object.
+    def create(self, request: components.ParcelRequest) -> components.Parcel:
+        r"""Create a new parcel
+        Creates a new parcel object.
         """
-        hook_ctx = HookContext(operation_id='CreateCustomsItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.CreateCustomsItemGlobals(
+        hook_ctx = HookContext(operation_id='CreateParcel', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.CreateParcelGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/customs/items', request, _globals)
+        url = utils.generate_url(base_url, '/parcels', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[components.CustomsItemCreateRequest], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, components.ParcelRequest, "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -127,44 +134,44 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsItem])
+                out = utils.unmarshal_json(http_res.text, Optional[components.Parcel])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def get(self, customs_item_id: str, page: Optional[int] = None) -> components.CustomsItem:
-        r"""Retrieve a customs item
-        Returns an existing customs item using an object ID
+    def get(self, parcel_id: str) -> components.Parcel:
+        r"""Retrieve an existing parcel
+        Returns parcel details using an existing parcel object ID (this will not return parcel details associated with un-purchased shipment/rate parcel object IDs).
         """
-        hook_ctx = HookContext(operation_id='GetCustomsItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetCustomsItemRequest(
-            customs_item_id=customs_item_id,
-            page=page,
+        hook_ctx = HookContext(operation_id='GetParcel', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetParcelRequest(
+            parcel_id=parcel_id,
         )
         
-        _globals = operations.GetCustomsItemGlobals(
+        _globals = operations.GetParcelGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/customs/items/{CustomsItemId}', request, _globals)
+        url = utils.generate_url(base_url, '/parcels/{ParcelId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -191,16 +198,17 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsItem])
+                out = utils.unmarshal_json(http_res.text, Optional[components.Parcel])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `shippo-3.3.4/src/shippo/debug.py` & `shippo-3.3.5/src/shippo/debug.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/manifests.py` & `shippo-3.3.5/src/shippo/manifests.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,28 +71,29 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.ManifestPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, request: Optional[components.ManifestCreateRequest]) -> components.Manifest:
+    def create(self, request: components.ManifestCreateRequest) -> components.Manifest:
         r"""Create a new manifest
         Creates a new manifest object.
         """
         hook_ctx = HookContext(operation_id='CreateManifest', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         _globals = operations.CreateManifestGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
@@ -103,17 +104,19 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[components.ManifestCreateRequest], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, components.ManifestCreateRequest, "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -133,14 +136,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Manifest])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -196,14 +200,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Manifest])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `shippo-3.3.4/src/shippo/models/components/__init__.py` & `shippo-3.3.5/src/shippo/models/components/__init__.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/address.py` & `shippo-3.3.5/src/shippo/models/components/address.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/addresscompletecreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/addresscompletecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/addresscreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/addresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/addressimporter.py` & `shippo-3.3.5/src/shippo/models/components/addressimporter.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/addresspaginatedlist.py` & `shippo-3.3.5/src/shippo/models/components/addresspaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/addressvalidationresults.py` & `shippo-3.3.5/src/shippo/models/components/addressvalidationresults.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/addressvalidationresultsmessage.py` & `shippo-3.3.5/src/shippo/models/components/addressvalidationresultsmessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/alcohol.py` & `shippo-3.3.5/src/shippo/models/components/alcohol.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/batch.py` & `shippo-3.3.5/src/shippo/models/components/batch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/batchcreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/batchcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/batchshipment.py` & `shippo-3.3.5/src/shippo/models/components/batchshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/batchshipmentbase.py` & `shippo-3.3.5/src/shippo/models/components/batchshipmentbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/batchshipmentpaginatedlist.py` & `shippo-3.3.5/src/shippo/models/components/batchshipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/billing.py` & `shippo-3.3.5/src/shippo/models/components/billing.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccount.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountbase.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountchronopostcreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountchronopostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountcolissimocreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountcolissimocreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountcorreoscreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountcorreoscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountdpddecreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountdpddecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountdpdukcreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountdpdukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountfedexcreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountfedexcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccounthermesukcreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccounthermesukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountmondialrelaycreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountpaginatedlist.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountregistrationstatus.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountservicelevel.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountupscreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountupscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountupscreaterequestparameters.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountupscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountuspscreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountuspscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrieraccountwithextrainfo.py` & `shippo-3.3.5/src/shippo/models/components/carrieraccountwithextrainfo.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carrierparceltemplate.py` & `shippo-3.3.5/src/shippo/models/components/carrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/carriersenum.py` & `shippo-3.3.5/src/shippo/models/components/carriersenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/cod.py` & `shippo-3.3.5/src/shippo/models/components/cod.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/connectexistingownaccountrequest.py` & `shippo-3.3.5/src/shippo/models/components/connectexistingownaccountrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/customerreference.py` & `shippo-3.3.5/src/shippo/models/components/customerreference.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/customsdeclaration.py` & `shippo-3.3.5/src/shippo/models/components/customsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py` & `shippo-3.3.5/src/shippo/models/components/customsdeclarationb13afilingoptionenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/customsdeclarationcreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/customsdeclarationcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/customsdeclarationeelpfcenum.py` & `shippo-3.3.5/src/shippo/models/components/customsdeclarationeelpfcenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/customsdeclarationincotermenum.py` & `shippo-3.3.5/src/shippo/models/components/customsdeclarationincotermenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/customsdeclarationpaginatedlist.py` & `shippo-3.3.5/src/shippo/models/components/customsdeclarationpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/customsexporteridentification.py` & `shippo-3.3.5/src/shippo/models/components/customsexporteridentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/customsinvoicedcharges.py` & `shippo-3.3.5/src/shippo/models/components/customsinvoicedcharges.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/customsitem.py` & `shippo-3.3.5/src/shippo/models/components/customsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/customsitemcreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/customsitemcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/customsitempaginatedlist.py` & `shippo-3.3.5/src/shippo/models/components/customsitempaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/customstaxidentification.py` & `shippo-3.3.5/src/shippo/models/components/customstaxidentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py` & `shippo-3.3.5/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/dangerousgoodslithiumbatteries.py` & `shippo-3.3.5/src/shippo/models/components/dangerousgoodslithiumbatteries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/dangerousgoodsobject.py` & `shippo-3.3.5/src/shippo/models/components/dangerousgoodsobject.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/defaultparceltemplate.py` & `shippo-3.3.5/src/shippo/models/components/defaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/defaultparceltemplateupdaterequest.py` & `shippo-3.3.5/src/shippo/models/components/defaultparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/departmentnumber.py` & `shippo-3.3.5/src/shippo/models/components/departmentnumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/dryice.py` & `shippo-3.3.5/src/shippo/models/components/dryice.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/errormessage.py` & `shippo-3.3.5/src/shippo/models/components/errormessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/fedexconnectexistingownaccountparameters.py` & `shippo-3.3.5/src/shippo/models/components/fedexconnectexistingownaccountparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/instanttransactioncreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/instanttransactioncreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/instanttransactioncreateresponse.py` & `shippo-3.3.5/src/shippo/models/components/instanttransactioncreateresponse.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/instanttransactionrate.py` & `shippo-3.3.5/src/shippo/models/components/instanttransactionrate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/insurance.py` & `shippo-3.3.5/src/shippo/models/components/insurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/invoicenumber.py` & `shippo-3.3.5/src/shippo/models/components/invoicenumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/labelfiletypeenum.py` & `shippo-3.3.5/src/shippo/models/components/labelfiletypeenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/lineitem.py` & `shippo-3.3.5/src/shippo/models/components/lineitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/lineitembase.py` & `shippo-3.3.5/src/shippo/models/components/lineitembase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/liverate.py` & `shippo-3.3.5/src/shippo/models/components/liverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/liveratecreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/liveratecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/liveratepaginatedlist.py` & `shippo-3.3.5/src/shippo/models/components/liveratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/location.py` & `shippo-3.3.5/src/shippo/models/components/location.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/manifest.py` & `shippo-3.3.5/src/shippo/models/components/manifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/manifestcreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/manifestcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/manifestpaginatedlist.py` & `shippo-3.3.5/src/shippo/models/components/manifestpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/order.py` & `shippo-3.3.5/src/shippo/models/components/order.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/ordercreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/ordercreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/orderpaginatedlist.py` & `shippo-3.3.5/src/shippo/models/components/orderpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/orderstatusenum.py` & `shippo-3.3.5/src/shippo/models/components/orderstatusenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/parcel.py` & `shippo-3.3.5/src/shippo/models/components/parcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/parcelcreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/parcelcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/parcelextra.py` & `shippo-3.3.5/src/shippo/models/components/parcelextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/parcelinsurance.py` & `shippo-3.3.5/src/shippo/models/components/parcelinsurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/parcelpaginatedlist.py` & `shippo-3.3.5/src/shippo/models/components/parcelpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/parcelrequest.py` & `shippo-3.3.5/src/shippo/models/components/parcelrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/parceltemplateenumset.py` & `shippo-3.3.5/src/shippo/models/components/parceltemplateenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/pickup.py` & `shippo-3.3.5/src/shippo/models/components/pickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/pickupbase.py` & `shippo-3.3.5/src/shippo/models/components/pickupbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/ponumber.py` & `shippo-3.3.5/src/shippo/models/components/ponumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/rate.py` & `shippo-3.3.5/src/shippo/models/components/rate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/ratemessage.py` & `shippo-3.3.5/src/shippo/models/components/ratemessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/ratepaginatedlist.py` & `shippo-3.3.5/src/shippo/models/components/ratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/refund.py` & `shippo-3.3.5/src/shippo/models/components/refund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/refundpaginatedlist.py` & `shippo-3.3.5/src/shippo/models/components/refundpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/refundrequestbody.py` & `shippo-3.3.5/src/shippo/models/components/refundrequestbody.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/rmanumber.py` & `shippo-3.3.5/src/shippo/models/components/rmanumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/servicegroup.py` & `shippo-3.3.5/src/shippo/models/components/servicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/servicegroupaccountandservicelevel.py` & `shippo-3.3.5/src/shippo/models/components/servicegroupaccountandservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/servicegroupcreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/servicegroupcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/servicegrouptypeenum.py` & `shippo-3.3.5/src/shippo/models/components/servicegrouptypeenum.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/servicegroupupdaterequest.py` & `shippo-3.3.5/src/shippo/models/components/servicegroupupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/servicelevel.py` & `shippo-3.3.5/src/shippo/models/components/servicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/servicelevelenumset.py` & `shippo-3.3.5/src/shippo/models/components/servicelevelenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/shipment.py` & `shippo-3.3.5/src/shippo/models/components/shipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/shipmentcreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/shipmentcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/shipmentextra.py` & `shippo-3.3.5/src/shippo/models/components/shipmentextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/shipmentpaginatedlist.py` & `shippo-3.3.5/src/shippo/models/components/shipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/shippoaccount.py` & `shippo-3.3.5/src/shippo/models/components/shippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/shippoaccountpaginatedlist.py` & `shippo-3.3.5/src/shippo/models/components/shippoaccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/shippoaccountupdaterequest.py` & `shippo-3.3.5/src/shippo/models/components/shippoaccountupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/track.py` & `shippo-3.3.5/src/shippo/models/components/track.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,35 +11,35 @@
 from shippo import utils
 from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Track:
-    address_from: TrackingStatusLocationBase = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_from') }})
-    r"""The sender address with city, state, zip and country information."""
     carrier: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('carrier') }})
     r"""Name of the carrier of the shipment to track. See <a href=\\"#tag/Carriers\\">Carriers</a>."""
     messages: List[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('messages') }})
-    servicelevel: ServiceLevel = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('servicelevel') }})
-    r"""Contains details regarding the service level for the given rate."""
     tracking_history: List[TrackingStatus] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_history') }})
     r"""A list of tracking events, following the same structure as <code>tracking_status</code>.
     It contains a full history of all tracking statuses, starting with the earlier tracking event first.
     """
     tracking_number: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_number') }})
     r"""Tracking number to track."""
+    address_from: Optional[TrackingStatusLocationBase] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_from'), 'exclude': lambda f: f is None }})
+    r"""The sender address with city, state, zip and country information."""
     address_to: Optional[TrackingStatusLocationBase] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address_to'), 'exclude': lambda f: f is None }})
     r"""The recipient address with city, state, zip and country information."""
     eta: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eta'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""The estimated time of arrival according to the carrier, this might be updated by carriers during the life of the shipment."""
     metadata: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""A string of up to 100 characters that can be filled with any additional information you want to attach to the object."""
     original_eta: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('original_eta'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'exclude': lambda f: f is None }})
     r"""The estimated time of arrival according to the carrier at the time the shipment first entered the system."""
+    servicelevel: Optional[ServiceLevel] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('servicelevel'), 'exclude': lambda f: f is None }})
+    r"""Contains details regarding the service level for the given rate."""
     tracking_status: Optional[TrackingStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_status'), 'exclude': lambda f: f is None }})
     r"""The latest tracking information of this shipment."""
     transaction: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transaction'), 'exclude': lambda f: f is None }})
     r"""The <code>object_id</code> of the transaction associated with this tracking object.
     This field is visible only to the object owner of the transaction.
     """
```

### Comparing `shippo-3.3.4/src/shippo/models/components/trackingstatus.py` & `shippo-3.3.5/src/shippo/models/components/trackingstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/trackingstatuslocationbase.py` & `shippo-3.3.5/src/shippo/models/components/trackingstatuslocationbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/trackingstatussubstatus.py` & `shippo-3.3.5/src/shippo/models/components/trackingstatussubstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/tracksrequest.py` & `shippo-3.3.5/src/shippo/models/components/tracksrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/transaction.py` & `shippo-3.3.5/src/shippo/models/components/transaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/transactioncreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/transactioncreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/transactionpaginatedlist.py` & `shippo-3.3.5/src/shippo/models/components/transactionpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/upsconnectexistingownaccountparameters.py` & `shippo-3.3.5/src/shippo/models/components/upsconnectexistingownaccountparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/userparceltemplate.py` & `shippo-3.3.5/src/shippo/models/components/userparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/userparceltemplateupdaterequest.py` & `shippo-3.3.5/src/shippo/models/components/userparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py` & `shippo-3.3.5/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/errors/initiateoauth2signin.py` & `shippo-3.3.5/src/shippo/models/errors/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/errors/sdkerror.py` & `shippo-3.3.5/src/shippo/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/__init__.py` & `shippo-3.3.5/src/shippo/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/addshipmentstobatch.py` & `shippo-3.3.5/src/shippo/models/operations/addshipmentstobatch.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,11 +14,11 @@
 
 
 
 @dataclasses.dataclass
 class AddShipmentsToBatchRequest:
     batch_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'BatchId', 'style': 'simple', 'explode': False }})
     r"""Object ID of the batch"""
-    request_body: Optional[List[components_batchshipmentbase.BatchShipmentBase]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    request_body: List[components_batchshipmentbase.BatchShipmentBase] = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     r"""Array of shipments to add to the batch"""
```

### Comparing `shippo-3.3.4/src/shippo/models/operations/deletedefaultparceltemplate.py` & `shippo-3.3.5/src/shippo/models/operations/deletedefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/deleteservicegroup.py` & `shippo-3.3.5/src/shippo/models/operations/deleteservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/deleteuserparceltemplate.py` & `shippo-3.3.5/src/shippo/models/operations/deleteuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/getaddress.py` & `shippo-3.3.5/src/shippo/models/operations/getaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/getbatch.py` & `shippo-3.3.5/src/shippo/models/operations/getbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/getcarrieraccount.py` & `shippo-3.3.5/src/shippo/models/operations/getcarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/getcarrierparceltemplate.py` & `shippo-3.3.5/src/shippo/models/operations/getcarrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/getcarrierregistrationstatus.py` & `shippo-3.3.5/src/shippo/models/operations/getcarrierregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/getcustomsdeclaration.py` & `shippo-3.3.5/src/shippo/models/operations/getcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/getcustomsitem.py` & `shippo-3.3.5/src/shippo/models/operations/getcustomsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/getdefaultparceltemplate.py` & `shippo-3.3.5/src/shippo/models/operations/getdefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/getmanifest.py` & `shippo-3.3.5/src/shippo/models/operations/getmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/getorder.py` & `shippo-3.3.5/src/shippo/models/operations/getorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/getparcel.py` & `shippo-3.3.5/src/shippo/models/operations/getparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/getrate.py` & `shippo-3.3.5/src/shippo/models/operations/getrate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/getrefund.py` & `shippo-3.3.5/src/shippo/models/operations/getrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/getshipment.py` & `shippo-3.3.5/src/shippo/models/operations/getshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/getshippoaccount.py` & `shippo-3.3.5/src/shippo/models/operations/getshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/gettrack.py` & `shippo-3.3.5/src/shippo/models/operations/gettrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/gettransaction.py` & `shippo-3.3.5/src/shippo/models/operations/gettransaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/getuserparceltemplate.py` & `shippo-3.3.5/src/shippo/models/operations/getuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/initiateoauth2signin.py` & `shippo-3.3.5/src/shippo/models/operations/initiateoauth2signin.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/listaddresses.py` & `shippo-3.3.5/src/shippo/models/operations/listaddresses.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/listcarrieraccounts.py` & `shippo-3.3.5/src/shippo/models/operations/listcarrieraccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/listcarrierparceltemplates.py` & `shippo-3.3.5/src/shippo/models/operations/listcarrierparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/listcustomsdeclarations.py` & `shippo-3.3.5/src/shippo/models/operations/listcustomsdeclarations.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/listcustomsitems.py` & `shippo-3.3.5/src/shippo/models/operations/listcustomsitems.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/listmanifests.py` & `shippo-3.3.5/src/shippo/models/operations/listmanifests.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/listorders.py` & `shippo-3.3.5/src/shippo/models/operations/listorders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/listparcels.py` & `shippo-3.3.5/src/shippo/models/operations/listparcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/listservicegroups.py` & `shippo-3.3.5/src/shippo/models/operations/listservicegroups.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/listshipmentrates.py` & `shippo-3.3.5/src/shippo/models/operations/listshipmentrates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/listshipmentratesbycurrencycode.py` & `shippo-3.3.5/src/shippo/models/operations/listshipmentratesbycurrencycode.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/listshipments.py` & `shippo-3.3.5/src/shippo/models/operations/listshipments.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/listshippoaccounts.py` & `shippo-3.3.5/src/shippo/models/operations/listshippoaccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/listtransactions.py` & `shippo-3.3.5/src/shippo/models/operations/listtransactions.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/listuserparceltemplates.py` & `shippo-3.3.5/src/shippo/models/operations/listuserparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/purchasebatch.py` & `shippo-3.3.5/src/shippo/models/operations/purchasebatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/removeshipmentsfrombatch.py` & `shippo-3.3.5/src/shippo/models/operations/removeshipmentsfrombatch.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,11 +13,11 @@
 
 
 
 @dataclasses.dataclass
 class RemoveShipmentsFromBatchRequest:
     batch_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'BatchId', 'style': 'simple', 'explode': False }})
     r"""Object ID of the batch"""
-    request_body: Optional[List[str]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    request_body: List[str] = dataclasses.field(metadata={'request': { 'media_type': 'application/json' }})
     r"""Array of shipments object ids to remove from the batch"""
```

### Comparing `shippo-3.3.4/src/shippo/models/operations/updatecarrieraccount.py` & `shippo-3.3.5/src/shippo/models/operations/updatecarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/updateshippoaccount.py` & `shippo-3.3.5/src/shippo/models/operations/updateshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/updateuserparceltemplate.py` & `shippo-3.3.5/src/shippo/models/operations/updateuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/models/operations/validateaddress.py` & `shippo-3.3.5/src/shippo/models/operations/validateaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/orders.py` & `shippo-3.3.5/src/shippo/orders.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,28 +76,29 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.OrderPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, request: Optional[components.OrderCreateRequest]) -> components.Order:
+    def create(self, request: components.OrderCreateRequest) -> components.Order:
         r"""Create a new order
         Creates a new order object.
         """
         hook_ctx = HookContext(operation_id='CreateOrder', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         _globals = operations.CreateOrderGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
@@ -108,17 +109,19 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[components.OrderCreateRequest], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, components.OrderCreateRequest, "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -138,14 +141,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Order])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -201,14 +205,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Order])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `shippo-3.3.4/src/shippo/parcels.py` & `shippo-3.3.5/src/shippo/refunds.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,60 +3,61 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
 from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
-class Parcels:
-    r"""A parcel is an item you are shipping. The parcel object includes details about its physical make-up of the parcel. It includes dimensions and weight that Shippo uses to calculate rates.
-    <SchemaDefinition schemaRef=\"#/components/schemas/Parcel\"/>
-
-    # Parcel Extras
-    The following values are supported for the `extra` field of the parcel object.
-    <SchemaDefinition schemaRef=\"#/components/schemas/ParcelExtra\"/>
+class Refunds:
+    r"""Refunds are reimbursements for successfully created but unused shipping labels or other charges.
+    <SchemaDefinition schemaRef=\"#/components/schemas/Refund\"/>
     """
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def list(self, page: Optional[int] = None, results: Optional[int] = None) -> components.ParcelPaginatedList:
-        r"""List all parcels
-        Returns a list of all parcel objects.
+    def create(self, transaction: str, async_: Optional[bool] = None) -> components.Refund:
+        r"""Create a refund
+        Creates a new refund object.
         """
-        hook_ctx = HookContext(operation_id='ListParcels', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.ListParcelsRequest(
-            page=page,
-            results=results,
+        hook_ctx = HookContext(operation_id='CreateRefund', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = components.RefundRequestBody(
+            transaction=transaction,
+            async_=async_,
         )
         
-        _globals = operations.ListParcelsGlobals(
+        _globals = operations.CreateRefundGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/parcels', request, _globals)
+        url = utils.generate_url(base_url, '/refunds', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, components.RefundRequestBody, "request", False, False, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -68,57 +69,58 @@
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
-        if http_res.status_code == 200:
+        if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.ParcelPaginatedList])
+                out = utils.unmarshal_json(http_res.text, Optional[components.Refund])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, request: Optional[components.ParcelRequest]) -> components.Parcel:
-        r"""Create a new parcel
-        Creates a new parcel object.
+    def list(self) -> components.RefundPaginatedList:
+        r"""List all refunds
+        Returns a list all refund objects.
         """
-        hook_ctx = HookContext(operation_id='CreateParcel', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        _globals = operations.CreateParcelGlobals(
+        hook_ctx = HookContext(operation_id='ListRefunds', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.ListRefundsRequest(
+        )
+        
+        _globals = operations.ListRefundsGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/parcels', request, _globals)
+        url = utils.generate_url(base_url, '/refunds/', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[components.ParcelRequest], "request", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -130,44 +132,45 @@
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
-        if http_res.status_code == 201:
+        if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Parcel])
+                out = utils.unmarshal_json(http_res.text, Optional[components.RefundPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def get(self, parcel_id: str) -> components.Parcel:
-        r"""Retrieve an existing parcel
-        Returns parcel details using an existing parcel object ID (this will not return parcel details associated with un-purchased shipment/rate parcel object IDs).
+    def get(self, refund_id: str) -> components.Refund:
+        r"""Retrieve a refund
+        Returns an existing rate using a rate object ID.
         """
-        hook_ctx = HookContext(operation_id='GetParcel', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetParcelRequest(
-            parcel_id=parcel_id,
+        hook_ctx = HookContext(operation_id='GetRefund', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetRefundRequest(
+            refund_id=refund_id,
         )
         
-        _globals = operations.GetParcelGlobals(
+        _globals = operations.GetRefundGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/parcels/{ParcelId}', request, _globals)
+        url = utils.generate_url(base_url, '/refunds/{RefundId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -194,16 +197,17 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Parcel])
+                out = utils.unmarshal_json(http_res.text, Optional[components.Refund])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `shippo-3.3.4/src/shippo/pickups.py` & `shippo-3.3.5/src/shippo/pickups.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, request: Optional[components.PickupBase]) -> components.Pickup:
+    def create(self, request: components.PickupBase) -> components.Pickup:
         r"""Create a pickup
         Creates a pickup object. This request is for a carrier to come to a specified location to take a package for shipping.
         """
         hook_ctx = HookContext(operation_id='CreatePickup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         _globals = operations.CreatePickupGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
@@ -34,17 +34,19 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[components.PickupBase], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, components.PickupBase, "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -64,14 +66,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Pickup])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `shippo-3.3.4/src/shippo/rates.py` & `shippo-3.3.5/src/shippo/rates.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Rate])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -129,14 +130,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.RatePaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -194,14 +196,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.RatePaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `shippo-3.3.4/src/shippo/rates_at_checkout.py` & `shippo-3.3.5/src/shippo/rates_at_checkout.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, request: Optional[components.LiveRateCreateRequest]) -> components.LiveRatePaginatedList:
+    def create(self, request: components.LiveRateCreateRequest) -> components.LiveRatePaginatedList:
         r"""Generate a live rates request
         Initiates a live rates request. Include either the object ID for
         an existing address record or a fully formed address object when entering
         an address value. You can also enter the object ID of an existing user parcel
         template or a fully formed user parcel template object as the parcel value.
         """
         hook_ctx = HookContext(operation_id='CreateLiveRate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
@@ -43,17 +43,19 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[components.LiveRateCreateRequest], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, components.LiveRateCreateRequest, "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -73,14 +75,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.LiveRatePaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -135,14 +138,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.DefaultParcelTemplate])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -201,14 +205,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.DefaultParcelTemplate])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `shippo-3.3.4/src/shippo/refunds.py` & `shippo-3.3.5/src/shippo/tracking_status.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,52 +3,64 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
 from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
-class Refunds:
-    r"""Refunds are reimbursements for successfully created but unused shipping labels or other charges.
-    <SchemaDefinition schemaRef=\"#/components/schemas/Refund\"/>
+class TrackingStatus:
+    r"""<p style=\\"text-align: center; background-color: #F2F3F4;\\"></br>
+    If you purchased your shipping label through Shippo, you can also get all the tracking details of your Shipment 
+    from the <a href=\"#tag/Transactions\">Transaction</a> object.
+    </br></br></p>
+    A tracking status of a package is an indication of current location of a package in the supply chain. For example,  sorting, warehousing, or out for delivery. Use the tracking status object to track the location of your shipments.
+
+    When using your <a href=\"https://docs.goshippo.com/docs/guides_general/authentication/\">Test</a> token for tracking, you need to use Shippo's 
+    predefined tokens for testing different tracking statuses. You can find more information in our 
+    <a href=\"https://docs.goshippo.com/docs/tracking/tracking/\">Tracking tutorial</a> on how to do this, and what the 
+    payloads look like.      
+    <SchemaDefinition schemaRef=\"#/components/schemas/Track\"/>
     """
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, transaction: str, async_: Optional[bool] = None) -> components.Refund:
-        r"""Create a refund
-        Creates a new refund object.
+    def create(self, carrier: str, tracking_number: str, metadata: Optional[str] = None) -> components.Track:
+        r"""Register a tracking webhook
+        Registers a webhook that will send HTTP notifications to you when the status of your tracked package changes. For more details on creating a webhook, see our guides on <a href=\"https://docs.goshippo.com/docs/tracking/webhooks/\">Webhooks</a> and <a href=\"https://docs.goshippo.com/docs/tracking/tracking/\">Tracking</a>.
         """
-        hook_ctx = HookContext(operation_id='CreateRefund', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = components.RefundRequestBody(
-            transaction=transaction,
-            async_=async_,
+        hook_ctx = HookContext(operation_id='CreateTrack', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = components.TracksRequest(
+            carrier=carrier,
+            tracking_number=tracking_number,
+            metadata=metadata,
         )
         
-        _globals = operations.CreateRefundGlobals(
+        _globals = operations.CreateTrackGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/refunds', request, _globals)
+        url = utils.generate_url(base_url, '/tracks', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[components.RefundRequestBody], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, components.TracksRequest, "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -68,42 +80,45 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Refund])
+                out = utils.unmarshal_json(http_res.text, Optional[components.Track])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def list(self) -> components.RefundPaginatedList:
-        r"""List all refunds
-        Returns a list all refund objects.
+    def get(self, tracking_number: str, carrier: str) -> components.Track:
+        r"""Get a tracking status
+        Returns the tracking status of a shipment using a carrier name and a tracking number.
         """
-        hook_ctx = HookContext(operation_id='ListRefunds', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.ListRefundsRequest(
+        hook_ctx = HookContext(operation_id='GetTrack', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetTrackRequest(
+            tracking_number=tracking_number,
+            carrier=carrier,
         )
         
-        _globals = operations.ListRefundsGlobals(
+        _globals = operations.GetTrackGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/refunds/', request, _globals)
+        url = utils.generate_url(base_url, '/tracks/{Carrier}/{TrackingNumber}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -130,79 +145,17 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.RefundPaginatedList])
-                return out
-            
-            content_type = http_res.headers.get('Content-Type')
-            raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        else:
-            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
-
-    
-    
-    def get(self, refund_id: str) -> components.Refund:
-        r"""Retrieve a refund
-        Returns an existing rate using a rate object ID.
-        """
-        hook_ctx = HookContext(operation_id='GetRefund', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetRefundRequest(
-            refund_id=refund_id,
-        )
-        
-        _globals = operations.GetRefundGlobals(
-            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
-        )
-        
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = utils.generate_url(base_url, '/refunds/{RefundId}', request, _globals)
-        
-        if callable(self.sdk_configuration.security):
-            headers, query_params = utils.get_security(self.sdk_configuration.security())
-        else:
-            headers, query_params = utils.get_security(self.sdk_configuration.security)
-        
-        headers = { **utils.get_headers(request, _globals), **headers }
-        query_params = { **utils.get_query_params(request, _globals), **query_params }
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        client = self.sdk_configuration.client
-        
-        try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
-            http_res = client.send(req)
-        except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
-
-        if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
-                raise e
-            if result is not None:
-                http_res = result
-        else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
-        
-        
-        
-        if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Refund])
+                out = utils.unmarshal_json(http_res.text, Optional[components.Track])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `shippo-3.3.4/src/shippo/sdk.py` & `shippo-3.3.5/src/shippo/sdk.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/sdkconfiguration.py` & `shippo-3.3.5/src/shippo/sdkconfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '2018-02-08'
-    sdk_version: str = '3.3.4'
-    gen_version: str = '2.322.5'
-    user_agent: str = 'speakeasy-sdk/python 3.3.4 2.322.5 2018-02-08 shippo'
+    sdk_version: str = '3.3.5'
+    gen_version: str = '2.324.0'
+    user_agent: str = 'speakeasy-sdk/python 3.3.5 2.324.0 2018-02-08 shippo'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `shippo-3.3.4/src/shippo/service_groups.py` & `shippo-3.3.5/src/shippo/service_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,28 +64,29 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[components.ServiceGroup]])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, request: Optional[components.ServiceGroupCreateRequest]) -> components.ServiceGroup:
+    def create(self, request: components.ServiceGroupCreateRequest) -> components.ServiceGroup:
         r"""Create a new service group
         Creates a new service group.
         """
         hook_ctx = HookContext(operation_id='CreateServiceGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         _globals = operations.CreateServiceGroupGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
@@ -96,17 +97,19 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[components.ServiceGroupCreateRequest], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, components.ServiceGroupCreateRequest, "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -126,14 +129,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.ServiceGroup])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -188,14 +192,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.ServiceGroup])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `shippo-3.3.4/src/shippo/shipments.py` & `shippo-3.3.5/src/shippo/shipments.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,28 +86,29 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.ShipmentPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, request: Optional[components.ShipmentCreateRequest]) -> components.Shipment:
+    def create(self, request: components.ShipmentCreateRequest) -> components.Shipment:
         r"""Create a new shipment
         Creates a new shipment object.
         """
         hook_ctx = HookContext(operation_id='CreateShipment', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         _globals = operations.CreateShipmentGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
@@ -118,17 +119,19 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[components.ShipmentCreateRequest], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, components.ShipmentCreateRequest, "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -148,14 +151,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Shipment])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -211,14 +215,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Shipment])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `shippo-3.3.4/src/shippo/shippo_accounts.py` & `shippo-3.3.5/src/shippo/shippo_accounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,28 +67,29 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.ShippoAccountPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, request: Optional[components.ShippoAccountUpdateRequest]) -> components.ShippoAccount:
+    def create(self, request: components.ShippoAccountUpdateRequest) -> components.ShippoAccount:
         r"""Create a Shippo Account
         Creates a Shippo Account object
         """
         hook_ctx = HookContext(operation_id='CreateShippoAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         _globals = operations.CreateShippoAccountGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
@@ -99,17 +100,19 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[components.ShippoAccountUpdateRequest], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, components.ShippoAccountUpdateRequest, "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -129,14 +132,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.ShippoAccount])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -192,14 +196,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.ShippoAccount])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -259,14 +264,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.ShippoAccount])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `shippo-3.3.4/src/shippo/tracking_status.py` & `shippo-3.3.5/src/shippo/customs_items.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,62 +3,114 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
 from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
-class TrackingStatus:
-    r"""<p style=\\"text-align: center; background-color: #F2F3F4;\\"></br>
-    If you purchased your shipping label through Shippo, you can also get all the tracking details of your Shipment 
-    from the <a href=\"#tag/Transactions\">Transaction</a> object.
-    </br></br></p>
-    A tracking status of a package is an indication of current location of a package in the supply chain. For example,  sorting, warehousing, or out for delivery. Use the tracking status object to track the location of your shipments.
-
-    When using your <a href=\"https://docs.goshippo.com/docs/guides_general/authentication/\">Test</a> token for tracking, you need to use Shippo's 
-    predefined tokens for testing different tracking statuses. You can find more information in our 
-    <a href=\"https://docs.goshippo.com/docs/tracking/tracking/\">Tracking tutorial</a> on how to do this, and what the 
-    payloads look like.      
-    <SchemaDefinition schemaRef=\"#/components/schemas/Track\"/>
+class CustomsItems:
+    r"""Customs declarations are relevant information, including one or multiple customs items, you need to provide for customs clearance for your international shipments.
+    <SchemaDefinition schemaRef=\"#/components/schemas/CustomsItem\"/>
     """
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, carrier: str, tracking_number: str, metadata: Optional[str] = None) -> components.Track:
-        r"""Register a tracking webhook
-        Registers a webhook that will send HTTP notifications to you when the status of your tracked package changes. For more details on creating a webhook, see our guides on <a href=\"https://docs.goshippo.com/docs/tracking/webhooks/\">Webhooks</a> and <a href=\"https://docs.goshippo.com/docs/tracking/tracking/\">Tracking</a>.
+    def list(self, page: Optional[int] = None, results: Optional[int] = None) -> components.CustomsItemPaginatedList:
+        r"""List all customs items
+        Returns a list all customs items objects.
         """
-        hook_ctx = HookContext(operation_id='CreateTrack', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = components.TracksRequest(
-            carrier=carrier,
-            tracking_number=tracking_number,
-            metadata=metadata,
+        hook_ctx = HookContext(operation_id='ListCustomsItems', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.ListCustomsItemsRequest(
+            page=page,
+            results=results,
         )
         
-        _globals = operations.CreateTrackGlobals(
+        _globals = operations.ListCustomsItemsGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/tracks', request, _globals)
+        url = utils.generate_url(base_url, '/customs/items', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[components.TracksRequest], "request", False, True, 'json')
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
+        
+        try:
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            http_res = client.send(req)
+        except Exception as e:
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
+
+        if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
+                raise e
+            if result is not None:
+                http_res = result
+        else:
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
+        
+        
+        
+        if http_res.status_code == 200:
+            # pylint: disable=no-else-return
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsItemPaginatedList])
+                return out
+            
+            content_type = http_res.headers.get('Content-Type')
+            raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
+            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
+
+    
+    
+    def create(self, request: components.CustomsItemCreateRequest) -> components.CustomsItem:
+        r"""Create a new customs item
+        Creates a new customs item object.
+        """
+        hook_ctx = HookContext(operation_id='CreateCustomsItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.CreateCustomsItemGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        
+        url = utils.generate_url(base_url, '/customs/items', request, _globals)
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
+        headers = { **utils.get_headers(request, _globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, components.CustomsItemCreateRequest, "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -78,44 +130,45 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Track])
+                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsItem])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def get(self, tracking_number: str, carrier: str) -> components.Track:
-        r"""Get a tracking status
-        Returns the tracking status of a shipment using a carrier name and a tracking number.
+    def get(self, customs_item_id: str, page: Optional[int] = None) -> components.CustomsItem:
+        r"""Retrieve a customs item
+        Returns an existing customs item using an object ID
         """
-        hook_ctx = HookContext(operation_id='GetTrack', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetTrackRequest(
-            tracking_number=tracking_number,
-            carrier=carrier,
+        hook_ctx = HookContext(operation_id='GetCustomsItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetCustomsItemRequest(
+            customs_item_id=customs_item_id,
+            page=page,
         )
         
-        _globals = operations.GetTrackGlobals(
+        _globals = operations.GetCustomsItemGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/tracks/{Carrier}/{TrackingNumber}', request, _globals)
+        url = utils.generate_url(base_url, '/customs/items/{CustomsItemId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
@@ -142,16 +195,17 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Track])
+                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsItem])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `shippo-3.3.4/src/shippo/transactions.py` & `shippo-3.3.5/src/shippo/transactions.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,28 +60,29 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.TransactionPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, request: Optional[Union[components.TransactionCreateRequest, components.InstantTransactionCreateRequest]]) -> Union[components.Transaction, components.InstantTransactionCreateResponse]:
+    def create(self, request: Union[components.TransactionCreateRequest, components.InstantTransactionCreateRequest]) -> Union[components.Transaction, components.InstantTransactionCreateResponse]:
         r"""Create a shipping label
         Creates a new transaction object and purchases the shipping label using a rate object that has previously been created. <br> OR <br> Creates a new transaction object and purchases the shipping label instantly using shipment details, an existing carrier account, and an existing service level token.
         """
         hook_ctx = HookContext(operation_id='CreateTransaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         _globals = operations.CreateTransactionGlobals(
             shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
@@ -92,17 +93,19 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[Union[components.TransactionCreateRequest, components.InstantTransactionCreateRequest]], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, Union[components.TransactionCreateRequest, components.InstantTransactionCreateRequest], "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -122,14 +125,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 201:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[Union[components.Transaction, components.InstantTransactionCreateResponse]])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -185,14 +189,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Transaction])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `shippo-3.3.4/src/shippo/user_parcel_templates.py` & `shippo-3.3.5/src/shippo/user_parcel_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,28 +68,29 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[components.UserParcelTemplate]])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, request: Optional[Union[components.UserParcelTemplateWithCarrierTemplateCreateRequest, components.UserParcelTemplateWithoutCarrierTemplateCreateRequest]]) -> components.UserParcelTemplate:
+    def create(self, request: Union[components.UserParcelTemplateWithCarrierTemplateCreateRequest, components.UserParcelTemplateWithoutCarrierTemplateCreateRequest]) -> components.UserParcelTemplate:
         r"""Create a new user parcel template
         Creates a new user parcel template. <br>You can choose to create a
         parcel template using a preset carrier template as a starting point, or
         you can create an entirely custom one. To use a preset carrier template,
         pass in a unique template token from <a href=\"#tag/Parcel-Templates\">this list</a>
         plus the weight fields (**weight** and **weight_unit**). Otherwise, omit
         the template field and pass the other fields, for the weight, length, height,
@@ -106,17 +107,19 @@
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request, _globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, Optional[Union[components.UserParcelTemplateWithCarrierTemplateCreateRequest, components.UserParcelTemplateWithoutCarrierTemplateCreateRequest]], "request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, Union[components.UserParcelTemplateWithCarrierTemplateCreateRequest, components.UserParcelTemplateWithoutCarrierTemplateCreateRequest], "request", False, False, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        if data is None and form is None:
+            raise Exception('request body is required')
         query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
@@ -136,14 +139,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.UserParcelTemplate])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -261,14 +265,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.UserParcelTemplate])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -328,14 +333,15 @@
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
+            # pylint: disable=no-else-return
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.UserParcelTemplate])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `shippo-3.3.4/src/shippo/utils/retries.py` & `shippo-3.3.5/src/shippo/utils/retries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo/utils/utils.py` & `shippo-3.3.5/src/shippo/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shippo-3.3.4/src/shippo.egg-info/PKG-INFO` & `shippo-3.3.5/src/shippo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.3.4
-Summary: Python Client SDK Generated by Speakeasy
+Version: 3.3.5
+Summary: Shipping API Python library (USPS, FedEx, UPS and more)
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
```

### Comparing `shippo-3.3.4/src/shippo.egg-info/SOURCES.txt` & `shippo-3.3.5/src/shippo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

