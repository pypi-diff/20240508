# Comparing `tmp/pih-plb-0.20.tar.gz` & `tmp/pih-plb-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-plb-0.20.tar", last modified: Wed Apr 17 14:42:04 2024, max compression
+gzip compressed data, was "pih-plb-0.22.tar", last modified: Wed May  8 02:56:26 2024, max compression
```

## Comparing `pih-plb-0.20.tar` & `pih-plb-0.22.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 14:42:04.564057 pih-plb-0.20/
--rw-rw-rw-   0        0        0      293 2024-04-17 14:42:04.548434 pih-plb-0.20/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 14:42:04.170349 pih-plb-0.20/PolibaseService/
--rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.20/PolibaseService/__init__.py
--rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.20/PolibaseService/__main__.py
--rw-rw-rw-   0        0        0    45781 2024-04-17 14:41:03.000000 pih-plb-0.20/PolibaseService/api.py
--rw-rw-rw-   0        0        0     3618 2024-04-17 14:41:15.000000 pih-plb-0.20/PolibaseService/const.py
--rw-rw-rw-   0        0        0    14886 2024-04-17 13:38:35.000000 pih-plb-0.20/PolibaseService/service.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:42:04.501557 pih-plb-0.20/pih_plb.egg-info/
--rw-rw-rw-   0        0        0      293 2024-04-17 14:42:03.000000 pih-plb-0.20/pih_plb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-04-17 14:42:03.000000 pih-plb-0.20/pih_plb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 14:42:03.000000 pih-plb-0.20/pih_plb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-04-17 14:42:03.000000 pih-plb-0.20/pih_plb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-04-17 14:42:03.000000 pih-plb-0.20/pih_plb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-17 14:42:03.000000 pih-plb-0.20/pih_plb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 14:42:04.579679 pih-plb-0.20/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 02:56:26.815874 pih-plb-0.22/
+-rw-rw-rw-   0        0        0      293 2024-05-08 02:56:26.784624 pih-plb-0.22/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-08 02:56:26.357579 pih-plb-0.22/PolibaseService/
+-rw-rw-rw-   0        0        0        0 2023-10-13 06:33:11.000000 pih-plb-0.22/PolibaseService/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-02-14 23:40:07.000000 pih-plb-0.22/PolibaseService/__main__.py
+-rw-rw-rw-   0        0        0    45820 2024-05-08 02:28:38.000000 pih-plb-0.22/PolibaseService/api.py
+-rw-rw-rw-   0        0        0     3694 2024-05-08 02:53:02.000000 pih-plb-0.22/PolibaseService/const.py
+-rw-rw-rw-   0        0        0    14990 2024-05-08 02:40:04.000000 pih-plb-0.22/PolibaseService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-08 02:56:26.737753 pih-plb-0.22/pih_plb.egg-info/
+-rw-rw-rw-   0        0        0      293 2024-05-08 02:56:25.000000 pih-plb-0.22/pih_plb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-05-08 02:56:26.000000 pih-plb-0.22/pih_plb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 02:56:25.000000 pih-plb-0.22/pih_plb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-08 02:56:25.000000 pih-plb-0.22/pih_plb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-08 02:56:25.000000 pih-plb-0.22/pih_plb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-08 02:56:25.000000 pih-plb-0.22/pih_plb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 02:56:26.831506 pih-plb-0.22/setup.cfg
```

### Comparing `pih-plb-0.20/PolibaseService/api.py` & `pih-plb-0.22/PolibaseService/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,15 +418,15 @@
     @staticmethod
     def query_person_visits_with_condition(
         value: str, test: bool | None = None
     ) -> list[PolibasePersonVisit]:
         result: list[dict[str, Any]] = []
         with PolibaseApi.get_cursor(test) as cursor:
             query_string: str = (
-                f"select {VISIT_NO} {esc(A.CT_FNC.ID)}, {VISIT_PATIENT_NO} {esc(A.CT_FNC.PIN)}, {VISIT_PATIENT_FULL_NAME} {esc(A.CT_FNC.FULL_NAME)}, DOC.{PERSON_FULL_NAME} {esc(A.CT_FNC.DOCTOR_FULL_NAME)}, {VISIT_PATIENT_TELEPHONE_NUMBER} {esc(A.CT_FNC.TELEPHONE_NUMBER)}, {VISIT_PATIENT_REGISTRATION_DATE} {esc(A.CT_FNC.REGISTRATION_DATE)}, {VISIT_DATE_PS} {esc(A.CT_FNC.BEGIN_DATE)}, {VISIT_DATE_PF} {esc(A.CT_FNC.COMPLETE_DATE)}, {VISIT_DATE_FS} {esc(j((A.CT_FNC.BEGIN_DATE, '2')))}, {VISIT_DATE_FF} {esc(j((A.CT_FNC.COMPLETE_DATE, '2')))}, {VISIT_PATIENTS_STATUS} {esc(A.CT_FNC.STATUS)}, {VISIT_CABINET_NO} {esc(A.CT_FNC.CABINET_ID)}, {VISIT_DOCTOR_NO} {esc(A.CT_FNC.DOCTOR_ID)}, DOC.{PERSON_FULL_NAME} {esc(A.CT_FNC.DOCTOR_FULL_NAME)} from {PERSON_VISIT_TABLE_NAME} inner join {PERSON_TABLE_NAME} DOC on {VISIT_DOCTOR_NO} = DOC.{PERSON_NO} {value}"
+                f"select {VISIT_NO} {esc(A.CT_FNC.ID)}, {VISIT_NOTES} {esc(A.CT_FNC.COMMENT)}, {VISIT_PATIENT_NO} {esc(A.CT_FNC.PIN)}, {VISIT_PATIENT_FULL_NAME} {esc(A.CT_FNC.FULL_NAME)}, DOC.{PERSON_FULL_NAME} {esc(A.CT_FNC.DOCTOR_FULL_NAME)}, {VISIT_PATIENT_TELEPHONE_NUMBER} {esc(A.CT_FNC.TELEPHONE_NUMBER)}, {VISIT_PATIENT_REGISTRATION_DATE} {esc(A.CT_FNC.REGISTRATION_DATE)}, {VISIT_DATE_PS} {esc(A.CT_FNC.BEGIN_DATE)}, {VISIT_DATE_PF} {esc(A.CT_FNC.COMPLETE_DATE)}, {VISIT_DATE_FS} {esc(j((A.CT_FNC.BEGIN_DATE, '2')))}, {VISIT_DATE_FF} {esc(j((A.CT_FNC.COMPLETE_DATE, '2')))}, {VISIT_PATIENTS_STATUS} {esc(A.CT_FNC.STATUS)}, {VISIT_CABINET_NO} {esc(A.CT_FNC.CABINET_ID)}, {VISIT_DOCTOR_NO} {esc(A.CT_FNC.DOCTOR_ID)}, DOC.{PERSON_FULL_NAME} {esc(A.CT_FNC.DOCTOR_FULL_NAME)} from {PERSON_VISIT_TABLE_NAME} inner join {PERSON_TABLE_NAME} DOC on {VISIT_DOCTOR_NO} = DOC.{PERSON_NO} {value}"
             )
             result = PolibaseApi.fill_data(
                 cursor.execute(query_string), cursor.description
             )  # type: ignore
         return A.D.fill_data_from_list_source(PolibasePersonVisit, result)
 
     @staticmethod
