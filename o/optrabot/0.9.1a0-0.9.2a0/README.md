# Comparing `tmp/optrabot-0.9.1a0.tar.gz` & `tmp/optrabot-0.9.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optrabot-0.9.1a0.tar", max compression
+gzip compressed data, was "optrabot-0.9.2a0.tar", max compression
```

## Comparing `optrabot-0.9.1a0.tar` & `optrabot-0.9.2a0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      742 2023-12-14 21:15:50.230643 optrabot-0.9.1a0/README.md
--rw-r--r--   0        0        0        0 2023-12-12 13:10:12.039398 optrabot-0.9.1a0/optrabot/__init__.py
--rw-r--r--   0        0        0       38 2024-02-22 12:22:44.563187 optrabot-0.9.1a0/optrabot/alembic/README
--rw-r--r--   0        0        0     2717 2024-02-29 07:20:04.745375 optrabot-0.9.1a0/optrabot/alembic/env.py
--rw-r--r--   0        0        0      635 2024-02-22 12:22:44.563872 optrabot-0.9.1a0/optrabot/alembic/script.py.mako
--rw-r--r--   0        0        0     1996 2024-02-22 12:22:44.564106 optrabot-0.9.1a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py
--rw-r--r--   0        0        0     3633 2024-02-22 12:22:44.562937 optrabot-0.9.1a0/optrabot/alembic.ini
--rw-r--r--   0        0        0    11856 2024-04-15 10:20:52.308184 optrabot-0.9.1a0/optrabot/config.py
--rw-r--r--   0        0        0     3133 2024-04-15 10:20:52.308983 optrabot-0.9.1a0/optrabot/crud.py
--rw-r--r--   0        0        0     1106 2024-02-22 12:22:44.565150 optrabot-0.9.1a0/optrabot/database.py
--rw-r--r--   0        0        0     2323 2024-04-10 09:35:05.013016 optrabot-0.9.1a0/optrabot/main.py
--rw-r--r--   0        0        0      936 2023-12-21 19:35:29.667749 optrabot-0.9.1a0/optrabot/marketdatatype.py
--rw-r--r--   0        0        0     1613 2024-02-22 12:22:44.565732 optrabot-0.9.1a0/optrabot/models.py
--rw-r--r--   0        0        0      966 2024-02-22 12:22:44.566114 optrabot-0.9.1a0/optrabot/optionhelper.py
--rw-r--r--   0        0        0    10650 2024-04-15 18:21:56.755586 optrabot-0.9.1a0/optrabot/optrabot.py
--rw-r--r--   0        0        0      855 2024-02-22 12:22:44.566593 optrabot-0.9.1a0/optrabot/schemas.py
--rw-r--r--   0        0        0     2859 2024-02-29 07:20:04.746827 optrabot-0.9.1a0/optrabot/stoplossadjuster.py
--rw-r--r--   0        0        0     2936 2024-02-22 12:22:44.567158 optrabot-0.9.1a0/optrabot/tradehelper.py
--rw-r--r--   0        0        0        0 2024-02-22 12:22:44.567199 optrabot-0.9.1a0/optrabot/tradetemplate/__init__.py
--rw-r--r--   0        0        0      177 2024-02-22 12:22:44.567811 optrabot-0.9.1a0/optrabot/tradetemplate/ironfly.py
--rw-r--r--   0        0        0      181 2024-02-22 12:22:44.568125 optrabot-0.9.1a0/optrabot/tradetemplate/putspread.py
--rw-r--r--   0        0        0     3405 2024-03-19 15:36:19.404722 optrabot-0.9.1a0/optrabot/tradetemplate/template.py
--rw-r--r--   0        0        0     2273 2024-04-22 05:51:40.165667 optrabot-0.9.1a0/optrabot/tradetemplate/templatefactory.py
--rw-r--r--   0        0        0      564 2024-02-22 12:22:44.568968 optrabot-0.9.1a0/optrabot/tradetemplate/templatetrigger.py
--rw-r--r--   0        0        0    40177 2024-04-22 10:57:10.421697 optrabot-0.9.1a0/optrabot/tradinghubclient.py
--rw-r--r--   0        0        0      821 2024-04-22 11:18:08.466139 optrabot-0.9.1a0/pyproject.toml
--rw-r--r--   0        0        0     1842 1970-01-01 00:00:00.000000 optrabot-0.9.1a0/PKG-INFO
+-rw-r--r--   0        0        0      742 2023-12-14 21:15:50.230643 optrabot-0.9.2a0/README.md
+-rw-r--r--   0        0        0        0 2023-12-12 13:10:12.039398 optrabot-0.9.2a0/optrabot/__init__.py
+-rw-r--r--   0        0        0       38 2024-02-22 12:22:44.563187 optrabot-0.9.2a0/optrabot/alembic/README
+-rw-r--r--   0        0        0     2717 2024-02-29 07:20:04.745375 optrabot-0.9.2a0/optrabot/alembic/env.py
+-rw-r--r--   0        0        0      635 2024-02-22 12:22:44.563872 optrabot-0.9.2a0/optrabot/alembic/script.py.mako
+-rw-r--r--   0        0        0     1996 2024-02-22 12:22:44.564106 optrabot-0.9.2a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py
+-rw-r--r--   0        0        0     3633 2024-02-22 12:22:44.562937 optrabot-0.9.2a0/optrabot/alembic.ini
+-rw-r--r--   0        0        0    11856 2024-04-15 10:20:52.308184 optrabot-0.9.2a0/optrabot/config.py
+-rw-r--r--   0        0        0     3133 2024-04-15 10:20:52.308983 optrabot-0.9.2a0/optrabot/crud.py
+-rw-r--r--   0        0        0     1106 2024-02-22 12:22:44.565150 optrabot-0.9.2a0/optrabot/database.py
+-rw-r--r--   0        0        0     2323 2024-05-07 18:46:58.969402 optrabot-0.9.2a0/optrabot/main.py
+-rw-r--r--   0        0        0      936 2023-12-21 19:35:29.667749 optrabot-0.9.2a0/optrabot/marketdatatype.py
+-rw-r--r--   0        0        0     1613 2024-02-22 12:22:44.565732 optrabot-0.9.2a0/optrabot/models.py
+-rw-r--r--   0        0        0      966 2024-02-22 12:22:44.566114 optrabot-0.9.2a0/optrabot/optionhelper.py
+-rw-r--r--   0        0        0    10733 2024-05-08 11:10:23.701664 optrabot-0.9.2a0/optrabot/optrabot.py
+-rw-r--r--   0        0        0      855 2024-02-22 12:22:44.566593 optrabot-0.9.2a0/optrabot/schemas.py
+-rw-r--r--   0        0        0     2859 2024-02-29 07:20:04.746827 optrabot-0.9.2a0/optrabot/stoplossadjuster.py
+-rw-r--r--   0        0        0     2936 2024-02-22 12:22:44.567158 optrabot-0.9.2a0/optrabot/tradehelper.py
+-rw-r--r--   0        0        0        0 2024-02-22 12:22:44.567199 optrabot-0.9.2a0/optrabot/tradetemplate/__init__.py
+-rw-r--r--   0        0        0      177 2024-05-08 06:34:31.950408 optrabot-0.9.2a0/optrabot/tradetemplate/ironfly.py
+-rw-r--r--   0        0        0      181 2024-02-22 12:22:44.568125 optrabot-0.9.2a0/optrabot/tradetemplate/putspread.py
+-rw-r--r--   0        0        0     3405 2024-03-19 15:36:19.404722 optrabot-0.9.2a0/optrabot/tradetemplate/template.py
+-rw-r--r--   0        0        0     2273 2024-04-22 05:51:40.165667 optrabot-0.9.2a0/optrabot/tradetemplate/templatefactory.py
+-rw-r--r--   0        0        0      564 2024-02-22 12:22:44.568968 optrabot-0.9.2a0/optrabot/tradetemplate/templatetrigger.py
+-rw-r--r--   0        0        0    49985 2024-05-08 11:10:23.702123 optrabot-0.9.2a0/optrabot/tradinghubclient.py
+-rw-r--r--   0        0        0      821 2024-05-08 11:15:41.630244 optrabot-0.9.2a0/pyproject.toml
+-rw-r--r--   0        0        0     1842 1970-01-01 00:00:00.000000 optrabot-0.9.2a0/PKG-INFO
```

### Comparing `optrabot-0.9.1a0/README.md` & `optrabot-0.9.2a0/README.md`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/alembic/env.py` & `optrabot-0.9.2a0/optrabot/alembic/env.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/alembic/script.py.mako` & `optrabot-0.9.2a0/optrabot/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py` & `optrabot-0.9.2a0/optrabot/alembic/versions/cc3c6f4d83dc_initial_database.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/alembic.ini` & `optrabot-0.9.2a0/optrabot/alembic.ini`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/config.py` & `optrabot-0.9.2a0/optrabot/config.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/crud.py` & `optrabot-0.9.2a0/optrabot/crud.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/database.py` & `optrabot-0.9.2a0/optrabot/database.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/main.py` & `optrabot-0.9.2a0/optrabot/main.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/marketdatatype.py` & `optrabot-0.9.2a0/optrabot/marketdatatype.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/models.py` & `optrabot-0.9.2a0/optrabot/models.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/optionhelper.py` & `optrabot-0.9.2a0/optrabot/optionhelper.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/optrabot.py` & `optrabot-0.9.2a0/optrabot/optrabot.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,26 @@
 from optrabot.marketdatatype import MarketDataType
 from optrabot.optionhelper import OptionHelper
 from optrabot.config import Config
 from .tradinghubclient import TradinghubClient
 import pkg_resources
 from .database import *
 from . import crud
