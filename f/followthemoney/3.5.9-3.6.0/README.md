# Comparing `tmp/followthemoney-3.5.9.tar.gz` & `tmp/followthemoney-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "followthemoney-3.5.9.tar", last modified: Sun Jan 14 12:26:58 2024, max compression
+gzip compressed data, was "followthemoney-3.6.0.tar", last modified: Wed May  8 09:30:56 2024, max compression
```

## Comparing `followthemoney-3.5.9.tar` & `followthemoney-3.6.0.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.919663 followthemoney-3.5.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-01-14 12:25:30.000000 followthemoney-3.5.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-14 12:25:30.000000 followthemoney-3.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-01-14 12:26:58.919663 followthemoney-3.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-01-14 12:25:30.000000 followthemoney-3.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.895662 followthemoney-3.5.9/followthemoney/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.899663 followthemoney-3.5.9/followthemoney/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/cli/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/cli/exports.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/cli/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/cli/sieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.899663 followthemoney-3.5.9/followthemoney/export/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/export/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/export/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/export/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/export/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/export/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/export/rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.899663 followthemoney-3.5.9/followthemoney/mapping/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/mapping/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/mapping/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/mapping/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/mapping/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/mapping/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/mapping/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/offshore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/property.py
--rw-r--r--   0 runner    (1001) docker     (127)    19871 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/rdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.907663 followthemoney-3.5.9/followthemoney/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Address.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Airplane.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Analyzable.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Article.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Assessment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Asset.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Associate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Audio.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/BankAccount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Call.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/CallForTenders.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Company.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Contract.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/ContractAward.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/CourtCase.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/CourtCaseParty.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/CryptoWallet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Debt.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Directorship.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Document.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/EconomicActivity.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Email.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Employment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Event.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Family.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Folder.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/HyperText.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Identification.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Image.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Interest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Interval.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/LegalEntity.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/License.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Membership.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Mention.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Message.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Note.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Occupancy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Ownership.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Package.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Page.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Pages.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Passport.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Payment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Person.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/PlainText.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Position.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Post.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Project.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/ProjectParticipant.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/PublicBody.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/RealEstate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Representation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Sanction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Security.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Similar.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Succession.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Table.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/TaxRoll.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Thing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Trip.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/UnknownLink.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/UserAccount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Value.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Vehicle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Vessel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Video.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema/Workbook.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    16774 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.907663 followthemoney-3.5.9/followthemoney/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.891662 followthemoney-3.5.9/followthemoney/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.911663 followthemoney-3.5.9/followthemoney/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    38795 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)   121331 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.891662 followthemoney-3.5.9/followthemoney/translations/bs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.911663 followthemoney-3.5.9/followthemoney/translations/bs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    10751 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)    93147 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.891662 followthemoney-3.5.9/followthemoney/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.911663 followthemoney-3.5.9/followthemoney/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    36070 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)   115533 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/de/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.891662 followthemoney-3.5.9/followthemoney/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.911663 followthemoney-3.5.9/followthemoney/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    32142 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)   115183 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/es/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.911663 followthemoney-3.5.9/followthemoney/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.911663 followthemoney-3.5.9/followthemoney/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    42517 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)   119965 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (127)   106802 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/fr/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (127)   105130 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.891662 followthemoney-3.5.9/followthemoney/translations/nb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.911663 followthemoney-3.5.9/followthemoney/translations/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/nb/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)    89796 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.891662 followthemoney-3.5.9/followthemoney/translations/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.911663 followthemoney-3.5.9/followthemoney/translations/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/nl/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)    90876 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.891662 followthemoney-3.5.9/followthemoney/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.915663 followthemoney-3.5.9/followthemoney/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)    89847 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.915663 followthemoney-3.5.9/followthemoney/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.915663 followthemoney-3.5.9/followthemoney/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    64182 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)   139453 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (127)   130621 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/ru/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.895662 followthemoney-3.5.9/followthemoney/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.915663 followthemoney-3.5.9/followthemoney/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/tr/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (127)    89829 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.919663 followthemoney-3.5.9/followthemoney/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/address.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     9560 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/country.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/gender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/iban.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/mimetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/name.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/phone.py
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/types/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-01-14 12:25:30.000000 followthemoney-3.5.9/followthemoney/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 12:26:58.899663 followthemoney-3.5.9/followthemoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-01-14 12:26:58.000000 followthemoney-3.5.9/followthemoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-01-14 12:26:58.000000 followthemoney-3.5.9/followthemoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 12:26:58.000000 followthemoney-3.5.9/followthemoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-01-14 12:26:58.000000 followthemoney-3.5.9/followthemoney.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 12:26:58.000000 followthemoney-3.5.9/followthemoney.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 12:26:42.000000 followthemoney-3.5.9/followthemoney.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-14 12:26:58.000000 followthemoney-3.5.9/followthemoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-14 12:26:58.000000 followthemoney-3.5.9/followthemoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-14 12:26:58.919663 followthemoney-3.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-01-14 12:25:30.000000 followthemoney-3.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.230000 followthemoney-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-08 09:29:16.000000 followthemoney-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-08 09:29:16.000000 followthemoney-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-08 09:30:56.230000 followthemoney-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-08 09:29:16.000000 followthemoney-3.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.210000 followthemoney-3.6.0/followthemoney/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.210000 followthemoney-3.6.0/followthemoney/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/cli/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/cli/exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/cli/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/cli/sieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.210000 followthemoney-3.6.0/followthemoney/export/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/export/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/export/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/export/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/export/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/export/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/export/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.210000 followthemoney-3.6.0/followthemoney/mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/mapping/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/mapping/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/mapping/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/mapping/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/mapping/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/mapping/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6426 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/offshore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20033 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/rdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Address.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Airplane.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Analyzable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Article.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Assessment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Asset.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Associate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Audio.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/BankAccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Call.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/CallForTenders.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Company.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Contract.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/ContractAward.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/CourtCase.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/CourtCaseParty.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/CryptoWallet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Debt.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Directorship.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Document.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/EconomicActivity.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Email.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Employment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Event.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Family.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Folder.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/HyperText.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Identification.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Image.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Interest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Interval.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/LegalEntity.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/License.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Membership.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Mention.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Message.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Note.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Occupancy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Ownership.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Package.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Page.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Passport.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Payment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Person.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/PlainText.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Position.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Post.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Project.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/ProjectParticipant.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/PublicBody.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/RealEstate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Representation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Sanction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Security.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Similar.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Succession.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Table.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/TaxRoll.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Thing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Trip.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/UnknownLink.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/UserAccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Value.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Vehicle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Vessel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Video.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema/Workbook.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16774 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.206000 followthemoney-3.6.0/followthemoney/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    38795 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   121331 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.206000 followthemoney-3.6.0/followthemoney/translations/bs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/bs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10751 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    93147 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.206000 followthemoney-3.6.0/followthemoney/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    36070 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   115533 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.206000 followthemoney-3.6.0/followthemoney/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    32142 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   115183 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    42517 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   119965 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (127)   106802 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/fr/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (127)   105130 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.206000 followthemoney-3.6.0/followthemoney/translations/nb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    89796 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.206000 followthemoney-3.6.0/followthemoney/translations/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    90876 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.206000 followthemoney-3.6.0/followthemoney/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.222000 followthemoney-3.6.0/followthemoney/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    89847 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.226000 followthemoney-3.6.0/followthemoney/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.226000 followthemoney-3.6.0/followthemoney/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    64182 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   139453 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (127)   130621 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/ru/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.206000 followthemoney-3.6.0/followthemoney/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.226000 followthemoney-3.6.0/followthemoney/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    89829 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.230000 followthemoney-3.6.0/followthemoney/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/country.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/iban.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/mimetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/phone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/types/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-08 09:29:16.000000 followthemoney-3.6.0/followthemoney/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:30:56.210000 followthemoney-3.6.0/followthemoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-08 09:30:56.000000 followthemoney-3.6.0/followthemoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-05-08 09:30:56.000000 followthemoney-3.6.0/followthemoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:30:56.000000 followthemoney-3.6.0/followthemoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-08 09:30:56.000000 followthemoney-3.6.0/followthemoney.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:30:56.000000 followthemoney-3.6.0/followthemoney.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:30:36.000000 followthemoney-3.6.0/followthemoney.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-08 09:30:56.000000 followthemoney-3.6.0/followthemoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-08 09:30:56.000000 followthemoney-3.6.0/followthemoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-08 09:30:56.230000 followthemoney-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-08 09:29:16.000000 followthemoney-3.6.0/setup.py
```

### Comparing `followthemoney-3.5.9/LICENSE` & `followthemoney-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/PKG-INFO` & `followthemoney-3.6.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,90 @@
 Metadata-Version: 2.1
 Name: followthemoney
