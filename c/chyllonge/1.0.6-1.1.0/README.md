# Comparing `tmp/chyllonge-1.0.6.tar.gz` & `tmp/chyllonge-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chyllonge-1.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "chyllonge-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `chyllonge-1.0.6.tar` & `chyllonge-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1683 2024-05-08 00:32:31.306919 chyllonge-1.0.6/LICENSE.txt
--rw-r--r--   0        0        0     3833 2024-05-08 00:32:31.306919 chyllonge-1.0.6/README.md
--rw-r--r--   0        0        0     1140 2024-05-08 00:32:31.646918 chyllonge-1.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-08 00:32:31.306919 chyllonge-1.0.6/src/chyllonge/__init__.py
--rw-r--r--   0        0        0    40100 2024-05-08 00:32:31.306919 chyllonge-1.0.6/src/chyllonge/api.py
--rw-r--r--   0        0        0     4699 1970-01-01 00:00:00.000000 chyllonge-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1683 2024-05-08 16:30:33.522190 chyllonge-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     3580 2024-05-08 16:30:33.522190 chyllonge-1.1.0/README.md
+-rw-r--r--   0        0        0     1140 2024-05-08 16:30:33.778192 chyllonge-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-08 16:30:33.522190 chyllonge-1.1.0/src/chyllonge/__init__.py
+-rw-r--r--   0        0        0    42398 2024-05-08 16:30:33.522190 chyllonge-1.1.0/src/chyllonge/api.py
+-rw-r--r--   0        0        0     4446 1970-01-01 00:00:00.000000 chyllonge-1.1.0/PKG-INFO
```

### Comparing `chyllonge-1.0.6/LICENSE.txt` & `chyllonge-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chyllonge-1.0.6/README.md` & `chyllonge-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -18,48 +18,43 @@
 To install `chyllonge`, execute `pip install chyllonge`.
 
 ## Usage
 
 Detailed API documentation is available at https://api.challonge.com/v1.
 
 ```python
-from chyllonge.api import TournamentAPI, ParticipantAPI, MatchAPI, AttachmentAPI
+from chyllonge.api import ChallongeAPI
 from datetime import datetime, timedelta
 
-# instantiate base api classes
-tournaments_api = TournamentAPI()
-participants_api = ParticipantAPI()
-match_api = MatchAPI()
-attachment_api = AttachmentAPI()
+api = ChallongeAPI()
 
 # create a basic tournament
-tournament = tournaments_api.create(name="My Chyllonge Tournament")
-print(tournament["tournament"]["id"])
+tournament = api.tournaments.create(name="My Chyllonge Tournament")
+print(tournament["id"])
 
 # create a tournament that starts in an hour
-an_hour_from_now = (datetime.now() + timedelta(hours=1)).isoformat() + tournaments_api.tz_utc_offset_string
-tournament = tournaments_api.create(name="My Chyllonge Tournament", start_at=an_hour_from_now, check_in_duration=60)
-print(tournament["tournament"]["id"])
+an_hour_from_now = (datetime.now() + timedelta(hours=1)).isoformat() + api.http.tz_utc_offset_string
+tournament = api.tournaments.create(name="My Chyllonge Tournament", start_at=an_hour_from_now, check_in_duration=60)
+print(tournament["id"])
 
 # create a tournament, add Alice and Bob, process their check-ins, start the tournment, set their match underway,
 # score their match (congratulations Alice!), finalize the tournament
-an_hour_from_now = (datetime.now() + timedelta(hours=1)).isoformat() + tournaments_api.tz_utc_offset_string
-tournament = tournaments_api.create(name="Alice and Bob Play Bingo", start_at=an_hour_from_now, check_in_duration=60)
-tournament_id = tournament["tournament"]["id"]
-
-participants_api.add(tournament_id, name="Alice")
-participants_api.add(tournament_id, name="Bob")
-tournaments_api.process_checkins(tournament_id)
-tournaments_api.start(tournament_id)
-match_id = match_api.get_all(tournament_id=tournament_id)[0]["match"]["id"]
-alice_id = participants_api.get_all(tournament_id)[0]["participant"]["id"]
-match_api.set_underway(tournament_id, match_id)
-match_api.update(tournament_id, match_id, match_scores_csv="3-1,2-2", match_winner_id=alice_id)
-tournaments_api.finalize(tournament_id)
-finished_tournment = tournaments_api.get(tournament_id)
+an_hour_from_now = (datetime.now() + timedelta(hours=1)).isoformat() + api.http.tz_utc_offset_string
+tournament = api.tournaments.create(name="Alice and Bob Play Bingo", start_at=an_hour_from_now, check_in_duration=60)
+tournament_id = tournament["id"]
+api.participants.add(tournament_id, name="Alice")
+api.participants.add(tournament_id, name="Bob")
+api.tournaments.process_checkins(tournament_id)
+api.tournaments.start(tournament_id)
+match_id = api.matches.get_all(tournament_id=tournament_id)[0]["id"]
+alice_id = api.participants.get_all(tournament_id)[0]["id"]
+api.matches.set_underway(tournament_id, match_id)
+api.matches.update(tournament_id, match_id, match_scores_csv="3-1,2-2", match_winner_id=alice_id)
+api.tournaments.finalize(tournament_id)
+finished_tournment = api.tournaments.get(tournament_id)
 ```
 
 ## History
 
 `chyllonge` was inspired by `pychallonge` - developed by Russ Amos - which (in turn) includes `pychal`. 
 
 See `CONTRIBUTORS.txt` for the original authors.