+from apscheduler.schedulers.asyncio import AsyncIOScheduler
 
 class OptraBot():
 	def __init__(self, app: FastAPI):
 		self.app = app
 		self._apiKey = None
 		self.thc : TradinghubClient = None
 		self._tradingEnabled = False
 		self._marketDataType : MarketDataType = None
 		self.Version = pkg_resources.get_distribution('optrabot').version
+		self._backgroundScheduler = AsyncIOScheduler()
+		self._backgroundScheduler.start()
 		if self.Version == '0.1.0':
 			self.Version = '0.8.1' # Set Version to 0.8.1 for the loca development environment
 
 	def __setitem__(self, key, value):
 		setattr(self, key, value)
 
 	def __getitem__(self, key):
@@ -51,17 +54,16 @@
 		except Exception as excp:
 			logger.error('Problem on Startup: {}', excp)
 			logger.error('OptraBot halted!')
 			return
 		
 		logger.info('Sucessfully connected to OptraBot Hub')
 		await self.connect_ib()
-		await self.thc.start_polling()
-		task = asyncio.create_task(self._statusInfoDelayed())
-		task.add_done_callback(self.handleTaskDone)
+		self.thc.start_polling(self._backgroundScheduler)
+		self._backgroundScheduler.add_job(self._statusInfo, 'interval', minutes=5, id='statusInfo')
 
 	async def shutdown(self):
 		logger.debug('OptraBot shutdown()')
 		try:
 			logger.info('Disconnecting from OptraBot Hub ...')
 			await self.thc.reportAction(action='SD')
 		except Exception as excp:
@@ -73,28 +75,26 @@
 			if ib.isConnected():
 				logger.info('Disconnect from IB')
 				ib.disconnectedEvent -= self.onDisconnected
 				ib.disconnect()
 		except Exception as excp:
 			pass
 
-	async def _statusInfoDelayed(self):
-		await asyncio.sleep(60*5)
-		asyncio.create_task(self._statusInfo())
+		self._backgroundScheduler.shutdown()
 
-	async def _statusInfo(self):
+	def _statusInfo(self):
 		siTradingEnabled = 'Yes' if self._tradingEnabled == True else 'No' 
 		siPosition = 'Yes' if self.thc._position == True else 'No'
 		siHubConnection = 'OK' if self.thc.isHubConnectionOK() == True else 'Problem!'
 		if self._tradingEnabled == True:
 			logger.info("Status Info: Hub Connection: {} Trading Enabled: {} Open Position: {}", siHubConnection, siTradingEnabled, siPosition)
 		else:
 			logger.warning("Status Info: Hub Connection: {} Trading Enabled: {} Open Position: {}", siHubConnection, siTradingEnabled, siPosition)
 
-		asyncio.create_task(self._statusInfoDelayed())
+		#asyncio.create_task(self._statusInfoDelayed())
 
 	async def connect_ib(self):
 		logger.debug('Trying to connect with IB ...')
 		delaySecs = 30
 		ib = IB()
 		self['ib'] = ib
 		asyncio.create_task(self._connect_ib_task(0, delaySecs))
```

### Comparing `optrabot-0.9.1a0/optrabot/schemas.py` & `optrabot-0.9.2a0/optrabot/schemas.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/stoplossadjuster.py` & `optrabot-0.9.2a0/optrabot/stoplossadjuster.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/tradehelper.py` & `optrabot-0.9.2a0/optrabot/tradehelper.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/tradetemplate/template.py` & `optrabot-0.9.2a0/optrabot/tradetemplate/template.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/tradetemplate/templatefactory.py` & `optrabot-0.9.2a0/optrabot/tradetemplate/templatefactory.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/tradetemplate/templatetrigger.py` & `optrabot-0.9.2a0/optrabot/tradetemplate/templatetrigger.py`

 * *Files identical despite different names*

### Comparing `optrabot-0.9.1a0/optrabot/tradinghubclient.py` & `optrabot-0.9.2a0/optrabot/tradinghubclient.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import Any, List
 from fastapi import status
 from sqlalchemy.orm import Session
 from optrabot.database import get_db_engine
 from optrabot.tradehelper import TradeHelper
 from optrabot.optionhelper import OptionHelper
 from optrabot.stoplossadjuster import StopLossAdjuster
