# Comparing `tmp/pih-answ_auto-0.20.tar.gz` & `tmp/pih-answ_auto-0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-answ_auto-0.20.tar", last modified: Fri May  3 10:35:47 2024, max compression
+gzip compressed data, was "pih-answ_auto-0.22.tar", last modified: Wed May  8 06:46:39 2024, max compression
```

## Comparing `pih-answ_auto-0.20.tar` & `pih-answ_auto-0.22.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 10:35:47.771843 pih-answ_auto-0.20/
-drwxrwxrwx   0        0        0        0 2024-05-03 10:35:47.390865 pih-answ_auto-0.20/AnswerAutomationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-answ_auto-0.20/AnswerAutomationService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-04-16 00:17:31.000000 pih-answ_auto-0.20/AnswerAutomationService/__main__.py
--rw-rw-rw-   0        0        0      412 2024-05-03 10:35:29.000000 pih-answ_auto-0.20/AnswerAutomationService/const.py
--rw-rw-rw-   0        0        0     7065 2024-05-03 10:35:19.000000 pih-answ_auto-0.20/AnswerAutomationService/service.py
--rw-rw-rw-   0        0        0      283 2024-05-03 10:35:47.739541 pih-answ_auto-0.20/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-03 10:35:47.707286 pih-answ_auto-0.20/pih_answ_auto.egg-info/
--rw-rw-rw-   0        0        0      283 2024-05-03 10:35:46.000000 pih-answ_auto-0.20/pih_answ_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2024-05-03 10:35:47.000000 pih-answ_auto-0.20/pih_answ_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 10:35:47.000000 pih-answ_auto-0.20/pih_answ_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-05-03 10:35:47.000000 pih-answ_auto-0.20/pih_answ_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-03 10:35:47.000000 pih-answ_auto-0.20/pih_answ_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-03 10:35:47.000000 pih-answ_auto-0.20/pih_answ_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 10:35:47.771843 pih-answ_auto-0.20/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-08 06:46:39.317679 pih-answ_auto-0.22/
+drwxrwxrwx   0        0        0        0 2024-05-08 06:46:36.298643 pih-answ_auto-0.22/AnswerAutomationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-answ_auto-0.22/AnswerAutomationService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-04-16 00:17:31.000000 pih-answ_auto-0.22/AnswerAutomationService/__main__.py
+-rw-rw-rw-   0        0        0      412 2024-05-08 06:46:21.000000 pih-answ_auto-0.22/AnswerAutomationService/const.py
+-rw-rw-rw-   0        0        0    10093 2024-05-08 06:40:05.000000 pih-answ_auto-0.22/AnswerAutomationService/service.py
+-rw-rw-rw-   0        0        0      283 2024-05-08 06:46:39.270801 pih-answ_auto-0.22/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-08 06:46:39.223965 pih-answ_auto-0.22/pih_answ_auto.egg-info/
+-rw-rw-rw-   0        0        0      283 2024-05-08 06:46:35.000000 pih-answ_auto-0.22/pih_answ_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2024-05-08 06:46:36.000000 pih-answ_auto-0.22/pih_answ_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 06:46:35.000000 pih-answ_auto-0.22/pih_answ_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-08 06:46:35.000000 pih-answ_auto-0.22/pih_answ_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-08 06:46:35.000000 pih-answ_auto-0.22/pih_answ_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-08 06:46:35.000000 pih-answ_auto-0.22/pih_answ_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 06:46:39.317679 pih-answ_auto-0.22/setup.cfg
```

### Comparing `pih-answ_auto-0.20/AnswerAutomationService/service.py` & `pih-answ_auto-0.22/AnswerAutomationService/service.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
 
 class ANSWER_TYPE:
 
     VISIT = 1
     TAX_CERTIFICATE = 2
     VISIT_MODIFICATION = 4