```

### Comparing `pih-plb-0.20/PolibaseService/const.py` & `pih-plb-0.22/PolibaseService/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pih import A
 from pih.tools import j
 from pih.consts import CONST
 from pih.collections.service import ServiceDescription
 
 NAME: str = "Polibase"
 
-VERSION: str = "0.20"
+VERSION: str = "0.22"
 
 HOST = A.CT_H.POLIBASE
 
 PACKAGES: tuple[str, ...] = ("oracledb",)
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
@@ -56,16 +56,18 @@
 PERSON_PREFIX: str = "per_"
 VISIT_PREFIX: str = "vis_"
 PATIENT_PREFIX: str = "pat_"
 USER_PREFIX: str = "use_"
 PATIENT_SALDO_PREFIX: str = "psa_"
 #
 PERSON_TABLE_NAME: str = "persons"
-NOTE_EMAILED_TABLE_NAME: str = "notes_emailed"
-NOTE_TABLE_NAME: str = "notes"
+NOTES: str = "notes"
+NOTE_EMAILED_TABLE_NAME: str = j((NOTES, "_emailed"))
+
+NOTE_TABLE_NAME: str = NOTES
 PERSON_VISIT_TABLE_NAME: str = "visits"
 USERS_TABLE_NAME: str = "users"
 PATIENT_SALDO_TABLE: str = "patsaldo"
 #
 ROWID: str = "rowid"
 REGISTRATION_DATE: str = "reg_date"
 PERSON_BARCODE: str = f"{PERSON_PREFIX}bar"
