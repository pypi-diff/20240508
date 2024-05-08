# Comparing `tmp/synapse_auto_accept_invite-1.1.3.tar.gz` & `tmp/synapse_auto_accept_invite-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synapse_auto_accept_invite-1.1.3.tar", last modified: Tue May 23 19:40:36 2023, max compression
+gzip compressed data, was "synapse_auto_accept_invite-1.2.0.tar", last modified: Mon May  6 21:11:32 2024, max compression
```

## Comparing `synapse_auto_accept_invite-1.1.3.tar` & `synapse_auto_accept_invite-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxr-x   0 shay      (1000) shay      (1000)        0 2023-05-23 19:40:35.995905 synapse_auto_accept_invite-1.1.3/
--rw-rw-r--   0 shay      (1000) shay      (1000)    10174 2023-05-04 18:07:33.000000 synapse_auto_accept_invite-1.1.3/LICENSE
--rw-rw-r--   0 shay      (1000) shay      (1000)     3158 2023-05-23 19:40:35.995905 synapse_auto_accept_invite-1.1.3/PKG-INFO
--rw-rw-r--   0 shay      (1000) shay      (1000)     2749 2023-05-23 19:03:03.000000 synapse_auto_accept_invite-1.1.3/README.md
--rw-rw-r--   0 shay      (1000) shay      (1000)      192 2023-05-04 18:07:33.000000 synapse_auto_accept_invite-1.1.3/pyproject.toml
--rw-rw-r--   0 shay      (1000) shay      (1000)      664 2023-05-23 19:40:35.995905 synapse_auto_accept_invite-1.1.3/setup.cfg
--rw-rw-r--   0 shay      (1000) shay      (1000)       36 2023-05-12 19:46:18.000000 synapse_auto_accept_invite-1.1.3/setup.py
-drwxrwxr-x   0 shay      (1000) shay      (1000)        0 2023-05-23 19:40:35.995905 synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite/
--rw-rw-r--   0 shay      (1000) shay      (1000)     7216 2023-05-16 20:22:10.000000 synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite/__init__.py
-drwxrwxr-x   0 shay      (1000) shay      (1000)        0 2023-05-23 19:40:35.995905 synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite.egg-info/
--rw-rw-r--   0 shay      (1000) shay      (1000)     3158 2023-05-23 19:40:35.000000 synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite.egg-info/PKG-INFO
--rw-rw-r--   0 shay      (1000) shay      (1000)      367 2023-05-23 19:40:35.000000 synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite.egg-info/SOURCES.txt
--rw-rw-r--   0 shay      (1000) shay      (1000)        1 2023-05-23 19:40:35.000000 synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite.egg-info/dependency_links.txt
--rw-rw-r--   0 shay      (1000) shay      (1000)      141 2023-05-23 19:40:35.000000 synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite.egg-info/requires.txt
--rw-rw-r--   0 shay      (1000) shay      (1000)       27 2023-05-23 19:40:35.000000 synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite.egg-info/top_level.txt
-drwxrwxr-x   0 shay      (1000) shay      (1000)        0 2023-05-23 19:40:35.995905 synapse_auto_accept_invite-1.1.3/tests/
--rw-rw-r--   0 shay      (1000) shay      (1000)    14715 2023-05-16 20:22:10.000000 synapse_auto_accept_invite-1.1.3/tests/test_accept_invite.py
+drwxrwxr-x   0 cmdr      (1000) cmdr      (1000)        0 2024-05-06 21:11:32.195046 synapse_auto_accept_invite-1.2.0/
+-rw-rw-r--   0 cmdr      (1000) cmdr      (1000)    10174 2024-04-29 20:34:16.000000 synapse_auto_accept_invite-1.2.0/LICENSE
+-rw-r--r--   0 cmdr      (1000) cmdr      (1000)     3770 2024-05-06 21:11:32.195046 synapse_auto_accept_invite-1.2.0/PKG-INFO
+-rw-rw-r--   0 cmdr      (1000) cmdr      (1000)     2886 2024-05-06 20:51:13.000000 synapse_auto_accept_invite-1.2.0/README.md
+-rw-rw-r--   0 cmdr      (1000) cmdr      (1000)      192 2024-04-29 20:34:16.000000 synapse_auto_accept_invite-1.2.0/pyproject.toml
+-rw-rw-r--   0 cmdr      (1000) cmdr      (1000)      664 2024-05-06 21:11:32.195046 synapse_auto_accept_invite-1.2.0/setup.cfg
+drwxrwxr-x   0 cmdr      (1000) cmdr      (1000)        0 2024-05-06 21:11:32.191046 synapse_auto_accept_invite-1.2.0/synapse_auto_accept_invite/
+-rw-rw-r--   0 cmdr      (1000) cmdr      (1000)     7888 2024-05-06 20:51:13.000000 synapse_auto_accept_invite-1.2.0/synapse_auto_accept_invite/__init__.py
+drwxrwxr-x   0 cmdr      (1000) cmdr      (1000)        0 2024-05-06 21:11:32.191046 synapse_auto_accept_invite-1.2.0/synapse_auto_accept_invite.egg-info/
+-rw-r--r--   0 cmdr      (1000) cmdr      (1000)     3770 2024-05-06 21:11:32.000000 synapse_auto_accept_invite-1.2.0/synapse_auto_accept_invite.egg-info/PKG-INFO
+-rw-rw-r--   0 cmdr      (1000) cmdr      (1000)      358 2024-05-06 21:11:32.000000 synapse_auto_accept_invite-1.2.0/synapse_auto_accept_invite.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmdr      (1000) cmdr      (1000)        1 2024-05-06 21:11:32.000000 synapse_auto_accept_invite-1.2.0/synapse_auto_accept_invite.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmdr      (1000) cmdr      (1000)      141 2024-05-06 21:11:32.000000 synapse_auto_accept_invite-1.2.0/synapse_auto_accept_invite.egg-info/requires.txt
+-rw-rw-r--   0 cmdr      (1000) cmdr      (1000)       27 2024-05-06 21:11:32.000000 synapse_auto_accept_invite-1.2.0/synapse_auto_accept_invite.egg-info/top_level.txt
+drwxrwxr-x   0 cmdr      (1000) cmdr      (1000)        0 2024-05-06 21:11:32.191046 synapse_auto_accept_invite-1.2.0/tests/
+-rw-rw-r--   0 cmdr      (1000) cmdr      (1000)    18628 2024-05-06 20:51:13.000000 synapse_auto_accept_invite-1.2.0/tests/test_accept_invite.py
```

### Comparing `synapse_auto_accept_invite-1.1.3/LICENSE` & `synapse_auto_accept_invite-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synapse_auto_accept_invite-1.1.3/PKG-INFO` & `synapse_auto_accept_invite-1.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: synapse_auto_accept_invite
-Version: 1.1.3
-Summary: "Synapse module to automatically accept invites"
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # Auto-accept invites
 
 Synapse module to automatically accept invites.
 
 Compatible with Synapse v1.84.0 and later.
 
 ## Installation
