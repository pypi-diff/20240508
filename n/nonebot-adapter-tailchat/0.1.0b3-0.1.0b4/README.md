# Comparing `tmp/nonebot_adapter_tailchat-0.1.0b3.tar.gz` & `tmp/nonebot_adapter_tailchat-0.1.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_tailchat-0.1.0b3.tar", max compression
+gzip compressed data, was "nonebot_adapter_tailchat-0.1.0b4.tar", max compression
```

## Comparing `nonebot_adapter_tailchat-0.1.0b3.tar` & `nonebot_adapter_tailchat-0.1.0b4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11335 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/LICENSE
--rw-r--r--   0        0        0     1189 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/README.md
--rw-r--r--   0        0        0      260 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/__init__.py
--rw-r--r--   0        0        0     6259 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/adapter.py
--rw-r--r--   0        0        0    21563 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/api.py
--rw-r--r--   0        0        0     6659 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/bbcode.py
--rw-r--r--   0        0        0     3759 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/bot.py
--rw-r--r--   0        0        0      675 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/config.py
--rw-r--r--   0        0        0       26 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/const.py
--rw-r--r--   0        0        0     6135 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/event.py
--rw-r--r--   0        0        0      761 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/exception.py
--rw-r--r--   0        0        0     8711 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/message.py
--rw-r--r--   0        0        0     4505 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/model.py
--rw-r--r--   0        0        0      374 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/permission.py
--rw-r--r--   0        0        0      203 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/rule.py
--rw-r--r--   0        0        0     1697 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/util.py
--rw-r--r--   0        0        0     1146 2024-05-06 08:46:56.045021 nonebot_adapter_tailchat-0.1.0b3/pyproject.toml
--rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 nonebot_adapter_tailchat-0.1.0b3/PKG-INFO
+-rw-r--r--   0        0        0    11335 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/LICENSE
+-rw-r--r--   0        0        0     1488 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/README.md
+-rw-r--r--   0        0        0      260 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/__init__.py
+-rw-r--r--   0        0        0     6874 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/adapter.py
+-rw-r--r--   0        0        0    21563 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/api.py
+-rw-r--r--   0        0        0     8081 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/bbcode.py
+-rw-r--r--   0        0        0     3759 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/bot.py
+-rw-r--r--   0        0        0      675 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/config.py
+-rw-r--r--   0        0        0       26 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/const.py
+-rw-r--r--   0        0        0     6135 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/event.py
+-rw-r--r--   0        0        0      761 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/exception.py
+-rw-r--r--   0        0        0    11184 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/message.py
+-rw-r--r--   0        0        0     4505 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/model.py
+-rw-r--r--   0        0        0      374 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/permission.py
+-rw-r--r--   0        0        0      203 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/rule.py
+-rw-r--r--   0        0        0     2103 2024-05-07 14:52:26.127946 nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/util.py
+-rw-r--r--   0        0        0     1232 2024-05-07 14:52:26.131946 nonebot_adapter_tailchat-0.1.0b4/pyproject.toml
+-rw-r--r--   0        0        0     2272 1970-01-01 00:00:00.000000 nonebot_adapter_tailchat-0.1.0b4/PKG-INFO
```

### Comparing `nonebot_adapter_tailchat-0.1.0b3/LICENSE` & `nonebot_adapter_tailchat-0.1.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b3/README.md` & `nonebot_adapter_tailchat-0.1.0b4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -49,8 +49,16 @@
 
 TAILCHAT_RECONNECT_INTERVAL=5
 TAILCHAT_TIME_OUT=5
 ```
 
 ## 详细配置项
 
-[config.py](./nonebot_adapter_tailchat/config.py)
+[config.py](./nonebot_adapter_tailchat/config.py)
+
+## 相关项目
+- [dcwatson/bbcode](https://github.com/dcwatson/bbcode)
+- [Tailchat](https://github.com/msgbyte/tailchat)
+- [python-socketio](https://github.com/miguelgrinberg/python-socketio)
+- [nonebot2](https://github.com/nonebot/nonebot2)
+- [pydantic2](https://docs.pydantic.dev/latest/)
+- ...
```

