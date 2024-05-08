# Comparing `tmp/primebotframework-1.0.56.tar.gz` & `tmp/primebotframework-1.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-6lgfgeg_/primebotframework-1.0.56.tar", last modified: Tue Apr 30 19:36:43 2024, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-blz3lug_/primebotframework-1.0.60.tar", last modified: Tue May  7 14:33:28 2024, max compression
```

## Comparing `primebotframework-1.0.56.tar` & `primebotframework-1.0.60.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.207252 primebotframework-1.0.56/
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-30 19:36:43.207252 primebotframework-1.0.56/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.203251 primebotframework-1.0.56/PrimeBot/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.203251 primebotframework-1.0.56/PrimeBot/B2E/
--rw-rw-rw-   0 root         (0) root         (0)     4028 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/B2E/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.203251 primebotframework-1.0.56/PrimeBot/Cnab750/
--rw-rw-rw-   0 root         (0) root         (0)    10261 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/Cnab750/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.203251 primebotframework-1.0.56/PrimeBot/CpfCnpj/
--rw-rw-rw-   0 root         (0) root         (0)     1963 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/CpfCnpj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/CpfCnpj/api_codes.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/CpfCnpj/model.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.203251 primebotframework-1.0.56/PrimeBot/D4Sign/
--rw-rw-rw-   0 root         (0) root         (0)     2600 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/D4Sign/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.203251 primebotframework-1.0.56/PrimeBot/DeathByCaptcha/
--rw-rw-rw-   0 root         (0) root         (0)     5755 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/DeathByCaptcha/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.203251 primebotframework-1.0.56/PrimeBot/Documents/
--rw-rw-rw-   0 root         (0) root         (0)     1098 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/Documents/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.203251 primebotframework-1.0.56/PrimeBot/Elastic/
--rw-rw-rw-   0 root         (0) root         (0)     1239 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/Elastic/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.203251 primebotframework-1.0.56/PrimeBot/EmailAlert/
--rw-rw-rw-   0 root         (0) root         (0)     3652 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/EmailAlert/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.203251 primebotframework-1.0.56/PrimeBot/ExchangeGraph/
--rw-rw-rw-   0 root         (0) root         (0)     8987 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/ExchangeGraph/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.203251 primebotframework-1.0.56/PrimeBot/FeriadosBancarios/
--rw-rw-rw-   0 root         (0) root         (0)     1925 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/FeriadosBancarios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/FeriadosBancarios/model.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.207252 primebotframework-1.0.56/PrimeBot/IntegracaoSendGrid/
--rw-rw-rw-   0 root         (0) root         (0)     4251 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/IntegracaoSendGrid/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.207252 primebotframework-1.0.56/PrimeBot/ListenerECS/
--rw-rw-rw-   0 root         (0) root         (0)     4096 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/ListenerECS/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.207252 primebotframework-1.0.56/PrimeBot/Mongo/
--rw-rw-rw-   0 root         (0) root         (0)      465 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/Mongo/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.207252 primebotframework-1.0.56/PrimeBot/OracleDB/
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/OracleDB/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.207252 primebotframework-1.0.56/PrimeBot/Vault/
--rw-rw-rw-   0 root         (0) root         (0)     2740 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/Vault/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 19:36:33.000000 primebotframework-1.0.56/PrimeBot/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-30 19:36:43.207252 primebotframework-1.0.56/PrimeBotFramework.egg-info/
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-30 19:36:43.000000 primebotframework-1.0.56/PrimeBotFramework.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      814 2024-04-30 19:36:43.000000 primebotframework-1.0.56/PrimeBotFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-30 19:36:43.000000 primebotframework-1.0.56/PrimeBotFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-30 19:36:43.000000 primebotframework-1.0.56/PrimeBotFramework.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2024-04-30 19:36:43.000000 primebotframework-1.0.56/PrimeBotFramework.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-30 19:36:43.207252 primebotframework-1.0.56/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      928 2024-04-30 19:36:33.000000 primebotframework-1.0.56/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.382867 primebotframework-1.0.60/
+-rw-r--r--   0 root         (0) root         (0)      891 2024-05-07 14:33:28.382867 primebotframework-1.0.60/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.370867 primebotframework-1.0.60/PrimeBot/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.370867 primebotframework-1.0.60/PrimeBot/B2E/
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/B2E/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.370867 primebotframework-1.0.60/PrimeBot/Cnab750/
+-rw-rw-rw-   0 root         (0) root         (0)    10261 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/Cnab750/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.370867 primebotframework-1.0.60/PrimeBot/CpfCnpj/
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/CpfCnpj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/CpfCnpj/api_codes.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/CpfCnpj/model.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.374867 primebotframework-1.0.60/PrimeBot/D4Sign/
+-rw-rw-rw-   0 root         (0) root         (0)     2600 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/D4Sign/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.374867 primebotframework-1.0.60/PrimeBot/DeathByCaptcha/
+-rw-rw-rw-   0 root         (0) root         (0)     5755 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/DeathByCaptcha/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.374867 primebotframework-1.0.60/PrimeBot/Documents/
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/Documents/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.374867 primebotframework-1.0.60/PrimeBot/Elastic/
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/Elastic/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.374867 primebotframework-1.0.60/PrimeBot/EmailAlert/
+-rw-rw-rw-   0 root         (0) root         (0)     3758 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/EmailAlert/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.374867 primebotframework-1.0.60/PrimeBot/ExchangeGraph/
+-rw-rw-rw-   0 root         (0) root         (0)     8987 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/ExchangeGraph/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.374867 primebotframework-1.0.60/PrimeBot/FeriadosBancarios/
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/FeriadosBancarios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/FeriadosBancarios/model.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.374867 primebotframework-1.0.60/PrimeBot/IntegracaoSendGrid/
+-rw-rw-rw-   0 root         (0) root         (0)     4251 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/IntegracaoSendGrid/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.378867 primebotframework-1.0.60/PrimeBot/ListenerECS/
+-rw-rw-rw-   0 root         (0) root         (0)     4096 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/ListenerECS/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.378867 primebotframework-1.0.60/PrimeBot/Mongo/
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/Mongo/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.378867 primebotframework-1.0.60/PrimeBot/OracleDB/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/OracleDB/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.378867 primebotframework-1.0.60/PrimeBot/Vault/
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/Vault/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-07 14:33:15.000000 primebotframework-1.0.60/PrimeBot/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-07 14:33:28.378867 primebotframework-1.0.60/PrimeBotFramework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      891 2024-05-07 14:33:28.000000 primebotframework-1.0.60/PrimeBotFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      814 2024-05-07 14:33:28.000000 primebotframework-1.0.60/PrimeBotFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-07 14:33:28.000000 primebotframework-1.0.60/PrimeBotFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-05-07 14:33:28.000000 primebotframework-1.0.60/PrimeBotFramework.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2024-05-07 14:33:28.000000 primebotframework-1.0.60/PrimeBotFramework.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-07 14:33:28.382867 primebotframework-1.0.60/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      928 2024-05-07 14:33:15.000000 primebotframework-1.0.60/setup.py
```

### Comparing `primebotframework-1.0.56/PKG-INFO` & `primebotframework-1.0.60/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.56
+Version: 1.0.60
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `primebotframework-1.0.56/PrimeBot/B2E/__init__.py` & `primebotframework-1.0.60/PrimeBot/B2E/__init__.py`

 * *Files identical despite different names*