@@ -27,18 +15,23 @@
 
 Then alter your homeserver configuration, adding to your `modules` configuration:
 ```yaml
 modules:
   - module: synapse_auto_accept_invite.InviteAutoAccepter
     config:
       # Optional: if set to true, then only invites for direct messages (1:1 rooms)
-      # will be auto accepted. Otherwise, all room invites are accepted.
+      # will be auto accepted.
       # Defaults to false.
       accept_invites_only_for_direct_messages: false
 
+      # Optional: if set to true, then only invites from local users will be auto 
+      # accepted.
+      # Defaults to false.
+      accept_invites_only_from_local_users: false
+
       # (For workerised Synapse deployments)
       #
       # This module should only be active on a single worker process at once,
       # otherwise invites may be accepted by multiple workers simultaneously.
       #
       # By default, this module is only enabled on the main process, and is disabled
       # on workers. To choose a worker to run this module on (to reduce load on the
```

### Comparing `synapse_auto_accept_invite-1.1.3/setup.cfg` & `synapse_auto_accept_invite-1.2.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = synapse_auto_accept_invite
 description = "Synapse module to automatically accept invites"
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 1.1.3
+version = 1.2.0
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 python_requires = >= 3.7
@@ -16,18 +16,18 @@
 dev = 
 	matrix-synapse >= 1.84.0
 	tox
 	twisted
 	aiounittest
 	attrs
 	frozendict
-	mypy == 0.931
+	mypy == 1.4.1
 	types-frozendict
 	black == 22.3.0
-	flake8 == 4.0.1
+	flake8 == 5.0.4
 	isort == 5.9.3
 
 [flake8]
 ignore = W503,W504,E203,E501
 
 [egg_info]
 tag_build =
```

### Comparing `synapse_auto_accept_invite-1.1.3/synapse_auto_accept_invite/__init__.py` & `synapse_auto_accept_invite-1.2.0/synapse_auto_accept_invite/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 logger = logging.getLogger(__name__)
 ACCOUNT_DATA_DIRECT_MESSAGE_LIST = "m.direct"
 
 
 @attr.s(auto_attribs=True, frozen=True)
 class InviteAutoAccepterConfig:
     accept_invites_only_for_direct_messages: bool = False