-Version: 3.5.9
-Summary: UNKNOWN
+Version: 3.6.0
 Home-page: https://followthemoney.tech/
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
-Description: # Follow the Money
-        
-        [![ftm-build](https://github.com/alephdata/followthemoney/actions/workflows/build.yml/badge.svg)](https://github.com/alephdata/followthemoney/actions/workflows/build.yml)
-        
-        This repository contains a pragmatic data model for the entities most
-        commonly used in investigative reporting: people, companies, assets,
-        payments, court cases, etc.
-        
-        The purpose of this is not to model reality in an ideal data model, but
-        rather to have a working data structure for researchers.
-        
-        `followthemoney` also contains code used to validate and normalize many
-        of the elements of data, and to map tabular data into the model.
-        
-        ## Documentation
-        
-        For a general introduction to `followthemoney`, check the high-level introduction:
-        
-        * https://followthemoney.tech
-        
-        Part of this package is a command-line tool that can be used to process and
-        transform data in various ways. You can find a tutorial here:
-        
-        * https://followthemoney.tech/docs/cli/
-        
-        Besides the introductions, there is also a full reference documentation for the
-        library and the contained ontology: 
-        
-        * https://followthemoney.tech/explorer/
-        
-        There's also a number of viewers for the RDF schema definitions generated
-        from FollowTheMoney, e.g.:
-        
-        * [LODE documentation](http://150.146.207.114/lode/extract?url=https%3A%2F%2Falephdata.github.io%2Ffollowthemoney%2Fns%2Fftm.xml&owlapi=true&imported=true&lang=en)
-        * [WebVOWL](https://service.tib.eu/webvowl/#iri=https://alephdata.github.io/followthemoney/ns/ftm.xml)
-        * RDF/OWL specification in [XML](https://alephdata.github.io/followthemoney/ns/ftm.xml).
-        
-        ## Development environment
-        
-        For local development with a virtualenv:
-        
-        ```bash
-        python3 -mvenv .env
-        source .env/bin/activate
-        pip install -e ".[dev]"
-        ```
-        
-        Now you can run the tests with
-        
-        ```bash
-        make test
-        ```
-        
-        ## Releasing
-        
-        We release a lot of version of `followthemoney` because even small changes
-        to the code base require a pypi release to begin being used in `aleph`. To
-        this end, here's the steps for making a release:
-        
-        ```bash
-        git pull --rebase
-        make build
-        make test
-        git add . && git commit -m "Updating translation files"
-        bumpversion patch
-        git push --atomic origin main $(git describe --tags --abbrev=0)
-        ```
-        
-        This will create a new patch release and upload a distribution of it. If
-        the changes are more significant, you can run `bumpversion` with the `minor`
-        or `major` arguments.
-        
-        When the schema is updated, please update the docs, ideally including the
-        diagrams. For the RDF namespace and JavaScript version of the model, 
-        run `make generate`.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# Follow the Money
+
+[![ftm-build](https://github.com/alephdata/followthemoney/actions/workflows/build.yml/badge.svg)](https://github.com/alephdata/followthemoney/actions/workflows/build.yml)
+
+This repository contains a pragmatic data model for the entities most
+commonly used in investigative reporting: people, companies, assets,
+payments, court cases, etc.
+
+The purpose of this is not to model reality in an ideal data model, but
+rather to have a working data structure for researchers.
+
+`followthemoney` also contains code used to validate and normalize many
+of the elements of data, and to map tabular data into the model.
+
+## Documentation
+
+For a general introduction to `followthemoney`, check the high-level introduction:
+
+* https://followthemoney.tech
+
+Part of this package is a command-line tool that can be used to process and
+transform data in various ways. You can find a tutorial here:
+
+* https://followthemoney.tech/docs/cli/
+
+Besides the introductions, there is also a full reference documentation for the
+library and the contained ontology: 
+
+* https://followthemoney.tech/explorer/
+
+There's also a number of viewers for the RDF schema definitions generated
+from FollowTheMoney, e.g.:
+
+* [LODE documentation](http://150.146.207.114/lode/extract?url=https%3A%2F%2Falephdata.github.io%2Ffollowthemoney%2Fns%2Fftm.xml&owlapi=true&imported=true&lang=en)
+* [WebVOWL](https://service.tib.eu/webvowl/#iri=https://alephdata.github.io/followthemoney/ns/ftm.xml)
+* RDF/OWL specification in [XML](https://alephdata.github.io/followthemoney/ns/ftm.xml).
+
+## Development environment
+
+For local development with a virtualenv:
+
+```bash
+python3 -mvenv .env
+source .env/bin/activate
+pip install -e ".[dev]"
+```
+
+Now you can run the tests with
+
+```bash
+make test
+```
+
+## Releasing
+
+We release a lot of version of `followthemoney` because even small changes
+to the code base require a pypi release to begin being used in `aleph`. To
+this end, here's the steps for making a release:
+
+```bash
+git pull --rebase
+make build
+make test
+git add . && git commit -m "Updating translation files"
+bumpversion patch
+git push --atomic origin main $(git describe --tags --abbrev=0)
+```
+
+This will create a new patch release and upload a distribution of it. If
+the changes are more significant, you can run `bumpversion` with the `minor`
+or `major` arguments.
+
+When the schema is updated, please update the docs, ideally including the
+diagrams. For the RDF namespace and JavaScript version of the model, 
+run `make generate`.
```

### Comparing `followthemoney-3.5.9/README.md` & `followthemoney-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/cli/aggregate.py` & `followthemoney-3.6.0/followthemoney/cli/aggregate.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/cli/cli.py` & `followthemoney-3.6.0/followthemoney/cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,64 @@
 import sys
-import json
 import click
+import orjson
 import logging
 from pathlib import Path
-from typing import Optional, TextIO
+from typing import Optional, BinaryIO, List, Any, Dict
 from banal import ensure_list
 
 from followthemoney import model
 from followthemoney.namespace import Namespace
-from followthemoney.cli.util import InPath, OutPath, path_entities, read_entities
+from followthemoney.cli.util import InPath, OutPath, path_entities
 from followthemoney.cli.util import path_writer, write_entity
 from followthemoney.proxy import EntityProxy
 
 
 @click.group(help="Utility for FollowTheMoney graph data")
 def cli() -> None:
     fmt = "%(name)s [%(levelname)s] %(message)s"
     logging.basicConfig(stream=sys.stderr, level=logging.INFO, format=fmt)
 
 
 @cli.command("dump-model", help="Export the current schema model")
-@click.option("-o", "--outfile", type=click.File("w"), default="-")
-def dump_model(outfile: TextIO) -> None:
-    outfile.write(json.dumps(model.to_dict(), indent=2, sort_keys=True))
+@click.option("-o", "--outfile", type=click.File("wb"), default="-")
+def dump_model(outfile: BinaryIO) -> None:
+    f = orjson.OPT_INDENT_2 | orjson.OPT_SORT_KEYS
+    outfile.write(orjson.dumps(model.to_dict(), option=f))
 
 
 @cli.command("validate", help="Re-parse and validate the given data")
 @click.option("-i", "--infile", type=InPath, default="-")
 @click.option("-o", "--outfile", type=OutPath, default="-")
 def validate(infile: Path, outfile: Path) -> None:
     try:
         with path_writer(outfile) as outfh:
             for entity in path_entities(infile, EntityProxy, cleaned=False):
                 clean = model.make_entity(entity.schema)
                 clean.id = entity.id
-                for (prop, value) in entity.itervalues():
+                for prop, value in entity.itervalues():
                     clean.add(prop, value)
                 write_entity(outfh, clean)
     except BrokenPipeError:
         raise click.Abort()
 
 
 @cli.command("import-vis", help="Load a .VIS file and get entities")
 @click.option("-i", "--infile", type=InPath, default="-")  # noqa
 @click.option("-o", "--outfile", type=OutPath, default="-")  # noqa
 def import_vis(infile: Path, outfile: Path) -> None:
     with path_writer(outfile) as outfh:
-        with open(infile, "r") as infh:
-            data = json.load(infh)
+        with open(infile, "rb") as infh:
+            data: Dict[str, Any] = orjson.loads(infh.read())
             if "entities" in data:
-                entities = data.get("entities", data)
-            if "layout" in data:
+                entities: List[Dict[str, Any]] = data.get("entities", data)
+            elif "layout" in data:
                 entities = data.get("layout", {}).get("entities", data)
+            else:
+                raise click.ClickException("No entities found in VIS file")
             for entity_data in ensure_list(entities):
                 entity = EntityProxy.from_dict(model, entity_data)
                 write_entity(outfh, entity)
 
 
 @cli.command("sign", help="Apply a HMAC signature to entity IDs")
 @click.option("-i", "--infile", type=InPath, default="-")  # noqa
@@ -71,14 +74,15 @@
     except BrokenPipeError:
         raise click.Abort()
 
 
 @cli.command(help="Format a stream of entities to make it readable")
 @click.option("-i", "--infile", type=InPath, default="-")  # noqa
 def pretty(infile: Path) -> None:
-    stdout = click.get_text_stream("stdout")
+    stdout = click.get_binary_stream("stdout")
     try:
+        f = orjson.OPT_INDENT_2 | orjson.OPT_APPEND_NEWLINE
         for entity in path_entities(infile, EntityProxy):
-            data = json.dumps(entity.to_dict(), indent=2)
-            stdout.write(data + "\n")
+            data = orjson.dumps(entity.to_dict(), option=f)
+            stdout.write(data)
     except BrokenPipeError:
         raise click.Abort()
```

### Comparing `followthemoney-3.5.9/followthemoney/cli/exports.py` & `followthemoney-3.6.0/followthemoney/cli/exports.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/cli/mapping.py` & `followthemoney-3.6.0/followthemoney/cli/mapping.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/cli/sieve.py` & `followthemoney-3.6.0/followthemoney/cli/sieve.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/cli/util.py` & `followthemoney-3.6.0/followthemoney/cli/util.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/compare.py` & `followthemoney-3.6.0/followthemoney/compare.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/exc.py` & `followthemoney-3.6.0/followthemoney/exc.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/export/common.py` & `followthemoney-3.6.0/followthemoney/export/common.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/export/csv.py` & `followthemoney-3.6.0/followthemoney/export/csv.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/export/excel.py` & `followthemoney-3.6.0/followthemoney/export/excel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from io import BytesIO
 from typing import Dict, List, Optional
-from openpyxl import Workbook  # type: ignore
-from openpyxl.cell import WriteOnlyCell  # type: ignore
-from openpyxl.styles import Font, PatternFill  # type: ignore
-from openpyxl.worksheet.worksheet import Worksheet  # type: ignore
-from openpyxl.utils.exceptions import IllegalCharacterError  # type: ignore
+from openpyxl import Workbook
+from openpyxl.cell import WriteOnlyCell
+from openpyxl.styles import Font, PatternFill
+from openpyxl.worksheet.worksheet import Worksheet
+from openpyxl.utils.exceptions import IllegalCharacterError
 
 from followthemoney.export.common import Exporter
 from followthemoney.proxy import E
 from followthemoney.schema import Schema
 from followthemoney.util import PathLike, sanitize_text
 
 log = logging.getLogger(__name__)
@@ -21,15 +21,15 @@
         start_color="982022", end_color="982022", fill_type="solid"
     )
 
     def __init__(self) -> None:
         self.workbook = Workbook(write_only=True)
 
     def make_sheet(self, title: str, headers: List[str]) -> Worksheet:
-        sheet = self.workbook.create_sheet(title=title)
+        sheet: Worksheet = self.workbook.create_sheet(title=title)
         sheet.freeze_panes = "A2"
         sheet.sheet_properties.filterMode = True
         cells = []
         for header in headers:
             header_ = sanitize_text(header)
             cell = WriteOnlyCell(sheet, value=header_)
             cell.font = self.HEADER_FONT
```

### Comparing `followthemoney-3.5.9/followthemoney/export/graph.py` & `followthemoney-3.6.0/followthemoney/export/graph.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/export/neo4j.py` & `followthemoney-3.6.0/followthemoney/export/neo4j.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/export/rdf.py` & `followthemoney-3.6.0/followthemoney/export/rdf.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/graph.py` & `followthemoney-3.6.0/followthemoney/graph.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/helpers.py` & `followthemoney-3.6.0/followthemoney/helpers.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/mapping/csv.py` & `followthemoney-3.6.0/followthemoney/mapping/csv.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/mapping/entity.py` & `followthemoney-3.6.0/followthemoney/mapping/entity.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 from hashlib import sha1
 from warnings import warn
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Set
 from banal import keys_values
 from normality import stringify
 
 from followthemoney.types import registry
@@ -11,14 +12,16 @@
 from followthemoney.mapping.source import Record
 from followthemoney.exc import InvalidMapping
 
 if TYPE_CHECKING:
     from followthemoney.model import Model
     from followthemoney.mapping.query import QueryMapping
 
+log = logging.getLogger(__name__)
+
 
 class EntityMapping(object):
 
     __slots__ = (
         "model",
         "name",
         "seed",
@@ -108,30 +111,39 @@
         # THIS IS HACKY
         # Some of the converters, e.g. for phone numbers, work better if they
         # know the country which the number is from. In order to provide that
         # detail, we are first running country fields, then making the data
         # from that accessible to phone and address parsers.
         for prop in self.properties:
             if prop.prop.type == registry.country:
-                prop.map(proxy, record, entities)
+                discarded_values = prop.map(proxy, record, entities)
+                for value in discarded_values:
+                    log.warn(f"[{self.name}] Discarded unclean value \"{value}\" for property \"{prop.prop.qname}\".")
 
         for prop in self.properties:
             if prop.prop.type != registry.country:
-                prop.map(proxy, record, entities)
+                discarded_values = prop.map(proxy, record, entities)
+                for value in discarded_values:
+                    log.warn(f"[{self.name}] Discarding unclean value \"{value}\" for property \"{prop.prop.qname}\".")
 
         # Generate the ID at the end to avoid self-reference checks on empty
         # keys.
         proxy.id = self.compute_key(record)
         if proxy.id is None:
+            if self.id_column:
+                log.warn(f"[{self.name}] Skipping entity because no ID could be computed. Make sure that there are no empty values in the \"{self.id_column}\" column.")
+            if self.keys:
+                log.warn(f"[{self.name}] Skipping entity because no ID could be computed. Make sure that there are no empty values in key columns.")
             return None
 
         for prop in self.properties:
             if prop.required and not proxy.has(prop.prop):
                 # This is a bit weird, it flags fields to be required in
                 # the mapping, not in the model. Basically it means: if
                 # this row of source data doesn't have that field, then do
                 # not map it again.
+                log.warn(f"[{self.name}] Skipping entity because required property \"{prop.prop.name}\" is empty.")
                 return None
         return proxy
 
     def __repr__(self) -> str:
         return "<EntityMapping(%r)>" % self.name
```

### Comparing `followthemoney-3.5.9/followthemoney/mapping/property.py` & `followthemoney-3.6.0/followthemoney/mapping/property.py`

 * *Files 10% similar despite different names*

```diff
@@ -108,30 +108,42 @@
             rec_value = record.get(ref)
             if rec_value is not None:
                 values.append(rec_value)
         return values
 
     def map(
         self, proxy: EntityProxy, record: Record, entities: Dict[str, EntityProxy]
-    ) -> None:
+    ) -> List[str]:
         if self.entity is not None:
             entity = entities.get(self.entity)
             if entity is not None:
                 proxy.unsafe_add(self.prop, entity.id, cleaned=True)
                 inline_names(proxy, entity)
-            return None
+            return []
 
         # clean the values returned by the query, or by using literals, or
         # formats.
         values: List[str] = self.record_values(record)
 
         if self.join is not None:
             values = [self.join.join(values)]
 
         if self.split is not None:
             splote = []
             for value in values:
                 splote.extend(value.split(self.split))
             values = splote
 
+        discarded_values: List[str] = []
+
         for value in values:
-            proxy.unsafe_add(self.prop, value, fuzzy=self.fuzzy, format=self.format)
+            added_value = proxy.unsafe_add(
+                prop=self.prop,
+                value=value,
+                fuzzy=self.fuzzy,
+                format=self.format,
+            )
+
+            if value is not None and added_value is None:
+                discarded_values.append(value)
+
+        return discarded_values
```

### Comparing `followthemoney-3.5.9/followthemoney/mapping/query.py` & `followthemoney-3.6.0/followthemoney/mapping/query.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/mapping/source.py` & `followthemoney-3.6.0/followthemoney/mapping/source.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/mapping/sql.py` & `followthemoney-3.6.0/followthemoney/mapping/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     def __init__(self, query: "QueryMapping", data: Dict[str, Any]) -> None:
         super(SQLSource, self).__init__(query, data)
         database = data.get("database")
         if database is None:
             raise InvalidMapping("No database in SQL mapping!")
         self.database_uri = cast(str, os.path.expandvars(database))
-        self.engine = create_engine(self.database_uri, poolclass=NullPool)  
+        self.engine = create_engine(self.database_uri, poolclass=NullPool)
         self.meta = MetaData()
 
         tables = keys_values(data, "table", "tables")
         self.tables = [QueryTable(self.meta, self.engine, f) for f in tables]
         self.joins = cast(List[Dict[str, str]], ensure_list(data.get("joins")))
 
     def get_column(self, ref: Optional[str]) -> Label[Any]:
```

### Comparing `followthemoney-3.5.9/followthemoney/messages.py` & `followthemoney-3.6.0/followthemoney/messages.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/model.py` & `followthemoney-3.6.0/followthemoney/model.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/namespace.py` & `followthemoney-3.6.0/followthemoney/namespace.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/offshore.py` & `followthemoney-3.6.0/followthemoney/offshore.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/ontology.py` & `followthemoney-3.6.0/followthemoney/ontology.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/property.py` & `followthemoney-3.6.0/followthemoney/property.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     type: Optional[str]
     hidden: Optional[bool]
     matchable: Optional[bool]
     deprecated: Optional[bool]
     # stub: Optional[bool]
     rdf: Optional[str]
     range: Optional[str]
+    format: Optional[str]
 
 
 class PropertySpec(PropertyDict):
     reverse: ReverseSpec
 
 
 class PropertyToDict(PropertyDict, total=False):
@@ -54,14 +55,15 @@
         "_hash",
         "_description",
         "hidden",
         "type",
         "matchable",
         "deprecated",
         "_range",
+        "format",
         "range",
         "stub",
         "_reverse",
         "reverse",
         "uri",
     )
 
@@ -109,14 +111,19 @@
 
         #: If the property is of type ``entity``, the set of valid schema to be added
         #: in this property can be constrained. For example, an asset can be owned,
         #: but a person cannot be owned.
         self._range = data.get("range")
         self.range: Optional["Schema"] = None
 
+        #: If the property is of type ``identifier``, a more narrow definition of the
+        #: identifier format can be provided. For example, LEI, INN or IBAN codes
+        #: can be automatically validated.
+        self.format: Optional[str] = data.get("format")
+
         #: When a property points to another schema, a reverse property is added for
         #: various administrative reasons. These properties are, however, not real
         #: and cannot be written to. That's why they are marked as stubs and adding
         #: values to them will raise an exception.
         self.stub: Optional[bool] = False
 
         #: When a property points to another schema, a stub reverse property is
@@ -165,14 +172,16 @@
         tries to normalize the value to see if it passes strict parsing.
         """
         values = []
         for val in data:
             if self.stub:
                 return gettext("Property cannot be written")
             val = get_entity_id(val)
+            if val is None:
+                continue
             if not self.type.validate(val):
                 return gettext("Invalid value")
             if val is not None:
                 values.append(val)
         return None
 
     def __eq__(self, other: Any) -> bool:
@@ -199,14 +208,16 @@
             data["hidden"] = True
         if self.deprecated:
             data["deprecated"] = True
         if self.range is not None:
             data["range"] = self.range.name
         if self.reverse is not None:
             data["reverse"] = self.reverse.name
+        if self.format is not None:
+            data["format"] = self.format
         return data
 
     def __repr__(self) -> str:
         return "<Property(%r)>" % self.qname
 
     def __str__(self) -> str:
         return self.qname
```

### Comparing `followthemoney-3.5.9/followthemoney/proxy.py` & `followthemoney-3.6.0/followthemoney/proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,45 +190,52 @@
             if quiet:
                 return None
             msg = gettext("Stub property (%s): %s")
             raise InvalidData(msg % (self.schema, prop))
 
         for value in value_list(values):
             if not cleaned:
+                format = format or prop.format
                 value = prop.type.clean(value, proxy=self, fuzzy=fuzzy, format=format)
             self.unsafe_add(prop, value, cleaned=True)
         return None
 
     def unsafe_add(
         self,
         prop: Property,
         value: Optional[str],
         cleaned: bool = False,
         fuzzy: bool = False,
         format: Optional[str] = None,
-    ) -> None:
+    ) -> Optional[str]:
         """A version of `add()` to be used only in type-checking code. This accepts
         only a single value, and performs input cleaning on the premise that the
-        value is already valid unicode."""
+        value is already valid unicode. Returns the value that has been added."""
         if not cleaned and value is not None:
+            format = format or prop.format
             value = prop.type.clean_text(value, fuzzy=fuzzy, format=format, proxy=self)
-        if value is not None:
-            # Somewhat hacky: limit the maximum size of any particular
-            # field to avoid overloading upstream aleph/elasticsearch.
-            value_size = len(value)
-            if prop.type.max_size is not None:
-                if self._size + value_size > prop.type.max_size:
-                    # msg = "[%s] too large. Rejecting additional values."
-                    # log.warning(msg, prop.name)
-                    return None
-            self._size += value_size
-            self._properties.setdefault(prop.name, list())
-            if value not in self._properties[prop.name]:
-                self._properties[prop.name].append(value)
-        return None
+
+        if value is None:
+            return None
+
+        # Somewhat hacky: limit the maximum size of any particular
+        # field to avoid overloading upstream aleph/elasticsearch.
+        value_size = len(value)
+        if prop.type.max_size is not None:
+            if self._size + value_size > prop.type.max_size:
+                # msg = "[%s] too large. Rejecting additional values."
+                # log.warning(msg, prop.name)
+                return None
+        self._size += value_size
+        self._properties.setdefault(prop.name, list())
+
+        if value not in self._properties[prop.name]:
+            self._properties[prop.name].append(value)
+
+        return value
 
     def set(
         self,
         prop: P,
         values: Any,
         cleaned: bool = False,
         quiet: bool = False,
@@ -420,17 +427,20 @@
 
     def to_dict(self) -> Dict[str, Any]:
         """Serialise the proxy into a dictionary with the defined properties, ID,
         schema and any contextual values that were handed in initially. The resulting
         dictionary can be used to make a new proxy, and it is commonly written to disk
         or a database."""
         data = dict(self.context)
-        data.update(
-            {"id": self.id, "schema": self.schema.name, "properties": self.properties}
-        )
+        extra = {
+            "id": self.id,
+            "schema": self.schema.name,
+            "properties": self.properties,
+        }
+        data.update(extra)
         return data
 
     def to_full_dict(self, matchable: bool = False) -> Dict[str, Any]:
         """Return a serialised version of the entity with inverted type groups mixed
         in. See :meth:`~get_type_inverted`."""
         data = self.to_dict()
         data.update(self.get_type_inverted(matchable=matchable))
```

### Comparing `followthemoney-3.5.9/followthemoney/schema/Address.yaml` & `followthemoney-3.6.0/followthemoney/schema/Address.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Airplane.yaml` & `followthemoney-3.6.0/followthemoney/schema/Airplane.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Analyzable.yaml` & `followthemoney-3.6.0/followthemoney/schema/Analyzable.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     companiesMentioned:
       label: "Detected companies"
       hidden: true
       type: name
     ibanMentioned:
       label: "Detected IBANs"
       hidden: true
+      # type: identifier
+      # format: iban
       type: iban
     ipMentioned:
       label: "Detected IP addresses"
       hidden: true
       type: ip
     locationMentioned:
       label: "Detected locations"
```

### Comparing `followthemoney-3.5.9/followthemoney/schema/Assessment.yaml` & `followthemoney-3.6.0/followthemoney/schema/Assessment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Associate.yaml` & `followthemoney-3.6.0/followthemoney/schema/Associate.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/BankAccount.yaml` & `followthemoney-3.6.0/followthemoney/schema/BankAccount.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,21 @@
     bankName:
       label: Bank name
     accountNumber:
       label: Account number
       type: identifier
     iban:
       label: IBAN
+      # type: identifier
+      # format: iban
       type: iban
     bic:
       label: Bank Identifier Code
       type: identifier
+      format: bic
     bank:
       label: Bank
       type: entity
       range: Organization
       reverse:
         name: bankAccounts
         label: "Bank accounts"
```

### Comparing `followthemoney-3.5.9/followthemoney/schema/Call.yaml` & `followthemoney-3.6.0/followthemoney/schema/Call.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/CallForTenders.yaml` & `followthemoney-3.6.0/followthemoney/schema/CallForTenders.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Company.yaml` & `followthemoney-3.6.0/followthemoney/schema/Company.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Contract.yaml` & `followthemoney-3.6.0/followthemoney/schema/Contract.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/ContractAward.yaml` & `followthemoney-3.6.0/followthemoney/schema/ContractAward.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/CourtCase.yaml` & `followthemoney-3.6.0/followthemoney/schema/CourtCase.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/CourtCaseParty.yaml` & `followthemoney-3.6.0/followthemoney/schema/CourtCaseParty.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/CryptoWallet.yaml` & `followthemoney-3.6.0/followthemoney/schema/CryptoWallet.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Debt.yaml` & `followthemoney-3.6.0/followthemoney/schema/Debt.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Directorship.yaml` & `followthemoney-3.6.0/followthemoney/schema/Directorship.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Document.yaml` & `followthemoney-3.6.0/followthemoney/schema/Document.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Documentation.yml` & `followthemoney-3.6.0/followthemoney/schema/Documentation.yml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/EconomicActivity.yaml` & `followthemoney-3.6.0/followthemoney/schema/EconomicActivity.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Email.yaml` & `followthemoney-3.6.0/followthemoney/schema/Email.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Employment.yaml` & `followthemoney-3.6.0/followthemoney/schema/Employment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Event.yaml` & `followthemoney-3.6.0/followthemoney/schema/Event.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Family.yaml` & `followthemoney-3.6.0/followthemoney/schema/Family.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Identification.yaml` & `followthemoney-3.6.0/followthemoney/schema/Identification.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Interval.yaml` & `followthemoney-3.6.0/followthemoney/schema/Interval.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/LegalEntity.yaml` & `followthemoney-3.6.0/followthemoney/schema/LegalEntity.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -103,31 +103,35 @@
       description: "Russian industry classifier"
       type: identifier
       matchable: false
     innCode:
       label: "INN"
       description: "Russian company ID"
       type: identifier
+      # format: inn
     ogrnCode:
       label: "OGRN"
       description: "Major State Registration Number"
       type: identifier
+      # format: ogrn
     leiCode:
       # cf. https://www.gleif.org/en/about-lei/introducing-the-legal-entity-identifier-lei
       label: "LEI"
       description: "Legal Entity Identifier"
       type: identifier
+      format: lei
     dunsCode:
       label: "D-U-N-S"
       description: "Dun & Bradstreet identifier"
       type: identifier
     swiftBic:
       label: "SWIFT/BIC"
       description: "Bank identifier code"
       type: identifier
+      format: bic
     parent:
       label: "Parent company"
       description: "If this entity is a subsidiary, another entity (company or organisation) is its parent"
       reverse:
         label: "Subsidiaries"
         name: subsidiaries
       type: entity
```

### Comparing `followthemoney-3.5.9/followthemoney/schema/Membership.yaml` & `followthemoney-3.6.0/followthemoney/schema/Membership.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Mention.yaml` & `followthemoney-3.6.0/followthemoney/schema/Mention.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Message.yaml` & `followthemoney-3.6.0/followthemoney/schema/Message.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Occupancy.yaml` & `followthemoney-3.6.0/followthemoney/schema/Occupancy.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Ownership.yaml` & `followthemoney-3.6.0/followthemoney/schema/Ownership.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Page.yaml` & `followthemoney-3.6.0/followthemoney/schema/Page.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Passport.yaml` & `followthemoney-3.6.0/followthemoney/schema/Passport.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Payment.yaml` & `followthemoney-3.6.0/followthemoney/schema/Payment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Person.yaml` & `followthemoney-3.6.0/followthemoney/schema/Person.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,18 @@
       - birthDate
     end:
       - deathDate
   properties:
     title:
       label: Title
       rdf: http://xmlns.com/foaf/0.1/title
+    # The `firstName`, `lastName`, `secondName` etc. properties intentionally do not use
+    # the `name` property type. Many FtM tools (including Aleph) use name properties to
+    # compare/match entities, but matching entites just on e.g. a first name would lead to
+    # too many false positives.
     firstName:
       label: First name
       rdf: http://xmlns.com/foaf/0.1/givenName
     secondName:
       label: Second name
     middleName:
       label: Middle name
```

### Comparing `followthemoney-3.5.9/followthemoney/schema/Position.yaml` & `followthemoney-3.6.0/followthemoney/schema/Position.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Post.yaml` & `followthemoney-3.6.0/followthemoney/schema/Post.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/ProjectParticipant.yaml` & `followthemoney-3.6.0/followthemoney/schema/ProjectParticipant.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/RealEstate.yaml` & `followthemoney-3.6.0/followthemoney/schema/RealEstate.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Representation.yaml` & `followthemoney-3.6.0/followthemoney/schema/Representation.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Sanction.yaml` & `followthemoney-3.6.0/followthemoney/schema/Sanction.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Security.yaml` & `followthemoney-3.6.0/followthemoney/schema/Security.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -19,23 +19,25 @@
     end:
       - maturityDate
   properties:
     isin:
       label: ISIN
       description: International Securities Identification Number
       type: identifier
+      format: isin
     registrationNumber:
       label: Registration number
       type: identifier
     ticker:
       label: Stock ticker symbol
       type: identifier
     figiCode:
       label: Financial Instrument Global Identifier
       type: identifier
+      format: figi
     issuer:
       label: "Issuer"
       type: entity
       range: LegalEntity
       reverse:
         label: "Issued securities"
         name: securities
```

### Comparing `followthemoney-3.5.9/followthemoney/schema/Similar.yaml` & `followthemoney-3.6.0/followthemoney/schema/Similar.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Succession.yaml` & `followthemoney-3.6.0/followthemoney/schema/Succession.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Table.yaml` & `followthemoney-3.6.0/followthemoney/schema/Table.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/TaxRoll.yaml` & `followthemoney-3.6.0/followthemoney/schema/TaxRoll.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Thing.yaml` & `followthemoney-3.6.0/followthemoney/schema/Thing.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
       matchable: false
     wikipediaUrl:
       label: Wikipedia Article
       type: url
     wikidataId:
       label: Wikidata ID
       type: identifier
+      format: qid
     keywords:
       label: Keywords
     topics:
       label: Topics
       type: topic
     address:
       label: Address
```

### Comparing `followthemoney-3.5.9/followthemoney/schema/Trip.yaml` & `followthemoney-3.6.0/followthemoney/schema/Trip.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/UnknownLink.yaml` & `followthemoney-3.6.0/followthemoney/schema/UnknownLink.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/UserAccount.yaml` & `followthemoney-3.6.0/followthemoney/schema/UserAccount.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Vehicle.yaml` & `followthemoney-3.6.0/followthemoney/schema/Vehicle.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema/Vessel.yaml` & `followthemoney-3.6.0/followthemoney/schema/Vessel.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/schema.py` & `followthemoney-3.6.0/followthemoney/schema.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.6.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.6.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.6.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/de/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.6.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/es/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.6.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/fr/followthemoney.po` & `followthemoney-3.6.0/followthemoney/translations/fr/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/messages.pot` & `followthemoney-3.6.0/followthemoney/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.6.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/ru/followthemoney.po` & `followthemoney-3.6.0/followthemoney/translations/ru/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po` & `followthemoney-3.6.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/types/__init__.py` & `followthemoney-3.6.0/followthemoney/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from followthemoney.types.registry import Registry
 from followthemoney.types.url import UrlType
 from followthemoney.types.name import NameType
 from followthemoney.types.email import EmailType
 from followthemoney.types.ip import IpType
-from followthemoney.types.iban import IbanType
 from followthemoney.types.address import AddressType
 from followthemoney.types.date import DateType
 from followthemoney.types.phone import PhoneType
 from followthemoney.types.country import CountryType
 from followthemoney.types.language import LanguageType
 from followthemoney.types.mimetype import MimeType
 from followthemoney.types.checksum import ChecksumType
 from followthemoney.types.identifier import IdentifierType
+from followthemoney.types.iban import IbanType
 from followthemoney.types.entity import EntityType
 from followthemoney.types.topic import TopicType
 from followthemoney.types.gender import GenderType
 from followthemoney.types.json import JsonType
 from followthemoney.types.string import TextType
 from followthemoney.types.string import HTMLType
 from followthemoney.types.string import StringType
@@ -23,23 +23,23 @@
 from followthemoney.types.common import PropertyType
 
 registry = Registry()
 registry.add(UrlType)
 registry.add(NameType)
 registry.add(EmailType)
 registry.add(IpType)
-registry.add(IbanType)
 registry.add(AddressType)
 registry.add(DateType)
 registry.add(PhoneType)
 registry.add(CountryType)
 registry.add(LanguageType)
 registry.add(MimeType)
 registry.add(ChecksumType)
 registry.add(IdentifierType)
+registry.add(IbanType)  # TODO: remove
 registry.add(EntityType)
 registry.add(TopicType)
 registry.add(GenderType)
 registry.add(JsonType)
 registry.add(TextType)
 registry.add(HTMLType)
 registry.add(StringType)
```

### Comparing `followthemoney-3.5.9/followthemoney/types/address.py` & `followthemoney-3.6.0/followthemoney/types/address.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/types/checksum.py` & `followthemoney-3.6.0/followthemoney/types/checksum.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/types/common.py` & `followthemoney-3.6.0/followthemoney/types/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from inspect import cleandoc
 from itertools import product
 from babel.core import Locale
 from banal import ensure_list
 from normality import stringify
 from typing import Any, Dict, Optional, Sequence, Callable, TYPE_CHECKING, TypedDict
 
 from followthemoney.rdf import Literal, Identifier
@@ -60,20 +61,25 @@
     """Some types have overall size limitations in place in order to avoid generating
     entities that are very large (upstream ElasticSearch has a 100MB document limit).
     Once the total size of all properties of this type has exceed the given limit,
     an entity will refuse to add further values."""
 
     @property
     def docs(self) -> Optional[str]:
-        return self.__doc__
+        if not self.__doc__:
+            return None
+
+        return cleandoc(self.__doc__)
 
-    def validate(self, value: str) -> bool:
+    def validate(
+        self, value: str, fuzzy: bool = False, format: Optional[str] = None
+    ) -> bool:
         """Returns a boolean to indicate if the given value is a valid instance of
         the type."""
-        cleaned = self.clean(value)
+        cleaned = self.clean(value, fuzzy=fuzzy, format=format)
         return cleaned is not None
 
     def clean(
         self,
         raw: Any,
         fuzzy: bool = False,
         format: Optional[str] = None,
@@ -137,15 +143,15 @@
         self,
         left: Sequence[str],
         right: Sequence[str],
         func: Callable[[Sequence[float]], float] = max,
     ) -> float:
         """Compare two sets of values and select the highest-scored result."""
         results = []
-        for (l, r) in product(ensure_list(left), ensure_list(right)):
+        for l, r in product(ensure_list(left), ensure_list(right)):
             results.append(self.compare(l, r))
         if not len(results):
             return 0.0
         return func(results)
 
     def country_hint(self, value: str) -> Optional[str]:
         """Determine if the given value allows us to infer a country that it may
@@ -225,15 +231,17 @@
         """Return a mapping from property values to their labels in the current
         locale."""
         locale = get_locale()
         if locale not in self._names:
             self._names[locale] = self._locale_names(locale)
         return self._names[locale]
 
-    def validate(self, value: str) -> bool:
+    def validate(
+        self, value: str, fuzzy: bool = False, format: Optional[str] = None
+    ) -> bool:
         """Make sure that the given code value is one of the supported set."""
         if value is None:
             return False
         return str(value).lower().strip() in self.codes
 
     def clean_text(
         self,
```

### Comparing `followthemoney-3.5.9/followthemoney/types/country.py` & `followthemoney-3.6.0/followthemoney/types/country.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/types/date.py` & `followthemoney-3.6.0/followthemoney/types/date.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,22 @@
 
     name = "date"
     group = "dates"
     label = _("Date")
     plural = _("Dates")
     matchable = True
 
-    def validate(self, value: str) -> bool:
+    def validate(
+        self, value: str, fuzzy: bool = False, format: Optional[str] = None
+    ) -> bool:
         """Check if a thing is a valid date."""
-        prefix = parse(value)
+        if format is not None:
+            prefix = parse_format(value, format)
+        else:
+            prefix = parse(value)
         return prefix.precision != Precision.EMPTY
 
     def clean_text(
         self,
         text: str,
         fuzzy: bool = False,
         format: Optional[str] = None,
```

### Comparing `followthemoney-3.5.9/followthemoney/types/email.py` & `followthemoney-3.6.0/followthemoney/types/email.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,17 @@
     #     try:
     #         domain = domain.encode('idna').lower()
     #         socket.getaddrinfo(domain, None)
     #         return True
     #     except:
     #         return False
 
-    def validate(self, value: str) -> bool:
+    def validate(
+        self, value: str, fuzzy: bool = False, format: Optional[str] = None
+    ) -> bool:
         """Check to see if this is a valid email address."""
         # TODO: adopt email.utils.parseaddr
         email = sanitize_text(value)
         if email is None or not self.REGEX.match(email):
             return False
         _, domain = email.rsplit("@", 1)
         if len(domain) < 4 or "." not in domain:
```

### Comparing `followthemoney-3.5.9/followthemoney/types/entity.py` & `followthemoney-3.6.0/followthemoney/types/entity.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,17 @@
     name = "entity"
     group = "entities"
     label = _("Entity")
     plural = _("Entities")
     matchable = True
     pivot = True
 
-    def validate(self, value: str) -> bool:
+    def validate(
+        self, value: str, fuzzy: bool = False, format: Optional[str] = None
+    ) -> bool:
         text = sanitize_text(value)
         if text is None:
             return False
         return self.REGEX.match(text) is not None
 
     def clean(
         self,
```

### Comparing `followthemoney-3.5.9/followthemoney/types/gender.py` & `followthemoney-3.6.0/followthemoney/types/gender.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/types/iban.py` & `followthemoney-3.6.0/followthemoney/types/iban.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from typing import Optional, TYPE_CHECKING, cast
-from stdnum import iban  # type: ignore
-from stdnum.exceptions import ValidationError  # type: ignore
+from typing import Optional, TYPE_CHECKING
+from rigour.ids import IBAN
 
 from followthemoney.types.common import PropertyType
 from followthemoney.rdf import URIRef, Identifier
 from followthemoney.util import sanitize_text, defer as _
 
 if TYPE_CHECKING:
     from followthemoney.proxy import EntityProxy
@@ -22,36 +21,35 @@
     name = "iban"
     group = "ibans"
     label = _("IBAN")
     plural = _("IBANs")
     matchable = True
     pivot = True
 
-    def validate(self, value: str) -> bool:
+    def validate(self, value: str, fuzzy: bool = False, format: Optional[str] = None) -> bool:
         text = sanitize_text(value)
-        try:
-            return cast(bool, iban.validate(text))
-        except ValidationError:
+        if text is None:
             return False
+        return IBAN.is_valid(text)
 
     def clean_text(
         self,
         text: str,
         fuzzy: bool = False,
         format: Optional[str] = None,
         proxy: Optional["EntityProxy"] = None,
     ) -> Optional[str]:
         """Create a more clean, but still user-facing version of an
         instance of the type."""
-        return text.replace(" ", "").upper()
+        return IBAN.normalize(text)
 
     def country_hint(self, value: str) -> str:
         return value[:2].lower()
 
     def rdf(self, value: str) -> Identifier:
         return URIRef(self.node_id(value))
 
     def node_id(self, value: str) -> str:
         return f"iban:{value.upper()}"
 
     def caption(self, value: str) -> str:
-        return cast(str, iban.format(value))
+        return IBAN.format(value)
```

### Comparing `followthemoney-3.5.9/followthemoney/types/identifier.py` & `followthemoney-3.6.0/followthemoney/types/identifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import re
+from typing import Optional, TYPE_CHECKING
+from rigour.ids import get_identifier_format_names, get_identifier_format
 
 from followthemoney.types.common import PropertyType
 from followthemoney.util import dampen, shortest, longest
 from followthemoney.util import defer as _
 
+if TYPE_CHECKING:
+    from followthemoney.proxy import EntityProxy
+
 
 class IdentifierType(PropertyType):
     """Used for registration numbers and other codes assigned by an authority
     to identify an entity. This might include tax identifiers and statistical
     codes.
 
     Since identifiers are high-value criteria when comparing two entities, numbers
@@ -18,14 +23,26 @@
     name = "identifier"
     group = "identifiers"
     label = _("Identifier")
     plural = _("Identifiers")
     matchable = True
     pivot = True
 
+    def clean_text(
+        self,
+        text: str,
+        fuzzy: bool = False,
+        format: Optional[str] = None,
+        proxy: Optional["EntityProxy"] = None,
+    ) -> Optional[str]:
+        if format in get_identifier_format_names():
+            format_ = get_identifier_format(format)
+            return format_.normalize(text)
+        return text
+
     def clean_compare(self, value: str) -> str:
         # TODO: should this be used for normalization?
         value = self.COMPARE_CLEAN.sub("", value)
         return value.lower()
 
     def compare(self, left: str, right: str) -> float:
         left = self.clean_compare(left)
```

### Comparing `followthemoney-3.5.9/followthemoney/types/ip.py` & `followthemoney-3.6.0/followthemoney/types/ip.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,17 @@
     name = "ip"
     group = "ips"
     label = _("IP-Address")
     plural = _("IP-Addresses")
     matchable = True
     pivot = True
 
-    def validate(self, value: str) -> bool:
+    def validate(
+        self, value: str, fuzzy: bool = False, format: Optional[str] = None
+    ) -> bool:
         """Check to see if this is a valid ip address."""
         try:
             ip_address(value)
             return True
         except ValueError:
             return False
```

### Comparing `followthemoney-3.5.9/followthemoney/types/json.py` & `followthemoney-3.6.0/followthemoney/types/json.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/types/language.py` & `followthemoney-3.6.0/followthemoney/types/language.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, TYPE_CHECKING
 from babel.core import Locale
-from languagecodes import iso_639_alpha3
+from rigour.langs import iso_639_alpha3
 
 from followthemoney.types.common import EnumType, EnumValues
 from followthemoney.rdf import URIRef, Identifier
 from followthemoney.util import defer as _
 from followthemoney.util import get_env_list
 
 if TYPE_CHECKING:
```

### Comparing `followthemoney-3.5.9/followthemoney/types/mimetype.py` & `followthemoney-3.6.0/followthemoney/types/mimetype.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, TYPE_CHECKING
-from pantomime import normalize_mimetype, parse_mimetype
-from pantomime import DEFAULT
+from rigour.mime import normalize_mimetype, parse_mimetype
+from rigour.mime import DEFAULT
 
 from followthemoney.types.common import PropertyType
 from followthemoney.rdf import URIRef, Identifier
 from followthemoney.util import defer as _
 
 if TYPE_CHECKING:
     from followthemoney.proxy import EntityProxy
```

### Comparing `followthemoney-3.5.9/followthemoney/types/name.py` & `followthemoney-3.6.0/followthemoney/types/name.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import TYPE_CHECKING, Dict, List, Optional, Sequence, Union
-
-from Levenshtein import distance, setmedian
+from typing import TYPE_CHECKING, Optional, Sequence
+from rigour.text.distance import levenshtein_similarity
+from rigour.names import pick_name
 from normality import slugify
 from normality.cleaning import collapse_spaces, strip_quotes
 
 from followthemoney.types.common import PropertyType
 from followthemoney.util import dampen
 from followthemoney.util import defer as _
 
@@ -36,51 +36,22 @@
     ) -> Optional[str]:
         """Basic clean-up."""
         name = strip_quotes(text)
         return collapse_spaces(name)
 
     def pick(self, values: Sequence[str]) -> Optional[str]:
         """From a set of names, pick the most plausible user-facing one."""
-        # Sort to get stable results when it's a coin toss:
-        values = sorted(values)
-        if not len(values):
-            return None
-        normalised: List[Union[str, bytes]] = []
-        lookup: Dict[str, List[Union[str, bytes]]] = {}
-        # We're doing this in two stages, to avoid name forms with varied casing
-        # (e.g. Smith vs. SMITH) are counted as widly different, leading to
-        # implausible median outcomes.
-        for value in values:
-            norm = slugify(value, sep=" ")
-            if norm is None:
-                continue
-            normalised.append(norm)
-            lookup.setdefault(norm, [])
-            lookup[norm].append(value)
-
-        if not normalised:
-            return None
-
-        norm = setmedian(normalised)
-        if norm is None:
-            return None
-        forms = lookup.get(norm, [])
-        if len(forms) > 1:
-            return setmedian(forms)
-        for form in forms:
-            return str(form)
-        return None
+        return pick_name(list(values))
 
     def _specificity(self, value: str) -> float:
         # TODO: insert artificial intelligence here.
         return dampen(3, 50, value)
 
     def compare(self, left: str, right: str) -> float:
-        longest = float(max(len(left), len(right), 1))
-        edits = float(distance(left[:255], right[:255]))
-        return (longest - edits) / longest
+        """Compare two names for similarity."""
+        return levenshtein_similarity(left, right)
 
     def node_id(self, value: str) -> Optional[str]:
         slug = slugify(value)
         if slug is None:
             return None
         return f"name:{slug}"
```

### Comparing `followthemoney-3.5.9/followthemoney/types/number.py` & `followthemoney-3.6.0/followthemoney/types/number.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/types/phone.py` & `followthemoney-3.6.0/followthemoney/types/phone.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,17 @@
         """
         for code in self._clean_countries(proxy):
             try:
                 yield parse_number(number, code)
             except NumberParseException:
                 pass
 
-    def validate(self, value: str) -> bool:
+    def validate(
+        self, value: str, fuzzy: bool = False, format: Optional[str] = None
+    ) -> bool:
         for num in self._parse_number(value):
             if is_valid_number(num):
                 return True
         return False
 
     def clean_text(
         self,
```

### Comparing `followthemoney-3.5.9/followthemoney/types/registry.py` & `followthemoney-3.6.0/followthemoney/types/registry.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/types/string.py` & `followthemoney-3.6.0/followthemoney/types/string.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney/types/topic.py` & `followthemoney-3.6.0/followthemoney/types/topic.py`

 * *Files 15% similar despite different names*

```diff
@@ -52,15 +52,18 @@
         "gov.judicial": _("Judicial branch of government"),
         "gov.security": _("Security services"),
         "gov.financial": _("Central banking and financial integrity"),
         "fin": _("Financial services"),
         "fin.bank": _("Bank"),
         "fin.fund": _("Fund"),
         "fin.adivsor": _("Financial advisor"),
-        "role.pep": _("Political"),
+        "reg.action": _("Regulator action"),
+        "reg.warn": _("Regulator warning"),
+        "role.pep": _("Politican"),
+        "role.pol": _("Non-PEP"),
         "role.rca": _("Close Associate"),
         "role.judge": _("Judge"),
         "role.civil": _("Civil servant"),
         "role.diplo": _("Diplomat"),
         "role.lawyer": _("Lawyer"),
         "role.acct": _("Accountant"),
         "role.spy": _("Spy"),
@@ -70,14 +73,15 @@
         "pol.party": _("Political party"),
         "pol.union": _("Union"),
         "rel": _("Religion"),
         "mil": _("Military"),
         "asset.frozen": _("Frozen asset"),
         "sanction": _("Sanctioned entity"),
         "sanction.linked": _("Sanction-linked entity"),
+        "sanction.counter": _("Counter-sanctioned entity"),
         "export.control": _("Export controlled"),
         "debarment": _("Debarred entity"),
         "poi": _("Person of interest"),
     }
 
     def _locale_names(self, locale: Locale) -> EnumValues:
         return {k: gettext(v) for (k, v) in self._TOPICS.items()}
```

### Comparing `followthemoney-3.5.9/followthemoney/types/url.py` & `followthemoney-3.6.0/followthemoney/types/url.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, TYPE_CHECKING
-from urllib.parse import urlparse
+from rigour.urls import clean_url, compare_urls
 
 from followthemoney.types.common import PropertyType
 from followthemoney.rdf import URIRef, Identifier
 from followthemoney.util import dampen, defer as _
 
 if TYPE_CHECKING:
     from followthemoney.proxy import EntityProxy
@@ -29,34 +29,18 @@
         text: str,
         fuzzy: bool = False,
         format: Optional[str] = None,
         proxy: Optional["EntityProxy"] = None,
     ) -> Optional[str]:
         """Perform intensive care on URLs to make sure they have a scheme
         and a host name. If no scheme is given HTTP is assumed."""
-        try:
-            parsed = urlparse(text)
-        except (TypeError, ValueError):
-            return None
-        if not len(parsed.netloc):
-            if "." in parsed.path and not text.startswith("//"):
-                # This is a pretty weird rule meant to catch things like
-                # 'www.google.com', but it'll likely backfire in some
-                # really creative ways.
-                return self.clean_text(f"//{text}")
-            return None
-        if not len(parsed.scheme):
-            parsed = parsed._replace(scheme=self.DEFAULT_SCHEME)
-        else:
-            parsed = parsed._replace(scheme=parsed.scheme.lower())
-        if parsed.scheme not in self.SCHEMES:
-            return None
-        if not len(parsed.path):
-            parsed = parsed._replace(path="/")
-        return parsed.geturl()
+        return clean_url(text)
+
+    def compare(self, left: str, right: str) -> float:
+        return compare_urls(left, right)
 
     def _specificity(self, value: str) -> float:
         return dampen(10, 120, value)
 
     def rdf(self, value: str) -> Identifier:
         return URIRef(value)
```

### Comparing `followthemoney-3.5.9/followthemoney/util.py` & `followthemoney-3.6.0/followthemoney/util.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney.egg-info/PKG-INFO` & `followthemoney-3.6.0/followthemoney.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,90 @@
 Metadata-Version: 2.1
 Name: followthemoney
-Version: 3.5.9
-Summary: UNKNOWN
+Version: 3.6.0
 Home-page: https://followthemoney.tech/
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
-Description: # Follow the Money
-        
-        [![ftm-build](https://github.com/alephdata/followthemoney/actions/workflows/build.yml/badge.svg)](https://github.com/alephdata/followthemoney/actions/workflows/build.yml)
-        
-        This repository contains a pragmatic data model for the entities most
-        commonly used in investigative reporting: people, companies, assets,
-        payments, court cases, etc.
-        
-        The purpose of this is not to model reality in an ideal data model, but
-        rather to have a working data structure for researchers.
-        
-        `followthemoney` also contains code used to validate and normalize many
-        of the elements of data, and to map tabular data into the model.
-        
-        ## Documentation
-        
-        For a general introduction to `followthemoney`, check the high-level introduction:
-        
-        * https://followthemoney.tech
-        
-        Part of this package is a command-line tool that can be used to process and
-        transform data in various ways. You can find a tutorial here:
-        
-        * https://followthemoney.tech/docs/cli/
-        
-        Besides the introductions, there is also a full reference documentation for the
-        library and the contained ontology: 
-        
-        * https://followthemoney.tech/explorer/
-        
-        There's also a number of viewers for the RDF schema definitions generated
-        from FollowTheMoney, e.g.:
-        
-        * [LODE documentation](http://150.146.207.114/lode/extract?url=https%3A%2F%2Falephdata.github.io%2Ffollowthemoney%2Fns%2Fftm.xml&owlapi=true&imported=true&lang=en)
-        * [WebVOWL](https://service.tib.eu/webvowl/#iri=https://alephdata.github.io/followthemoney/ns/ftm.xml)
-        * RDF/OWL specification in [XML](https://alephdata.github.io/followthemoney/ns/ftm.xml).
-        
-        ## Development environment
-        
-        For local development with a virtualenv:
-        
-        ```bash
-        python3 -mvenv .env
-        source .env/bin/activate
-        pip install -e ".[dev]"
-        ```
-        
-        Now you can run the tests with
-        
-        ```bash
-        make test
-        ```
-        
-        ## Releasing
-        
-        We release a lot of version of `followthemoney` because even small changes
-        to the code base require a pypi release to begin being used in `aleph`. To
-        this end, here's the steps for making a release:
-        
-        ```bash
-        git pull --rebase
-        make build
-        make test
-        git add . && git commit -m "Updating translation files"
-        bumpversion patch
-        git push --atomic origin main $(git describe --tags --abbrev=0)
-        ```
-        
-        This will create a new patch release and upload a distribution of it. If
-        the changes are more significant, you can run `bumpversion` with the `minor`
-        or `major` arguments.
-        
-        When the schema is updated, please update the docs, ideally including the
-        diagrams. For the RDF namespace and JavaScript version of the model, 
-        run `make generate`.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# Follow the Money
+
+[![ftm-build](https://github.com/alephdata/followthemoney/actions/workflows/build.yml/badge.svg)](https://github.com/alephdata/followthemoney/actions/workflows/build.yml)
+
+This repository contains a pragmatic data model for the entities most
+commonly used in investigative reporting: people, companies, assets,
+payments, court cases, etc.
+
+The purpose of this is not to model reality in an ideal data model, but
+rather to have a working data structure for researchers.
+
+`followthemoney` also contains code used to validate and normalize many
+of the elements of data, and to map tabular data into the model.
+
+## Documentation
+
+For a general introduction to `followthemoney`, check the high-level introduction:
+
+* https://followthemoney.tech
+
+Part of this package is a command-line tool that can be used to process and
+transform data in various ways. You can find a tutorial here:
+
+* https://followthemoney.tech/docs/cli/
+
+Besides the introductions, there is also a full reference documentation for the
+library and the contained ontology: 
+
+* https://followthemoney.tech/explorer/
+
+There's also a number of viewers for the RDF schema definitions generated
+from FollowTheMoney, e.g.:
+
+* [LODE documentation](http://150.146.207.114/lode/extract?url=https%3A%2F%2Falephdata.github.io%2Ffollowthemoney%2Fns%2Fftm.xml&owlapi=true&imported=true&lang=en)
+* [WebVOWL](https://service.tib.eu/webvowl/#iri=https://alephdata.github.io/followthemoney/ns/ftm.xml)
+* RDF/OWL specification in [XML](https://alephdata.github.io/followthemoney/ns/ftm.xml).
+
+## Development environment
+
+For local development with a virtualenv:
+
+```bash
+python3 -mvenv .env
+source .env/bin/activate
+pip install -e ".[dev]"
+```
+
+Now you can run the tests with
+
+```bash
+make test
+```
+
+## Releasing
+
+We release a lot of version of `followthemoney` because even small changes
+to the code base require a pypi release to begin being used in `aleph`. To
+this end, here's the steps for making a release:
+
+```bash
+git pull --rebase
+make build
+make test
+git add . && git commit -m "Updating translation files"
+bumpversion patch
+git push --atomic origin main $(git describe --tags --abbrev=0)
+```
+
+This will create a new patch release and upload a distribution of it. If
+the changes are more significant, you can run `bumpversion` with the `minor`
+or `major` arguments.
+
+When the schema is updated, please update the docs, ideally including the
+diagrams. For the RDF namespace and JavaScript version of the model, 
+run `make generate`.
```

### Comparing `followthemoney-3.5.9/followthemoney.egg-info/SOURCES.txt` & `followthemoney-3.6.0/followthemoney.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `followthemoney-3.5.9/followthemoney.egg-info/entry_points.txt` & `followthemoney-3.6.0/followthemoney.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,7 @@
 csv = followthemoney.cli.exports:export_csv
 cypher = followthemoney.cli.exports:export_cypher
 excel = followthemoney.cli.exports:export_excel
 gexf = followthemoney.cli.exports:export_gexf
 mapping = followthemoney.cli.mapping:run_mapping
 rdf = followthemoney.cli.exports:export_rdf
 sieve = followthemoney.cli.sieve:sieve
-
```

### Comparing `followthemoney-3.5.9/followthemoney.egg-info/requires.txt` & `followthemoney-3.6.0/followthemoney.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-babel<3.0.0,>=2.9.1
+babel<3.0.0,>=2.14.0
 pyyaml<7.0.0,>=5.0.0
 types-PyYAML
 sqlalchemy2-stubs
 banal<1.1.0,>=1.0.6
+rigour<1.0.0,>=0.5.1
 click<9.0.0,>=8.0
 stringcase<2.0.0,>=1.2.0
 requests<3.0.0,>=2.21.0
-python-levenshtein<1.0.0,>=0.12.0
 normality<3.0.0,>=2.4.0
 sqlalchemy<3.0.0,>=1.4.49
 countrynames<2.0.0,>=1.13.0
-languagecodes<2.0.0,>=1.1.0
 prefixdate<1.0.0,>=0.4.0
 fingerprints<2.0.0,>=1.0.1
 phonenumbers<9.0.0,>=8.12.22
 python-stdnum<2.0.0,>=1.16
-pantomime<1.0.0,>=0.5.1
 pytz>=2021.1
 rdflib<7.1.0,>=6.2.0
-networkx<3.3,>=2.5
+networkx<3.4,>=2.5
 openpyxl<4.0.0,>=3.0.5
 orjson<4.0,>=3.7
 
 [dev]
 pip>=10.0.0
 bump2version
 wheel>=0.29.0
 twine
 mypy
 pytest
 pytest-cov
 types-PyYAML
 types-requests
 types-setuptools
+types-openpyxl
 flake8>=2.6.0
 transifex-client
 responses>=0.9.0
 coverage>=4.1
 recommonmark>=0.4.0
```

### Comparing `followthemoney-3.5.9/setup.py` & `followthemoney-3.6.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages  # type: ignore
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="followthemoney",
-    version="3.5.9",
+    version="3.6.0",
     author="Organized Crime and Corruption Reporting Project",
     author_email="data@occrp.org",
     url="https://followthemoney.tech/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
@@ -26,35 +26,33 @@
             "followthemoney/schema/*",
             "followthemoney/translations/*",
             "followthemoney/py.typed",
         ]
     },
     zip_safe=False,
     install_requires=[
-        "babel >= 2.9.1, < 3.0.0",
+        "babel >= 2.14.0, < 3.0.0",
         "pyyaml >= 5.0.0, < 7.0.0",
         "types-PyYAML",
         "sqlalchemy2-stubs",
         "banal >= 1.0.6, < 1.1.0",
+        "rigour >= 0.5.1, < 1.0.0",
         "click >= 8.0, < 9.0.0",
         "stringcase >= 1.2.0, < 2.0.0",
         "requests >= 2.21.0, < 3.0.0",
-        "python-levenshtein >= 0.12.0, < 1.0.0",
         "normality >= 2.4.0, < 3.0.0",
         "sqlalchemy >= 1.4.49, < 3.0.0",
         "countrynames >= 1.13.0, < 2.0.0",
-        "languagecodes >= 1.1.0, < 2.0.0",
         "prefixdate >= 0.4.0, < 1.0.0",
         "fingerprints >= 1.0.1, < 2.0.0",
         "phonenumbers >= 8.12.22, < 9.0.0",
         "python-stdnum >= 1.16, < 2.0.0",
-        "pantomime >= 0.5.1, < 1.0.0",
         "pytz >= 2021.1",
         "rdflib >= 6.2.0, < 7.1.0",
-        "networkx >= 2.5, < 3.3",
+        "networkx >= 2.5, < 3.4",
         "openpyxl >= 3.0.5, < 4.0.0",
         "orjson >= 3.7, < 4.0",
     ],
     extras_require={
         "dev": [
             "pip>=10.0.0",
             "bump2version",
@@ -62,14 +60,15 @@
             "twine",
             "mypy",
             "pytest",
             "pytest-cov",
             "types-PyYAML",
             "types-requests",
             "types-setuptools",
+            "types-openpyxl",
             "flake8>=2.6.0",
             "transifex-client",
             "responses>=0.9.0",
             "coverage>=4.1",
             "recommonmark>=0.4.0",
         ],
     },
```

