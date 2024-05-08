# Comparing `tmp/neon-skill-personal-1.0.1a4.tar.gz` & `tmp/neon-skill-personal-1.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-personal-1.0.1a4.tar", last modified: Tue Apr  2 19:16:10 2024, max compression
+gzip compressed data, was "neon-skill-personal-1.0.2a1.tar", last modified: Wed May  8 19:02:19 2024, max compression
```

## Comparing `neon-skill-personal-1.0.1a4.tar` & `neon-skill-personal-1.0.2a1.tar`

### file list

```diff
@@ -1,248 +1,248 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.547497 neon-skill-personal-1.0.1a4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-02 19:16:10.547497 neon-skill-personal-1.0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.519497 neon-skill-personal-1.0.1a4/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.515497 neon-skill-personal-1.0.1a4/locale/ca-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.519497 neon-skill-personal-1.0.1a4/locale/ca-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/ca-es/dialog/what_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/ca-es/dialog/when_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/ca-es/dialog/where_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/ca-es/dialog/who_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/ca-es/dialog/who_made_me.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.519497 neon-skill-personal-1.0.1a4/locale/ca-es/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/ca-es/vocab/WhatAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/ca-es/vocab/WhenWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/ca-es/vocab/WhereWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/ca-es/vocab/WhoAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/ca-es/vocab/WhoMadeYou.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.515497 neon-skill-personal-1.0.1a4/locale/cs-cz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.523497 neon-skill-personal-1.0.1a4/locale/cs-cz/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/cs-cz/dialog/what_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/cs-cz/dialog/when_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/cs-cz/dialog/where_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/cs-cz/dialog/who_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/cs-cz/dialog/who_made_me.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.523497 neon-skill-personal-1.0.1a4/locale/cs-cz/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/cs-cz/vocab/WhatAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/cs-cz/vocab/WhenWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/cs-cz/vocab/WhereWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/cs-cz/vocab/WhoAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/cs-cz/vocab/WhoMadeYou.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.515497 neon-skill-personal-1.0.1a4/locale/da-dk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.523497 neon-skill-personal-1.0.1a4/locale/da-dk/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/da-dk/dialog/what_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/da-dk/dialog/when_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/da-dk/dialog/where_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/da-dk/dialog/who_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/da-dk/dialog/who_made_me.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.523497 neon-skill-personal-1.0.1a4/locale/da-dk/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/da-dk/vocab/WhatAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/da-dk/vocab/WhenWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/da-dk/vocab/WhereWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/da-dk/vocab/WhoAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/da-dk/vocab/WhoMadeYou.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.515497 neon-skill-personal-1.0.1a4/locale/de-de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.523497 neon-skill-personal-1.0.1a4/locale/de-de/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/de-de/dialog/what_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/de-de/dialog/when_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/de-de/dialog/where_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/de-de/dialog/who_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/de-de/dialog/who_made_me.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.523497 neon-skill-personal-1.0.1a4/locale/de-de/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/de-de/vocab/WhatAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/de-de/vocab/WhenWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/de-de/vocab/WhereWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/de-de/vocab/WhoAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/de-de/vocab/WhoMadeYou.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.515497 neon-skill-personal-1.0.1a4/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.527497 neon-skill-personal-1.0.1a4/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/dialog/birthplace.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/dialog/creator.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/dialog/how_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/dialog/my_email_address.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/dialog/my_name.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/dialog/neon.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/dialog/what_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/dialog/when_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/dialog/where_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/dialog/where_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/dialog/who_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/dialog/who_made_me.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/dialog/word_first_name.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/dialog/word_last_name.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/dialog/word_name.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.527497 neon-skill-personal-1.0.1a4/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/intent/WhatAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/intent/WhatIsYourEmail.intent
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/intent/WhenWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/intent/WhereAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/intent/WhereWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/intent/WhoAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/intent/WhoMadeYou.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.531497 neon-skill-personal-1.0.1a4/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/vocab/are.voc
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/vocab/born.voc
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/vocab/email.voc
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/vocab/first.voc
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/vocab/how.voc
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/vocab/last.voc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/vocab/made.voc
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/vocab/name.voc
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/vocab/what.voc
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/vocab/when.voc
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/vocab/where.voc
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/vocab/who.voc
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/en-us/vocab/you.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.515497 neon-skill-personal-1.0.1a4/locale/es-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.531497 neon-skill-personal-1.0.1a4/locale/es-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/es-es/dialog/what_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/es-es/dialog/when_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/es-es/dialog/where_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/es-es/dialog/who_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/es-es/dialog/who_made_me.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.531497 neon-skill-personal-1.0.1a4/locale/es-es/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/es-es/vocab/WhatAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/es-es/vocab/WhenWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/es-es/vocab/WhereWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/es-es/vocab/WhoAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/es-es/vocab/WhoMadeYou.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.515497 neon-skill-personal-1.0.1a4/locale/eu-eu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.531497 neon-skill-personal-1.0.1a4/locale/eu-eu/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/eu-eu/dialog/what_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/eu-eu/dialog/when_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/eu-eu/dialog/where_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/eu-eu/dialog/who_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/eu-eu/dialog/who_made_me.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.531497 neon-skill-personal-1.0.1a4/locale/eu-eu/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/eu-eu/vocab/WhatAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/eu-eu/vocab/WhenWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/eu-eu/vocab/WhereWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/eu-eu/vocab/WhoAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/eu-eu/vocab/WhoMadeYou.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.515497 neon-skill-personal-1.0.1a4/locale/fa-ir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.531497 neon-skill-personal-1.0.1a4/locale/fa-ir/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fa-ir/dialog/what_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fa-ir/dialog/when_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fa-ir/dialog/where_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fa-ir/dialog/who_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fa-ir/dialog/who_made_me.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.535497 neon-skill-personal-1.0.1a4/locale/fa-ir/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fa-ir/vocab/WhatAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fa-ir/vocab/WhenWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fa-ir/vocab/WhereWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fa-ir/vocab/WhoAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fa-ir/vocab/WhoMadeYou.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.515497 neon-skill-personal-1.0.1a4/locale/fr-fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.535497 neon-skill-personal-1.0.1a4/locale/fr-fr/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fr-fr/dialog/what_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fr-fr/dialog/when_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fr-fr/dialog/where_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fr-fr/dialog/who_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fr-fr/dialog/who_made_me.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.535497 neon-skill-personal-1.0.1a4/locale/fr-fr/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fr-fr/vocab/WhatAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fr-fr/vocab/WhenWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fr-fr/vocab/WhereWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fr-fr/vocab/WhoAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/fr-fr/vocab/WhoMadeYou.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.515497 neon-skill-personal-1.0.1a4/locale/gl-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.535497 neon-skill-personal-1.0.1a4/locale/gl-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/gl-es/dialog/what_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/gl-es/dialog/when_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/gl-es/dialog/where_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/gl-es/dialog/who_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/gl-es/dialog/who_made_me.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.535497 neon-skill-personal-1.0.1a4/locale/gl-es/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/gl-es/vocab/WhatAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/gl-es/vocab/WhenWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/gl-es/vocab/WhereWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/gl-es/vocab/WhoAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/gl-es/vocab/WhoMadeYou.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.515497 neon-skill-personal-1.0.1a4/locale/hu-hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.535497 neon-skill-personal-1.0.1a4/locale/hu-hu/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/hu-hu/dialog/what_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/hu-hu/dialog/when_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/hu-hu/dialog/where_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/hu-hu/dialog/who_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/hu-hu/dialog/who_made_me.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.539497 neon-skill-personal-1.0.1a4/locale/hu-hu/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/hu-hu/vocab/WhatAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/hu-hu/vocab/WhenWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/hu-hu/vocab/WhereWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/hu-hu/vocab/WhoAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/hu-hu/vocab/WhoMadeYou.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.515497 neon-skill-personal-1.0.1a4/locale/it-it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.539497 neon-skill-personal-1.0.1a4/locale/it-it/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/it-it/dialog/what_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/it-it/dialog/when_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/it-it/dialog/where_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/it-it/dialog/who_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/it-it/dialog/who_made_me.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.539497 neon-skill-personal-1.0.1a4/locale/it-it/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/it-it/vocab/WhatAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/it-it/vocab/WhenWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/it-it/vocab/WhereWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/it-it/vocab/WhoAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/it-it/vocab/WhoMadeYou.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.519497 neon-skill-personal-1.0.1a4/locale/nl-nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.539497 neon-skill-personal-1.0.1a4/locale/nl-nl/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/nl-nl/dialog/what_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/nl-nl/dialog/when_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/nl-nl/dialog/where_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/nl-nl/dialog/who_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/nl-nl/dialog/who_made_me.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.539497 neon-skill-personal-1.0.1a4/locale/nl-nl/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/nl-nl/vocab/WhatAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/nl-nl/vocab/WhenWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/nl-nl/vocab/WhereWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/nl-nl/vocab/WhoAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/nl-nl/vocab/WhoMadeYou.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.519497 neon-skill-personal-1.0.1a4/locale/pt-br/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.543497 neon-skill-personal-1.0.1a4/locale/pt-br/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/pt-br/dialog/what_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/pt-br/dialog/when_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/pt-br/dialog/where_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/pt-br/dialog/who_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/pt-br/dialog/who_made_me.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.543497 neon-skill-personal-1.0.1a4/locale/pt-br/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/pt-br/vocab/WhatAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/pt-br/vocab/WhenWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/pt-br/vocab/WhereWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/pt-br/vocab/WhoAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/pt-br/vocab/WhoMadeYou.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.519497 neon-skill-personal-1.0.1a4/locale/ru-ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.543497 neon-skill-personal-1.0.1a4/locale/ru-ru/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/ru-ru/dialog/what_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/ru-ru/dialog/when_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/ru-ru/dialog/where_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/ru-ru/dialog/who_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/ru-ru/dialog/who_made_me.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.519497 neon-skill-personal-1.0.1a4/locale/sv-se/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.543497 neon-skill-personal-1.0.1a4/locale/sv-se/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/sv-se/dialog/what_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/sv-se/dialog/when_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/sv-se/dialog/where_was_i_born.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/sv-se/dialog/who_am_i.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/sv-se/dialog/who_made_me.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.543497 neon-skill-personal-1.0.1a4/locale/sv-se/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/sv-se/vocab/WhatAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/sv-se/vocab/WhenWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/sv-se/vocab/WhereWereYouBorn.intent
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/sv-se/vocab/WhoAreYou.intent
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/locale/sv-se/vocab/WhoMadeYou.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.543497 neon-skill-personal-1.0.1a4/neon_skill_personal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-02 19:16:10.000000 neon-skill-personal-1.0.1a4/neon_skill_personal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-02 19:16:10.000000 neon-skill-personal-1.0.1a4/neon_skill_personal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:16:10.000000 neon-skill-personal-1.0.1a4/neon_skill_personal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 19:16:10.000000 neon-skill-personal-1.0.1a4/neon_skill_personal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 19:16:10.000000 neon-skill-personal-1.0.1a4/neon_skill_personal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 19:16:10.000000 neon-skill-personal-1.0.1a4/neon_skill_personal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 19:16:10.547497 neon-skill-personal-1.0.1a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:16:10.543497 neon-skill-personal-1.0.1a4/test/
--rw-r--r--   0 runner    (1001) docker     (127)    12103 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-02 19:16:06.000000 neon-skill-personal-1.0.1a4/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.440536 neon-skill-personal-1.0.2a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-08 19:02:19.440536 neon-skill-personal-1.0.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.412536 neon-skill-personal-1.0.2a1/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.408536 neon-skill-personal-1.0.2a1/locale/ca-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.412536 neon-skill-personal-1.0.2a1/locale/ca-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/ca-es/dialog/what_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/ca-es/dialog/when_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/ca-es/dialog/where_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/ca-es/dialog/who_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/ca-es/dialog/who_made_me.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.412536 neon-skill-personal-1.0.2a1/locale/ca-es/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/ca-es/vocab/WhatAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/ca-es/vocab/WhenWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/ca-es/vocab/WhereWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/ca-es/vocab/WhoAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/ca-es/vocab/WhoMadeYou.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.408536 neon-skill-personal-1.0.2a1/locale/cs-cz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.416536 neon-skill-personal-1.0.2a1/locale/cs-cz/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/cs-cz/dialog/what_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/cs-cz/dialog/when_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/cs-cz/dialog/where_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/cs-cz/dialog/who_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/cs-cz/dialog/who_made_me.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.416536 neon-skill-personal-1.0.2a1/locale/cs-cz/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/cs-cz/vocab/WhatAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/cs-cz/vocab/WhenWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/cs-cz/vocab/WhereWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/cs-cz/vocab/WhoAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/cs-cz/vocab/WhoMadeYou.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.408536 neon-skill-personal-1.0.2a1/locale/da-dk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.416536 neon-skill-personal-1.0.2a1/locale/da-dk/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/da-dk/dialog/what_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/da-dk/dialog/when_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/da-dk/dialog/where_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/da-dk/dialog/who_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/da-dk/dialog/who_made_me.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.416536 neon-skill-personal-1.0.2a1/locale/da-dk/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/da-dk/vocab/WhatAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/da-dk/vocab/WhenWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/da-dk/vocab/WhereWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/da-dk/vocab/WhoAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/da-dk/vocab/WhoMadeYou.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.408536 neon-skill-personal-1.0.2a1/locale/de-de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.416536 neon-skill-personal-1.0.2a1/locale/de-de/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/de-de/dialog/what_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/de-de/dialog/when_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/de-de/dialog/where_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/de-de/dialog/who_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/de-de/dialog/who_made_me.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.416536 neon-skill-personal-1.0.2a1/locale/de-de/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/de-de/vocab/WhatAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/de-de/vocab/WhenWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/de-de/vocab/WhereWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/de-de/vocab/WhoAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/de-de/vocab/WhoMadeYou.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.408536 neon-skill-personal-1.0.2a1/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.420536 neon-skill-personal-1.0.2a1/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/dialog/birthplace.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/dialog/creator.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/dialog/how_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/dialog/my_email_address.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/dialog/my_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/dialog/neon.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/dialog/what_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/dialog/when_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/dialog/where_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/dialog/where_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/dialog/who_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/dialog/who_made_me.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/dialog/word_first_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/dialog/word_last_name.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/dialog/word_name.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.420536 neon-skill-personal-1.0.2a1/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/intent/WhatAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/intent/WhatIsYourEmail.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/intent/WhenWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/intent/WhereAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/intent/WhereWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/intent/WhoAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/intent/WhoMadeYou.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.424536 neon-skill-personal-1.0.2a1/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/vocab/are.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/vocab/born.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/vocab/email.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/vocab/first.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/vocab/how.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/vocab/last.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/vocab/made.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/vocab/name.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/vocab/what.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/vocab/when.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/vocab/where.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/vocab/who.voc
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/en-us/vocab/you.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.408536 neon-skill-personal-1.0.2a1/locale/es-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.424536 neon-skill-personal-1.0.2a1/locale/es-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/es-es/dialog/what_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/es-es/dialog/when_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/es-es/dialog/where_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/es-es/dialog/who_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/es-es/dialog/who_made_me.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.424536 neon-skill-personal-1.0.2a1/locale/es-es/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/es-es/vocab/WhatAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/es-es/vocab/WhenWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/es-es/vocab/WhereWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/es-es/vocab/WhoAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/es-es/vocab/WhoMadeYou.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.408536 neon-skill-personal-1.0.2a1/locale/eu-eu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.424536 neon-skill-personal-1.0.2a1/locale/eu-eu/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/eu-eu/dialog/what_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/eu-eu/dialog/when_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/eu-eu/dialog/where_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/eu-eu/dialog/who_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/eu-eu/dialog/who_made_me.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.424536 neon-skill-personal-1.0.2a1/locale/eu-eu/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/eu-eu/vocab/WhatAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/eu-eu/vocab/WhenWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/eu-eu/vocab/WhereWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/eu-eu/vocab/WhoAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/eu-eu/vocab/WhoMadeYou.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.408536 neon-skill-personal-1.0.2a1/locale/fa-ir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.424536 neon-skill-personal-1.0.2a1/locale/fa-ir/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fa-ir/dialog/what_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fa-ir/dialog/when_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fa-ir/dialog/where_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fa-ir/dialog/who_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fa-ir/dialog/who_made_me.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.428536 neon-skill-personal-1.0.2a1/locale/fa-ir/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fa-ir/vocab/WhatAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fa-ir/vocab/WhenWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fa-ir/vocab/WhereWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fa-ir/vocab/WhoAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fa-ir/vocab/WhoMadeYou.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.408536 neon-skill-personal-1.0.2a1/locale/fr-fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.428536 neon-skill-personal-1.0.2a1/locale/fr-fr/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fr-fr/dialog/what_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fr-fr/dialog/when_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fr-fr/dialog/where_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fr-fr/dialog/who_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fr-fr/dialog/who_made_me.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.428536 neon-skill-personal-1.0.2a1/locale/fr-fr/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fr-fr/vocab/WhatAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fr-fr/vocab/WhenWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fr-fr/vocab/WhereWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fr-fr/vocab/WhoAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/fr-fr/vocab/WhoMadeYou.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.408536 neon-skill-personal-1.0.2a1/locale/gl-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.428536 neon-skill-personal-1.0.2a1/locale/gl-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/gl-es/dialog/what_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/gl-es/dialog/when_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/gl-es/dialog/where_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/gl-es/dialog/who_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/gl-es/dialog/who_made_me.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.428536 neon-skill-personal-1.0.2a1/locale/gl-es/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/gl-es/vocab/WhatAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/gl-es/vocab/WhenWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/gl-es/vocab/WhereWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/gl-es/vocab/WhoAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/gl-es/vocab/WhoMadeYou.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.412536 neon-skill-personal-1.0.2a1/locale/hu-hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.428536 neon-skill-personal-1.0.2a1/locale/hu-hu/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/hu-hu/dialog/what_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/hu-hu/dialog/when_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/hu-hu/dialog/where_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/hu-hu/dialog/who_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/hu-hu/dialog/who_made_me.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.432536 neon-skill-personal-1.0.2a1/locale/hu-hu/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/hu-hu/vocab/WhatAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/hu-hu/vocab/WhenWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/hu-hu/vocab/WhereWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/hu-hu/vocab/WhoAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/hu-hu/vocab/WhoMadeYou.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.412536 neon-skill-personal-1.0.2a1/locale/it-it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.432536 neon-skill-personal-1.0.2a1/locale/it-it/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/it-it/dialog/what_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/it-it/dialog/when_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/it-it/dialog/where_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/it-it/dialog/who_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/it-it/dialog/who_made_me.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.432536 neon-skill-personal-1.0.2a1/locale/it-it/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/it-it/vocab/WhatAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/it-it/vocab/WhenWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/it-it/vocab/WhereWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/it-it/vocab/WhoAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/it-it/vocab/WhoMadeYou.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.412536 neon-skill-personal-1.0.2a1/locale/nl-nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.432536 neon-skill-personal-1.0.2a1/locale/nl-nl/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/nl-nl/dialog/what_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/nl-nl/dialog/when_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/nl-nl/dialog/where_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/nl-nl/dialog/who_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/nl-nl/dialog/who_made_me.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.432536 neon-skill-personal-1.0.2a1/locale/nl-nl/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/nl-nl/vocab/WhatAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/nl-nl/vocab/WhenWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/nl-nl/vocab/WhereWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/nl-nl/vocab/WhoAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/nl-nl/vocab/WhoMadeYou.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.412536 neon-skill-personal-1.0.2a1/locale/pt-br/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.436536 neon-skill-personal-1.0.2a1/locale/pt-br/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/pt-br/dialog/what_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/pt-br/dialog/when_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/pt-br/dialog/where_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/pt-br/dialog/who_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/pt-br/dialog/who_made_me.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.436536 neon-skill-personal-1.0.2a1/locale/pt-br/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/pt-br/vocab/WhatAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/pt-br/vocab/WhenWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/pt-br/vocab/WhereWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/pt-br/vocab/WhoAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/pt-br/vocab/WhoMadeYou.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.412536 neon-skill-personal-1.0.2a1/locale/ru-ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.436536 neon-skill-personal-1.0.2a1/locale/ru-ru/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/ru-ru/dialog/what_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/ru-ru/dialog/when_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/ru-ru/dialog/where_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/ru-ru/dialog/who_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/ru-ru/dialog/who_made_me.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.412536 neon-skill-personal-1.0.2a1/locale/sv-se/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.436536 neon-skill-personal-1.0.2a1/locale/sv-se/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/sv-se/dialog/what_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/sv-se/dialog/when_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/sv-se/dialog/where_was_i_born.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/sv-se/dialog/who_am_i.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/sv-se/dialog/who_made_me.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.436536 neon-skill-personal-1.0.2a1/locale/sv-se/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/sv-se/vocab/WhatAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/sv-se/vocab/WhenWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/sv-se/vocab/WhereWereYouBorn.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/sv-se/vocab/WhoAreYou.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/locale/sv-se/vocab/WhoMadeYou.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.436536 neon-skill-personal-1.0.2a1/neon_skill_personal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-08 19:02:19.000000 neon-skill-personal-1.0.2a1/neon_skill_personal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-08 19:02:19.000000 neon-skill-personal-1.0.2a1/neon_skill_personal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:02:19.000000 neon-skill-personal-1.0.2a1/neon_skill_personal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-08 19:02:19.000000 neon-skill-personal-1.0.2a1/neon_skill_personal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-08 19:02:19.000000 neon-skill-personal-1.0.2a1/neon_skill_personal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 19:02:19.000000 neon-skill-personal-1.0.2a1/neon_skill_personal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 19:02:19.440536 neon-skill-personal-1.0.2a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:02:19.440536 neon-skill-personal-1.0.2a1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    12103 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-08 19:02:16.000000 neon-skill-personal-1.0.2a1/version.py
```

### Comparing `neon-skill-personal-1.0.1a4/LICENSE` & `neon-skill-personal-1.0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-personal-1.0.1a4/LICENSE.md` & `neon-skill-personal-1.0.2a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-personal-1.0.1a4/PKG-INFO` & `neon-skill-personal-1.0.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-personal
-Version: 1.0.1a4
+Version: 1.0.2a1
 Home-page: https://github.com/NeonGeckoCom/skill-personal
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `neon-skill-personal-1.0.1a4/README.md` & `neon-skill-personal-1.0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-personal-1.0.1a4/__init__.py` & `neon-skill-personal-1.0.2a1/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,16 +27,15 @@
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from ovos_utils import classproperty
 from ovos_utils.log import LOG
 from ovos_utils.process_utils import RuntimeRequirements
 from neon_utils.skills.common_query_skill import CommonQuerySkill, CQSMatchLevel
 from adapt.intent import IntentBuilder
-
-from mycroft.skills.core import intent_handler, intent_file_handler
+from ovos_workshop.skills.decorators import intent_handler, intent_file_handler
 
 
 class PersonalSkill(CommonQuerySkill):
     @classproperty
     def runtime_requirements(self):
         return RuntimeRequirements(network_before_load=False,
                                    internet_before_load=False,
@@ -56,35 +55,37 @@
     def ai_name(self):
         """
         Get a speakable name for the assistant.
         If there is a name configured in skill settings,
         it will be treated as a dialog reference
         (spoken directly if the resource is unavailable).
         """
-        return self.translate(self.settings.get("name") or "neon")
+        return self.resources.render_dialog(self.settings.get("name") or "neon")
 
     @property
     def birthplace(self):
         """
         Get a speakable birthplace for the assistant.
         If there is a birthplace configured in skill settings,
         it will be treated as a dialog reference
         (spoken directly if the resource is unavailable).
         """
-        return self.translate(self.settings.get("birthplace") or "birthplace")
+        return self.resources.render_dialog(self.settings.get("birthplace") or
+                                            "birthplace")
 
     @property
     def creator(self):
         """
         Get a speakable creator of the assistant.
         If there is a birthplace configured in skill settings,
         it will be treated as a dialog reference
         (spoken directly if the resource is unavailable).
         """
-        return self.translate(self.settings.get("creator") or "creator")
+        return self.resources.render_dialog(self.settings.get("creator") or
+                                            "creator")
 
     @property
     def email(self):
         """
         Get a speakable email address for the assistant.
         """
         return self.settings.get("email") or "developers@neon.ai"
@@ -208,12 +209,13 @@
         elif message.data.get("last"):
             position = "word_last_name"
             spoken_name = self.ai_name.split()[-1]
         else:
             position = "word_name"
             spoken_name = self.ai_name
 
-        self.speak_dialog("my_name", {"position": self.translate(position),
-                                      "name": spoken_name})
+        self.speak_dialog("my_name",
+                          {"position": self.resources.render_dialog(position),
+                           "name": spoken_name})
 
     def stop(self):
         pass
```