+    accept_invites_only_from_local_users: bool = False
     worker_to_run_on: Optional[str] = None
 
 
 class InviteAutoAccepter:
     def __init__(self, config: InviteAutoAccepterConfig, api: ModuleApi):
         # Keep a reference to the Module API.
         self._api = api
@@ -62,61 +63,78 @@
 
         Returns:
             A InviteAutoAccepterConfig generated from this configuration
         """
         accept_invites_only_for_direct_messages = config.get(
             "accept_invites_only_for_direct_messages", False
         )
+        accept_invites_only_from_local_users = config.get(
+            "accept_invites_only_from_local_users", False
+        )
 
         worker_to_run_on = config.get("worker_to_run_on", None)
 
         return InviteAutoAccepterConfig(
             accept_invites_only_for_direct_messages=accept_invites_only_for_direct_messages,
+            accept_invites_only_from_local_users=accept_invites_only_from_local_users,
             worker_to_run_on=worker_to_run_on,
         )
 
     async def on_new_event(self, event: EventBase, *args: Any) -> None:
         """Listens for new events, and if the event is an invite for a local user then
         automatically accepts it.
 
         Args:
             event: The incoming event.
         """
         # Check if the event is an invite for a local user.
-        if (
+        is_invite_for_local_user = (
             event.type == "m.room.member"
             and event.is_state()
             and event.membership == "invite"
             and self._api.is_mine(event.state_key)
+        )
+
+        # Only accept invites for direct messages if the configuration mandates it.
+        is_direct_message = event.content.get("is_direct", False)
+        is_allowed_by_direct_message_rules = (
+            not self._config.accept_invites_only_for_direct_messages
+            or is_direct_message is True
+        )
+
+        # Only accept invites from remote users if the configuration mandates it.
+        is_from_local_user = self._api.is_mine(event.sender)
+        is_allowed_by_local_user_rules = (
+            not self._config.accept_invites_only_from_local_users
+            or is_from_local_user is True
+        )
+
+        if (
+            is_invite_for_local_user
+            and is_allowed_by_direct_message_rules
+            and is_allowed_by_local_user_rules
         ):
-            is_direct_message = event.content.get("is_direct", False)
+            # Make the user join the room. We run this as a background process to circumvent a race condition
+            # that occurs when responding to invites over federation (see https://github.com/matrix-org/synapse-auto-accept-invite/issues/12)
+            run_as_background_process(
+                "retry_make_join",
+                self._retry_make_join,
+                event.state_key,
+                event.state_key,
+                event.room_id,
+                "join",
+                bg_start_span=False,
+            )
 
-            # Only accept invites for direct messages if the configuration mandates it, otherwise accept all invites.
-            if (
-                not self._config.accept_invites_only_for_direct_messages
-                or is_direct_message is True
-            ):
-                # Make the user join the room. We run this as a background process to circumvent a race condition
-                # that occurs when responding to invites over federation (see https://github.com/matrix-org/synapse-auto-accept-invite/issues/12)
-                run_as_background_process(
-                    "retry_make_join",
-                    self._retry_make_join,
-                    event.state_key,
-                    event.state_key,
-                    event.room_id,
-                    "join",
-                    bg_start_span=False,
+            if is_direct_message:
+                # Mark this room as a direct message!
+                await self._mark_room_as_direct_message(
+                    event.state_key, event.sender, event.room_id
                 )
 
-                if is_direct_message:
-                    # Mark this room as a direct message!
-                    await self._mark_room_as_direct_message(
-                        event.state_key, event.sender, event.room_id
-                    )
-
     async def _mark_room_as_direct_message(
         self, user_id: str, dm_user_id: str, room_id: str
     ) -> None:
         """
         Marks a room (`room_id`) as a direct message with the counterparty `dm_user_id`
         from the perspective of the user `user_id`.
         """
```

### Comparing `synapse_auto_accept_invite-1.1.3/tests/test_accept_invite.py` & `synapse_auto_accept_invite-1.2.0/tests/test_accept_invite.py`

 * *Files 12% similar despite different names*

```diff
@@ -191,29 +191,59 @@
             "m.direct",
             {
                 "@someone:random": ("!somewhere:random",),
                 self.user_id: ("!the:room",),
             },
         )
 
-    async def test_remote_user(self) -> None:
+    async def test_invite_remote_user(self) -> None:
         """Tests that receiving an invite for a remote user does nothing."""
         invite = MockEvent(
             sender=self.user_id,
             state_key=self.remote_invitee,
             type="m.room.member",
             content={"membership": "invite"},
         )
 
         # Stop mypy from complaining that we give on_new_event a MockEvent rather than an
         # EventBase.
         await self.module.on_new_event(event=invite)  # type: ignore[arg-type]
 
         self.mocked_update_membership.assert_not_called()
 
+    async def test_invite_from_remote_user(self) -> None:
+        """Tests that receiving an invite for a local user, from a remote user, makes the
+        module attempt to make the invitee join the room."""
+        invite = MockEvent(
+            sender=self.remote_invitee,
+            state_key=self.invitee,
+            type="m.room.member",
+            content={"membership": "invite"},
+        )
+        join_event = MockEvent(
+            sender="someone",
+            state_key="someone",
+            type="m.room.member",
+            content={"membership": "join"},
+        )
+        self.mocked_update_membership.return_value = make_awaitable(join_event)
+
+        # Stop mypy from complaining that we give on_new_event a MockEvent rather than an
+        # EventBase.
+        await self.module.on_new_event(event=invite)  # type: ignore[arg-type]
+
+        await self.retry_assertions(
+            self.mocked_update_membership,
+            1,
+            sender=invite.state_key,
+            target=invite.state_key,
+            room_id=invite.room_id,
+            new_membership="join",
+        )
+
     async def test_not_state(self) -> None:
         """Tests that receiving an invite that's not a state event does nothing."""
         invite = MockEvent(
             sender=self.user_id, type="m.room.member", content={"membership": "invite"}
         )
 
         # Stop mypy from complaining that we give on_new_event a MockEvent rather than an