+from optrabot.tradetemplate.template import Template
 from optrabot.tradetemplate.templatetrigger import TriggerType
 
 class TradinghubClient():
 	def __init__(self, optraBot):
 		logger.debug("TradinghubClient Init")
 		self._lastAnswerReceivedAt = None
 		self.optraBot = optraBot
@@ -71,15 +72,15 @@
 		self._closingLongLegs = False
 		self._fillTransactionMap = {}
 		self._entryOrderFilled = 0   # Number of fills for the entry order
 		
 	async def shutdown(self):
 		logger.info('Shutting down Trading Hub Client.')
 		self._shuttingdown = True
-		self._stopPositionMonitoring()
+		#self._stopPositionMonitoring()
 
 	async def reportAction(self, action: str, additional_data: str = '') -> bool:
 		"""
 		Reports a livecycle action and relevant details to the OptraBot Hub and check if it is allowed.
 		- Instance with the same id must not be running already
 		- A subscription must be active
 		- The configured account numbers must not be used by another registered user already
@@ -101,15 +102,14 @@
 			jsonData = response.json()
 			if jsonData['detail']:
 				errorMessage = jsonData['detail']
 			else:
 				errorMessage = response.reason_phrase
 			raise Exception(errorMessage)
 
-
 	async def _poll(self):
 		try:
 			fetch_url = self.hub_host + '/fetch_signal'
 			url_params = {'agentid': self._agentId}
 			headers = {'X-API-Key': self._apiKey, 'X-Version': self.optraBot.Version}
 			if self._shuttingdown:
 				logger.debug("Client Session closed. Stop polling.")
@@ -119,14 +119,207 @@
 			response = httpx.get(fetch_url, params=url_params, follow_redirects=True, headers=headers)
 			logger.debug('Answer received ({}).', response.status_code)
 			if response.status_code != status.HTTP_200_OK:
 				if response.status_code == status.HTTP_401_UNAUTHORIZED:
 					logger.error("Error requesting signal from OptraBot Hub: {}", response.json()['detail'])
 				else:
 					logger.error("Error on HTTP request: {}", response.reason_phrase)
+				return
+			
+			self._lastAnswerReceivedAt = datetime.now()
+			if response.text != '\"\"' and response.text != '':
+				logger.debug("Response {}", response.content )
+
+				try:
+					response_data = json.loads(response.content)
+				except json.JSONDecodeError as jsonExcp:
+					logger.error("Didn't receive JSON data!")
+					return
+				
+				# Check if the signal is valid and configured
+				logger.debug('Received Signal: {}', response_data['strategy'])
+				triggeredTemplate = None
+				for template in self._config.getTemplates():
+					trigger = template.getTrigger()
+					if trigger.type == TriggerType.External and trigger.value == response_data['strategy']:
+						triggeredTemplate = template
+						break
+				if triggeredTemplate == None:
+					logger.warning('No template for external trigger value {} configured!', response_data['strategy'])
+					return
+			
+				signalTime = self._parseTimestamp(response_data['time'])
+				if signalTime == None or self._signalIsOutdated(signalTime):
+					logger.warning('Signal is outdated already or Signal timestamp is invalid!')
+					return
+				
+				# Check if there is no positions open already
+				if self._position != False:
+					logger.warning('Skipping signal, because there is a position open already!')
+					return
+				
+				# Obtain the Template Executor and schedule a job to process the signal
+				#await self.optraBot.executeTradeTemplate(triggeredTemplate)
+				self.optraBot._backgroundScheduler.add_job(self.excuteTradeTemplate, args=[triggeredTemplate, response_data], id='executetemplate')
+				return
+				
+		except Exception as anyEcxp:
+			logger.error("Exception occured during poll: {}", anyEcxp)
+
+	async def excuteTradeTemplate(self, template: Template, response_data: dict):
+		""" This method is called via Job Scheduler for executing the given Trade Template in the background.
+		"""
+		logger.debug(f"Excuting Trade Template {template.name}")
+		try:
+			ib: IB = self.optraBot['ib']
+			if not ib.isConnected():
+				logger.error("Interactive Brokers is not connected. Unable to process received signal!")
+				return
+			
+			if not self.optraBot.isTradingEnabled():
+				logger.error("Trading is not enabled. Looks like your Market Data Subscription is wrong. Skippimg this Trade!")
+				return
+			
+			spx = Index('SPX', 'CBOE')
+			qualifiedContracts = await ib.qualifyContractsAsync(spx) 
+			[ticker] = await ib.reqTickersAsync(spx)
+			spxValue = ticker.marketPrice()
+			#self.app['SPXPrice'] = spxValue
+			logger.debug("SPX Market Price {}", spxValue)
+
+			chains = await ib.reqSecDefOptParamsAsync(spx.symbol, '', spx.secType, spx.conId)
+			chain = next(c for c in chains if c.tradingClass == 'SPXW' and c.exchange == 'SMART')
+			if chain == None:
+				logger.error("No Option Chain for SPXW and CBOE found! Doing no trade!")
+				return
+			
+			# Options Kontrakte ermitteln
+			nan = float('nan')
+			self._currentTemplate = template
+			self._currentTemplate.resetStopLossAdjuster()
+			if not self._currentTemplate.wing:
+				wingSize = 70
+			else:
+				wingSize = self._currentTemplate.wing
+			amount = self._currentTemplate.amount
+			accountNo = self._currentTemplate.account
+			current_date = dt.date.today()
+			expiration = current_date.strftime('%Y%m%d')
+			shortLegStrike = float(response_data['vwaptarget'])
+			longPutStrike = shortLegStrike - wingSize
+			longCallStrike = shortLegStrike + wingSize
+			logger.info("Building Iron Fly combo with Short strike {}, Long Put strike {} and Long Call strike {}", shortLegStrike, longPutStrike, longCallStrike)
+			
+			# Überprüfen das auf den geplanten Legs keine anderen Orders liegen
+			logger.debug('Checking for open Trades if Combo Legs are colliding')
+			contractsWithOpenOrders = await self._getAllOpenOrderContracts(accountNo, spx.symbol)
+
+			shortPutContract = Option(spx.symbol, expiration, shortLegStrike, 'P', 'SMART', tradingClass = 'SPXW')
+			await ib.qualifyContractsAsync(shortPutContract)
+			if not OptionHelper.checkContractIsQualified(shortPutContract):
+				return
+			if shortPutContract.conId in contractsWithOpenOrders:
+				logger.error('Existing open order at stike price {}. Trade cannot be placed!', shortLegStrike)
+				return
+
+			shortCallContract = Option(spx.symbol, expiration, shortLegStrike, 'C', 'SMART', tradingClass = 'SPXW')				
+			await ib.qualifyContractsAsync(shortCallContract)
+			if not OptionHelper.checkContractIsQualified(shortCallContract):
+				return
+			if shortCallContract.conId in contractsWithOpenOrders:
+				logger.error('Existing open order at strike price {}. Trade cannot be placed!', shortLegStrike)
+				return
+			
+			longPutContract = await self._DetermineValidLongOption(spx.symbol, expiration, longPutStrike, 'P', contractsWithOpenOrders)
+			if longPutContract == None or not OptionHelper.checkContractIsQualified(longPutContract):
+				logger.error('Unable to determine a valid Long Put option for the trade!')
+				return
+			if longPutContract.strike != longPutStrike:
+				logger.warning('Using different Long Put strike {}, because of existing open orders on desired strike {}.', longPutContract.strike, longPutStrike)
+
+			longCallContract = await self._DetermineValidLongOption(spx.symbol, expiration, longCallStrike, 'C', contractsWithOpenOrders)
+			if longCallContract == None or not OptionHelper.checkContractIsQualified(longCallContract):
+				logger.error('Unable to determine a valid Long Call option for the trade!')
+				return
+			if longCallContract.strike != longCallStrike:
+				logger.warning('Using different Long Call strike {}, because of existing open orders on desired strike {}.', longCallContract.strike, longCallStrike)
+
+			self._ironFlyLongLegContracts = [longCallContract, longPutContract]
+			self._ironFlyContracts = [shortPutContract, shortCallContract, longPutContract, longCallContract]
+			self._ironFlyComboContract = Contract(symbol=spx.symbol, secType='BAG', exchange='SMART', currency='USD', comboLegs=[])
+			self._ironFlyShortComboContract = Contract(symbol=spx.symbol, secType='BAG', exchange='SMART', currency='USD', comboLegs=[])
+
+			ironFlyMidPrice = None
+			for i in range(5):
+				tickers = await ib.reqTickersAsync(*self._ironFlyContracts)
+				logger.debug("Tickers {}", tickers)
+				ironFlyMidPrice = self._calculateIronFlyMidPrice(tickers, ironFlyComboContract=self._ironFlyComboContract, 
+											   ironFlyShortComboContract=self._ironFlyShortComboContract, 
+											   shortPutContract=shortPutContract,
+											   shortCallContract=shortCallContract,
+											   longPutContract=longPutContract,
+											   longCallContract=longCallContract)
+				if ironFlyMidPrice != None:
+					break
+				await asyncio.sleep(1)
+			
+			#if util.isNan(ironFlyMidPrice):
+			if ironFlyMidPrice == None:
+				logger.error("No Mid Price for combo could be calculated!")
+				return
+
+			limitPrice = ironFlyMidPrice
+
+			logger.info("IronFly Combo Mid Price: {} Ask Price: {}", ironFlyMidPrice, self._ironFlyAskPrice)
+
+			if not self._meetsMinimumPremium(limitPrice):
+				logger.info('Premium below configured minimum premium of ${}. Trade is not executed!', self._currentTemplate.minPremium)
+				return
+			
+			order = LimitOrder('BUY', amount, limitPrice)
+			with Session(get_db_engine()) as session:
+				newTrade = schemas.TradeCreate(account=accountNo, symbol='SPX', strategy=self._currentTemplate.strategy)
+				self._currentTrade = crud.create_trade(session, newTrade)
+				order.orderRef = 'OTB (' + str(self._currentTrade.id) + '): ' + template.name + ' - Open'
+			order.account = accountNo
+			order.outsideRth = True
+			self._fillTransactionMap.clear()
+			self._entryTrade = ib.placeOrder(self._ironFlyComboContract, order)
+			self._entryTrade.statusEvent += self.onOrderStatusEvent
+			self._entryTradeContract = self._ironFlyComboContract
+			self._ironFlyAskPrice = 0.0
+			self._longLegFillsPrice = 0.0
+			self._longLegFillsReceived = 0
+			self._slShortTrade = None
+			self._tpTrade = None
+			self._entryOrderFilled = 0
+			self._closingLongLegs = False
+			logger.debug("Account: {} Trade placed: {} Number of contracts: {}", order.account, self._entryTrade, amount)
+			asyncio.create_task(self._trackEntryOrder()).add_done_callback(self.optraBot.handleTaskDone)
+
+		except Exception as excp:
+						logger.error("Exception: {}", excp)
+
+	async def _poll_old(self):
+		try:
+			fetch_url = self.hub_host + '/fetch_signal'
+			url_params = {'agentid': self._agentId}
+			headers = {'X-API-Key': self._apiKey, 'X-Version': self.optraBot.Version}
+			if self._shuttingdown:
+				logger.debug("Client Session closed. Stop polling.")
+				return
+			
+			logger.debug('Checking for Signal from Hub.')
+			response = httpx.get(fetch_url, params=url_params, follow_redirects=True, headers=headers)
+			logger.debug('Answer received ({}).', response.status_code)
+			if response.status_code != status.HTTP_200_OK:
+				if response.status_code == status.HTTP_401_UNAUTHORIZED:
+					logger.error("Error requesting signal from OptraBot Hub: {}", response.json()['detail'])
+				else:
+					logger.error("Error on HTTP request: {}", response.reason_phrase)
 				await self._scheduleNextPoll()
 				return
 
 			self._lastAnswerReceivedAt = datetime.now()
 			if response.text != '\"\"' and response.text != '':
 				logger.debug("Response {}", response.content )
 
@@ -347,14 +540,15 @@
 				midPrice = (ticker.ask + ticker.bid) / 2
 				if util.isNan(midPrice) or (ticker.ask == -1.00 and ticker.bid == -1.00):
 					midPrice = 0.05
 				ironFlyMidPrice += midPrice
 				if not util.isNan(ticker.ask):
 					self._ironFlyAskPrice += ticker.ask
 					ironFlyComboContract.comboLegs.append(ComboLeg(conId=longCallContract.conId, ratio=1, action='BUY', exchange='SMART'))
+		self._ironFlyAskPrice = OptionHelper.roundToTickSize(self._ironFlyAskPrice)
 		return OptionHelper.roundToTickSize(ironFlyMidPrice)
 
 	async def _trackEntryOrder(self):
 		await asyncio.sleep(5) # Wait 5 seconds for order Execution
 		ib: IB = self.optraBot['ib']
 		if self._entryTrade == None:
 			return
@@ -405,15 +599,16 @@
 				if self._position == False:
 					logger.info('Entry Order has been filled at ${} (Qty: {}) and trade is running now.', trade.orderStatus.avgFillPrice, trade.orderStatus.filled)
 					self._position = True
 					if self._currentTemplate.stopLossAdjuster:
 						self._currentTemplate.stopLossAdjuster.setBasePrice(round(self._entryTrade.orderStatus.avgFillPrice * -1, 2))
 					asyncio.create_task(self._placeTakeProfitAndStop(trade)).add_done_callback(self.optraBot.handleTaskDone)
 					#Run 1. Position Monitoring with delay
-					asyncio.create_task(self._monitorPositionDelayed()).add_done_callback(self.optraBot.handleTaskDone)
+					#asyncio.create_task(self._monitorPositionDelayed()).add_done_callback(self.optraBot.handleTaskDone)
+					self.optraBot._backgroundScheduler.add_job(self._monitorPosition, 'interval', seconds=10, id='MonitorPosition')
 				elif self._position == True:
 					logger.debug('Additionally fill quantity (Qty: {}) for the entry order...depending orders need to be adjusted.', trade.orderStatus.filled)
 					asyncio.create_task(self._adjustTakeProfitAndStop(trade)).add_done_callback(self.optraBot.handleTaskDone)
 
 				if trade.orderStatus.remaining > 0:
 					logger.warning('Partial fill for entry order. Remaining: {}', trade.orderStatus.remaining)
 				executedAmount = trade.orderStatus.filled - self._entryOrderFilled
@@ -697,21 +892,25 @@
 		logger.debug('Enter Monitor position()')
 		if self._position == False:
 			logger.debug('Position has been closed. Stopping Position-Monitoring now.')
 			#self._positionMonitorTask = None
 			self._stopPositionMonitoring()
 			return
 
-		asyncio.create_task(self._monitorPositionDelayed()).add_done_callback(self.optraBot.handleTaskDone)
+		#asyncio.create_task(self._monitorPositionDelayed()).add_done_callback(self.optraBot.handleTaskDone)
 
 		ib: IB = self.optraBot['ib']
 		if not ib.isConnected():
 			logger.error('Interactive Brokers is not connected. Unable to monitor position!')
 			return
 		
+		if self._position == False:
+			logger.debug('Position has been closed. Stopping Position-Monitoring now.')
+			return
+
 		tickers = await ib.reqTickersAsync(*self._ironFlyContracts)
 		longLegsValue = 0
 		currentIronFlyAskPrice = 0
 		currentIronFlyBidPrice = 0
 		adjustedStopLossPrice = None
 		for ticker in tickers:
 			if ticker.contract in self._ironFlyLongLegContracts:
@@ -719,15 +918,19 @@
 					longLegsValue += ticker.bid
 					currentIronFlyBidPrice -= ticker.bid
 					currentIronFlyAskPrice += ticker.ask
 			else:
 				# Für Short Legs müssen die Ask Preise addiert werden
 				currentIronFlyBidPrice += ticker.ask
 				currentIronFlyAskPrice -= ticker.bid
-			
+	
+		if self._position == False:
+			logger.debug('Position has been closed. Stopping Position-Monitoring now.')
+			return
+
 		if self._currentTemplate.stopLossAdjuster:
 			if not self._currentTemplate.stopLossAdjuster.isTriggered():
 				# Ask Preis muss positiv gemacht werden
 				currentIronFlyAskPrice = abs(currentIronFlyAskPrice)
 				currentIronFlyPrice = OptionHelper.calculateMidPrice(currentIronFlyBidPrice, currentIronFlyAskPrice)
 				#currentIronFlyPrice = round(currentIronFlyPrice, 2)
 				adjustedStopLossPrice = self._currentTemplate.stopLossAdjuster.execute(currentIronFlyPrice)
@@ -740,14 +943,19 @@
 				logger.debug('Stoploss adjustment has been performed already.')
 		else:
 			logger.debug('No StopLoss adjustment configured.')
 		desiredStopPrice = OptionHelper.roundToTickSize(self._ironFlyStopPrice + longLegsValue)
 		currentStopPrice = OptionHelper.roundToTickSize(self._slShortTrade.order.auxPrice)
 		logger.debug('Long Legs value {} Current Short SL Price: {} Desired Short SL Pice: {}', round(longLegsValue,2), currentStopPrice, desiredStopPrice)
 		openTrades = await ib.reqOpenOrdersAsync()
+
+		if self._position == False:
+			logger.debug('Position has been closed. Stopping Position-Monitoring now.')
+			return
+
 		if self._slShortTrade in openTrades:
 			if self._slShortTrade.isActive():
 				if currentStopPrice != desiredStopPrice:
 					self._slShortTrade.order.auxPrice = desiredStopPrice
 					logger.info('Adjusting Stop Loss price to ${}', desiredStopPrice)
 					ib.placeOrder(self._slShortTrade.contract, self._slShortTrade.order)
 					logger.debug('Updated SL order with id: {}', self._slShortTrade.order.orderId)
@@ -769,15 +977,15 @@
 	async def _reestablishStopLossOrder(self, desiredStopPrice: float):
 		"""
 		Tries to create a new Stop Loss order for the open position based on the given stop price.
 		"""
 		logger.debug('Reestablishing Stop Loss order for Short Legs')
 		ib: IB = self.optraBot['ib']
 		if not ib.isConnected():
-			logger.error('Interactive Brokers is not connected. Unable to monitor position!')
+			logger.error('Interactive Brokers is not connected. Unable to reestablish Stop Loss Order!')
 			return
 		
 		now = datetime.now()
 		ocaGroup = self._currentTemplate.account + '_' + now.strftime('%H%M%S')
 		stopShortsOrder = StopOrder('BUY', self._entryTrade.orderStatus.filled, desiredStopPrice)
 		stopShortsOrder.account = self._currentTemplate.account
 		stopShortsOrder.orderRef = 'OTB (' + str(self._currentTrade.id) + '): ' + self._currentTemplate.name + ' - SL Short Legs'
@@ -860,55 +1068,58 @@
 			return True
 		return False
 
 	async def _scheduleNextPoll(self):
 		await asyncio.sleep(5)
 		asyncio.create_task(self._poll()).add_done_callback(self.optraBot.handleTaskDone)
 		
-	async def start_polling(self):
+	def start_polling(self, scheduler):
 		"""
 		Tradinghub Polling runner
 		"""
 		logger.debug("start_polling")
 
 		if self._apiKey == None:
 			logger.debug("No API Key configured. Stop polling.")
 			return
 
 		if self._agentId == None:
 			logger.error("No Instance ID configured in config.yaml. Stop polling!")
 			return
 
-		try:
-			tasks: List[asyncio.Task[Any]] = [
-				asyncio.create_task(self._poll())
-			]
-			for task in tasks:
-				task.add_done_callback(self.optraBot.handleTaskDone)
-			#tasks.append(asyncio.create_task(self._stop_signal.wait()))
-			done, pending = await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
-
-			for task in pending:
-				# (mostly) Graceful shutdown unfinished tasks
-				task.cancel()
-				with suppress(asyncio.CancelledError):
-					await task
-				# Wait finished tasks to propagate unhandled exceptions
-				await asyncio.gather(*done)
-		except Exception as excp:
-			logger.error("Exception {}", excp)
+		scheduler.add_job(self._poll, 'interval', seconds=5)
+
+		# try:
+		# 	tasks: List[asyncio.Task[Any]] = [
+		# 		asyncio.create_task(self._poll())
+		# 	]
+		# 	for task in tasks:
+		# 		task.add_done_callback(self.optraBot.handleTaskDone)
+		# 	#tasks.append(asyncio.create_task(self._stop_signal.wait()))
+		# 	done, pending = await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
+
+		# 	for task in pending:
+		# 		# (mostly) Graceful shutdown unfinished tasks
+		# 		task.cancel()
+		# 		with suppress(asyncio.CancelledError):
+		# 			await task
+		# 		# Wait finished tasks to propagate unhandled exceptions
+		# 		await asyncio.gather(*done)
+		# except Exception as excp:
+		# 	logger.error("Exception {}", excp)
 
 	def _stopPositionMonitoring(self):
-		tasks = asyncio.all_tasks()
-		for task in tasks:
-			if task.get_name() == 'MonitorPosition':
-				task.cancel()
+		#tasks = asyncio.all_tasks()
+		#for task in tasks:
+		#	if task.get_name() == 'MonitorPosition':
+		#		task.cancel()
 		#if self._positionMonitorTask:
 		#	self._positionMonitorTask.cancel()
 		#	self._positionMonitorTask = None
+		self.optraBot._backgroundScheduler.remove_job('MonitorPosition')
 
 	def isHubConnectionOK(self) -> bool:
 		""" Returns True if the last request to the OptraBot Hub was responed 
 		30 seconds ago or less.
 		"""
 		if self._lastAnswerReceivedAt == None:
 			return False
```

### Comparing `optrabot-0.9.1a0/pyproject.toml` & `optrabot-0.9.2a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optrabot"
-version = "0.9.1a0"
+version = "0.9.2a0"
 description = "QuantX OptraBot is a Options Trading Bot for automatically trading options strategies with an Interactive Brokers account."
 authors = ["QuantX GmbH"]
 readme = "README.md"
 license = "MIT"
 homepage = "http://www.optrabot.com"
 keywords = ["tws"]
 packages =  [{include = "optrabot"}]
```

### Comparing `optrabot-0.9.1a0/PKG-INFO` & `optrabot-0.9.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optrabot
-Version: 0.9.1a0
+Version: 0.9.2a0
 Summary: QuantX OptraBot is a Options Trading Bot for automatically trading options strategies with an Interactive Brokers account.
 Home-page: http://www.optrabot.com
 License: MIT
 Keywords: tws
 Author: QuantX GmbH
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

