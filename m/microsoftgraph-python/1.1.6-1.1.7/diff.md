# Comparing `tmp/microsoftgraph_python-1.1.6.tar.gz` & `tmp/microsoftgraph_python-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoftgraph_python-1.1.6.tar", max compression
+gzip compressed data, was "microsoftgraph_python-1.1.7.tar", max compression
```

## Comparing `microsoftgraph_python-1.1.6.tar` & `microsoftgraph_python-1.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1065 2023-03-27 20:32:33.898149 microsoftgraph_python-1.1.6/LICENSE
--rw-r--r--   0        0        0     9280 2023-03-27 20:32:33.898418 microsoftgraph_python-1.1.6/README.md
--rw-r--r--   0        0        0        0 2023-03-27 20:32:33.898512 microsoftgraph_python-1.1.6/microsoftgraph/__init__.py
--rw-r--r--   0        0        0     5603 2023-03-27 20:32:33.898642 microsoftgraph_python-1.1.6/microsoftgraph/calendar.py
--rw-r--r--   0        0        0    13081 2023-03-27 20:32:33.898806 microsoftgraph_python-1.1.6/microsoftgraph/client.py
--rw-r--r--   0        0        0     4452 2023-03-27 20:32:33.898907 microsoftgraph_python-1.1.6/microsoftgraph/contacts.py
--rw-r--r--   0        0        0      632 2023-03-27 20:32:33.898994 microsoftgraph_python-1.1.6/microsoftgraph/decorators.py
--rw-r--r--   0        0        0     1073 2023-03-27 20:32:33.899233 microsoftgraph_python-1.1.6/microsoftgraph/exceptions.py
--rw-r--r--   0        0        0     8022 2023-03-27 20:32:33.899377 microsoftgraph_python-1.1.6/microsoftgraph/files.py
--rw-r--r--   0        0        0     6602 2023-03-27 20:32:33.899479 microsoftgraph_python-1.1.6/microsoftgraph/mail.py
--rw-r--r--   0        0        0     3103 2023-03-27 20:32:33.899592 microsoftgraph_python-1.1.6/microsoftgraph/notes.py
--rw-r--r--   0        0        0      871 2023-03-27 20:32:33.899686 microsoftgraph_python-1.1.6/microsoftgraph/response.py
--rw-r--r--   0        0        0     1174 2023-03-27 20:32:33.899797 microsoftgraph_python-1.1.6/microsoftgraph/users.py
--rw-r--r--   0        0        0      220 2023-03-27 20:32:33.899884 microsoftgraph_python-1.1.6/microsoftgraph/utils.py
--rw-r--r--   0        0        0     3321 2023-03-27 20:32:33.899980 microsoftgraph_python-1.1.6/microsoftgraph/webhooks.py
--rw-r--r--   0        0        0    12372 2023-03-27 20:32:33.900065 microsoftgraph_python-1.1.6/microsoftgraph/workbooks.py
--rw-r--r--   0        0        0      416 2023-03-27 20:35:00.604777 microsoftgraph_python-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     9942 1970-01-01 00:00:00.000000 microsoftgraph_python-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-04-03 16:04:40.073651 microsoftgraph_python-1.1.7/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-03 16:04:40.084643 microsoftgraph_python-1.1.7/microsoftgraph/__init__.py
+-rw-r--r--   0        0        0     5752 2024-04-03 16:04:40.085313 microsoftgraph_python-1.1.7/microsoftgraph/calendar.py
+-rw-r--r--   0        0        0    13497 2024-04-03 16:04:40.085951 microsoftgraph_python-1.1.7/microsoftgraph/client.py
+-rw-r--r--   0        0        0     4568 2024-04-03 16:04:40.086455 microsoftgraph_python-1.1.7/microsoftgraph/contacts.py
+-rw-r--r--   0        0        0      656 2024-04-03 16:04:40.111027 microsoftgraph_python-1.1.7/microsoftgraph/decorators.py
+-rw-r--r--   0        0        0     1167 2024-04-03 16:04:40.111531 microsoftgraph_python-1.1.7/microsoftgraph/exceptions.py
+-rw-r--r--   0        0        0     8215 2024-04-03 16:04:40.112045 microsoftgraph_python-1.1.7/microsoftgraph/files.py
+-rw-r--r--   0        0        0     6764 2024-04-03 16:04:40.112587 microsoftgraph_python-1.1.7/microsoftgraph/mail.py
+-rw-r--r--   0        0        0     3190 2024-04-03 16:04:40.113420 microsoftgraph_python-1.1.7/microsoftgraph/notes.py
+-rw-r--r--   0        0        0      902 2024-04-03 16:04:40.113928 microsoftgraph_python-1.1.7/microsoftgraph/response.py
+-rw-r--r--   0        0        0     1206 2024-04-03 16:04:40.114451 microsoftgraph_python-1.1.7/microsoftgraph/users.py
+-rw-r--r--   0        0        0      227 2024-04-03 16:04:40.115630 microsoftgraph_python-1.1.7/microsoftgraph/utils.py
+-rw-r--r--   0        0        0     3409 2024-04-03 16:04:40.116135 microsoftgraph_python-1.1.7/microsoftgraph/webhooks.py
+-rw-r--r--   0        0        0    12692 2024-04-03 16:04:40.116835 microsoftgraph_python-1.1.7/microsoftgraph/workbooks.py
+-rw-r--r--   0        0        0      425 2024-04-03 16:05:30.315317 microsoftgraph_python-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     9654 2024-04-03 16:04:40.084019 microsoftgraph_python-1.1.7/README.md
+-rw-r--r--   0        0        0     9984 1970-01-01 00:00:00.000000 microsoftgraph_python-1.1.7/PKG-INFO
```

### Comparing `microsoftgraph_python-1.1.6/LICENSE` & `microsoftgraph_python-1.1.7/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2018 GearPlug
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2018 GearPlug
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `microsoftgraph_python-1.1.6/README.md` & `microsoftgraph_python-1.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: microsoftgraph-python
+Version: 1.1.7
+Summary: API wrapper for Microsoft Graph written in Python
+License: MIT
+Author: Gearplug Team
+Author-email: apps@gearplug.io
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: requests (>=2.26.0,<3.0.0)
+Description-Content-Type: text/markdown
+
 # microsoftgraph-python
 Microsoft graph API wrapper for Microsoft Graph written in Python.
 
 ## Before start
 To use Microsoft Graph to read and write resources on behalf of a user, your app must get an access token from
 the Microsoft identity platform and attach the token to requests that it sends to Microsoft Graph. The exact
 authentication flow that you will use to get access tokens will depend on the kind of app you are developing and
@@ -368,7 +387,8 @@
 ## Requirements
 - requests
 
 ## Tests
 ```
 test/test.py
 ```
+
```