@@ -316,22 +346,91 @@
         # Stop mypy from complaining that we give on_new_event a MockEvent rather than an
         # EventBase.
         await module.on_new_event(event=invite)  # type: ignore[arg-type]
 
         mocked_update_membership: Mock = module._api.update_room_membership  # type: ignore[assignment]
         mocked_update_membership.assert_not_called()
 
+    async def test_accept_invite_local_user_if_only_enabled_from_local_users(
+        self,
+    ) -> None:
+        """Tests that, if the module is configured to only accept invites from local users, invites
+        from local users are still automatically accepted.
+        """
+        module = create_module(
+            config_override={"accept_invites_only_from_local_users": True},
+        )
+
+        # Patch out the account data get and put methods with dummy awaitables.
+        account_data_put: Mock = cast(Mock, module._api.account_data_manager.put_global)
+        account_data_put.return_value = make_awaitable(None)
+
+        account_data_get: Mock = cast(Mock, module._api.account_data_manager.get_global)
+        account_data_get.return_value = make_awaitable({})
+
+        mocked_update_membership: Mock = module._api.update_room_membership  # type: ignore[assignment]
+        join_event = MockEvent(
+            sender="someone",
+            state_key="someone",
+            type="m.room.member",
+            content={"membership": "join"},
+        )
+        mocked_update_membership.return_value = make_awaitable(join_event)
+
+        invite = MockEvent(
+            sender=self.user_id,
+            state_key=self.invitee,
+            type="m.room.member",
+            content={"membership": "invite", "is_direct": True},
+        )
+
+        # Stop mypy from complaining that we give on_new_event a MockEvent rather than an
+        # EventBase.
+        await module.on_new_event(event=invite)  # type: ignore[arg-type]
+
+        await self.retry_assertions(
+            mocked_update_membership,
+            1,
+            sender=invite.state_key,
+            target=invite.state_key,
+            room_id=invite.room_id,
+            new_membership="join",
+        )
+
+    async def test_ignore_invite_if_only_enabled_from_local_users(self) -> None:
+        """Tests that, if the module is configured to only accept invites from local users,
+        invites from non-local users are ignored."""
+        module = create_module(
+            config_override={"accept_invites_only_from_local_users": True},
+        )
+
+        invite = MockEvent(
+            sender=self.remote_invitee,
+            state_key=self.invitee,
+            type="m.room.member",
+            content={"membership": "invite"},
+        )
+
+        # Stop mypy from complaining that we give on_new_event a MockEvent rather than an
+        # EventBase.
+        await module.on_new_event(event=invite)  # type: ignore[arg-type]
+
+        mocked_update_membership: Mock = module._api.update_room_membership  # type: ignore[assignment]
+        mocked_update_membership.assert_not_called()
+
     def test_config_parse(self) -> None:
         """Tests that a correct configuration passes parse_config."""
         config = {
             "accept_invites_only_for_direct_messages": True,
+            "accept_invites_only_from_local_users": True,
         }
         parsed_config = InviteAutoAccepter.parse_config(config)
 
         self.assertTrue(parsed_config.accept_invites_only_for_direct_messages)
+        self.assertTrue(parsed_config.accept_invites_only_from_local_users)
 
     def test_runs_on_only_one_worker(self) -> None:
         """
         Tests that the module only runs on the specified worker.
         """
         # By default, we run on the main process...
         main_module = create_module(worker_name=None)
```