```

### Comparing `chyllonge-1.0.6/pyproject.toml` & `chyllonge-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "chyllonge"
-version = "1.0.6"
+version = "1.1.0"
 dependencies = ["tzlocal>=5.2", "requests>=2.31.0"]
 requires-python = ">=3.8"
 authors = [{name = "Alex Fredrickson", email = "alex.q.fredrickson@gmail.com"}]
 maintainers = [{name = "Alex Fredrickson", email = "alex.q.fredrickson@gmail.com"}]
 description = "A Python 3.8+ implementation of the challonge.com API."
 readme = "README.md"
 license = {file = "LICENSE.txt"}
```

### Comparing `chyllonge-1.0.6/src/chyllonge/api.py` & `chyllonge-1.1.0/src/chyllonge/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,41 @@
     # raise ChallongeAPIException('foo bar baz buzz')
     pass
 
 
 class ChallongeApi:
 
     def __init__(self):
+        self.http = ChallongeApiHttpMethods()
+
+        self.tournaments = TournamentAPI(self.http)
+        self.matches = MatchAPI(self.http)
+        self.participants = ParticipantAPI(self.http)
+        self.attachments = AttachmentAPI(self.http)
+
+    def get_heartbeat(self):
+        """
+        Invokes the most basic kind of API request.
+        """
+
+        response = requests.get(
+            self.http.base_challonge_url,
+            headers=self.http.user_agent_param,
+            auth=self.http.basic_auth_param
+        )
+
+        if response.status_code != 200:
+            raise ChallongeAPIException(f"ERROR: {', '.join([e for e in json.loads(response.text)['errors']])}")
+
+        return response.text
+
+
+class ChallongeApiHttpMethods:
+
+    def __init__(self):
         self.user = os.environ["CHALLONGE_USER"]
         self.key = os.environ["CHALLONGE_KEY"]
 
         if not self.user:
             raise ChallongeAPIException(
                 'ERROR: No API username was defined in the CHALLONGE_USER system environment variable.'
             )
@@ -53,40 +80,28 @@
         self.tz_utc_offset_string = self.tz_utc_offset[0:-2] + ":" + self.tz_utc_offset[-2:]
 
         # note that the user agent string is required to get around Cloudflare issues
         self.user_agent_param = {"User-Agent": "chyllonge"}
 
         self.base_challonge_url = "https://api.challonge.com/v1/"
 
-    def get_heartbeat(self):
-        """
-        Invokes the most basic kind of API request.
-        """
-
-        response = requests.get(self.base_challonge_url, headers=self.user_agent_param, auth=self.basic_auth_param)
-
-        if response.status_code != 200:
-            raise ChallongeAPIException(f"ERROR: {', '.join([e for e in json.loads(response.text)['errors']])}")
-
-        return response.text
-
-    def http_get(self, api_suffix='', params=None):
+    def get(self, api_suffix='', params=None):
         response = requests.get(
             self.base_challonge_url + api_suffix,
             headers=self.user_agent_param,
             auth=self.basic_auth_param,
             params=params
         )
 
         if response.status_code != 200:
             raise ChallongeAPIException(f"ERROR: {', '.join([e for e in json.loads(response.text)['errors']])}")
 
         return json.loads(response.text)
 
-    def http_post(self, api_suffix, params=None):
+    def post(self, api_suffix, params=None):
         response = requests.post(
             self.base_challonge_url + api_suffix,
             headers=self.user_agent_param,
             auth=self.basic_auth_param,
             data=params
         )
 
@@ -108,42 +123,46 @@
                 raise ChallongeAPIException(
                     f"ERROR: {self.base_challonge_url + api_suffix} | "
                     f"{ast.literal_eval(response.content.decode('utf-8'))}"
                 )
 
         return json.loads(response.text)
 
-    def http_put(self, api_suffix, params=None):
+    def put(self, api_suffix, params=None):
         response = requests.put(
             self.base_challonge_url + api_suffix,
             headers=self.user_agent_param,
             auth=self.basic_auth_param,
             data=params
         )
 
         if response.status_code != 200:
             raise ChallongeAPIException(f"ERROR: {', '.join([e for e in json.loads(response.text)['errors']])}")
 
         return json.loads(response.text)
 