### Comparing `primebotframework-1.0.56/PrimeBot/Cnab750/__init__.py` & `primebotframework-1.0.60/PrimeBot/Cnab750/__init__.py`

 * *Files identical despite different names*

### Comparing `primebotframework-1.0.56/PrimeBot/CpfCnpj/__init__.py` & `primebotframework-1.0.60/PrimeBot/CpfCnpj/__init__.py`

 * *Files identical despite different names*

### Comparing `primebotframework-1.0.56/PrimeBot/CpfCnpj/api_codes.py` & `primebotframework-1.0.60/PrimeBot/CpfCnpj/api_codes.py`

 * *Files identical despite different names*

### Comparing `primebotframework-1.0.56/PrimeBot/D4Sign/__init__.py` & `primebotframework-1.0.60/PrimeBot/D4Sign/__init__.py`

 * *Files identical despite different names*

### Comparing `primebotframework-1.0.56/PrimeBot/DeathByCaptcha/__init__.py` & `primebotframework-1.0.60/PrimeBot/DeathByCaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `primebotframework-1.0.56/PrimeBot/Documents/__init__.py` & `primebotframework-1.0.60/PrimeBot/Documents/__init__.py`

 * *Files identical despite different names*

### Comparing `primebotframework-1.0.56/PrimeBot/Elastic/__init__.py` & `primebotframework-1.0.60/PrimeBot/Elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `primebotframework-1.0.56/PrimeBot/EmailAlert/__init__.py` & `primebotframework-1.0.60/PrimeBot/EmailAlert/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 import datetime
 import glob
 from jinja2 import Template
 import os.path