+    HOW_TO_GET = 8
+    OTHER_QUESTION: int = 16
+    # LATE = 8
 
 
 def start(as_standalone: bool = False) -> None:
 
     from pih.collections import (
         Message,
         PolibasePerson,
@@ -75,48 +78,69 @@
                                 if A.A_P_N_C.update(telephone_number, sender, 1):
 
                                     answer_type: int = 0
 
                                     message: str = nnt(nnt(whatsapp_message).message)
 
                                     if ne(message):
-
                                         for index, variants in enumerate(
                                             [
-                                                A.S.get(
-                                                    A.CT_S.POLIBASE_ANSWER_PERSON_TAX_CERTIFICATE_VARIANTS
-                                                ),
-                                                A.S.get(
-                                                    A.CT_S.POLIBASE_PERSON_ANSWER_VISIT_MODIFICATION_VARIANTS
-                                                ),
+                                                A.S.get(item)
+                                                for item in (
+                                                    A.CT_S.POLIBASE_ANSWER_PERSON_TAX_CERTIFICATE_VARIANTS,
+                                                    A.CT_S.POLIBASE_PERSON_ANSWER_VISIT_MODIFICATION_VARIANTS,
+                                                    A.CT_S.POLIBASE_PERSON_ANSWER_HOW_TO_GET_VARIANTS,
+                                                )
                                             ],
                                         ):
                                             if A.D.has_one_of(message, variants):
-                                                answer_type |= 2 ** (index + 1)
+                                                answer_type = BM.set_index(
+                                                    answer_type, index + 1
+                                                )
 
                                     if answer_type == 0:
-                                        answer_type = ANSWER_TYPE.VISIT
+                                        answer_type = (
+                                            ANSWER_TYPE.OTHER_QUESTION
+                                            if nn(message) and message.find("?") != -1
+                                            else ANSWER_TYPE.VISIT
+                                        )
 
-                                    def send_message(value: str) -> None:
+                                    def send_message(
+                                        value: str | None = None,
+                                        image_url: str | None = None,
+                                        location: tuple[float, float] | None = None,
+                                    ) -> None:
                                         A.ME_WH_W_Q.add_message(
                                             Message(
                                                 value,
                                                 telephone_number,
                                                 sender,
+                                                image_url,
+                                                location,
                                             )
                                         )
 
                                     if BM.has(answer_type, ANSWER_TYPE.VISIT):
                                         send_message(
                                             A.S_P_V.offer_telegram_bot_url_text(person)
                                         )
                                         send_message(
                                             A.S.get(A.CT_S.TELEGRAM_BOT_URL),
                                         )
 
+                                    if BM.has(answer_type, ANSWER_TYPE.OTHER_QUESTION):
+                                        send_message(
+                                            polibase_person_name_format(
+                                                A.S.get(
+                                                    A.CT_S.POLIBASE_PERSON_ANSWER_OTHER_QUESTION_TEXT
+                                                ),
+                                                person,
+                                            )
+                                        )
+
                                     if BM.has(answer_type, ANSWER_TYPE.TAX_CERTIFICATE):
                                         send_message(
                                             polibase_person_name_format(
                                                 A.S.get(
                                                     A.CT_S.POLIBASE_PERSON_ANSWER_TAX_CERTIFICATE_TEXT
                                                 ),
                                                 person,
@@ -134,14 +158,39 @@
                                                 A.S.get(
                                                     A.CT_S.POLIBASE_PERSON_ANSWER_VISIT_MODIFICATION_TEXT
                                                 ),
                                                 person,
                                             ),
                                         )
 
+                                    if BM.has(answer_type, ANSWER_TYPE.HOW_TO_GET):
+                                        send_message(
+                                            A.S.get(
+                                                A.CT_S.POLIBASE_PERSON_ANSWER_HOW_TO_GET_TEXT
+                                            ),
+                                            location=A.CT.ADDRESS.LOCATION,
+                                        )
+                                        for index in range(4):
+                                            send_message(
+                                                A.S.get(
+                                                    getattr(
+                                                        A.CT_S,
+                                                        j(
+                                                            (
+                                                                A.CT_S.POLIBASE_PERSON_ANSWER_HOW_TO_GET_TEXT._name_,
+                                                                index + 1,
+                                                            )
+                                                        ),
+                                                    )
+                                                ),
+                                                image_url=A.PTH.APP_DATA.LOCATION_IMAGE_PATH(
+                                                    index + 1
+                                                ),
+                                            )
+
                                     A.L.polibase(js(("Тип ответа:", answer_type)))
                                     A.E.polibase_person_answered(person, message)
         return None
 
     def service_starts_handler() -> None:
         subscribe_on(SC.send_event)
```

