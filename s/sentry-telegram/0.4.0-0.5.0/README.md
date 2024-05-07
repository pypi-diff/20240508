# Comparing `tmp/sentry_telegram-0.4.0.tar.gz` & `tmp/sentry_telegram-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sentry_telegram-0.4.0.tar", last modified: Sun Apr 28 18:20:11 2019, max compression
+gzip compressed data, was "sentry_telegram-0.5.0.tar", last modified: Tue May  7 23:26:54 2024, max compression
```

## Comparing `sentry_telegram-0.4.0.tar` & `sentry_telegram-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-28 18:20:11.000000 sentry_telegram-0.4.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1656 2019-04-28 18:18:15.000000 sentry_telegram-0.4.0/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1411 2019-04-28 18:18:15.000000 sentry_telegram-0.4.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-28 18:20:11.000000 sentry_telegram-0.4.0/sentry_telegram.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2019-04-28 18:20:11.000000 sentry_telegram-0.4.0/sentry_telegram.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2972 2019-04-28 18:20:11.000000 sentry_telegram-0.4.0/sentry_telegram.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-04-28 18:20:11.000000 sentry_telegram-0.4.0/sentry_telegram.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       87 2019-04-28 18:20:11.000000 sentry_telegram-0.4.0/sentry_telegram.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      271 2019-04-28 18:20:11.000000 sentry_telegram-0.4.0/sentry_telegram.egg-info/SOURCES.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-04-28 18:20:11.000000 sentry_telegram-0.4.0/sentry_telegram/
--rw-rw-r--   0 travis    (2000) travis    (2000)      124 2019-04-28 18:18:15.000000 sentry_telegram-0.4.0/sentry_telegram/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5965 2019-04-28 18:18:15.000000 sentry_telegram-0.4.0/sentry_telegram/plugin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-04-28 18:20:11.000000 sentry_telegram-0.4.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2972 2019-04-28 18:20:11.000000 sentry_telegram-0.4.0/PKG-INFO
+drwxr-xr-x   0 shmele     (501) staff       (20)        0 2024-05-07 23:26:54.599381 sentry_telegram-0.5.0/
+-rw-r--r--   0 shmele     (501) staff       (20)     1075 2024-01-19 01:02:08.000000 sentry_telegram-0.5.0/LICENSE
+-rw-r--r--   0 shmele     (501) staff       (20)     2601 2024-05-07 23:26:54.599188 sentry_telegram-0.5.0/PKG-INFO
+-rw-r--r--   0 shmele     (501) staff       (20)     1656 2024-01-19 01:02:08.000000 sentry_telegram-0.5.0/README.rst
+drwxr-xr-x   0 shmele     (501) staff       (20)        0 2024-05-07 23:26:54.597322 sentry_telegram-0.5.0/sentry_telegram/
+-rw-r--r--   0 shmele     (501) staff       (20)      124 2024-05-07 23:22:38.000000 sentry_telegram-0.5.0/sentry_telegram/__init__.py
+-rw-r--r--   0 shmele     (501) staff       (20)     7724 2024-05-06 22:44:10.000000 sentry_telegram-0.5.0/sentry_telegram/plugin.py
+drwxr-xr-x   0 shmele     (501) staff       (20)        0 2024-05-07 23:26:54.598999 sentry_telegram-0.5.0/sentry_telegram.egg-info/
+-rw-r--r--   0 shmele     (501) staff       (20)     2601 2024-05-07 23:26:54.000000 sentry_telegram-0.5.0/sentry_telegram.egg-info/PKG-INFO
+-rw-r--r--   0 shmele     (501) staff       (20)      298 2024-05-07 23:26:54.000000 sentry_telegram-0.5.0/sentry_telegram.egg-info/SOURCES.txt
+-rw-r--r--   0 shmele     (501) staff       (20)        1 2024-05-07 23:26:54.000000 sentry_telegram-0.5.0/sentry_telegram.egg-info/dependency_links.txt
+-rw-r--r--   0 shmele     (501) staff       (20)       86 2024-05-07 23:26:54.000000 sentry_telegram-0.5.0/sentry_telegram.egg-info/entry_points.txt
+-rw-r--r--   0 shmele     (501) staff       (20)       16 2024-05-07 23:26:54.000000 sentry_telegram-0.5.0/sentry_telegram.egg-info/top_level.txt
+-rw-r--r--   0 shmele     (501) staff       (20)       38 2024-05-07 23:26:54.599437 sentry_telegram-0.5.0/setup.cfg
+-rw-r--r--   0 shmele     (501) staff       (20)     1409 2024-05-07 23:23:33.000000 sentry_telegram-0.5.0/setup.py
+drwxr-xr-x   0 shmele     (501) staff       (20)        0 2024-05-07 23:26:54.598483 sentry_telegram-0.5.0/tests/
+-rw-r--r--   0 shmele     (501) staff       (20)     4303 2024-01-28 21:48:41.000000 sentry_telegram-0.5.0/tests/test_base.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sentry_telegram-0.4.0/README.rst` & `sentry_telegram-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `sentry_telegram-0.4.0/setup.py` & `sentry_telegram-0.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Software Development :: Bug Tracking',
         'Topic :: Software Development :: Quality Assurance',
         'Topic :: System :: Monitoring',
     ],
     include_package_data=True,
 )
```