-    def http_delete(self, api_suffix, params=None):
+    def delete(self, api_suffix, params=None):
         response = requests.delete(
             self.base_challonge_url + api_suffix,
             headers=self.user_agent_param,
             auth=self.basic_auth_param,
             params=params
         )
 
         if response.status_code != 200:
             raise ChallongeAPIException(f"ERROR: {', '.join([e for e in json.loads(response.text)['errors']])}")
 
         return json.loads(response.text)
 
 
-class TournamentAPI(ChallongeApi):
+class TournamentAPI:
+
+    def __init__(self, http_methods):
+        self.http = http_methods
+        self.participant_api = ParticipantAPI(self.http)  # special case for a built-in sanity check
 
     def get_all(self, state: str = None, tournament_type: str = None, created_after: str = None,
                 created_before: str = None, subdomain=None):
         """
         Retrieve a set of tournaments created with your account.
 
         :param state: all, pending, in_progress, ended
@@ -160,16 +179,19 @@
         params = {
             "state": state,
             "tournament_type": tournament_type,
             "created_after": created_after,
             "created_before": created_before
         }
 
-        response = self.http_get("tournaments.json", params=params)
-        return response
+        response = self.http.get("tournaments.json", params=params)
+
+        tournaments = [t["tournament"] for t in response]
+
+        return tournaments
 
     def create(self, name: str = None, tournament_type: str = None, url: str = None, subdomain: str = None,
                description: str = None, open_signup: bool = None, hold_third_place_match: bool = None,
                pts_for_match_win: float = None, pts_for_match_tie: float = None,
                pts_for_game_win: float = None, pts_for_game_tie: float = None, pts_for_bye: float = None,
                swiss_rounds: int = None, ranked_by: str = None, rr_pts_for_match_win: float = None,
                rr_pts_for_match_tie: float = None, rr_pts_for_game_win: float = None,
@@ -263,16 +285,19 @@
             "tournament[signup_cap]": signup_cap,
             "tournament[start_at]": start_at,
             "tournament[check_in_duration]": check_in_duration,
             "tournament[grand_finals_modifier]": grand_finals_modifier,
             "tournament[prediction_method]": prediction_method,
         }
 
-        response = self.http_post("tournaments.json", params)
-        return response
+        response = self.http.post("tournaments.json", params)
+
+        tournament = response["tournament"]
+
+        return tournament
 
     def get(self, tournament_id: str, include_participants: int = None, include_matches: int = None):
         """
         Retrieve a single tournament record created with your account.
 
         :param tournament_id: Tournament ID (e.g. 10230) or URL (e.g. 'single_elim' for challonge.com/single_elim).
         If assigned to a subdomain, URL format must be :subdomain-:tournament_url (e.g. 'test-mytourney'
@@ -285,16 +310,19 @@
             raise ChallongeAPIException("ERROR: A tournament ID is required.")
 
         params = {
             "include_participants": include_participants,
             "include_matches": include_matches
         }
 
-        response = self.http_get(f"tournaments/{tournament_id}.json", params=params)
-        return response
+        response = self.http.get(f"tournaments/{tournament_id}.json", params=params)
+
+        tournament = response["tournament"]
+
+        return tournament
 
     def update(self, tournament_id: str, name: str = None, tournament_type: str = None,
                url: str = None, subdomain: str = None, description: str = None, open_signup: bool = None,
                hold_third_place_match: bool = None, pts_for_match_win: float = None,
                pts_for_match_tie: float = None, pts_for_game_win: float = None,
                pts_for_game_tie: float = None, pts_for_bye: float = None, swiss_rounds: int = None,
                ranked_by: str = None, rr_pts_for_match_win: float = None,
@@ -390,26 +418,32 @@
             "tournament[signup_cap]": signup_cap,
             "tournament[start_at]": start_at,
             "tournament[check_in_duration]": check_in_duration,
             "tournament[grand_finals_modifier]": grand_finals_modifier,
             "tournament[prediction_method]": prediction_method,
         }
 
-        response = self.http_put(f"tournaments/{tournament_id}.json", params=params)
-        return response
+        response = self.http.put(f"tournaments/{tournament_id}.json", params=params)
+
+        tournament = response["tournament"]
+
+        return tournament
 
     def delete(self, tournament_id: str):
         """
         Deletes a tournament along with all its associated records. There is no undo, so use with care!
 
         :param tournament_id: A tournament ID.
         """
 
-        response = self.http_delete(f"tournaments/{tournament_id}.json")
-        return response
+        response = self.http.delete(f"tournaments/{tournament_id}.json")
+
+        tournament = response["tournament"]
+
+        return tournament
 
     def process_checkins(self, tournament_id: str, include_participants: int = None,
                          include_matches: int = None):
         """
         This should be invoked after a tournament's check-in window closes before the tournament is started.
 
             - Marks participants who have not checked in as inactive.
@@ -426,16 +460,19 @@
         """
 
         params = {
             "include_participants": include_participants,
             "include_matches": include_matches
         }
 
-        response = self.http_post(f"tournaments/{tournament_id}/process_check_ins.json", params)
-        return response
+        response = self.http.post(f"tournaments/{tournament_id}/process_check_ins.json", params)
+
+        tournament = response["tournament"]
+
+        return tournament
 
     def abort_checkins(self, tournament_id: str, include_participants: int = None, include_matches: int = None):
         """
         When your tournament is in a 'checking_in' or 'checked_in' state, there's no way to edit the tournament's
         start time (start_at) or check-in duration (check_in_duration). You must first abort check-in,
         then you may edit those attributes.
 
@@ -450,43 +487,47 @@
         """
 
         params = {
             "include_participants": include_participants,
             "include_matches": include_matches
         }
 
-        response = self.http_post(f"tournaments/{tournament_id}/abort_check_in.json", params)
-        return response
+        response = self.http.post(f"tournaments/{tournament_id}/abort_check_in.json", params)
+
+        tournament = response["tournament"]
+
+        return tournament
 
     def start(self, tournament_id: str, include_participants: int = None, include_matches: int = None):
         """
         Start a tournament, opening up first round matches for score reporting. The tournament must have at least
         2 participants.
 
         :param tournament_id: Tournament ID (e.g. 10230) or URL (e.g. 'single_elim' for challonge.com/single_elim).
         If assigned to a subdomain, URL format must be :subdomain-:tournament_url (e.g. 'test-mytourney'
         for test.challonge.com/mytourney)
         :param include_participants: 0 or 1; includes an array of associated participant records
         :param include_matches: 0 or 1; includes an array of associated match records
         """
 
-        participant_api = ParticipantAPI()
-
         params = {
             "include_participants": include_participants,
             "include_matches": include_matches
         }
 
-        participants = participant_api.get_all(tournament_id)
+        participants = self.participant_api.get_all(tournament_id)
 
         if len(participants) <= 1:
             raise ChallongeAPIException("ERROR: A tournament needs at least two participants in order to start.")
         else:
-            response = self.http_post(f"tournaments/{tournament_id}/start.json", params)
-            return response
+            response = self.http.post(f"tournaments/{tournament_id}/start.json", params)
+
+            tournament = response["tournament"]
+
+            return tournament
 
     def finalize(self, tournament_id: str, include_participants: int = None, include_matches: int = None):
         """
         Finalize a tournament that has had all match scores submitted, rendering its results permanent.
 
         :param tournament_id: Tournament ID (e.g. 10230) or URL (e.g. 'single_elim' for challonge.com/single_elim).
         If assigned to a subdomain, URL format must be :subdomain-:tournament_url (e.g. 'test-mytourney'
@@ -496,16 +537,19 @@
         """
 
         params = {
             "include_participants": include_participants,
             "include_matches": include_matches
         }
 
-        response = self.http_post(f"tournaments/{tournament_id}/finalize.json", params)
-        return response
+        response = self.http.post(f"tournaments/{tournament_id}/finalize.json", params)
+
+        tournament = response["tournament"]
+
+        return tournament
 
     def reset(self, tournament_id: str, include_participants: int = None, include_matches: int = None):
         """
         Reset a tournament, clearing all of its scores and attachments. You can then add/remove/edit participants
         before starting the tournament again.
 
         :param tournament_id: Tournament ID (e.g. 10230) or URL (e.g. 'single_elim' for challonge.com/single_elim).
@@ -516,16 +560,19 @@
         """
 
         params = {
             "include_participants": include_participants,
             "include_matches": include_matches
         }
 
-        response = self.http_post(f"tournaments/{tournament_id}/reset.json", params)
-        return response
+        response = self.http.post(f"tournaments/{tournament_id}/reset.json", params)
+
+        tournament = response["tournament"]
+
+        return tournament
 
     def open_for_predictions(self, tournament_id: str, include_participants: int = None,
                              include_matches: int = None):
         """
         Sets the state of the tournament to start accepting predictions. Your tournament's 'prediction_method'
         attribute must be set to 1 (exponential scoring) or 2 (linear scoring) to use this option. Note: Once open
         for predictions, match records will be persisted, so participant additions and removals will no longer be
@@ -540,27 +587,36 @@
         """
 
         params = {
             "include_participants": include_participants,
             "include_matches": include_matches
         }
 
-        response = self.http_post(f"tournaments/{tournament_id}/open_for_predictions.json", params)
-        return response
+        response = self.http.post(f"tournaments/{tournament_id}/open_for_predictions.json", params)
+
+        tournament = response["tournament"]
 
+        return tournament
 
-class ParticipantAPI(ChallongeApi):
+
+class ParticipantAPI:
+
+    def __init__(self, http_methods):
+        self.http = http_methods
 
     def get_all(self, tournament_id: str):
         """
         Retrieve a tournament's participant list.
         """
 
-        response = self.http_get(f"tournaments/{tournament_id}/participants.json")
-        return response
+        response = self.http.get(f"tournaments/{tournament_id}/participants.json")
+
+        participants = [p["participant"] for p in response]
+
+        return participants
 
     def add(self, tournament_id: str, name: str = None, challonge_username: str = None, email: str = None,
             seed: str = None, misc: str = None):
         """
         Add a participant to a tournament (up until it is started).
         """
 
@@ -568,16 +624,19 @@
             "participant[name]": name,
             "participant[challonge_username]": challonge_username,
             "participant[email]": email,
             "participant[seed]": seed,
             "participant[misc]": misc,
         }
 