@@ -74,22 +76,23 @@
 PERSON_FULL_NAME: str = f"{PERSON_PREFIX}full_name"
 PERSON_NO: str = f"{PERSON_PREFIX}{NUMBER}"
 PERSON_REGISTRATOR_NO: str = f"{PERSON_PREFIX}reg_{NUMBER}"
 PERSON_OPERATOR_NO: str = f"{PERSON_PREFIX}ope_{NUMBER}"
 PERSON_EMAIL: str = f"{PERSON_PREFIX}{A.CT_FNC.EMAIL}"
 PERSON_TELEPHONE_NUMBER: str = f"{PERSON_PREFIX}phone"
 PERSON_BIRTH: str = f"{PERSON_PREFIX}birth"
-PERSON_NOTES: str = f"{PERSON_PREFIX}notes"
+PERSON_NOTES: str = f"{PERSON_PREFIX}{NOTES}"
 PERSON_REGISTRATION_DATE: str = f"{PERSON_PREFIX}{REGISTRATION_DATE}"
 #
 NOTE_NO: str = f"{NOTE_PREFIX}{NUMBER}"
 NOTE_EMAILED: str = f"{NOTE_PREFIX}{A.CT_FNC.EMAILED}"
 #
 NAME: str = "name"
 VISIT_NO: str = f"{VISIT_PREFIX}{NUMBER}"
+VISIT_NOTES: str = f"{VISIT_PREFIX}{NOTES}"
 VISIT_DATE_PREFFIX: str = f"{VISIT_PREFIX}date_"
 VISIT_DATE_PS: str = f"{VISIT_DATE_PREFFIX}ps"
 VISIT_DATE_PF: str = f"{VISIT_DATE_PREFFIX}pf"
 VISIT_DATE_FS: str = f"{VISIT_DATE_PREFFIX}fs"
 VISIT_DATE_FF: str = f"{VISIT_DATE_PREFFIX}ff"
 VISIT_PATIENT_NO: str = f"{VISIT_PREFIX}{PATIENT_PREFIX}{NUMBER}"
 VISIT_PATIENT_FULL_NAME: str = j((VISIT_PREFIX, PATIENT_PREFIX, NAME))
```

### Comparing `pih-plb-0.20/PolibaseService/service.py` & `pih-plb-0.22/PolibaseService/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ipih
 
 from pih import A
 from PolibaseService.const import *
 
 SC = A.CT_SC
-ISOLATED: bool = False
+ISOLATED: bool = True
 DEBUG: bool = False
 
 def start(as_standalone: bool = False) -> None:
 
     if A.U.for_service(SD, as_standalone=as_standalone):
 
         from pih.collections import (
@@ -222,14 +222,15 @@
                                             complete_date, A.CT.ISO_DATETIME_FORMAT
                                         ),
                                         person_visit_item.status,
                                         person_visit_item.cabinetID,
                                         person_visit_item.doctorID,
                                         person_visit_item.doctorFullName,
                                         person_visit_item.serviceGroupID or 0,
+                                        person_visit_item.Comment
                                     )
                                 )
                             else:
                                 pass
                         else:
                             pass
                     else:
@@ -276,19 +277,19 @@
             person_saldo_data: dict[str, float | int]
         ) -> None:
             id: int = person_saldo_data[A.CT_FNC.ID]  # type: ignore
             A.D_V.set(LAST_SALDO_OPERATION_ID_NAME, id, section=SD.name)
             doctor_id: int = person_saldo_data[A.CT_FNC.DOCTOR_ID]  # type: ignore
             bonus_minus: int = person_saldo_data["bonus_minus"] or 0  # type: ignore
             bonus_plus: int = person_saldo_data["bonus_plus"] or 0  # type: ignore
-            doctor_bonus_pin_list: list[int] = A.S.get(
-                A.CT_S.BONUS_DOCTOR_PERSON_PIN_LIST
+            bonus_program_doctor_person_pin_list: list[int] = A.S.get(
+                A.CT_S.BONUS_PROGRAM_DOCTOR_PERSON_PIN_LIST
             )
             if bonus_plus > 0:
-                if doctor_id in doctor_bonus_pin_list:
+                if doctor_id in bonus_program_doctor_person_pin_list:
                     A.E.send(
                         A.CT_E.POLIBASE_PERSON_BONUSES_WAS_UPDATED,
                         (person_saldo_data[A.CT_FNC.PERSON_PIN],),
                     )
                 else:
                     Api.drop_person_bonus_by_id(id)
             if bonus_minus > 0:
```