### Comparing `sentry_telegram-0.4.0/sentry_telegram.egg-info/PKG-INFO` & `sentry_telegram-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 Metadata-Version: 2.1
-Name: sentry-telegram
-Version: 0.4.0
+Name: sentry_telegram
+Version: 0.5.0
 Summary: Plugin for Sentry which allows sending notification via Telegram messenger.
 Home-page: https://github.com/butorov/sentry-telegram
 Author: Viacheslav Butorov
 Author-email: butorovv@gmail.com
 License: MIT
-Description: Sentry Telegram |travis| |codecov| |pypi|
-        =========================================
-        
-        Plugin for Sentry which allows sending notification via `Telegram <https://telegram.org/>`_ messenger.
-        
-        Presented plugin tested with Sentry from 8.9 to 9.1.1.
-        
-            **DISCLAIMER**: Sentry API is under development and `is not frozen <https://docs.sentry.io/server/plugins/>`_.
-        
-        
-        How will it look like
-        ---------------------
-        
-        .. image:: https://raw.githubusercontent.com/butorov/sentry-telegram/master/docs/images/telegram-window.png
-           :target: https://github.com/butorov/sentry-telegram/blob/master/docs/images/telegram-window.png
-           :alt: How will it look like
-        
-        Installation
-        ------------
-        
-        1. Install this package
-        
-        .. code-block:: bash
-        
-            pip install sentry-telegram
-        
-        2. Restart your Sentry instance.
-        3. Go to your Sentry web interface. Open ``Settings`` page of one of your projects.
-        4. On ``Integrations`` (or ``Legacy Integrations``) page, find ``Telegram Notifications`` plugin and enable it.
-        5. Configure plugin on ``Configure plugin`` page.
-        
-           See `Telegram's documentation <https://core.telegram.org/bots#3-how-do-i-create-a-bot>`_ to know how to create ``BotAPI Token``.
-        
-        6. Done!
-        
-        .. |travis| image:: https://travis-ci.org/butorov/sentry-telegram.svg?branch=master
-           :target: https://travis-ci.org/butorov/sentry-telegram
-           :alt: Build Status
-        
-        .. |codecov| image:: https://codecov.io/gh/butorov/sentry-telegram/branch/master/graph/badge.svg
-           :target: https://codecov.io/gh/butorov/sentry-telegram?branch=master
-           :alt: Coverage Status
-        
-        .. |pypi| image:: https://badge.fury.io/py/sentry-telegram.svg
-           :target: https://pypi.python.org/pypi/sentry-telegram
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: System :: Monitoring
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Sentry Telegram |travis| |codecov| |pypi|
+=========================================
+
+Plugin for Sentry which allows sending notification via `Telegram <https://telegram.org/>`_ messenger.
+
+Presented plugin tested with Sentry from 8.9 to 9.1.1.
+
+    **DISCLAIMER**: Sentry API is under development and `is not frozen <https://docs.sentry.io/server/plugins/>`_.
+
+
+How will it look like
+---------------------
+
+.. image:: https://raw.githubusercontent.com/butorov/sentry-telegram/master/docs/images/telegram-window.png
+   :target: https://github.com/butorov/sentry-telegram/blob/master/docs/images/telegram-window.png
+   :alt: How will it look like
+
+Installation
+------------
+
+1. Install this package
+
+.. code-block:: bash
+
+    pip install sentry-telegram
+
+2. Restart your Sentry instance.
+3. Go to your Sentry web interface. Open ``Settings`` page of one of your projects.
+4. On ``Integrations`` (or ``Legacy Integrations``) page, find ``Telegram Notifications`` plugin and enable it.
+5. Configure plugin on ``Configure plugin`` page.
+
+   See `Telegram's documentation <https://core.telegram.org/bots#3-how-do-i-create-a-bot>`_ to know how to create ``BotAPI Token``.
+
+6. Done!
+
+.. |travis| image:: https://travis-ci.org/butorov/sentry-telegram.svg?branch=master
+   :target: https://travis-ci.org/butorov/sentry-telegram
+   :alt: Build Status
+
+.. |codecov| image:: https://codecov.io/gh/butorov/sentry-telegram/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/butorov/sentry-telegram?branch=master
+   :alt: Coverage Status
+
+.. |pypi| image:: https://badge.fury.io/py/sentry-telegram.svg
+   :target: https://pypi.python.org/pypi/sentry-telegram
```

### Comparing `sentry_telegram-0.4.0/sentry_telegram/plugin.py` & `sentry_telegram-0.5.0/sentry_telegram/plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 # coding: utf-8
 import logging
 from collections import defaultdict
 
 from django import forms
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from sentry.plugins.bases import notify
 from sentry.http import safe_urlopen
 from sentry.utils.safe import safe_execute
 
 from . import __version__, __doc__ as package_doc
 
 