-        response = self.http_post(f"tournaments/{tournament_id}/participants.json", params)
-        return response
+        response = self.http.post(f"tournaments/{tournament_id}/participants.json", params)
+
+        participant = response["participant"]
+
+        return participant
 
     def add_multiple(self, tournament_id: str, names: List[str] = None,
                      challonge_usernames_or_emails: List[str] = None, seeds: List[str] = None,
                      miscs: List[str] = None):
         """
         Bulk add participants to a tournament (up until it is started). If an invalid participant is detected,
         bulk participant creation will halt and any previously added participants (from this API request) will
@@ -590,26 +649,32 @@
         params = {
             "participants[][name]": names,
             "participants[][invite_name_or_email]": challonge_usernames_or_emails,
             "participants[][seed]": seeds,
             "participants[][misc]": miscs,
         }
 
-        response = self.http_post(f"tournaments/{tournament_id}/participants/bulk_add.json", params)
-        return response
+        response = self.http.post(f"tournaments/{tournament_id}/participants/bulk_add.json", params)
+
+        participants = [p["participant"] for p in response]
+
+        return participants
 
     def get(self, tournament_id: str, participant_id: int = None, include_matches: bool = False):
         """
         Retrieve a single participant record for a tournament.
         """
 
         params = {"include_matches": include_matches}
 
-        response = self.http_get(f"tournaments/{tournament_id}/participants/{participant_id}.json", params)
-        return response
+        response = self.http.get(f"tournaments/{tournament_id}/participants/{participant_id}.json", params)
+
+        participant = response["participant"]
+
+        return participant
 
     def update(self, tournament_id: str, participant_id: str, participant_name: str = None,
                participant_challonge_username: str = None, participant_email: str = None,
                participant_seed: int = None, misc: str = None):
         """
         Update the attributes of a tournament participant.
         """
@@ -618,69 +683,183 @@
             "participant[name]": participant_name,
             "participant[challonge_username]": participant_challonge_username,
             "participant[email]": participant_email,
             "participant[seed]": participant_seed,
             "participant[misc]": misc,
         }
 
-        response = self.http_put(f"tournaments/{tournament_id}/participants/{participant_id}.json", params)
-        return response
+        response = self.http.put(f"tournaments/{tournament_id}/participants/{participant_id}.json", params)
+
+        participant = response["participant"]
+
+        return participant
 
     def check_in(self, tournament_id: str, participant_id: str):
         """
         Checks a participant in, setting checked_in_at to the current time.
         """
 
-        response = self.http_post(f"tournaments/{tournament_id}/participants/{participant_id}/check_in.json")
-        return response
+        response = self.http.post(f"tournaments/{tournament_id}/participants/{participant_id}/check_in.json")
+
+        participant = response["participant"]
+
+        return participant
 
     def check_out(self, tournament_id: str, participant_id: str):
         """
         Marks a participant as having not checked in, setting checked_in_at to nil - also called 'undo_check_in'.
         """
 
-        response = self.http_post(f"tournaments/{tournament_id}/participants/{participant_id}/undo_check_in.json")
-        return response
+        response = self.http.post(f"tournaments/{tournament_id}/participants/{participant_id}/undo_check_in.json")
+
+        participant = response["participant"]
+
+        return participant
 
     def remove(self, tournament_id: str, participant_id: str):
         """
         If the tournament has not started, delete a participant, automatically filling in the abandoned seed
         number. If tournament is underway, mark a participant inactive, automatically forfeiting his/her
         remaining matches.
         """
 
-        response = self.http_delete(f"tournaments/{tournament_id}/participants/{participant_id}.json")
-        return response
+        response = self.http.delete(f"tournaments/{tournament_id}/participants/{participant_id}.json")
+
+        participant = response["participant"]
+
+        return participant
 
     def remove_all(self, tournament_id: str):
         """
         Deletes all participants in a tournament. (Only allowed if tournament hasn't started yet)
         """
 
-        response = self.http_delete(f"tournaments/{tournament_id}/participants/clear.json")
-        return response
+        response = self.http.delete(f"tournaments/{tournament_id}/participants/clear.json")
+
+        return response["message"]  # "Cleared all participants"
 
     def randomize(self, tournament_id: str):
         """
         Randomize seeds among participants. Only applicable before a tournament has started.
         """
 
-        response = self.http_post(f"tournaments/{tournament_id}/participants/randomize.json")
-        return response
+        response = self.http.post(f"tournaments/{tournament_id}/participants/randomize.json")
+
+        participants = [p["participant"] for p in response]
+
+        return participants
+
+
+class MatchAPI:
+
+    def __init__(self, http_methods):
+        self.http = http_methods
+
+    def get_all(self, tournament_id: str, state: str = None, participant_id: str = None):
+        """
+        Retrieve a tournament's match list.
+        """
+
+        params = {"state": state, "participant_id": participant_id}
+        response = self.http.get(f"tournaments/{tournament_id}/matches.json", params)
+
+        matches = [m["match"] for m in response]
+
+        return matches
+
+    def get(self, tournament_id: str, match_id: str = None, include_attachments: int = 0):
+        """
+        Retrieve a single match record for a tournament.
+        """
+
+        params = {"include_attachments": include_attachments}
+        response = self.http.get(f"tournaments/{tournament_id}/matches/{match_id}.json", params)
+
+        match = response["match"]
 
+        return match
 
-class AttachmentAPI(ChallongeApi):
+    def update(self, tournament_id: str, match_id: str = None, match_scores_csv: str = None,
+               match_winner_id: str = None, match_player1_votes: str = None, match_player2_votes: str = None):
+        """
+        Update/submit the score(s) for a match. 'If you're updating winner_id, scores_csv must also be provided. You
+        may, however, update score_csv without providing winner_id for live score updates.'
+
+        :param tournament_id: A tournament ID.
+        :param match_id: A match ID.
+        :param match_scores_csv: Comma separated set/game scores with player 1 score first (e.g. "1-3,3-0,3-2")
+        :param match_winner_id: The participant ID of the winner or "tie" if applicable (Round Robin and Swiss).
+               NOTE: If you change the outcome of a completed match, all matches in the bracket that branch
+               from the updated match will be reset.
+        :param match_player1_votes: Overwrites the number of votes for player 1.
+        :param match_player2_votes: Overwrites the number of votes for player 2.
+        """
+
+        params = {
+            "match[scores_csv]": match_scores_csv,
+            "match[winner_id]": match_winner_id,
+            "match[player1_votes]": match_player1_votes,
+            "match[player2_votes]": match_player2_votes
+        }
+
+        response = self.http.put(f"tournaments/{tournament_id}/matches/{match_id}.json", params)
+
+        match = response["match"]
+
+        return match
+
+    def reopen(self, tournament_id: str, match_id: str = None):
+        """
+        Reopens a match that was marked completed, automatically resetting matches that follow it.
+        """
+
+        response = self.http.post(f"tournaments/{tournament_id}/matches/{match_id}/reopen.json")
+
+        match = response["match"]
+
+        return match
+
+    def set_underway(self, tournament_id: str, match_id: str = None):
+        """
+        Sets "underway_at" to the current time and highlights the match in the bracket
+        """
+
+        response = self.http.post(f"tournaments/{tournament_id}/matches/{match_id}/mark_as_underway.json")
+
+        match = response["match"]
+
+        return match
+
+    def unset_underway(self, tournament_id: str, match_id: str = None):
+        """
+        Clears "underway_at" and unhighlights the match in the bracket
+        """
+
+        response = self.http.post(f"tournaments/{tournament_id}/matches/{match_id}/unmark_as_underway.json")
+
+        match = response["match"]
+
+        return match
+
+
+class AttachmentAPI:
+
+    def __init__(self, http_methods):
+        self.http = http_methods
 
     def get_all(self, tournament_id: str, match_id: str = None):
         """
         Retrieve a set of attachments created for a specific match.
         """
 
-        response = self.http_get(f"tournaments/{tournament_id}/matches/{match_id}/attachments.json")
-        return response
+        response = self.http.get(f"tournaments/{tournament_id}/matches/{match_id}/attachments.json")
+
+        match_attachments = [ma["match_attachment"] for ma in response]
+
+        return match_attachments
 
     def create(self, tournament_id: str, match_id: str = None, match_attachment_asset: str = None,
                match_attachment_url: str = None, match_attachment_description: str = None):
         """
         Create a new attachment for the specific match.
 
         :param tournament_id: A tournament ID.
@@ -694,24 +873,30 @@
 
         params = {
             "match_attachment[asset]": match_attachment_asset,
             "match_attachment[url]": match_attachment_url,
             "match_attachment[description]": match_attachment_description
         }
 
-        response = self.http_post(f"tournaments/{tournament_id}/matches/{match_id}/attachments.json", params)
-        return response
+        response = self.http.post(f"tournaments/{tournament_id}/matches/{match_id}/attachments.json", params)
+
+        match_attachment = response["match_attachment"]
+
+        return match_attachment
 
     def get(self, tournament_id: str, match_id: str = None, attachment_id: str = None):
         """
         Retrieve a single match attachment record.
         """
 
-        response = self.http_get(f"tournaments/{tournament_id}/matches/{match_id}/attachments/{attachment_id}.json")
-        return response
+        response = self.http.get(f"tournaments/{tournament_id}/matches/{match_id}/attachments/{attachment_id}.json")
+
+        match_attachment = response["match_attachment"]
+
+        return match_attachment
 
     def update(self, tournament_id: str, match_id: str = None, attachment_id: str = None,
                match_attachment_asset: str = None, match_attachment_url: str = None,
                match_attachment_description: str = None):
         """
         Update the attributes of a match attachment.
 
@@ -728,90 +913,27 @@
 
         params = {
             "match_attachment[asset]": match_attachment_asset,
             "match_attachment[url]": match_attachment_url,
             "match_attachment[description]": match_attachment_description
         }
 
-        response = self.http_put(
+        response = self.http.put(
             f"tournaments/{tournament_id}/matches/{match_id}/attachments/{attachment_id}.json", params
         )
-        return response
-
-    def delete(self, tournament_id: str, match_id: str = None, attachment_id: str = None):
-        """
-        Delete a match attachment.
-        """
 
-        response = self.http_delete(f"tournaments/{tournament_id}/matches/{match_id}/attachments/{attachment_id}.json")
-        return response
+        match_attachment = response["match_attachment"]
 
+        return match_attachment
 
-class MatchAPI(ChallongeApi):
-
-    def get_all(self, tournament_id: str, state: str = None, participant_id: str = None):
-        """
-        Retrieve a tournament's match list.
-        """
-
-        params = {"state": state, "participant_id": participant_id}
-        response = self.http_get(f"tournaments/{tournament_id}/matches.json", params)
-        return response
-
-    def get(self, tournament_id: str, match_id: str = None, include_attachments: int = 0):
-        """
-        Retrieve a single match record for a tournament.
-        """
-
-        params = {"include_attachments": include_attachments}
-        response = self.http_get(f"tournaments/{tournament_id}/matches/{match_id}.json", params)
-        return response
-
-    def update(self, tournament_id: str, match_id: str = None, match_scores_csv: str = None,
-               match_winner_id: str = None, match_player1_votes: str = None, match_player2_votes: str = None):
-        """
-        Update/submit the score(s) for a match. 'If you're updating winner_id, scores_csv must also be provided. You
-        may, however, update score_csv without providing winner_id for live score updates.'
-
-        :param tournament_id: A tournament ID.
-        :param match_id: A match ID.
-        :param match_scores_csv: Comma separated set/game scores with player 1 score first (e.g. "1-3,3-0,3-2")
-        :param match_winner_id: The participant ID of the winner or "tie" if applicable (Round Robin and Swiss).
-               NOTE: If you change the outcome of a completed match, all matches in the bracket that branch
-               from the updated match will be reset.
-        :param match_player1_votes: Overwrites the number of votes for player 1.
-        :param match_player2_votes: Overwrites the number of votes for player 2.
-        """
-
-        params = {
-            "match[scores_csv]": match_scores_csv,
-            "match[winner_id]": match_winner_id,
-            "match[player1_votes]": match_player1_votes,
-            "match[player2_votes]": match_player2_votes
-        }
-
-        response = self.http_put(f"tournaments/{tournament_id}/matches/{match_id}.json", params)
-        return response
-
-    def reopen(self, tournament_id: str, match_id: str = None):
+    def delete(self, tournament_id: str, match_id: str = None, attachment_id: str = None):
         """
-        Reopens a match that was marked completed, automatically resetting matches that follow it.
+        Delete a match attachment.
         """
 
-        response = self.http_post(f"tournaments/{tournament_id}/matches/{match_id}/reopen.json")
-        return response
+        response = self.http.delete(f"tournaments/{tournament_id}/matches/{match_id}/attachments/{attachment_id}.json")
 
-    def set_underway(self, tournament_id: str, match_id: str = None):
-        """
-        Sets "underway_at" to the current time and highlights the match in the bracket
-        """
+        match_attachment = response["match_attachment"]
 
-        response = self.http_post(f"tournaments/{tournament_id}/matches/{match_id}/mark_as_underway.json")
-        return response
+        return match_attachment
 
-    def unset_underway(self, tournament_id: str, match_id: str = None):
-        """
-        Clears "underway_at" and unhighlights the match in the bracket
-        """
 
-        response = self.http_post(f"tournaments/{tournament_id}/matches/{match_id}/unmark_as_underway.json")
-        return response
```

### Comparing `chyllonge-1.0.6/PKG-INFO` & `chyllonge-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chyllonge
-Version: 1.0.6
+Version: 1.1.0
 Summary: A Python 3.8+ implementation of the challonge.com API.
 Keywords: challonge
 Author-email: Alex Fredrickson <alex.q.fredrickson@gmail.com>
 Maintainer-email: Alex Fredrickson <alex.q.fredrickson@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
@@ -38,48 +38,43 @@
 To install `chyllonge`, execute `pip install chyllonge`.
 
 ## Usage
 
 Detailed API documentation is available at https://api.challonge.com/v1.
 
 ```python
-from chyllonge.api import TournamentAPI, ParticipantAPI, MatchAPI, AttachmentAPI
+from chyllonge.api import ChallongeAPI
 from datetime import datetime, timedelta
 
-# instantiate base api classes
-tournaments_api = TournamentAPI()
-participants_api = ParticipantAPI()
-match_api = MatchAPI()
-attachment_api = AttachmentAPI()
+api = ChallongeAPI()
 
 # create a basic tournament
-tournament = tournaments_api.create(name="My Chyllonge Tournament")
-print(tournament["tournament"]["id"])
+tournament = api.tournaments.create(name="My Chyllonge Tournament")
+print(tournament["id"])
 
 # create a tournament that starts in an hour
-an_hour_from_now = (datetime.now() + timedelta(hours=1)).isoformat() + tournaments_api.tz_utc_offset_string
-tournament = tournaments_api.create(name="My Chyllonge Tournament", start_at=an_hour_from_now, check_in_duration=60)
-print(tournament["tournament"]["id"])
+an_hour_from_now = (datetime.now() + timedelta(hours=1)).isoformat() + api.http.tz_utc_offset_string
+tournament = api.tournaments.create(name="My Chyllonge Tournament", start_at=an_hour_from_now, check_in_duration=60)
+print(tournament["id"])
 
 # create a tournament, add Alice and Bob, process their check-ins, start the tournment, set their match underway,
 # score their match (congratulations Alice!), finalize the tournament
-an_hour_from_now = (datetime.now() + timedelta(hours=1)).isoformat() + tournaments_api.tz_utc_offset_string
-tournament = tournaments_api.create(name="Alice and Bob Play Bingo", start_at=an_hour_from_now, check_in_duration=60)
-tournament_id = tournament["tournament"]["id"]
-
-participants_api.add(tournament_id, name="Alice")
-participants_api.add(tournament_id, name="Bob")
-tournaments_api.process_checkins(tournament_id)
-tournaments_api.start(tournament_id)
-match_id = match_api.get_all(tournament_id=tournament_id)[0]["match"]["id"]
-alice_id = participants_api.get_all(tournament_id)[0]["participant"]["id"]
-match_api.set_underway(tournament_id, match_id)
-match_api.update(tournament_id, match_id, match_scores_csv="3-1,2-2", match_winner_id=alice_id)
-tournaments_api.finalize(tournament_id)
-finished_tournment = tournaments_api.get(tournament_id)
+an_hour_from_now = (datetime.now() + timedelta(hours=1)).isoformat() + api.http.tz_utc_offset_string
+tournament = api.tournaments.create(name="Alice and Bob Play Bingo", start_at=an_hour_from_now, check_in_duration=60)
+tournament_id = tournament["id"]
+api.participants.add(tournament_id, name="Alice")
+api.participants.add(tournament_id, name="Bob")
+api.tournaments.process_checkins(tournament_id)
+api.tournaments.start(tournament_id)
+match_id = api.matches.get_all(tournament_id=tournament_id)[0]["id"]
+alice_id = api.participants.get_all(tournament_id)[0]["id"]
+api.matches.set_underway(tournament_id, match_id)
+api.matches.update(tournament_id, match_id, match_scores_csv="3-1,2-2", match_winner_id=alice_id)
+api.tournaments.finalize(tournament_id)
+finished_tournment = api.tournaments.get(tournament_id)
 ```
 
 ## History
 
 `chyllonge` was inspired by `pychallonge` - developed by Russ Amos - which (in turn) includes `pychal`. 
 
 See `CONTRIBUTORS.txt` for the original authors.
```