-from robot.api import logger
+import logging
 from PrimeBot.IntegracaoSendGrid import IntegracaoSendGrid
 
 @dataclass
 class EmailAlert:
     """
         Envio de email para alertar falhas no funcionamento de um processo.
 
@@ -27,15 +27,15 @@
 
     def __post_init__(self) -> None:
         """
             Método pós-inicialização que realiza a conexão com a API do sendgrid.
         """
         self.sg = IntegracaoSendGrid(self.api_key, self.remetente)
 
-    def create_html(self, mensagem: str = '') -> str:
+    def converter_texto_para_html(self, mensagem: str = '') -> str:
         """
             Cria uma mensagem em HTML.
 
             Atributos:
                 mensagem (str): Mensagem para ser formatada em HTML.
             
             Retorna:
@@ -68,21 +68,23 @@
             Atributos:
                 task (str): Nome da task que falhou.
                 keyword (str): Nome da keyword processada no momento da falha.
                 mensagem_erro (str): Mensagem retornada pelo processo detalhando o erro.
         """
         data = datetime.datetime.now().strftime('%d/%m/%Y')
         hora = datetime.datetime.now().strftime('%H:%M:%S')
-        mensagem = f'<p>Olá, tudo bem?</p><p>Houve um erro durante a execução do processo: {self.nome_projeto}, que ocasionou a interrupção do mesmo antes de concluir o processo, segue informações:</p><p>Data: {data};</p><p>Hora: {hora};</p><p>Task: {task};</p><p>Keyword: {keyword};</p><p>Detalhe retornado do erro: {mensagem_erro}.</p>'
-        html = self.create_html(mensagem)
+        mensagem = f'<p>Olá, tudo bem?</p><p>Houve um erro durante a execução do processo: <b><font color="#FF0000">{self.nome_projeto}</font></b>, que ocasionou a interrupção do mesmo antes de concluir o processo, segue informações:</p><p><b>Data:</b> {data};</p><p><b>Hora:</b> {hora};</p><p><b>Task:</b> {task};</p><p><b>Keyword:</b> {keyword};</p><p><b>Detalhe retornado do erro:</b> {mensagem_erro}.</p>'
+        html = self.converter_texto_para_html(mensagem)
         to= self.destinatario
-        email = self.sg.create_message(to, f'Azul RPA Erro no projeto: {self.nome_projeto}', html)
+        email = self.sg.create_message(to, f'Azul RPA Falha no projeto: {self.nome_projeto}', html)
+        
         # Verifica se existe screenshot
         try:
             archives = os.listdir(self.pasta_screenshots)
             if len(archives) > 0:
                 screenshot = self.encontrar_ultimo_arquivo_pasta(self.pasta_screenshots)
                 email = self.sg.add_attachment(email, screenshot, 'image/png', 'attachment', 'anexo')
         except Exception as error:
-            logger.error(f'Erro ao acessar os arquivos da pasta de screenshots, detalhe: {error}!')
+            logging.error(f'Erro ao acessar os arquivos da pasta de screenshots, detalhe: {error}!')
+        
         result = self.sg.send_email(email)
-        logger.info(result, also_console=True)
+        logging.info(result, also_console=True)
```

### Comparing `primebotframework-1.0.56/PrimeBot/ExchangeGraph/__init__.py` & `primebotframework-1.0.60/PrimeBot/ExchangeGraph/__init__.py`

 * *Files identical despite different names*

### Comparing `primebotframework-1.0.56/PrimeBot/FeriadosBancarios/__init__.py` & `primebotframework-1.0.60/PrimeBot/FeriadosBancarios/__init__.py`

 * *Files identical despite different names*

### Comparing `primebotframework-1.0.56/PrimeBot/IntegracaoSendGrid/__init__.py` & `primebotframework-1.0.60/PrimeBot/IntegracaoSendGrid/__init__.py`

 * *Files identical despite different names*

### Comparing `primebotframework-1.0.56/PrimeBot/ListenerECS/__init__.py` & `primebotframework-1.0.60/PrimeBot/ListenerECS/__init__.py`

 * *Files identical despite different names*

### Comparing `primebotframework-1.0.56/PrimeBot/OracleDB/__init__.py` & `primebotframework-1.0.60/PrimeBot/OracleDB/__init__.py`

 * *Files identical despite different names*

### Comparing `primebotframework-1.0.56/PrimeBot/Vault/__init__.py` & `primebotframework-1.0.60/PrimeBot/Vault/__init__.py`

 * *Files identical despite different names*

### Comparing `primebotframework-1.0.56/PrimeBotFramework.egg-info/PKG-INFO` & `primebotframework-1.0.60/PrimeBotFramework.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.56
+Version: 1.0.60
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `primebotframework-1.0.56/PrimeBotFramework.egg-info/SOURCES.txt` & `primebotframework-1.0.60/PrimeBotFramework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `primebotframework-1.0.56/setup.py` & `primebotframework-1.0.60/setup.py`

 * *Files identical despite different names*