#### html2text {}

```diff
@@ -8,8 +8,12 @@
 - ~httpx - ~aiohttp ## Tailchatæºå¨äººå¼å¯æ¹å¼ 1. å®è£
 `å¼æ¾å¹³å°æä»¶` 2. è¿å¥ `è®¾ç½®` -> `å¼æ¾å¹³å°` -> `åå»ºåºç¨` -
 > `å¡«ååºæ¬ä¿¡æ¯` 3. è¿å¥ `åºç¨` -> `æºå¨äºº` -
 > `å¼å¯æºå¨äººè½å` 4. å¨ `åºæ¬ä¿¡æ¯` åè·å `appId` å
 `appSecret` > ææªæ¯æ `æ¶æ¯åè°å°å` ## éç½®æ¹å¼ `.env` æä»¶
 ```dotenv TAILCHAT_BOTS=' [ { "url": "https://xxxxxxx/", "appId": "ts_******",
 "appSecret": "****" } ] ' TAILCHAT_RECONNECT_INTERVAL=5 TAILCHAT_TIME_OUT=5 ```
-## è¯¦ç»éç½®é¡¹ [config.py](./nonebot_adapter_tailchat/config.py)
+## è¯¦ç»éç½®é¡¹ [config.py](./nonebot_adapter_tailchat/config.py) ##
+ç¸å³é¡¹ç® - [dcwatson/bbcode](https://github.com/dcwatson/bbcode) -
+[Tailchat](https://github.com/msgbyte/tailchat) - [python-socketio](https://
+github.com/miguelgrinberg/python-socketio) - [nonebot2](https://github.com/
+nonebot/nonebot2) - [pydantic2](https://docs.pydantic.dev/latest/) - ...
```

### Comparing `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/adapter.py` & `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from .bot import Bot
 from .config import BotInfo, Config
 from .const import ADAPTER_NAME
 from .event import EVENT_CLASSES, Event
 from .exception import ActionFailed, DisconnectException
 from .message import Message
-from .util import log
+from .util import log, retry
 
 
 class Adapter(BaseAdapter):
     @override
     def __init__(self, driver: Driver, **kwargs: Any):
         super().__init__(driver, **kwargs)
         self.adapter_config: Config = get_plugin_config(Config)
@@ -63,29 +63,35 @@
             self._handle_socketio_api(data)
         return data.get("data")
 
     async def _setup(self):
         if any(i.useHttp for i in self.adapter_config.bots_info) and not self.is_http_client_driver:
             raise RuntimeError("HTTPClientMixin is required when use http")
         for i in self.adapter_config.bots_info:
-            self.tasks.append(create_task(self._handle_bot(i), name=f"handle_bot_{i.appId}"))
+            self.tasks.append(
+                create_task(
+                    # 防止因 socketio/tailchat 奇怪错误导致的异常
+                    retry(self.adapter_config.reconnect_interval, self._handle_bot)(i),
+                    name=f"handle_bot_{i.appId}",
+                )
+            )
 
     async def _shutdown(self):
         for task in self.tasks:
             if not task.done():
                 task.cancel()
 
         await gather(*self.tasks, return_exceptions=True)
 
     async def _handle_bot(self, bot_info: BotInfo):
         first = True
         connected = False
         added = False
 
-        async def _wait():
+        async def _wait():  # 确保断连后打断wait
             nonlocal connected
             while True:
                 if not connected:
                     raise DisconnectException()
                 await sleep(1)
 
         def _check():
@@ -99,32 +105,44 @@
             try:
                 await wait_for(bot.login(bot.base_info.jwt), self.adapter_config.time_out)
                 if first:
                     await wait_for(self._connect_bot(bot, first), self.adapter_config.time_out)
                     first = False
                 await bot.update_info(bot.base_info.jwt)
                 if not added:
-                    self.bot_connect(bot)
+                    self._bot_connect(bot)
                     added = True
                 connected = True
                 await gather(bot.sio.wait(), _wait())
             except DisconnectException:
                 log.warning(f"Bot {escape_tag(str(bot))} socketio connection closed")
             except AsyncTimeoutError:
                 log.warning(f"Bot {escape_tag(str(bot))} connection timeout")
             except Exception as e:
                 log.error(f"Error when _handle_bot: {repr(e)}")
                 print_exc()
             connected = False
             if added:
-                self.bot_disconnect(bot)
+                self._bot_disconnect(bot)
                 added = False
             log.debug(f"Bot {escape_tag(str(bot))} will reconnect in {self.adapter_config.reconnect_interval} seconds")
             await sleep(self.adapter_config.reconnect_interval)
 
+    def _bot_connect(self, bot: Bot):
+        try:
+            self.bot_connect(bot)
+        except Exception as e:
+            log.trace(f"Error when bot_connect: {repr(e)}")
+
+    def _bot_disconnect(self, bot: Bot):
+        try:
+            self.bot_disconnect(bot)
+        except Exception as e:
+            log.trace(f"Error when bot_disconnect: {repr(e)}")
+
     @staticmethod
     async def _connect_bot(bot: Bot, first: bool = True):
         if first:
             log.debug(f"try to connect bot {escape_tag(str(bot))}")
             await bot.connect()
         else:
             log.info(f"try to reconnect bot {escape_tag(str(bot))}")
```

### Comparing `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/api.py` & `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/bot.py` & `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/config.py` & `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/event.py` & `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/exception.py` & `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/message.py` & `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/message.py`

 * *Files 23% similar despite different names*

```diff
@@ -66,33 +66,37 @@
         for _ in self.tags:
             self.main = self.main or self.get(_)
 
     @property
     def text(self) -> str:
         return self.box["text"]
 
+    def set_text(self, text: str):
+        self.box["text"] = text
+
     @property
     def head(self) -> str:
         return (
             "["
             + (
-                (f"{self.tag}={self.main} " if self.main else self.tag)
-                + " ".join(f"{k}={v}" for k, v in self.items() if k in self.keys_ and k not in self.tags)
+                (f"{self.tag}={self.main}" if self.main else self.tag)
+                + " "
+                + " ".join(f"{k}={v}" for k, v in self.items() if v and k in self.keys_ and k not in self.tags)
             ).rstrip(" ")
             + "]"
         )
 
     @property
     def tail(self) -> str:
         return f"[/{self.tag}]"
 
     @classmethod
     def tag_in(cls, msg: Union["MessageSegment", "Message"]) -> bool:
         if isinstance(msg, MessageSegment):
-            return any(type(_) is cls for _ in msg.data["tags"])
+            return any(isinstance(_, cls) for _ in msg.data["tags"])
 
         return any(BBCode.tag_in(_) for _ in msg)
 
     def __str__(self):
         return self.head + self.text + self.tail
 
     def __repr__(self):
@@ -173,14 +177,29 @@
     keys_ = {"url"}
 
     @property
     def url(self) -> str:
         return self["url"]
 
 
+@_register_bbcode
+class Img(BBCode):
+    tags = {"img"}
+    keys_ = {"width", "height"}
+
+    @property
+    def url(self) -> str:
+        return self.text
+
+
+@_register_bbcode
+class Code(BBCode):
+    tags = {"code"}
+
+
 @dataclass
 class MessageSegment(BaseMessageSegment["Message"]):
     data: Box
 
     @classmethod
     @override
     def get_message_class(cls) -> type["Message"]:
@@ -189,35 +208,47 @@
     @override
     def __str__(self) -> str:
         return self.data["text"]
 
     def get_text(self) -> str:
         return self.data["text"]
 
+    def set_text(self, text: str):
+        self.data["text"] = text
+
     @override
     def is_text(self) -> bool:
         return not any(not (_.tags & TEXTS) for _ in self.data["tags"])
 
     @classmethod
-    def card(cls, *, text: str, type_: str, data: str) -> "MessageSegment":
+    def card(cls, *, text: str, type_: str, data: str) -> Self:
         return cls.build(text, [Card], {"type": type_, "data": data})
 
     @classmethod
-    def at(cls, *, uid: str, nickname: Optional[str] = None) -> "MessageSegment":
+    def at(cls, *, uid: str, nickname: Optional[str] = None) -> Self:
         return cls.build(nickname or uid, [At], {"at": uid})
 
     @classmethod
-    def file(cls, *, name: str, url: str) -> "MessageSegment":
+    def file(cls, *, name: str, url: str) -> Self:
         return cls.build(name, [File], {"url": url})
 
     @classmethod
     def url(cls, *, url: str, text: Optional[str] = None) -> Self:
         return cls.build(text or url, [Url], {"url": url})
 
     @classmethod
+    def panel(cls, *, groupId: str, panelId: str, text: str) -> Self:
+        # 同url 例如 [url=/main/group/<groupId>/<panelId>]#大厅[/url]
+        return cls.build(text, [Url], {"url": f"/main/group/{groupId}/{panelId}"})
+
+    @classmethod
+    def code(cls, text: str) -> Self:
+        return cls.build(text, [Code])
+
+    @classmethod
     def text(cls, text: str, *, b: bool = False, i: bool = False, u: bool = False, s: bool = False) -> Self:
         _: list[type[B]] = []
         if b:
             _.append(Bold)
         if i:
             _.append(Italic)
         if u:
@@ -227,32 +258,53 @@
         return cls.build(text, _)
 
     @classmethod
     def emoji(cls, text: str) -> Self:
         return cls.build(text, [Emoji])
 
     @classmethod
+    def img(
+        cls, url: str, *, width: Optional[Union[str, int]] = None, height: Optional[Union[str, int]] = None
+    ) -> Self:
+        return cls.build(url, [Img], {"width": width, "height": height})
+
+    @classmethod
+    def md(cls, text: str) -> Self:
+        return cls.build(text, [Markdown])
+
+    @classmethod
     def build(cls, text: str, tags: list[type[B]], extra: Optional[dict[str, str]] = None) -> Self:
         if extra is None:
             extra = {}
-        _ = cls("text", {"text": text, "extra": extra, "tags": []})
+        _ = cls("rich" if len(tags) > 0 else "text", {"text": text, "extra": extra, "tags": []})
         for tag in tags:
             _.data["tags"].append(tag(box=_.data))
         return _
 
     def tag_relation(self) -> set[int]:
         return {_.relation for _ in self.data["tags"]}
 
-    def extend(self, seg: "MessageSegment", strict: bool = True) -> Self:
+    def merge_text(self, seg: Union[str, Self]) -> Self:
+        self.data["text"] += seg if isinstance(self, str) else seg.get_text()
+        return self
+
+    def extend(self, seg: Self, strict: bool = True) -> Self:
+        """
+        新消息段的 text = self.text or seg.text
+        :param seg: 要合并的消息段
+        :param strict: 严格模式
+        :return: 新消息段
+        """
         if strict and (relations := self.tag_relation()) and any(_.relation not in relations for _ in seg.data["tags"]):
             raise ValueError("Tag relation not match")
         self.data["extra"].update(seg.data["extra"])
         for idx, tag in enumerate(seg.data["tags"]):
             seg.data["tags"][idx] = tag.__class__(box=self.data)
         self.data["tags"].extend(seg.data["tags"])
+        self.set_text(self.get_text() or seg.get_text())
         return self
 
     def remove(self, bbcode: Union[B, type[B]]) -> Self:
         if bbcode is type[B]:
             bbcode: B = self.get_tag(bbcode)
         self.data["tags"].remove(bbcode)
         for _ in bbcode.keys_ | bbcode.tags:
@@ -269,17 +321,20 @@
 
     def get_tag(self, bbcode: type[B]) -> Optional[B]:
         for _ in self.data["tags"]:
             if _ is bbcode:
                 return _
         return None
 
+    def get_tags(self) -> list[B]:
+        return self.data["tags"]
+
     def decode(self) -> str:
         _ = deque([self.data["text"]])
-        for tag in self.data["tags"]:
+        for tag in self.data["tags"][::-1]:
             _.appendleft(tag.head)
             _.append(tag.tail)
         return "".join(_)
 
 
 def _update_parser(func):
     @wraps(func)
@@ -290,41 +345,69 @@
 
     return _
 
 
 class Message(BaseMessage[MessageSegment]):
     parser: Parser = Parser(MessageSegment, BBCODES)
 
+    def __init__(
+        self,
+        message: Union[str, None, Iterable[MessageSegment], MessageSegment] = None,
+    ):
+        super().__init__(message)
+        self.reduce()  # 合并连续的纯文本
+
+    def reduce(self):
+        # MIT https://github.com/nonebot/adapter-onebot/blob/v2.4.3/nonebot/adapters/onebot/v11/message.py#L334-L342
+        """合并消息内连续的纯文本段。"""
+        index = 1
+        while index < len(self):
+            if len(self[index - 1].get_tags()) == 0 and len(self[index].get_tags()) == 0:
+                self[index - 1].merge_text(self[index])
+                del self[index]
+            else:
+                index += 1
+
+    def merge_text(self) -> Self:
+        if len(self) < 2:
+            return self
+        _ = [self[0]]
+        for seg in self[1:]:
+            seg: MessageSegment
+            if len(seg.get_tags()) == 0 and len(_[-1].get_tags()) == 0:
+                _[-1].merge_text(seg)
+                continue
+            _.append(seg)
+        return Message(_)
+
     @classmethod
     def update_parser(cls):
         cls.parser = Parser(MessageSegment, BBCODES)
 
-    @staticmethod
-    def register_bbcode(code: Union[int, type[B]]):
-        return _register_bbcode(code)
+    @classmethod
+    def register_bbcode(cls, code: Union[int, type[B]]):
+        _register_bbcode(code)
+        cls.update_parser()
 
     @staticmethod
     def register_text(bbcode: type[B]) -> type[B]:
         """注册文本类型"""
         return _register_text(bbcode)
 
     def __contains__(  # pyright: ignore[reportIncompatibleMethodOverride]
-        self, value: Union[MessageSegment, str, B, type[B]]
+        self, value: Union[MessageSegment, str, type[B]]
     ) -> bool:
-        """检查消息段是否存在
-
-        参数:
-            value: 消息段或消息段类型
-        返回:
-            消息内是否存在给定消息段或给定类型的消息段
-        """
-        if value is type[B]:
+        if issubclass(value, BBCode):
             return value.tag_in(self)
         return super().__contains__(value)
 
+    @override
+    def has(self, value: Union[MessageSegment, str, type[B]]) -> bool:
+        return value in self
+
     @classmethod
     @override
     def get_segment_class(cls) -> type[MessageSegment]:
         return MessageSegment
 
     @classmethod
     @override
```

### Comparing `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/model.py` & `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b3/nonebot_adapter_tailchat/util.py` & `nonebot_adapter_tailchat-0.1.0b4/nonebot_adapter_tailchat/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+from asyncio import sleep
+from functools import wraps
 from io import StringIO
+from traceback import print_exc
 from typing import Any, Optional, Union
 
 from msgpack import ExtType
 from nonebot.utils import logger_wrapper
 
 from .const import ADAPTER_NAME
 
@@ -50,7 +53,20 @@
     def trace(self, *args, exception: Optional[Exception] = None):
         _ = StringIO()
         print(*args, file=_, end="")
         self.log("TRACE", _.getvalue(), exception)
 
 
 log = Log()
+
+
+def retry(wait_time: int, func):
+    @wraps(func)
+    async def wrapper(*args, **kwargs):
+        try:
+            await func(*args, **kwargs)
+        except Exception as e:
+            log.error(f"Error when exec {func.__name__}: {repr(e)}")
+            print_exc()
+        await sleep(wait_time)
+
+    return wrapper
```

### Comparing `nonebot_adapter_tailchat-0.1.0b3/pyproject.toml` & `nonebot_adapter_tailchat-0.1.0b4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-tailchat"
-version = "0.1.0b3"
+version = "0.1.0b4"
 description = "NoneBot2 Tailchat 适配器 / Tailchat adapter for nonebot2"
 authors = ["eya46 <61458340+eya46@users.noreply.github.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "nonebot_adapter_tailchat" }]
 
 [tool.poetry.dependencies]
@@ -16,14 +16,19 @@
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.4.2"
 nonebot2 = { extras = ["httpx"], version = "^2.3.0" }
 pyyaml = "^6.0.1"
 
+
+[tool.poetry.group.test.dependencies]
+nonebug = "^0.3.7"
+pytest-asyncio = "^0.23.6"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 120
 target-version = "py39"
```

### Comparing `nonebot_adapter_tailchat-0.1.0b3/PKG-INFO` & `nonebot_adapter_tailchat-0.1.0b4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-tailchat
-Version: 0.1.0b3
+Version: 0.1.0b4
 Summary: NoneBot2 Tailchat 适配器 / Tailchat adapter for nonebot2
 License: Apache-2.0
 Author: eya46
 Author-email: 61458340+eya46@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -70,7 +70,15 @@
 TAILCHAT_RECONNECT_INTERVAL=5
 TAILCHAT_TIME_OUT=5
 ```
 
 ## 详细配置项
 
 [config.py](./nonebot_adapter_tailchat/config.py)
+
+## 相关项目
+- [dcwatson/bbcode](https://github.com/dcwatson/bbcode)
+- [Tailchat](https://github.com/msgbyte/tailchat)
+- [python-socketio](https://github.com/miguelgrinberg/python-socketio)
+- [nonebot2](https://github.com/nonebot/nonebot2)
+- [pydantic2](https://docs.pydantic.dev/latest/)
+- ...
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-tailchat Version: 0.1.0b3 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-tailchat Version: 0.1.0b4 Summary:
 NoneBot2 Tailchat ééå¨ / Tailchat adapter for nonebot2 License: Apache-2.0
 Author: eya46 Author-email: 61458340+eya46@users.noreply.github.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: msgpack (>=1.0.8,<2.0.0) Requires-
@@ -19,8 +19,12 @@
 - ~httpx - ~aiohttp ## Tailchatæºå¨äººå¼å¯æ¹å¼ 1. å®è£
 `å¼æ¾å¹³å°æä»¶` 2. è¿å¥ `è®¾ç½®` -> `å¼æ¾å¹³å°` -> `åå»ºåºç¨` -
 > `å¡«ååºæ¬ä¿¡æ¯` 3. è¿å¥ `åºç¨` -> `æºå¨äºº` -
 > `å¼å¯æºå¨äººè½å` 4. å¨ `åºæ¬ä¿¡æ¯` åè·å `appId` å
 `appSecret` > ææªæ¯æ `æ¶æ¯åè°å°å` ## éç½®æ¹å¼ `.env` æä»¶
 ```dotenv TAILCHAT_BOTS=' [ { "url": "https://xxxxxxx/", "appId": "ts_******",
 "appSecret": "****" } ] ' TAILCHAT_RECONNECT_INTERVAL=5 TAILCHAT_TIME_OUT=5 ```
-## è¯¦ç»éç½®é¡¹ [config.py](./nonebot_adapter_tailchat/config.py)
+## è¯¦ç»éç½®é¡¹ [config.py](./nonebot_adapter_tailchat/config.py) ##
+ç¸å³é¡¹ç® - [dcwatson/bbcode](https://github.com/dcwatson/bbcode) -
+[Tailchat](https://github.com/msgbyte/tailchat) - [python-socketio](https://
+github.com/miguelgrinberg/python-socketio) - [nonebot2](https://github.com/
+nonebot/nonebot2) - [pydantic2](https://docs.pydantic.dev/latest/) - ...
```