+TELEGRAM_MAX_MESSAGE_LENGTH = 4096  # https://core.telegram.org/bots/api#sendmessage:~:text=be%20sent%2C%201%2D-,4096,-characters%20after%20entities
+EVENT_TITLE_MAX_LENGTH = 500
+
+
 class TelegramNotificationsOptionsForm(notify.NotificationConfigurationForm):
     api_origin = forms.CharField(
         label=_('Telegram API origin'),
         widget=forms.TextInput(attrs={'placeholder': 'https://api.telegram.org'}),
         initial='https://api.telegram.org'
     )
     api_token = forms.CharField(
         label=_('BotAPI token'),
         widget=forms.TextInput(attrs={'placeholder': '123456:ABC-DEF1234ghIkl-zyx57W2v1u123ew11'}),
         help_text=_('Read more: https://core.telegram.org/bots/api#authorizing-your-bot'),
     )
     receivers = forms.CharField(
         label=_('Receivers'),
         widget=forms.Textarea(attrs={'class': 'span6'}),
-        help_text=_('Enter receivers IDs (one per line). Personal messages, group chats and channels also available.'))
-
+        help_text=_('Enter receivers IDs (one per line). Personal messages, group chats and channels also available. '
+                    'If you want to specify a thread ID, separate it with "/" (e.g. "12345/12").'),
+    )
     message_template = forms.CharField(
         label=_('Message template'),
         widget=forms.Textarea(attrs={'class': 'span4'}),
         help_text=_('Set in standard python\'s {}-format convention, available names are: '
                     '{project_name}, {url}, {title}, {message}, {tag[%your_tag%]}'),
-        initial='*[Sentry]* {project_name} {tag[level]}: *{title}*\n```{message}```\n{url}'
+        initial='*[Sentry]* {project_name} {tag[level]}: *{title}*\n```\n{message}```\n{url}'
     )
 
 
 class TelegramNotificationsPlugin(notify.NotificationPlugin):
     title = 'Telegram Notifications'
     slug = 'sentry_telegram'
     description = package_doc
@@ -79,75 +84,104 @@
                 'validators': [],
                 'required': True,
             },
             {
                 'name': 'receivers',
                 'label': 'Receivers',
                 'type': 'textarea',
-                'help': 'Enter receivers IDs (one per line). Personal messages, group chats and channels also available.',
+                'help': 'Enter receivers IDs (one per line). Personal messages, group chats and channels also available. '
+                        'If you want to specify a thread ID, separate it with "/" (e.g. "12345/12").',
                 'validators': [],
                 'required': True,
             },
             {
                 'name': 'message_template',
                 'label': 'Message Template',
                 'type': 'textarea',
                 'help': 'Set in standard python\'s {}-format convention, available names are: '
-                    '{project_name}, {url}, {title}, {message}, {tag[%your_tag%]}. Undefined tags will be shown as [NA]',
+                        '{project_name}, {url}, {title}, {message}, {tag[%your_tag%]}. Undefined tags will be shown as [NA]',
                 'validators': [],
                 'required': True,
                 'default': '*[Sentry]* {project_name} {tag[level]}: *{title}*\n```{message}```\n{url}'
             },
         ]
 