### Comparing `microsoftgraph_python-1.1.6/microsoftgraph/calendar.py` & `microsoftgraph_python-1.1.7/microsoftgraph/calendar.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-from datetime import datetime
-
-from microsoftgraph.decorators import token_required
-from microsoftgraph.response import Response
-from microsoftgraph.utils import format_time
-
-
-class Calendar(object):
-    def __init__(self, client) -> None:
-        """Working with Outlook Calendar.
-
-        https://docs.microsoft.com/en-us/graph/api/resources/calendar?view=graph-rest-1.0
-
-        Args:
-            client (Client): Library Client.
-        """
-        self._client = client
-
-    @token_required
-    def list_events(self, calendar_id: str = None, params: dict = None) -> Response:
-        """Get a list of event objects in the user's mailbox. The list contains single instance meetings and series
-        masters.
-
-        https://docs.microsoft.com/en-us/graph/api/user-list-events?view=graph-rest-1.0&tabs=http
-
-        Args:
-            calendar_id (str): Calendar ID.
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        url = "me/calendars/{}/events".format(calendar_id) if calendar_id else "me/events"
-        return self._client._get(self._client.base_url + url, params=params)
-
-    @token_required
-    def get_event(self, event_id: str, params: dict = None) -> Response:
-        """Get the properties and relationships of the specified event object.
-
-        https://docs.microsoft.com/en-us/graph/api/event-get?view=graph-rest-1.0&tabs=http
-
-        Args:
-            event_id (str): Event ID.
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        return self._client._get(self._client.base_url + "me/events/{}".format(event_id), params=params)
-
-    @token_required
-    def create_event(
-        self,
-        subject: str,
-        content: str,
-        start_datetime: datetime,
-        start_timezone: str,
-        end_datetime: datetime,
-        end_timezone: str,
-        location: str,
-        calendar_id: str = None,
-        content_type: str = "HTML",
-        attendees: list = None,
-        is_online_meeting: bool = False,
-        online_meeting_provider: str = 'teamsForBusiness',
-        **kwargs,
-    ) -> Response:
-        """Create an event in the user's default calendar or specified calendar.
-
-        https://docs.microsoft.com/en-us/graph/api/user-post-events?view=graph-rest-1.0&tabs=http
-
-        Additional time zones: https://docs.microsoft.com/en-us/graph/api/resources/datetimetimezone?view=graph-rest-1.0
-
-        Args:
-            subject (str): The text of the event's subject line.
-            content (str): The body of the message associated with the event.
-            start_datetime (datetime): A single point of time in a combined date and time representation ({date}T{time};
-            start_timezone (str): Represents a time zone, for example, "Pacific Standard Time".
-            end_datetime (datetime): A single point of time in a combined date and time representation ({date}T{time}; for
-            end_timezone (str): Represents a time zone, for example, "Pacific Standard Time".
-            location (str): The location of the event.
-            calendar_id (str, optional): Calendar ID. Defaults to None.
-            content_type (str, optional): It can be in HTML or text format. Defaults to HTML.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        if isinstance(start_datetime, datetime):
-            start_datetime = format_time(start_datetime)
-        if isinstance(end_datetime, datetime):
-            end_datetime = format_time(end_datetime)
-
-        body = {
-            "subject": subject,
-            "body": {
-                "contentType": content_type,
-                "content": content,
-            },
-            "start": {
-                "dateTime": start_datetime,
-                "timeZone": start_timezone,
-            },
-            "end": {
-                "dateTime": end_datetime,
-                "timeZone": end_timezone,
-            },
-            "location": {"displayName": location},
-            "isOnlineMeeting": is_online_meeting,
-        }
-
-        if is_online_meeting:
-            body["onlineMeetingProvider"] = online_meeting_provider
-
-        if attendees:
-            body["attendees"] = attendees
-
-        body.update(kwargs)
-        url = "me/calendars/{}/events".format(calendar_id) if calendar_id is not None else "me/events"
-        return self._client._post(self._client.base_url + url, json=body)
-
-    @token_required
-    def list_calendars(self, params: dict = None) -> Response:
-        """Get all the user's calendars (/calendars navigation property), get the calendars from the default calendar
-        group or from a specific calendar group.
-
-        https://docs.microsoft.com/en-us/graph/api/user-list-calendars?view=graph-rest-1.0&tabs=http
-
-        Args:
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        return self._client._get(self._client.base_url + "me/calendars", params=params)
-
-    @token_required
-    def create_calendar(self, name: str) -> Response:
-        """Create a new calendar for a user.
-
-        https://docs.microsoft.com/en-us/graph/api/user-post-calendars?view=graph-rest-1.0&tabs=http
-
-        Args:
-            name (str): The calendar name.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        body = {"name": "{}".format(name)}
-        return self._client._post(self._client.base_url + "me/calendars", json=body)
+from datetime import datetime
+
+from microsoftgraph.decorators import token_required
+from microsoftgraph.response import Response
+from microsoftgraph.utils import format_time
+
+
+class Calendar(object):
+    def __init__(self, client) -> None:
+        """Working with Outlook Calendar.
+
+        https://docs.microsoft.com/en-us/graph/api/resources/calendar?view=graph-rest-1.0
+
+        Args:
+            client (Client): Library Client.
+        """
+        self._client = client
+
+    @token_required
+    def list_events(self, calendar_id: str = None, params: dict = None) -> Response:
+        """Get a list of event objects in the user's mailbox. The list contains single instance meetings and series
+        masters.
+
+        https://docs.microsoft.com/en-us/graph/api/user-list-events?view=graph-rest-1.0&tabs=http
+
+        Args:
+            calendar_id (str): Calendar ID.
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        url = "me/calendars/{}/events".format(calendar_id) if calendar_id else "me/events"
+        return self._client._get(self._client.base_url + url, params=params)
+
+    @token_required
+    def get_event(self, event_id: str, params: dict = None) -> Response:
+        """Get the properties and relationships of the specified event object.
+
+        https://docs.microsoft.com/en-us/graph/api/event-get?view=graph-rest-1.0&tabs=http
+
+        Args:
+            event_id (str): Event ID.
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        return self._client._get(self._client.base_url + "me/events/{}".format(event_id), params=params)
+
+    @token_required
+    def create_event(
+        self,
+        subject: str,
+        content: str,
+        start_datetime: datetime,
+        start_timezone: str,
+        end_datetime: datetime,
+        end_timezone: str,
+        location: str,
+        calendar_id: str = None,
+        content_type: str = "HTML",
+        attendees: list = None,
+        is_online_meeting: bool = False,
+        online_meeting_provider: str = 'teamsForBusiness',
+        **kwargs,
+    ) -> Response:
+        """Create an event in the user's default calendar or specified calendar.
+
+        https://docs.microsoft.com/en-us/graph/api/user-post-events?view=graph-rest-1.0&tabs=http
+
+        Additional time zones: https://docs.microsoft.com/en-us/graph/api/resources/datetimetimezone?view=graph-rest-1.0
+
+        Args:
+            subject (str): The text of the event's subject line.
+            content (str): The body of the message associated with the event.
+            start_datetime (datetime): A single point of time in a combined date and time representation ({date}T{time};
+            start_timezone (str): Represents a time zone, for example, "Pacific Standard Time".
+            end_datetime (datetime): A single point of time in a combined date and time representation ({date}T{time}; for
+            end_timezone (str): Represents a time zone, for example, "Pacific Standard Time".
+            location (str): The location of the event.
+            calendar_id (str, optional): Calendar ID. Defaults to None.
+            content_type (str, optional): It can be in HTML or text format. Defaults to HTML.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        if isinstance(start_datetime, datetime):
+            start_datetime = format_time(start_datetime)
+        if isinstance(end_datetime, datetime):
+            end_datetime = format_time(end_datetime)
+
+        body = {
+            "subject": subject,
+            "body": {
+                "contentType": content_type,
+                "content": content,
+            },
+            "start": {
+                "dateTime": start_datetime,
+                "timeZone": start_timezone,
+            },
+            "end": {
+                "dateTime": end_datetime,
+                "timeZone": end_timezone,
+            },
+            "location": {"displayName": location},
+            "isOnlineMeeting": is_online_meeting,
+        }
+
+        if is_online_meeting:
+            body["onlineMeetingProvider"] = online_meeting_provider
+
+        if attendees:
+            body["attendees"] = attendees
+
+        body.update(kwargs)
+        url = "me/calendars/{}/events".format(calendar_id) if calendar_id is not None else "me/events"
+        return self._client._post(self._client.base_url + url, json=body)
+
+    @token_required
+    def list_calendars(self, params: dict = None) -> Response:
+        """Get all the user's calendars (/calendars navigation property), get the calendars from the default calendar
+        group or from a specific calendar group.
+
+        https://docs.microsoft.com/en-us/graph/api/user-list-calendars?view=graph-rest-1.0&tabs=http
+
+        Args:
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        return self._client._get(self._client.base_url + "me/calendars", params=params)
+
+    @token_required
+    def create_calendar(self, name: str) -> Response:
+        """Create a new calendar for a user.
+
+        https://docs.microsoft.com/en-us/graph/api/user-post-calendars?view=graph-rest-1.0&tabs=http
+
+        Args:
+            name (str): The calendar name.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        body = {"name": "{}".format(name)}
+        return self._client._post(self._client.base_url + "me/calendars", json=body)
```

### Comparing `microsoftgraph_python-1.1.6/microsoftgraph/client.py` & `microsoftgraph_python-1.1.7/microsoftgraph/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,313 +1,319 @@
-from typing import Optional
-from urllib.parse import urlencode
-
-import requests
-
-from microsoftgraph import exceptions
-from microsoftgraph.calendar import Calendar
-from microsoftgraph.contacts import Contacts
-from microsoftgraph.files import Files
-from microsoftgraph.mail import Mail
-from microsoftgraph.notes import Notes
-from microsoftgraph.response import Response
-from microsoftgraph.users import Users
-from microsoftgraph.webhooks import Webhooks
-from microsoftgraph.workbooks import Workbooks
-
-
-class Client(object):
-    AUTHORITY_URL = "https://login.microsoftonline.com/"
-    AUTH_ENDPOINT = "/oauth2/v2.0/authorize?"
-    TOKEN_ENDPOINT = "/oauth2/v2.0/token"
-    RESOURCE = "https://graph.microsoft.com/"
-
-    def __init__(
-        self,
-        client_id: str,
-        client_secret: str,
-        api_version: str = "v1.0",
-        account_type: str = "common",
-        requests_hooks: dict = None,
-        paginate: bool = True,
-    ) -> None:
-        """Instantiates library.
-
-        Args:
-            client_id (str): Application client id.
-            client_secret (str): Application client secret.
-            api_version (str, optional): v1.0 or beta. Defaults to "v1.0".
-            account_type (str, optional): common, organizations or consumers. Defaults to "common".
-            requests_hooks (dict, optional): Requests library event hooks. Defaults to None.
-
-        Raises:
-            Exception: requests_hooks is not a dict.
-        """
-        self.client_id = client_id
-        self.client_secret = client_secret
-        self.api_version = api_version
-        self.account_type = account_type
-
-        self.base_url = self.RESOURCE + self.api_version + "/"
-        self.token = None
-        self.workbook_session_id = None
-        self.paginate = paginate
-
-        self.calendar = Calendar(self)
-        self.contacts = Contacts(self)
-        self.files = Files(self)
-        self.mail = Mail(self)
-        self.notes = Notes(self)
-        self.users = Users(self)
-        self.webhooks = Webhooks(self)
-        self.workbooks = Workbooks(self)
-
-        if requests_hooks and not isinstance(requests_hooks, dict):
-            raise Exception(
-                'requests_hooks must be a dict. e.g. {"response": func}. http://docs.python-requests.org/en/master/user/advanced/#event-hooks'
-            )
-        self.requests_hooks = requests_hooks
-
-    def authorization_url(self, redirect_uri: str, scope: list, state: str = None) -> str:
-        """Generates an Authorization URL.
-
-        The first step to getting an access token for many OpenID Connect (OIDC) and OAuth 2.0 flows is to redirect the
-        user to the Microsoft identity platform /authorize endpoint. Azure AD will sign the user in and ensure their
-        consent for the permissions your app requests. In the authorization code grant flow, after consent is obtained,
-        Azure AD will return an authorization_code to your app that it can redeem at the Microsoft identity platform
-        /token endpoint for an access token.
-
-        https://docs.microsoft.com/en-us/graph/auth-v2-user#2-get-authorization
-
-        Args:
-            redirect_uri (str): The redirect_uri of your app, where authentication responses can be sent and received by
-            your app. It must exactly match one of the redirect_uris you registered in the app registration portal.
-            scope (list): A list of the Microsoft Graph permissions that you want the user to consent to. This may also
-            include OpenID scopes.
-            state (str, optional): A value included in the request that will also be returned in the token response.
-            It can be a string of any content that you wish.  A randomly generated unique value is typically
-            used for preventing cross-site request forgery attacks.  The state is also used to encode information
-            about the user's state in the app before the authentication request occurred, such as the page or view
-            they were on. Defaults to None.
-
-        Returns:
-            str: Url for OAuth 2.0.
-        """
-        params = {
-            "client_id": self.client_id,
-            "redirect_uri": redirect_uri,
-            "scope": " ".join(scope),
-            "response_type": "code",
-            "response_mode": "query",
-        }
-
-        if state:
-            params["state"] = state
-        response = self.AUTHORITY_URL + self.account_type + self.AUTH_ENDPOINT + urlencode(params)
-        return response
-
-    def exchange_code(self, redirect_uri: str, code: str) -> Response:
-        """Exchanges an oauth code for an user token.
-
-        Your app uses the authorization code received in the previous step to request an access token by sending a POST
-        request to the /token endpoint.
-
-        https://docs.microsoft.com/en-us/graph/auth-v2-user#3-get-a-token
-
-        Args:
-            redirect_uri (str): The redirect_uri of your app, where authentication responses can be sent and received by
-            your app.  It must exactly match one of the redirect_uris you registered in the app registration portal.
-            code (str): The authorization_code that you acquired in the first leg of the flow.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        data = {
-            "client_id": self.client_id,
-            "redirect_uri": redirect_uri,
-            "client_secret": self.client_secret,
-            "code": code,
-            "grant_type": "authorization_code",
-        }
-        response = requests.post(self.AUTHORITY_URL + self.account_type + self.TOKEN_ENDPOINT, data=data)
-        return self._parse(response)
-
-    def refresh_token(self, redirect_uri: str, refresh_token: str) -> Response:
-        """Exchanges a refresh token for an user token.
-
-        Access tokens are short lived, and you must refresh them after they expire to continue accessing resources.
-        You can do so by submitting another POST request to the /token endpoint, this time providing the refresh_token
-        instead of the code.
-
-        https://docs.microsoft.com/en-us/graph/auth-v2-user#5-use-the-refresh-token-to-get-a-new-access-token
-
-        Args:
-            redirect_uri (str): The redirect_uri of your app, where authentication responses can be sent and received by
-            your app.  It must exactly match one of the redirect_uris you registered in the app registration portal.
-            refresh_token (str): An OAuth 2.0 refresh token. Your app can use this token acquire additional access tokens
-            after the current access token expires. Refresh tokens are long-lived, and can be used to retain access
-            to resources for extended periods of time.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        data = {
-            "client_id": self.client_id,
-            "redirect_uri": redirect_uri,
-            "client_secret": self.client_secret,
-            "refresh_token": refresh_token,
-            "grant_type": "refresh_token",
-        }
-        response = requests.post(self.AUTHORITY_URL + self.account_type + self.TOKEN_ENDPOINT, data=data)
-        return self._parse(response)
-
-    def set_token(self, token: dict) -> None:
-        """Sets the User token for its use in this library.
-
-        Args:
-            token (dict): User token data.
-        """
-        self.token = token
-
-    def set_workbook_session_id(self, workbook_session_id: dict) -> None:
-        """Sets the Workbook Session Id token for its use in this library.
-
-        Args:
-            token (dict): Workbook Session ID.
-        """
-        self.workbook_session_id = workbook_session_id
-
-    def get_next(self, response: Response) -> Optional[Response]:
-        """Retrieves the next page for the argument response if any. This allows to perform a loop in case you
-        want to paginate the response yourself.
-
-        Args:
-            response (Response): Graph API Response.
-
-        Returns:
-            Optional[Response]: Graph API Response if available, None otherwise
-        """
-        if not isinstance(response.data, dict):
-            return None
-
-        if "@odata.nextLink" not in response.data:
-            return None
-
-        return self._do_get(response.data["@odata.nextLink"])
-
-    def _paginate_response(self, response: Response) -> Response:
-        """Some queries against Microsoft Graph return multiple pages of data either due to server-side paging or due to
-        the use of the $top query parameter to specifically limit the page size in a request. When a result set spans
-        multiple pages, Microsoft Graph returns an @odata.nextLink property in the response that contains a URL to the
-        next page of results.
-
-        https://docs.microsoft.com/en-us/graph/paging?context=graph%2Fapi%2F1.0&view=graph-rest-1.0
-
-        Args:
-            response (Response): Graph API Response.
-
-        Returns:
-            Response: Graph API Response.
-        """
-        if not isinstance(response.data, dict) or "value" not in response.data:
-            return response
-
-        # Copy data to avoid side effects
-        data = list(response.data["value"])
-
-        while "@odata.nextLink" in response.data:
-            response = self.get_next(response)
-            if isinstance(response.data, dict) and "value" in response.data:
-                data.extend(response.data["value"])
-
-        response.data["value"] = data
-        return response
-
-    def _get(self, url, **kwargs) -> Response:
-        response = self._do_get(url, **kwargs)
-        if self.paginate:
-            return self._paginate_response(response)
-
-        return response
-
-    def _do_get(self, url, **kwargs) -> Response:
-        return self._request("GET", url, **kwargs)
-
-    def _post(self, url, **kwargs):
-        return self._request("POST", url, **kwargs)
-
-    def _put(self, url, **kwargs):
-        return self._request("PUT", url, **kwargs)
-
-    def _patch(self, url, **kwargs):
-        return self._request("PATCH", url, **kwargs)
-
-    def _delete(self, url, **kwargs):
-        return self._request("DELETE", url, **kwargs)
-
-    def _request(self, method, url, headers=None, **kwargs) -> Response:
-        _headers = {
-            "Accept": "application/json",
-        }
-        _headers["Authorization"] = "Bearer " + self.token["access_token"]
-        if headers:
-            _headers.update(headers)
-        if self.requests_hooks:
-            kwargs.update({"hooks": self.requests_hooks})
-        if "Content-Type" not in _headers:
-            _headers["Content-Type"] = "application/json"
-        return self._parse(requests.request(method, url, headers=_headers, **kwargs))
-
-    def _parse(self, response) -> Response:
-        status_code = response.status_code
-        r = Response(original=response)
-        if status_code in (200, 201, 202, 204, 206):
-            return r
-        elif status_code == 400:
-            raise exceptions.BadRequest(r.data)
-        elif status_code == 401:
-            raise exceptions.Unauthorized(r.data)
-        elif status_code == 403:
-            raise exceptions.Forbidden(r.data)
-        elif status_code == 404:
-            raise exceptions.NotFound(r.data)
-        elif status_code == 405:
-            raise exceptions.MethodNotAllowed(r.data)
-        elif status_code == 406:
-            raise exceptions.NotAcceptable(r.data)
-        elif status_code == 409:
-            raise exceptions.Conflict(r.data)
-        elif status_code == 410:
-            raise exceptions.Gone(r.data)
-        elif status_code == 411:
-            raise exceptions.LengthRequired(r.data)
-        elif status_code == 412:
-            raise exceptions.PreconditionFailed(r.data)
-        elif status_code == 413:
-            raise exceptions.RequestEntityTooLarge(r.data)
-        elif status_code == 415:
-            raise exceptions.UnsupportedMediaType(r.data)
-        elif status_code == 416:
-            raise exceptions.RequestedRangeNotSatisfiable(r.data)
-        elif status_code == 422:
-            raise exceptions.UnprocessableEntity(r.data)
-        elif status_code == 429:
-            raise exceptions.TooManyRequests(r.data)
-        elif status_code == 500:
-            raise exceptions.InternalServerError(r.data)
-        elif status_code == 501:
-            raise exceptions.NotImplemented(r.data)
-        elif status_code == 503:
-            raise exceptions.ServiceUnavailable(r.data)
-        elif status_code == 504:
-            raise exceptions.GatewayTimeout(r.data)
-        elif status_code == 507:
-            raise exceptions.InsufficientStorage(r.data)
-        elif status_code == 509:
-            raise exceptions.BandwidthLimitExceeded(r.data)
-        else:
-            if r["error"]["innerError"]["code"] == "lockMismatch":
-                # File is currently locked due to being open in the web browser
-                # while attempting to reupload a new version to the drive.
-                # Thus temporarily unavailable.
-                raise exceptions.ServiceUnavailable(r.data)
-            raise exceptions.UnknownError(r.data)
+from typing import Optional
+from urllib.parse import urlencode
+
+import requests
+
+from microsoftgraph import exceptions
+from microsoftgraph.calendar import Calendar
+from microsoftgraph.contacts import Contacts
+from microsoftgraph.files import Files
+from microsoftgraph.mail import Mail
+from microsoftgraph.notes import Notes
+from microsoftgraph.response import Response
+from microsoftgraph.users import Users
+from microsoftgraph.webhooks import Webhooks
+from microsoftgraph.workbooks import Workbooks
+
+
+class Client(object):
+    AUTHORITY_URL = "https://login.microsoftonline.com/"
+    AUTH_ENDPOINT = "/oauth2/v2.0/authorize?"
+    TOKEN_ENDPOINT = "/oauth2/v2.0/token"
+    RESOURCE = "https://graph.microsoft.com/"
+
+    def __init__(
+        self,
+        client_id: str,
+        client_secret: str,
+        api_version: str = "v1.0",
+        account_type: str = "common",
+        requests_hooks: dict = None,
+        paginate: bool = True,
+    ) -> None:
+        """Instantiates library.
+
+        Args:
+            client_id (str): Application client id.
+            client_secret (str): Application client secret.
+            api_version (str, optional): v1.0 or beta. Defaults to "v1.0".
+            account_type (str, optional): common, organizations or consumers. Defaults to "common".
+            requests_hooks (dict, optional): Requests library event hooks. Defaults to None.
+
+        Raises:
+            Exception: requests_hooks is not a dict.
+        """
+        self.client_id = client_id
+        self.client_secret = client_secret
+        self.api_version = api_version
+        self.account_type = account_type
+
+        self.base_url = self.RESOURCE + self.api_version + "/"
+        self.token = None
+        self.workbook_session_id = None
+        self.paginate = paginate
+
+        self.calendar = Calendar(self)
+        self.contacts = Contacts(self)
+        self.files = Files(self)
+        self.mail = Mail(self)
+        self.notes = Notes(self)
+        self.users = Users(self)
+        self.webhooks = Webhooks(self)
+        self.workbooks = Workbooks(self)
+
+        if requests_hooks and not isinstance(requests_hooks, dict):
+            raise Exception(
+                'requests_hooks must be a dict. e.g. {"response": func}. http://docs.python-requests.org/en/master/user/advanced/#event-hooks'
+            )
+        self.requests_hooks = requests_hooks
+
+    def authorization_url(self, redirect_uri: str, scope: list, state: str = None) -> str:
+        """Generates an Authorization URL.
+
+        The first step to getting an access token for many OpenID Connect (OIDC) and OAuth 2.0 flows is to redirect the
+        user to the Microsoft identity platform /authorize endpoint. Azure AD will sign the user in and ensure their
+        consent for the permissions your app requests. In the authorization code grant flow, after consent is obtained,
+        Azure AD will return an authorization_code to your app that it can redeem at the Microsoft identity platform
+        /token endpoint for an access token.
+
+        https://docs.microsoft.com/en-us/graph/auth-v2-user#2-get-authorization
+
+        Args:
+            redirect_uri (str): The redirect_uri of your app, where authentication responses can be sent and received by
+            your app. It must exactly match one of the redirect_uris you registered in the app registration portal.
+            scope (list): A list of the Microsoft Graph permissions that you want the user to consent to. This may also
+            include OpenID scopes.
+            state (str, optional): A value included in the request that will also be returned in the token response.
+            It can be a string of any content that you wish.  A randomly generated unique value is typically
+            used for preventing cross-site request forgery attacks.  The state is also used to encode information
+            about the user's state in the app before the authentication request occurred, such as the page or view
+            they were on. Defaults to None.
+
+        Returns:
+            str: Url for OAuth 2.0.
+        """
+        params = {
+            "client_id": self.client_id,
+            "redirect_uri": redirect_uri,
+            "scope": " ".join(scope),
+            "response_type": "code",
+            "response_mode": "query",
+        }
+
+        if state:
+            params["state"] = state
+        response = self.AUTHORITY_URL + self.account_type + self.AUTH_ENDPOINT + urlencode(params)
+        return response
+
+    def exchange_code(self, redirect_uri: str, code: str) -> Response:
+        """Exchanges an oauth code for an user token.
+
+        Your app uses the authorization code received in the previous step to request an access token by sending a POST
+        request to the /token endpoint.
+
+        https://docs.microsoft.com/en-us/graph/auth-v2-user#3-get-a-token
+
+        Args:
+            redirect_uri (str): The redirect_uri of your app, where authentication responses can be sent and received by
+            your app.  It must exactly match one of the redirect_uris you registered in the app registration portal.
+            code (str): The authorization_code that you acquired in the first leg of the flow.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        data = {
+            "client_id": self.client_id,
+            "redirect_uri": redirect_uri,
+            "client_secret": self.client_secret,
+            "code": code,
+            "grant_type": "authorization_code",
+        }
+        response = requests.post(self.AUTHORITY_URL + self.account_type + self.TOKEN_ENDPOINT, data=data)
+        return self._parse(response)
+
+    def refresh_token(self, redirect_uri: str, refresh_token: str) -> Response:
+        """Exchanges a refresh token for an user token.
+
+        Access tokens are short lived, and you must refresh them after they expire to continue accessing resources.
+        You can do so by submitting another POST request to the /token endpoint, this time providing the refresh_token
+        instead of the code.
+
+        https://docs.microsoft.com/en-us/graph/auth-v2-user#5-use-the-refresh-token-to-get-a-new-access-token
+
+        Args:
+            redirect_uri (str): The redirect_uri of your app, where authentication responses can be sent and received by
+            your app.  It must exactly match one of the redirect_uris you registered in the app registration portal.
+            refresh_token (str): An OAuth 2.0 refresh token. Your app can use this token acquire additional access tokens
+            after the current access token expires. Refresh tokens are long-lived, and can be used to retain access
+            to resources for extended periods of time.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        data = {
+            "client_id": self.client_id,
+            "redirect_uri": redirect_uri,
+            "client_secret": self.client_secret,
+            "refresh_token": refresh_token,
+            "grant_type": "refresh_token",
+        }
+        response = requests.post(self.AUTHORITY_URL + self.account_type + self.TOKEN_ENDPOINT, data=data)
+        return self._parse(response)
+
+    def set_token(self, token: dict) -> None:
+        """Sets the User token for its use in this library.
+
+        Args:
+            token (dict): User token data.
+        """
+        self.token = token
+
+    def set_workbook_session_id(self, workbook_session_id: dict) -> None:
+        """Sets the Workbook Session Id token for its use in this library.
+
+        Args:
+            token (dict): Workbook Session ID.
+        """
+        self.workbook_session_id = workbook_session_id
+
+    def get_next(self, response: Response) -> Optional[Response]:
+        """Retrieves the next page for the argument response if any. This allows to perform a loop in case you
+        want to paginate the response yourself.
+
+        Args:
+            response (Response): Graph API Response.
+
+        Returns:
+            Optional[Response]: Graph API Response if available, None otherwise
+        """
+        if not isinstance(response.data, dict):
+            return None
+
+        if "@odata.nextLink" not in response.data:
+            return None
+
+        return self._do_get(response.data["@odata.nextLink"])
+
+    def _paginate_response(self, response: Response) -> Response:
+        """Some queries against Microsoft Graph return multiple pages of data either due to server-side paging or due to
+        the use of the $top query parameter to specifically limit the page size in a request. When a result set spans
+        multiple pages, Microsoft Graph returns an @odata.nextLink property in the response that contains a URL to the
+        next page of results.
+
+        https://docs.microsoft.com/en-us/graph/paging?context=graph%2Fapi%2F1.0&view=graph-rest-1.0
+
+        Args:
+            response (Response): Graph API Response.
+
+        Returns:
+            Response: Graph API Response.
+        """
+        if not isinstance(response.data, dict) or "value" not in response.data:
+            return response
+
+        # Copy data to avoid side effects
+        data = list(response.data["value"])
+
+        while "@odata.nextLink" in response.data:
+            response = self.get_next(response)
+            if isinstance(response.data, dict) and "value" in response.data:
+                data.extend(response.data["value"])
+
+        response.data["value"] = data
+        return response
+
+    def _get(self, url, **kwargs) -> Response:
+        response = self._do_get(url, **kwargs)
+        if self.paginate:
+            return self._paginate_response(response)
+
+        return response
+
+    def _do_get(self, url, **kwargs) -> Response:
+        return self._request("GET", url, **kwargs)
+
+    def _post(self, url, **kwargs):
+        return self._request("POST", url, **kwargs)
+
+    def _put(self, url, **kwargs):
+        return self._request("PUT", url, **kwargs)
+
+    def _patch(self, url, **kwargs):
+        return self._request("PATCH", url, **kwargs)
+
+    def _delete(self, url, **kwargs):
+        return self._request("DELETE", url, **kwargs)
+
+    def _request(self, method, url, headers=None, **kwargs) -> Response:
+        _headers = {
+            "Accept": "application/json",
+        }
+
+        if headers:
+            _headers.update(headers)
+
+        if headers in ("JWT_REQUIRED"):
+            _headers["Authorization"] = "JWT " + self.token["access_token"]
+
+        _headers["Authorization"] = "Bearer " + self.token["access_token"]
+
+        if self.requests_hooks:
+            kwargs.update({"hooks": self.requests_hooks})
+        if "Content-Type" not in _headers:
+            _headers["Content-Type"] = "application/json"
+        return self._parse(requests.request(method, url, headers=_headers, **kwargs))
+
+    def _parse(self, response) -> Response:
+        status_code = response.status_code
+        r = Response(original=response)
+        if status_code < 299:
+            return r
+        elif status_code == 400:
+            raise exceptions.BadRequest(r.data)
+        elif status_code == 401:
+            raise exceptions.Unauthorized(r.data)
+        elif status_code == 403:
+            raise exceptions.Forbidden(r.data)
+        elif status_code == 404:
+            raise exceptions.NotFound(r.data)
+        elif status_code == 405:
+            raise exceptions.MethodNotAllowed(r.data)
+        elif status_code == 406:
+            raise exceptions.NotAcceptable(r.data)
+        elif status_code == 409:
+            raise exceptions.Conflict(r.data)
+        elif status_code == 410:
+            raise exceptions.Gone(r.data)
+        elif status_code == 411:
+            raise exceptions.LengthRequired(r.data)
+        elif status_code == 412:
+            raise exceptions.PreconditionFailed(r.data)
+        elif status_code == 413:
+            raise exceptions.RequestEntityTooLarge(r.data)
+        elif status_code == 415:
+            raise exceptions.UnsupportedMediaType(r.data)
+        elif status_code == 416:
+            raise exceptions.RequestedRangeNotSatisfiable(r.data)
+        elif status_code == 422:
+            raise exceptions.UnprocessableEntity(r.data)
+        elif status_code == 429:
+            raise exceptions.TooManyRequests(r.data)
+        elif status_code == 500:
+            raise exceptions.InternalServerError(r.data)
+        elif status_code == 501:
+            raise exceptions.NotImplemented(r.data)
+        elif status_code == 503:
+            raise exceptions.ServiceUnavailable(r.data)
+        elif status_code == 504:
+            raise exceptions.GatewayTimeout(r.data)
+        elif status_code == 507:
+            raise exceptions.InsufficientStorage(r.data)
+        elif status_code == 509:
+            raise exceptions.BandwidthLimitExceeded(r.data)
+        else:
+            if r["error"]["innerError"]["code"] == "lockMismatch":
+                # File is currently locked due to being open in the web browser
+                # while attempting to reupload a new version to the drive.
+                # Thus temporarily unavailable.
+                raise exceptions.ServiceUnavailable(r.data)
+            raise exceptions.UnknownError(r.data)
```

### Comparing `microsoftgraph_python-1.1.6/microsoftgraph/contacts.py` & `microsoftgraph_python-1.1.7/microsoftgraph/contacts.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-from microsoftgraph.decorators import token_required
-from microsoftgraph.response import Response
-
-
-class Contacts(object):
-    def __init__(self, client) -> None:
-        """Working with Outlook Contacts.
-
-        https://docs.microsoft.com/en-us/graph/api/resources/contact?view=graph-rest-1.0
-
-        Args:
-            client (Client): Library Client.
-        """
-        self._client = client
-
-    @token_required
-    def get_contact(self, contact_id: str, params: dict = None) -> Response:
-        """Retrieve the properties and relationships of a contact object.
-
-        https://docs.microsoft.com/en-us/graph/api/contact-get?view=graph-rest-1.0&tabs=http
-
-        Args:
-            contact_id (str): The contact's unique identifier.
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        return self._client._get(self._client.base_url + "me/contacts/{}".format(contact_id), params=params)
-
-    @token_required
-    def list_contacts(self, folder_id: str = None, params: dict = None) -> Response:
-        """Get a contact collection from the default contacts folder of the signed-in user.
-
-        https://docs.microsoft.com/en-us/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=http
-
-        Args:
-            folder_id (str): Folder ID.
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        url = "me/contactfolders/{}/contacts".format(folder_id) if folder_id else "me/contacts"
-        return self._client._get(self._client.base_url + url, params=params)
-
-    @token_required
-    def create_contact(
-        self,
-        given_name: str,
-        surname: str,
-        email_addresses: list,
-        business_phones: list,
-        folder_id: str = None,
-        **kwargs
-    ) -> Response:
-        """Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.
-
-        https://docs.microsoft.com/en-us/graph/api/user-post-contacts?view=graph-rest-1.0&tabs=http
-
-        Args:
-            given_name (str): The contact's given name.
-            surname (str): The contact's surname.
-            email_addresses (list): The contact's email addresses.
-            business_phones (list): The contact's business phone numbers.
-            folder_id (str, optional): Unique identifier of the contact folder. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        if isinstance(email_addresses, str):
-            email_addresses = [{"address": email_addresses, "name": "{} {}".format(given_name, surname)}]
-
-        if isinstance(business_phones, str):
-            business_phones = [business_phones]
-
-        body = {
-            "givenName": given_name,
-            "surname": surname,
-            "emailAddresses": email_addresses,
-            "businessPhones": business_phones,
-        }
-        body.update(kwargs)
-        url = "me/contactFolders/{}/contacts".format(folder_id) if folder_id else "me/contacts"
-        return self._client._post(self._client.base_url + url, json=body)
-
-    @token_required
-    def list_contact_folders(self, params: dict = None) -> Response:
-        """Get the contact folder collection in the default Contacts folder of the signed-in user.
-
-        https://docs.microsoft.com/en-us/graph/api/user-list-contactfolders?view=graph-rest-1.0&tabs=http
-
-        Args:
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        return self._client._get(self._client.base_url + "me/contactFolders", params=params)
-
-    @token_required
-    def create_contact_folder(self, display_name: str, parent_folder_id: str, **kwargs) -> Response:
-        """Create a new contactFolder under the user's default contacts folder.
-
-        https://docs.microsoft.com/en-us/graph/api/user-post-contactfolders?view=graph-rest-1.0&tabs=http
-
-        Args:
-            display_name (str): The folder's display name.
-            parent_folder_id (str): The ID of the folder's parent folder.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        data = {"displayName": display_name, "parentFolderId": parent_folder_id}
-        data.update(kwargs)
-        return self._client._post(self._client.base_url + "me/contactFolders", json=data)
+from microsoftgraph.decorators import token_required
+from microsoftgraph.response import Response
+
+
+class Contacts(object):
+    def __init__(self, client) -> None:
+        """Working with Outlook Contacts.
+
+        https://docs.microsoft.com/en-us/graph/api/resources/contact?view=graph-rest-1.0
+
+        Args:
+            client (Client): Library Client.
+        """
+        self._client = client
+
+    @token_required
+    def get_contact(self, contact_id: str, params: dict = None) -> Response:
+        """Retrieve the properties and relationships of a contact object.
+
+        https://docs.microsoft.com/en-us/graph/api/contact-get?view=graph-rest-1.0&tabs=http
+
+        Args:
+            contact_id (str): The contact's unique identifier.
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        return self._client._get(self._client.base_url + "me/contacts/{}".format(contact_id), params=params)
+
+    @token_required
+    def list_contacts(self, folder_id: str = None, params: dict = None) -> Response:
+        """Get a contact collection from the default contacts folder of the signed-in user.
+
+        https://docs.microsoft.com/en-us/graph/api/user-list-contacts?view=graph-rest-1.0&tabs=http
+
+        Args:
+            folder_id (str): Folder ID.
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        url = "me/contactfolders/{}/contacts".format(folder_id) if folder_id else "me/contacts"
+        return self._client._get(self._client.base_url + url, params=params)
+
+    @token_required
+    def create_contact(
+        self,
+        given_name: str,
+        surname: str,
+        email_addresses: list,
+        business_phones: list,
+        folder_id: str = None,
+        **kwargs
+    ) -> Response:
+        """Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.
+
+        https://docs.microsoft.com/en-us/graph/api/user-post-contacts?view=graph-rest-1.0&tabs=http
+
+        Args:
+            given_name (str): The contact's given name.
+            surname (str): The contact's surname.
+            email_addresses (list): The contact's email addresses.
+            business_phones (list): The contact's business phone numbers.
+            folder_id (str, optional): Unique identifier of the contact folder. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        if isinstance(email_addresses, str):
+            email_addresses = [{"address": email_addresses, "name": "{} {}".format(given_name, surname)}]
+
+        if isinstance(business_phones, str):
+            business_phones = [business_phones]
+
+        body = {
+            "givenName": given_name,
+            "surname": surname,
+            "emailAddresses": email_addresses,
+            "businessPhones": business_phones,
+        }
+        body.update(kwargs)
+        url = "me/contactFolders/{}/contacts".format(folder_id) if folder_id else "me/contacts"
+        return self._client._post(self._client.base_url + url, json=body)
+
+    @token_required
+    def list_contact_folders(self, params: dict = None) -> Response:
+        """Get the contact folder collection in the default Contacts folder of the signed-in user.
+
+        https://docs.microsoft.com/en-us/graph/api/user-list-contactfolders?view=graph-rest-1.0&tabs=http
+
+        Args:
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        return self._client._get(self._client.base_url + "me/contactFolders", params=params)
+
+    @token_required
+    def create_contact_folder(self, display_name: str, parent_folder_id: str, **kwargs) -> Response:
+        """Create a new contactFolder under the user's default contacts folder.
+
+        https://docs.microsoft.com/en-us/graph/api/user-post-contactfolders?view=graph-rest-1.0&tabs=http
+
+        Args:
+            display_name (str): The folder's display name.
+            parent_folder_id (str): The ID of the folder's parent folder.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        data = {"displayName": display_name, "parentFolderId": parent_folder_id}
+        data.update(kwargs)
+        return self._client._post(self._client.base_url + "me/contactFolders", json=data)
```

### Comparing `microsoftgraph_python-1.1.6/microsoftgraph/decorators.py` & `microsoftgraph_python-1.1.7/microsoftgraph/decorators.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from microsoftgraph.exceptions import TokenRequired
-from functools import wraps
-
-
-def token_required(func):
-    @wraps(func)
-    def helper(*args, **kwargs):
-        module = args[0]
-        if not module._client.token:
-            raise TokenRequired("You must set the Token.")
-        return func(*args, **kwargs)
-
-    return helper
-
-
-def workbook_session_id_required(func):
-    @wraps(func)
-    def helper(*args, **kwargs):
-        module = args[0]
-        if not module._client.workbook_session_id:
-            raise TokenRequired("You must set the Workbook Session Id.")
-        return func(*args, **kwargs)
-
-    return helper
+from microsoftgraph.exceptions import TokenRequired
+from functools import wraps
+
+
+def token_required(func):
+    @wraps(func)
+    def helper(*args, **kwargs):
+        module = args[0]
+        if not module._client.token:
+            raise TokenRequired("You must set the Token.")
+        return func(*args, **kwargs)
+
+    return helper
+
+
+def workbook_session_id_required(func):
+    @wraps(func)
+    def helper(*args, **kwargs):
+        module = args[0]
+        if not module._client.workbook_session_id:
+            raise TokenRequired("You must set the Workbook Session Id.")
+        return func(*args, **kwargs)
+
+    return helper
```

### Comparing `microsoftgraph_python-1.1.6/microsoftgraph/exceptions.py` & `microsoftgraph_python-1.1.7/microsoftgraph/exceptions.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-class BaseError(Exception):
-    pass
-
-
-class UnknownError(BaseError):
-    pass
-
-
-class TokenRequired(BaseError):
-    pass
-
-
-class BadRequest(BaseError):
-    pass
-
-
-class Unauthorized(BaseError):
-    pass
-
-
-class Forbidden(BaseError):
-    pass
-
-
-class NotFound(BaseError):
-    pass
-
-
-class MethodNotAllowed(BaseError):
-    pass
-
-
-class NotAcceptable(BaseError):
-    pass
-
-
-class Conflict(BaseError):
-    pass
-
-
-class Gone(BaseError):
-    pass
-
-
-class LengthRequired(BaseError):
-    pass
-
-
-class PreconditionFailed(BaseError):
-    pass
-
-
-class RequestEntityTooLarge(BaseError):
-    pass
-
-
-class UnsupportedMediaType(BaseError):
-    pass
-
-
-class RequestedRangeNotSatisfiable(BaseError):
-    pass
-
-
-class UnprocessableEntity(BaseError):
-    pass
-
-
-class TooManyRequests(BaseError):
-    pass
-
-
-class InternalServerError(BaseError):
-    pass
-
-
-class NotImplemented(BaseError):
-    pass
-
-
-class ServiceUnavailable(BaseError):
-    pass
-
-
-class GatewayTimeout(BaseError):
-    pass
-
-
-class InsufficientStorage(BaseError):
-    pass
-
-
-class BandwidthLimitExceeded(BaseError):
-    pass
+class BaseError(Exception):
+    pass
+
+
+class UnknownError(BaseError):
+    pass
+
+
+class TokenRequired(BaseError):
+    pass
+
+
+class BadRequest(BaseError):
+    pass
+
+
+class Unauthorized(BaseError):
+    pass
+
+
+class Forbidden(BaseError):
+    pass
+
+
+class NotFound(BaseError):
+    pass
+
+
+class MethodNotAllowed(BaseError):
+    pass
+
+
+class NotAcceptable(BaseError):
+    pass
+
+
+class Conflict(BaseError):
+    pass
+
+
+class Gone(BaseError):
+    pass
+
+
+class LengthRequired(BaseError):
+    pass
+
+
+class PreconditionFailed(BaseError):
+    pass
+
+
+class RequestEntityTooLarge(BaseError):
+    pass
+
+
+class UnsupportedMediaType(BaseError):
+    pass
+
+
+class RequestedRangeNotSatisfiable(BaseError):
+    pass
+
+
+class UnprocessableEntity(BaseError):
+    pass
+
+
+class TooManyRequests(BaseError):
+    pass
+
+
+class InternalServerError(BaseError):
+    pass
+
+
+class NotImplemented(BaseError):
+    pass
+
+
+class ServiceUnavailable(BaseError):
+    pass
+
+
+class GatewayTimeout(BaseError):
+    pass
+
+
+class InsufficientStorage(BaseError):
+    pass
+
+
+class BandwidthLimitExceeded(BaseError):
+    pass
```

### Comparing `microsoftgraph_python-1.1.6/microsoftgraph/files.py` & `microsoftgraph_python-1.1.7/microsoftgraph/files.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-import base64
-
-import requests
-
-from microsoftgraph.decorators import token_required
-from microsoftgraph.response import Response
-
-
-class Files(object):
-    def __init__(self, client) -> None:
-        """Working with files in Microsoft Graph
-
-        https://docs.microsoft.com/en-us/graph/api/resources/onedrive?view=graph-rest-1.0
-
-        Args:
-            client (Client): Library Client.
-        """
-        self._client = client
-
-    @token_required
-    def drive_root_items(self, params: dict = None) -> Response:
-        """Return a collection of DriveItems in the children relationship of a DriveItem.
-
-        https://docs.microsoft.com/en-us/graph/api/driveitem-list-children?view=graph-rest-1.0&tabs=http
-
-        Args:
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        return self._client._get(self._client.base_url + "me/drive/root", params=params)
-
-    @token_required
-    def drive_root_children_items(self, params: dict = None) -> Response:
-        """Return a collection of DriveItems in the children relationship of a DriveItem.
-
-        https://docs.microsoft.com/en-us/graph/api/driveitem-list-children?view=graph-rest-1.0&tabs=http
-
-        Args:
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        return self._client._get(self._client.base_url + "me/drive/root/children", params=params)
-
-    @token_required
-    def drive_specific_folder(self, folder_id: str, params: dict = None) -> Response:
-        """Return a collection of DriveItems in the children relationship of a DriveItem.
-
-        https://docs.microsoft.com/en-us/graph/api/driveitem-list-children?view=graph-rest-1.0&tabs=http
-
-        Args:
-            folder_id (str): Unique identifier of the folder.
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        url = "me/drive/items/{}/children".format(folder_id)
-        return self._client._get(self._client.base_url + url, params=params)
-
-    @token_required
-    def drive_get_item(self, item_id: str, params: dict = None, **kwargs) -> Response:
-        """Retrieve the metadata for a driveItem in a drive by file system path or ID. It may also be the unique ID of a
-        SharePoint list item.
-
-        https://docs.microsoft.com/en-us/graph/api/driveitem-get?view=graph-rest-1.0&tabs=http
-
-        Args:
-            item_id (str): ID of a driveItem.
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        url = "me/drive/items/{}".format(item_id)
-        return self._client._get(self._client.base_url + url, params=params, **kwargs)
-
-    @token_required
-    def drive_download_contents(self, item_id: str, params: dict = None, **kwargs) -> Response:
-        """Download the contents of the primary stream (file) of a DriveItem. Only driveItems with the file property can
-        be downloaded.
-
-        https://docs.microsoft.com/en-us/graph/api/driveitem-get-content?view=graph-rest-1.0&tabs=http
-
-        Args:
-            item_id (str): ID of a driveItem.
-            params (dict, optional): Extra params. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        url = "me/drive/items/{}/content".format(item_id)
-        return self._client._get(self._client.base_url + url, params=params, **kwargs)
-
-    @token_required
-    def drive_download_shared_contents(self, share_id: str, params: dict = None, **kwargs) -> Response:
-        """Download the contents of the primary stream (file) of a DriveItem. Only driveItems with the file property can
-        be downloaded.
-
-        https://docs.microsoft.com/en-us/graph/api/driveitem-get-content?view=graph-rest-1.0&tabs=http
-
-        Args:
-            share_id (str): ID of a driveItem.
-            params (dict, optional): Extra params. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        base64_value = base64.b64encode(share_id.encode()).decode()
-        encoded_share_url = "u!" + base64_value.rstrip("=").replace("/", "_").replace("+", "-")
-        url = self._client.base_url + "shares/{}/driveItem".format(encoded_share_url)
-        drive_item = self._client._get(url)
-        file_download_url = drive_item["@microsoft.graph.downloadUrl"]
-        return drive_item["name"], requests.get(file_download_url).content
-
-    @token_required
-    def drive_download_large_contents(self, downloadUrl: str, offset: int, size: int) -> Response:
-        """Download the contents of the primary stream (file) of a DriveItem. Only driveItems with the file property can
-        be downloaded.
-
-        https://docs.microsoft.com/en-us/graph/api/driveitem-get-content?view=graph-rest-1.0&tabs=http
-
-        Args:
-            downloadUrl (str): Url of the driveItem.
-            offset (int): offset.
-            size (int): size.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        headers = {"Range": f"bytes={offset}-{size + offset - 1}"}
-        return self._client._get(downloadUrl, headers=headers)
-
-    @token_required
-    def drive_upload_new_file(self, filename: str, file_path: str, params: dict = None, **kwargs) -> Response:
-        """The simple upload API allows you to provide the contents of a new file in a single API call. This method only
-        supports files up to 4MB in size.
-
-        https://docs.microsoft.com/en-us/graph/api/driveitem-put-content?view=graph-rest-1.0&tabs=http
-
-        Args:
-            filename (str): The name of the item (filename and extension).
-            file_path (str): File path to upload.
-            params (dict, optional): Extra params. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        kwargs["headers"] = {"Content-Type": "text/plain"}
-        content = open(file_path, "rb").read()
-        url = "me/drive/root:{}:/content".format(filename)
-        return self._client._put(self._client.base_url + url, params=params, data=content, **kwargs)
-
-    @token_required
-    def drive_update_existing_file(self, item_id: str, file_path: str, params: dict = None, **kwargs) -> Response:
-        """The simple upload API allows you to update the contents of an existing file in a single API call. This method
-        only supports files up to 4MB in size.
-
-        https://docs.microsoft.com/en-us/graph/api/driveitem-put-content?view=graph-rest-1.0&tabs=http
-
-        Args:
-            item_id (str): Id of a driveItem.
-            file_path (str): File path to upload.
-            params (dict, optional): Extra params. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        kwargs["headers"] = {"Content-Type": "text/plain"}
-        content = open(file_path, "rb").read()
-        url = "me/drive/items/{}/content".format(item_id)
-        return self._client._put(self._client.base_url + url, params=params, data=content, **kwargs)
-
-    @token_required
-    def search_items(self, q: str, params: dict = None, **kwargs) -> Response:
-        """Search the hierarchy of items for items matching a query. You can search within a folder hierarchy, a whole
-        drive, or files shared with the current user.
-
-        https://docs.microsoft.com/en-us/graph/api/driveitem-search?view=graph-rest-1.0&tabs=http
-
-        Args:
-            q (str): The query text used to search for items. Values may be matched across several fields including
-            filename, metadata, and file content.
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        url = "me/drive/root/search(q='{}')".format(q)
-        return self._client._get(self._client.base_url + url, params=params, **kwargs)
+import base64
+
+import requests
+
+from microsoftgraph.decorators import token_required
+from microsoftgraph.response import Response
+
+
+class Files(object):
+    def __init__(self, client) -> None:
+        """Working with files in Microsoft Graph
+
+        https://docs.microsoft.com/en-us/graph/api/resources/onedrive?view=graph-rest-1.0
+
+        Args:
+            client (Client): Library Client.
+        """
+        self._client = client
+
+    @token_required
+    def drive_root_items(self, params: dict = None) -> Response:
+        """Return a collection of DriveItems in the children relationship of a DriveItem.
+
+        https://docs.microsoft.com/en-us/graph/api/driveitem-list-children?view=graph-rest-1.0&tabs=http
+
+        Args:
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        return self._client._get(self._client.base_url + "me/drive/root", params=params)
+
+    @token_required
+    def drive_root_children_items(self, params: dict = None) -> Response:
+        """Return a collection of DriveItems in the children relationship of a DriveItem.
+
+        https://docs.microsoft.com/en-us/graph/api/driveitem-list-children?view=graph-rest-1.0&tabs=http
+
+        Args:
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        return self._client._get(self._client.base_url + "me/drive/root/children", params=params)
+
+    @token_required
+    def drive_specific_folder(self, folder_id: str, params: dict = None) -> Response:
+        """Return a collection of DriveItems in the children relationship of a DriveItem.
+
+        https://docs.microsoft.com/en-us/graph/api/driveitem-list-children?view=graph-rest-1.0&tabs=http
+
+        Args:
+            folder_id (str): Unique identifier of the folder.
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        url = "me/drive/items/{}/children".format(folder_id)
+        return self._client._get(self._client.base_url + url, params=params)
+
+    @token_required
+    def drive_get_item(self, item_id: str, params: dict = None, **kwargs) -> Response:
+        """Retrieve the metadata for a driveItem in a drive by file system path or ID. It may also be the unique ID of a
+        SharePoint list item.
+
+        https://docs.microsoft.com/en-us/graph/api/driveitem-get?view=graph-rest-1.0&tabs=http
+
+        Args:
+            item_id (str): ID of a driveItem.
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        url = "me/drive/items/{}".format(item_id)
+        return self._client._get(self._client.base_url + url, params=params, **kwargs)
+
+    @token_required
+    def drive_download_contents(self, item_id: str, params: dict = None, **kwargs) -> Response:
+        """Download the contents of the primary stream (file) of a DriveItem. Only driveItems with the file property can
+        be downloaded.
+
+        https://docs.microsoft.com/en-us/graph/api/driveitem-get-content?view=graph-rest-1.0&tabs=http
+
+        Args:
+            item_id (str): ID of a driveItem.
+            params (dict, optional): Extra params. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        url = "me/drive/items/{}/content".format(item_id)
+        return self._client._get(self._client.base_url + url, params=params, **kwargs)
+
+    @token_required
+    def drive_download_shared_contents(self, share_id: str, params: dict = None, **kwargs) -> Response:
+        """Download the contents of the primary stream (file) of a DriveItem. Only driveItems with the file property can
+        be downloaded.
+
+        https://docs.microsoft.com/en-us/graph/api/driveitem-get-content?view=graph-rest-1.0&tabs=http
+
+        Args:
+            share_id (str): ID of a driveItem.
+            params (dict, optional): Extra params. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        base64_value = base64.b64encode(share_id.encode()).decode()
+        encoded_share_url = "u!" + base64_value.rstrip("=").replace("/", "_").replace("+", "-")
+        url = self._client.base_url + "shares/{}/driveItem".format(encoded_share_url)
+        drive_item = self._client._get(url)
+        file_download_url = drive_item["@microsoft.graph.downloadUrl"]
+        return drive_item["name"], requests.get(file_download_url).content
+
+    @token_required
+    def drive_download_large_contents(self, downloadUrl: str, offset: int, size: int) -> Response:
+        """Download the contents of the primary stream (file) of a DriveItem. Only driveItems with the file property can
+        be downloaded.
+
+        https://docs.microsoft.com/en-us/graph/api/driveitem-get-content?view=graph-rest-1.0&tabs=http
+
+        Args:
+            downloadUrl (str): Url of the driveItem.
+            offset (int): offset.
+            size (int): size.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        headers = {"Range": f"bytes={offset}-{size + offset - 1}"}
+        return self._client._get(downloadUrl, headers=headers)
+
+    @token_required
+    def drive_upload_new_file(self, filename: str, file_path: str, params: dict = None, **kwargs) -> Response:
+        """The simple upload API allows you to provide the contents of a new file in a single API call. This method only
+        supports files up to 4MB in size.
+
+        https://docs.microsoft.com/en-us/graph/api/driveitem-put-content?view=graph-rest-1.0&tabs=http
+
+        Args:
+            filename (str): The name of the item (filename and extension).
+            file_path (str): File path to upload.
+            params (dict, optional): Extra params. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        kwargs["headers"] = {"Content-Type": "text/plain"}
+        content = open(file_path, "rb").read()
+        url = "me/drive/root:{}:/content".format(filename)
+        return self._client._put(self._client.base_url + url, params=params, data=content, **kwargs)
+
+    @token_required
+    def drive_update_existing_file(self, item_id: str, file_path: str, params: dict = None, **kwargs) -> Response:
+        """The simple upload API allows you to update the contents of an existing file in a single API call. This method
+        only supports files up to 4MB in size.
+
+        https://docs.microsoft.com/en-us/graph/api/driveitem-put-content?view=graph-rest-1.0&tabs=http
+
+        Args:
+            item_id (str): Id of a driveItem.
+            file_path (str): File path to upload.
+            params (dict, optional): Extra params. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        kwargs["headers"] = {"Content-Type": "text/plain"}
+        content = open(file_path, "rb").read()
+        url = "me/drive/items/{}/content".format(item_id)
+        return self._client._put(self._client.base_url + url, params=params, data=content, **kwargs)
+
+    @token_required
+    def search_items(self, q: str, params: dict = None, **kwargs) -> Response:
+        """Search the hierarchy of items for items matching a query. You can search within a folder hierarchy, a whole
+        drive, or files shared with the current user.
+
+        https://docs.microsoft.com/en-us/graph/api/driveitem-search?view=graph-rest-1.0&tabs=http
+
+        Args:
+            q (str): The query text used to search for items. Values may be matched across several fields including
+            filename, metadata, and file content.
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        url = "me/drive/root/search(q='{}')".format(q)
+        return self._client._get(self._client.base_url + url, params=params, **kwargs)
```

### Comparing `microsoftgraph_python-1.1.6/microsoftgraph/mail.py` & `microsoftgraph_python-1.1.7/microsoftgraph/mail.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-import base64
-import mimetypes
-
-from microsoftgraph.decorators import token_required
-from microsoftgraph.response import Response
-
-
-class Mail(object):
-    def __init__(self, client) -> None:
-        """Use the Outlook mail REST API
-
-        https://docs.microsoft.com/en-us/graph/api/resources/mail-api-overview?view=graph-rest-1.0
-
-        Args:
-            client (Client): Library Client.
-        """
-        self._client = client
-
-    @token_required
-    def list_messages(self, folder_id: str = None, params: dict = None) -> Response:
-        """Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).
-
-        https://docs.microsoft.com/en-us/graph/api/user-list-messages?view=graph-rest-1.0&tabs=http
-
-        Args:
-            folder_id (str, optional): Mail Folder ID.
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        url = "me/mailFolders/{}/messages".format(folder_id) if folder_id else "me/messages"
-        return self._client._get(self._client.base_url + url, params=params)
-
-    @token_required
-    def get_message(self, message_id: str, params: dict = None) -> Response:
-        """Retrieve the properties and relationships of a message object.
-
-        https://docs.microsoft.com/en-us/graph/api/message-get?view=graph-rest-1.0&tabs=http
-
-        Args:
-            message_id (str): Unique identifier for the message.
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        return self._client._get(self._client.base_url + "me/messages/" + message_id, params=params)
-
-    @token_required
-    def send_mail(
-        self,
-        subject: str,
-        content: str,
-        to_recipients: list,
-        cc_recipients: list = None,
-        content_type: str = "HTML",
-        attachments: list = None,
-        save_to_sent_items: bool = True,
-        **kwargs,
-    ) -> Response:
-        """Send the message specified in the request body using either JSON or MIME format.
-
-        https://docs.microsoft.com/en-us/graph/api/user-sendmail?view=graph-rest-1.0&tabs=http
-
-        Args:
-            subject (str): The subject of the message.
-            content (str): The body of the message.
-            to_recipients (list, optional): The To: recipients for the message.
-            cc_recipients (list, optional): The Cc: recipients for the message. Defaults to None.
-            content_type (str, optional): It can be in HTML or text format. Defaults to "HTML".
-            attachments (list, optional): The fileAttachment and itemAttachment attachments for the message. Defaults to None.
-            save_to_sent_items (bool, optional): Indicates whether to save the message in Sent Items. Defaults to True.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        # Create recipient list in required format.
-        if isinstance(to_recipients, list):
-            if all([isinstance(e, str) for e in to_recipients]):
-                to_recipients = [{"EmailAddress": {"Address": address}} for address in to_recipients]
-        elif isinstance(to_recipients, str):
-            to_recipients = [{"EmailAddress": {"Address": to_recipients}}]
-        else:
-            raise Exception("to_recipients value is invalid.")
-
-        if cc_recipients and isinstance(cc_recipients, list):
-            if all([isinstance(e, str) for e in cc_recipients]):
-                cc_recipients = [{"EmailAddress": {"Address": address}} for address in cc_recipients]
-        elif cc_recipients and isinstance(cc_recipients, str):
-            cc_recipients = [{"EmailAddress": {"Address": cc_recipients}}]
-        else:
-            cc_recipients = []
-
-        # Create list of attachments in required format.
-        attached_files = []
-        if attachments:
-            for filename in attachments:
-                b64_content = base64.b64encode(open(filename, "rb").read())
-                mime_type = mimetypes.guess_type(filename)[0]
-                mime_type = mime_type if mime_type else ""
-                attached_files.append(
-                    {
-                        "@odata.type": "#microsoft.graph.fileAttachment",
-                        "ContentBytes": b64_content.decode("utf-8"),
-                        "ContentType": mime_type,
-                        "Name": filename,
-                    }
-                )
-
-        # Create email message in required format.
-        email_msg = {
-            "Message": {
-                "Subject": subject,
-                "Body": {"ContentType": content_type, "Content": content},
-                "ToRecipients": to_recipients,
-                "ccRecipients": cc_recipients,
-                "Attachments": attached_files,
-            },
-            "SaveToSentItems": save_to_sent_items,
-        }
-        email_msg.update(kwargs)
-
-        # Do a POST to Graph's sendMail API and return the response.
-        return self._client._post(self._client.base_url + "me/sendMail", json=email_msg)
-
-    @token_required
-    def list_mail_folders(self, params: dict = None) -> Response:
-        """Get the mail folder collection directly under the root folder of the signed-in user. The returned collection
-        includes any mail search folders directly under the root.
-
-        By default, this operation does not return hidden folders. Use a query parameter includeHiddenFolders to include
-        them in the response.
-
-        https://docs.microsoft.com/en-us/graph/api/user-list-mailfolders?view=graph-rest-1.0&tabs=http
-
-        Args:
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        return self._client._get(self._client.base_url + "me/mailFolders", params=params)
-
-    @token_required
-    def create_mail_folder(self, display_name: str, is_hidden: bool = False) -> Response:
-        """Use this API to create a new mail folder in the root folder of the user's mailbox.
-
-        https://docs.microsoft.com/en-us/graph/api/user-post-mailfolders?view=graph-rest-1.0&tabs=http
-
-        Args:
-            display_name (str): Query.
-            is_hidden (bool, optional): Is the folder hidden. Defaults to False.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        data = {
-            "displayName": display_name,
-            "isHidden": is_hidden,
-        }
-        return self._client._post(self._client.base_url + "me/mailFolders", json=data)
+import base64
+import mimetypes
+
+from microsoftgraph.decorators import token_required
+from microsoftgraph.response import Response
+
+
+class Mail(object):
+    def __init__(self, client) -> None:
+        """Use the Outlook mail REST API
+
+        https://docs.microsoft.com/en-us/graph/api/resources/mail-api-overview?view=graph-rest-1.0
+
+        Args:
+            client (Client): Library Client.
+        """
+        self._client = client
+
+    @token_required
+    def list_messages(self, folder_id: str = None, params: dict = None) -> Response:
+        """Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).
+
+        https://docs.microsoft.com/en-us/graph/api/user-list-messages?view=graph-rest-1.0&tabs=http
+
+        Args:
+            folder_id (str, optional): Mail Folder ID.
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        url = "me/mailFolders/{}/messages".format(folder_id) if folder_id else "me/messages"
+        return self._client._get(self._client.base_url + url, params=params)
+
+    @token_required
+    def get_message(self, message_id: str, params: dict = None) -> Response:
+        """Retrieve the properties and relationships of a message object.
+
+        https://docs.microsoft.com/en-us/graph/api/message-get?view=graph-rest-1.0&tabs=http
+
+        Args:
+            message_id (str): Unique identifier for the message.
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        return self._client._get(self._client.base_url + "me/messages/" + message_id, params=params)
+
+    @token_required
+    def send_mail(
+        self,
+        subject: str,
+        content: str,
+        to_recipients: list,
+        cc_recipients: list = None,
+        content_type: str = "HTML",
+        attachments: list = None,
+        save_to_sent_items: bool = True,
+        **kwargs,
+    ) -> Response:
+        """Send the message specified in the request body using either JSON or MIME format.
+
+        https://docs.microsoft.com/en-us/graph/api/user-sendmail?view=graph-rest-1.0&tabs=http
+
+        Args:
+            subject (str): The subject of the message.
+            content (str): The body of the message.
+            to_recipients (list, optional): The To: recipients for the message.
+            cc_recipients (list, optional): The Cc: recipients for the message. Defaults to None.
+            content_type (str, optional): It can be in HTML or text format. Defaults to "HTML".
+            attachments (list, optional): The fileAttachment and itemAttachment attachments for the message. Defaults to None.
+            save_to_sent_items (bool, optional): Indicates whether to save the message in Sent Items. Defaults to True.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        # Create recipient list in required format.
+        if isinstance(to_recipients, list):
+            if all([isinstance(e, str) for e in to_recipients]):
+                to_recipients = [{"EmailAddress": {"Address": address}} for address in to_recipients]
+        elif isinstance(to_recipients, str):
+            to_recipients = [{"EmailAddress": {"Address": to_recipients}}]
+        else:
+            raise Exception("to_recipients value is invalid.")
+
+        if cc_recipients and isinstance(cc_recipients, list):
+            if all([isinstance(e, str) for e in cc_recipients]):
+                cc_recipients = [{"EmailAddress": {"Address": address}} for address in cc_recipients]
+        elif cc_recipients and isinstance(cc_recipients, str):
+            cc_recipients = [{"EmailAddress": {"Address": cc_recipients}}]
+        else:
+            cc_recipients = []
+
+        # Create list of attachments in required format.
+        attached_files = []
+        if attachments:
+            for filename in attachments:
+                b64_content = base64.b64encode(open(filename, "rb").read())
+                mime_type = mimetypes.guess_type(filename)[0]
+                mime_type = mime_type if mime_type else ""
+                attached_files.append(
+                    {
+                        "@odata.type": "#microsoft.graph.fileAttachment",
+                        "ContentBytes": b64_content.decode("utf-8"),
+                        "ContentType": mime_type,
+                        "Name": filename,
+                    }
+                )
+
+        # Create email message in required format.
+        email_msg = {
+            "Message": {
+                "Subject": subject,
+                "Body": {"ContentType": content_type, "Content": content},
+                "ToRecipients": to_recipients,
+                "ccRecipients": cc_recipients,
+                "Attachments": attached_files,
+            },
+            "SaveToSentItems": save_to_sent_items,
+        }
+        email_msg.update(kwargs)
+
+        # Do a POST to Graph's sendMail API and return the response.
+        return self._client._post(self._client.base_url + "me/sendMail", json=email_msg)
+
+    @token_required
+    def list_mail_folders(self, params: dict = None) -> Response:
+        """Get the mail folder collection directly under the root folder of the signed-in user. The returned collection
+        includes any mail search folders directly under the root.
+
+        By default, this operation does not return hidden folders. Use a query parameter includeHiddenFolders to include
+        them in the response.
+
+        https://docs.microsoft.com/en-us/graph/api/user-list-mailfolders?view=graph-rest-1.0&tabs=http
+
+        Args:
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        return self._client._get(self._client.base_url + "me/mailFolders", params=params)
+
+    @token_required
+    def create_mail_folder(self, display_name: str, is_hidden: bool = False) -> Response:
+        """Use this API to create a new mail folder in the root folder of the user's mailbox.
+
+        https://docs.microsoft.com/en-us/graph/api/user-post-mailfolders?view=graph-rest-1.0&tabs=http
+
+        Args:
+            display_name (str): Query.
+            is_hidden (bool, optional): Is the folder hidden. Defaults to False.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        data = {
+            "displayName": display_name,
+            "isHidden": is_hidden,
+        }
+        return self._client._post(self._client.base_url + "me/mailFolders", json=data)
```

### Comparing `microsoftgraph_python-1.1.6/microsoftgraph/notes.py` & `microsoftgraph_python-1.1.7/microsoftgraph/notes.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-from microsoftgraph.decorators import token_required
-from microsoftgraph.response import Response
-
-
-class Notes(object):
-    def __init__(self, client) -> None:
-        """Use the OneNote REST API.
-
-        https://docs.microsoft.com/en-us/graph/api/resources/onenote-api-overview?view=graph-rest-1.0
-
-        Args:
-            client (Client): Library Client.
-        """
-        self._client = client
-
-    @token_required
-    def list_notebooks(self, params: dict = None) -> Response:
-        """Retrieve a list of notebook objects.
-
-        https://docs.microsoft.com/en-us/graph/api/onenote-list-notebooks?view=graph-rest-1.0&tabs=http
-
-        Args:
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        return self._client._get(self._client.base_url + "me/onenote/notebooks", params=params)
-
-    @token_required
-    def get_notebook(self, notebook_id: str, params: dict = None) -> Response:
-        """Retrieve the properties and relationships of a notebook object.
-
-        https://docs.microsoft.com/en-us/graph/api/notebook-get?view=graph-rest-1.0&tabs=http
-
-        Args:
-            notebook_id (str): The unique identifier of the notebook.
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        return self._client._get(self._client.base_url + "me/onenote/notebooks/" + notebook_id, params=params)
-
-    @token_required
-    def list_sections(self, notebook_id: str, params: dict = None) -> Response:
-        """Retrieve a list of onenoteSection objects from the specified notebook.
-
-        https://docs.microsoft.com/en-us/graph/api/notebook-list-sections?view=graph-rest-1.0&tabs=http
-
-        Args:
-            notebook_id (str): The unique identifier of the notebook.
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        url = "me/onenote/notebooks/{}/sections".format(notebook_id)
-        return self._client._get(self._client.base_url + url, params=params)
-
-    @token_required
-    def list_pages(self, params: dict = None) -> Response:
-        """Retrieve a list of page objects.
-
-        Args:
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        return self._client._get(self._client.base_url + "me/onenote/pages", params=params)
-
-    @token_required
-    def create_page(self, section_id: str, files: list) -> Response:
-        """Create a new page in the specified section.
-
-        https://docs.microsoft.com/en-us/graph/api/section-post-pages?view=graph-rest-1.0
-
-        Args:
-            section_id (str): The unique identifier of the section.
-            files (list): Attachments.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        url = "me/onenote/sections/{}/pages".format(section_id)
-        return self._client._post(self._client.base_url + url, files=files)
+from microsoftgraph.decorators import token_required
+from microsoftgraph.response import Response
+
+
+class Notes(object):
+    def __init__(self, client) -> None:
+        """Use the OneNote REST API.
+
+        https://docs.microsoft.com/en-us/graph/api/resources/onenote-api-overview?view=graph-rest-1.0
+
+        Args:
+            client (Client): Library Client.
+        """
+        self._client = client
+
+    @token_required
+    def list_notebooks(self, params: dict = None) -> Response:
+        """Retrieve a list of notebook objects.
+
+        https://docs.microsoft.com/en-us/graph/api/onenote-list-notebooks?view=graph-rest-1.0&tabs=http
+
+        Args:
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        return self._client._get(self._client.base_url + "me/onenote/notebooks", params=params)
+
+    @token_required
+    def get_notebook(self, notebook_id: str, params: dict = None) -> Response:
+        """Retrieve the properties and relationships of a notebook object.
+
+        https://docs.microsoft.com/en-us/graph/api/notebook-get?view=graph-rest-1.0&tabs=http
+
+        Args:
+            notebook_id (str): The unique identifier of the notebook.
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        return self._client._get(self._client.base_url + "me/onenote/notebooks/" + notebook_id, params=params)
+
+    @token_required
+    def list_sections(self, notebook_id: str, params: dict = None) -> Response:
+        """Retrieve a list of onenoteSection objects from the specified notebook.
+
+        https://docs.microsoft.com/en-us/graph/api/notebook-list-sections?view=graph-rest-1.0&tabs=http
+
+        Args:
+            notebook_id (str): The unique identifier of the notebook.
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        url = "me/onenote/notebooks/{}/sections".format(notebook_id)
+        return self._client._get(self._client.base_url + url, params=params)
+
+    @token_required
+    def list_pages(self, params: dict = None) -> Response:
+        """Retrieve a list of page objects.
+
+        Args:
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        return self._client._get(self._client.base_url + "me/onenote/pages", params=params)
+
+    @token_required
+    def create_page(self, section_id: str, files: list) -> Response:
+        """Create a new page in the specified section.
+
+        https://docs.microsoft.com/en-us/graph/api/section-post-pages?view=graph-rest-1.0
+
+        Args:
+            section_id (str): The unique identifier of the section.
+            files (list): Attachments.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        url = "me/onenote/sections/{}/pages".format(section_id)
+        return self._client._post(self._client.base_url + url, files=files)
```

### Comparing `microsoftgraph_python-1.1.6/microsoftgraph/response.py` & `microsoftgraph_python-1.1.7/microsoftgraph/response.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from datetime import datetime, timedelta
-
-
-class Response:
-    def __init__(self, original) -> None:
-        self.original = original
-
-        if "application/json" in self.original.headers.get("Content-Type", ""):
-            self.data = self.original.json()
-        else:
-            self.data = self.original.content
-
-    def __repr__(self) -> str:
-        return "<Response [{}]>".format(self.status_code)
-
-    @property
-    def status_code(self):
-        return self.original.status_code
-
-    @property
-    def throttling(self) -> datetime:
-        """Microsoft Graph throttling
-
-        https://docs.microsoft.com/en-us/graph/throttling
-
-        Returns:
-            datetime: Retry after.
-        """
-        if "Retry-After" in self.original.headers:
-            return datetime.now() + timedelta(seconds=self.original.headers["Retry-After"])
-        return None
+from datetime import datetime, timedelta
+
+
+class Response:
+    def __init__(self, original) -> None:
+        self.original = original
+
+        if "application/json" in self.original.headers.get("Content-Type", ""):
+            self.data = self.original.json()
+        else:
+            self.data = self.original.content
+
+    def __repr__(self) -> str:
+        return "<Response [{}]>".format(self.status_code)
+
+    @property
+    def status_code(self):
+        return self.original.status_code
+
+    @property
+    def throttling(self) -> datetime:
+        """Microsoft Graph throttling
+
+        https://docs.microsoft.com/en-us/graph/throttling
+
+        Returns:
+            datetime: Retry after.
+        """
+        if "Retry-After" in self.original.headers:
+            return datetime.now() + timedelta(seconds=self.original.headers["Retry-After"])
+        return None
```

### Comparing `microsoftgraph_python-1.1.6/microsoftgraph/users.py` & `microsoftgraph_python-1.1.7/microsoftgraph/users.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from microsoftgraph.decorators import token_required
-from microsoftgraph.response import Response
-
-
-class Users(object):
-    def __init__(self, client) -> None:
-        """Working with users in Microsoft Graph.
-
-        https://docs.microsoft.com/en-us/graph/api/resources/users?view=graph-rest-1.0
-
-        Args:
-            client (Client): Library Client.
-        """
-        self._client = client
-
-    @token_required
-    def get_me(self, params: dict = None) -> Response:
-        """Retrieve the properties and relationships of user object.
-
-        Note: Getting a user returns a default set of properties only (businessPhones, displayName, givenName, id,
-        jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName).
-        Use $select to get the other properties and relationships for the user object.
-
-        https://docs.microsoft.com/en-us/graph/api/user-get?view=graph-rest-1.0&tabs=http
-
-        Args:
-            params (dict, optional): Query. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        return self._client._get(self._client.base_url + "me", params=params)
+from microsoftgraph.decorators import token_required
+from microsoftgraph.response import Response
+
+
+class Users(object):
+    def __init__(self, client) -> None:
+        """Working with users in Microsoft Graph.
+
+        https://docs.microsoft.com/en-us/graph/api/resources/users?view=graph-rest-1.0
+
+        Args:
+            client (Client): Library Client.
+        """
+        self._client = client
+
+    @token_required
+    def get_me(self, params: dict = None) -> Response:
+        """Retrieve the properties and relationships of user object.
+
+        Note: Getting a user returns a default set of properties only (businessPhones, displayName, givenName, id,
+        jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName).
+        Use $select to get the other properties and relationships for the user object.
+
+        https://docs.microsoft.com/en-us/graph/api/user-get?view=graph-rest-1.0&tabs=http
+
+        Args:
+            params (dict, optional): Query. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        return self._client._get(self._client.base_url + "me", params=params)
```

### Comparing `microsoftgraph_python-1.1.6/microsoftgraph/webhooks.py` & `microsoftgraph_python-1.1.7/microsoftgraph/webhooks.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-from datetime import datetime
-
-from microsoftgraph.decorators import token_required
-from microsoftgraph.response import Response
-from microsoftgraph.utils import format_time
-
-
-class Webhooks(object):
-    def __init__(self, client) -> None:
-        """Set up notifications for changes in user data.
-
-        https://docs.microsoft.com/en-us/graph/webhooks?view=graph-rest-1.0
-
-        Args:
-            client (Client): Library Client.
-        """
-        self._client = client
-
-    @token_required
-    def create_subscription(
-        self,
-        change_type: str,
-        notification_url: str,
-        resource: str,
-        expiration_datetime: datetime,
-        client_state: str = None,
-        **kwargs,
-    ) -> Response:
-        """Creates a subscription to start receiving notifications for a resource.
-
-        https://docs.microsoft.com/en-us/graph/webhooks#creating-a-subscription
-
-        Args:
-            change_type (str): The event type that caused the notification. For example, created on mail receive, or
-            updated on marking a message read.
-            notification_url (str): Url to receive notifications.
-            resource (str): The URI of the resource relative to https://graph.microsoft.com.
-            expiration_datetime (datetime): The expiration time for the subscription.
-            client_state (str, optional): The clientState property specified in the subscription request. Defaults to None.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        if isinstance(expiration_datetime, datetime):
-            expiration_datetime = format_time(expiration_datetime, is_webhook=True)
-
-        data = {
-            "changeType": change_type,
-            "notificationUrl": notification_url,
-            "resource": resource,
-            "expirationDateTime": expiration_datetime,
-            "clientState": client_state,
-        }
-        data.update(kwargs)
-        return self._client._post(self._client.base_url + "subscriptions", json=data)
-
-    @token_required
-    def renew_subscription(self, subscription_id: str, expiration_datetime: datetime) -> Response:
-        """Renews a subscription to keep receiving notifications for a resource.
-
-        https://docs.microsoft.com/en-us/graph/webhooks#renewing-a-subscription
-
-        Args:
-            subscription_id (str): Subscription ID.
-            expiration_datetime (datetime): Expiration date.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        if isinstance(expiration_datetime, datetime):
-            expiration_datetime = format_time(expiration_datetime, is_webhook=True)
-
-        data = {"expirationDateTime": expiration_datetime}
-        return self._client._patch(self._client.base_url + "subscriptions/{}".format(subscription_id), json=data)
-
-    @token_required
-    def delete_subscription(self, subscription_id: str) -> Response:
-        """Deletes a subscription to stop receiving notifications for a resource.
-
-        https://docs.microsoft.com/en-us/graph/webhooks#deleting-a-subscription
-
-        Args:
-            subscription_id (str): Subscription ID.
-
-        Returns:
-            Response: Microsoft Graph Response.
-        """
-        return self._client._delete(self._client.base_url + "subscriptions/{}".format(subscription_id))
+from datetime import datetime
+
+from microsoftgraph.decorators import token_required
+from microsoftgraph.response import Response
+from microsoftgraph.utils import format_time
+
+
+class Webhooks(object):
+    def __init__(self, client) -> None:
+        """Set up notifications for changes in user data.
+
+        https://docs.microsoft.com/en-us/graph/webhooks?view=graph-rest-1.0
+
+        Args:
+            client (Client): Library Client.
+        """
+        self._client = client
+
+    @token_required
+    def create_subscription(
+        self,
+        change_type: str,
+        notification_url: str,
+        resource: str,
+        expiration_datetime: datetime,
+        client_state: str = None,
+        **kwargs,
+    ) -> Response:
+        """Creates a subscription to start receiving notifications for a resource.
+
+        https://docs.microsoft.com/en-us/graph/webhooks#creating-a-subscription
+
+        Args:
+            change_type (str): The event type that caused the notification. For example, created on mail receive, or
+            updated on marking a message read.
+            notification_url (str): Url to receive notifications.
+            resource (str): The URI of the resource relative to https://graph.microsoft.com.
+            expiration_datetime (datetime): The expiration time for the subscription.
+            client_state (str, optional): The clientState property specified in the subscription request. Defaults to None.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        if isinstance(expiration_datetime, datetime):
+            expiration_datetime = format_time(expiration_datetime, is_webhook=True)
+
+        data = {
+            "changeType": change_type,
+            "notificationUrl": notification_url,
+            "resource": resource,
+            "expirationDateTime": expiration_datetime,
+            "clientState": client_state,
+        }
+        data.update(kwargs)
+        return self._client._post(self._client.base_url + "subscriptions", json=data)
+
+    @token_required
+    def renew_subscription(self, subscription_id: str, expiration_datetime: datetime) -> Response:
+        """Renews a subscription to keep receiving notifications for a resource.
+
+        https://docs.microsoft.com/en-us/graph/webhooks#renewing-a-subscription
+
+        Args:
+            subscription_id (str): Subscription ID.
+            expiration_datetime (datetime): Expiration date.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        if isinstance(expiration_datetime, datetime):
+            expiration_datetime = format_time(expiration_datetime, is_webhook=True)
+
+        data = {"expirationDateTime": expiration_datetime}
+        return self._client._patch(self._client.base_url + "subscriptions/{}".format(subscription_id), json=data)
+
+    @token_required
+    def delete_subscription(self, subscription_id: str) -> Response:
+        """Deletes a subscription to stop receiving notifications for a resource.
+
+        https://docs.microsoft.com/en-us/graph/webhooks#deleting-a-subscription
+
+        Args:
+            subscription_id (str): Subscription ID.
+
+        Returns:
+            Response: Microsoft Graph Response.
+        """
+        return self._client._delete(self._client.base_url + "subscriptions/{}".format(subscription_id))
```