### Comparing `neon-skill-personal-1.0.1a4/neon_skill_personal.egg-info/PKG-INFO` & `neon-skill-personal-1.0.2a1/neon_skill_personal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-personal
-Version: 1.0.1a4
+Version: 1.0.2a1
 Home-page: https://github.com/NeonGeckoCom/skill-personal
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `neon-skill-personal-1.0.1a4/neon_skill_personal.egg-info/SOURCES.txt` & `neon-skill-personal-1.0.2a1/neon_skill_personal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-personal-1.0.1a4/setup.py` & `neon-skill-personal-1.0.2a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-personal-1.0.1a4/skill.json` & `neon-skill-personal-1.0.2a1/skill.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987373737373737%*

 * *Differences: {"'requirements'": "{'python': {insert: [(2, 'ovos-workshop~=0.0.15')]}}"}*

```diff
@@ -35,15 +35,16 @@
         "ia64",
         "arm64",
         "arm"
     ],
     "requirements": {
         "python": [
             "neon-utils~=1.0",
-            "ovos-utils~=0.0, >=0.0.28"
+            "ovos-utils~=0.0, >=0.0.28",
+            "ovos-workshop~=0.0.15"
         ],
         "skill": [],
         "system": {}
     },
     "short_description": "Skill used for introduction between the user and Neon.",
     "skillname": "skill-personal",
     "summary": "Skill used for introduction between the user and Neon.",
```

### Comparing `neon-skill-personal-1.0.1a4/test/test_skill.py` & `neon-skill-personal-1.0.2a1/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-personal-1.0.1a4/version.py` & `neon-skill-personal-1.0.2a1/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a4"
+__version__ = "1.0.2a1"
```