+    def compile_message_text(self, message_template: str, message_params: dict, event_message: str) -> str:
+        """
+        Compiles message text from template and event message.
+        Truncates the original event message (`event.message`) to fit Telegram message length limit.
+        """
+        # TODO: add tests
+        truncate_warning_text = '... (truncated)'
+        truncate_warning_length = len(truncate_warning_text)
+
+        truncated = False
+        while True:
+            message_text = message_template.format(**message_params, message=event_message)
+            message_text_size = len(message_text)
+
+            if truncated or message_text_size <= TELEGRAM_MAX_MESSAGE_LENGTH:
+                break
+            else:
+                truncate_size = (message_text_size - TELEGRAM_MAX_MESSAGE_LENGTH) + truncate_warning_length
+                event_message = event_message[:-truncate_size] + truncate_warning_text
+                truncated = True
+
+        return message_text
+
     def build_message(self, group, event):
-        the_tags = defaultdict(lambda: '[NA]')
-        the_tags.update({k:v for k, v in event.tags})
-        names = {
-            'title': event.title,
-            'tag': the_tags,
-            'message': event.message,
+        event_tags = defaultdict(lambda: '[NA]')
+        event_tags.update({k: v for k, v in event.tags})
+
+        message_params = {
+            'title': event.title[:EVENT_TITLE_MAX_LENGTH],
+            'tag': event_tags,
             'project_name': group.project.name,
             'url': group.get_absolute_url(),
         }
-
-        template = self.get_message_template(group.project)
-
-        text = template.format(**names)
+        text = self.compile_message_text(
+            self.get_message_template(group.project),
+            message_params,
+            event.message,
+        )
 
         return {
             'text': text,
             'parse_mode': 'Markdown',
         }
 
     def build_url(self, project):
         return '%s/bot%s/sendMessage' % (self.get_option('api_origin', project), self.get_option('api_token', project))
 
     def get_message_template(self, project):
         return self.get_option('message_template', project)
 
-    def get_receivers(self, project):
-        receivers = self.get_option('receivers', project)
+    def get_receivers(self, project) -> list[list[str, str]]:
+        receivers = self.get_option('receivers', project).strip()
         if not receivers:
             return []
-        return filter(bool, receivers.strip().splitlines())
+        return list([line.strip().split('/', maxsplit=1) for line in receivers.splitlines() if line.strip()])
 
-    def send_message(self, url, payload, receiver):
-        payload['chat_id'] = receiver
-        self.logger.debug('Sending message to %s ' % receiver)
+    def send_message(self, url, payload, receiver: list[str, str]):
+        payload['chat_id'] = receiver[0]
+        if len(receiver) > 1:
+            payload['message_thread_id'] = receiver[1]
+        self.logger.debug('Sending message to %s' % receiver)
         response = safe_urlopen(
             method='POST',
             url=url,
             json=payload,
         )
         self.logger.debug('Response code: %s, content: %s' % (response.status_code, response.content))
+        if response.status_code > 299:
+            raise ConnectionError(response.content)
 
     def notify_users(self, group, event, fail_silently=False, **kwargs):
         self.logger.debug('Received notification for event: %s' % event)
         receivers = self.get_receivers(group.project)
-        self.logger.debug('for receivers: %s' % ', '.join(receivers or ()))
+        self.logger.debug('for receivers: %s' % ', '.join(['/'.join(item) for item in receivers] or ()))
         payload = self.build_message(group, event)
         self.logger.debug('Built payload: %s' % payload)
         url = self.build_url(group.project)
         self.logger.debug('Built url: %s' % url)
         for receiver in receivers:
             safe_execute(self.send_message, url, payload, receiver, _with_transaction=False)
```

### Comparing `sentry_telegram-0.4.0/PKG-INFO` & `sentry_telegram-0.5.0/sentry_telegram.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 Metadata-Version: 2.1
 Name: sentry_telegram
-Version: 0.4.0
+Version: 0.5.0
 Summary: Plugin for Sentry which allows sending notification via Telegram messenger.
 Home-page: https://github.com/butorov/sentry-telegram
 Author: Viacheslav Butorov
 Author-email: butorovv@gmail.com
 License: MIT
-Description: Sentry Telegram |travis| |codecov| |pypi|
-        =========================================
-        
-        Plugin for Sentry which allows sending notification via `Telegram <https://telegram.org/>`_ messenger.
-        
-        Presented plugin tested with Sentry from 8.9 to 9.1.1.
-        
-            **DISCLAIMER**: Sentry API is under development and `is not frozen <https://docs.sentry.io/server/plugins/>`_.
-        
-        
-        How will it look like
-        ---------------------
-        
-        .. image:: https://raw.githubusercontent.com/butorov/sentry-telegram/master/docs/images/telegram-window.png
-           :target: https://github.com/butorov/sentry-telegram/blob/master/docs/images/telegram-window.png
-           :alt: How will it look like
-        
-        Installation
-        ------------
-        
-        1. Install this package
-        
-        .. code-block:: bash
-        
-            pip install sentry-telegram
-        
-        2. Restart your Sentry instance.
-        3. Go to your Sentry web interface. Open ``Settings`` page of one of your projects.
-        4. On ``Integrations`` (or ``Legacy Integrations``) page, find ``Telegram Notifications`` plugin and enable it.
-        5. Configure plugin on ``Configure plugin`` page.
-        
-           See `Telegram's documentation <https://core.telegram.org/bots#3-how-do-i-create-a-bot>`_ to know how to create ``BotAPI Token``.
-        
-        6. Done!
-        
-        .. |travis| image:: https://travis-ci.org/butorov/sentry-telegram.svg?branch=master
-           :target: https://travis-ci.org/butorov/sentry-telegram
-           :alt: Build Status
-        
-        .. |codecov| image:: https://codecov.io/gh/butorov/sentry-telegram/branch/master/graph/badge.svg
-           :target: https://codecov.io/gh/butorov/sentry-telegram?branch=master
-           :alt: Coverage Status
-        
-        .. |pypi| image:: https://badge.fury.io/py/sentry-telegram.svg
-           :target: https://pypi.python.org/pypi/sentry-telegram
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: System :: Monitoring
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Sentry Telegram |travis| |codecov| |pypi|
+=========================================
+
+Plugin for Sentry which allows sending notification via `Telegram <https://telegram.org/>`_ messenger.
+
+Presented plugin tested with Sentry from 8.9 to 9.1.1.
+
+    **DISCLAIMER**: Sentry API is under development and `is not frozen <https://docs.sentry.io/server/plugins/>`_.
+
+
+How will it look like
+---------------------
+
+.. image:: https://raw.githubusercontent.com/butorov/sentry-telegram/master/docs/images/telegram-window.png
+   :target: https://github.com/butorov/sentry-telegram/blob/master/docs/images/telegram-window.png
+   :alt: How will it look like
+
+Installation
+------------
+
+1. Install this package
+
+.. code-block:: bash
+
+    pip install sentry-telegram
+
+2. Restart your Sentry instance.
+3. Go to your Sentry web interface. Open ``Settings`` page of one of your projects.
+4. On ``Integrations`` (or ``Legacy Integrations``) page, find ``Telegram Notifications`` plugin and enable it.
+5. Configure plugin on ``Configure plugin`` page.
+
+   See `Telegram's documentation <https://core.telegram.org/bots#3-how-do-i-create-a-bot>`_ to know how to create ``BotAPI Token``.
+
+6. Done!
+
+.. |travis| image:: https://travis-ci.org/butorov/sentry-telegram.svg?branch=master
+   :target: https://travis-ci.org/butorov/sentry-telegram
+   :alt: Build Status
+
+.. |codecov| image:: https://codecov.io/gh/butorov/sentry-telegram/branch/master/graph/badge.svg
+   :target: https://codecov.io/gh/butorov/sentry-telegram?branch=master
+   :alt: Coverage Status
+
+.. |pypi| image:: https://badge.fury.io/py/sentry-telegram.svg
+   :target: https://pypi.python.org/pypi/sentry-telegram
```

