# Comparing `tmp/infinitode.py-1.0.4.tar.gz` & `tmp/infinitode.py-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infinitode.py-1.0.4.tar", last modified: Fri Apr  7 14:55:37 2023, max compression
+gzip compressed data, was "infinitode.py-1.0.5.tar", last modified: Sat Jul 15 21:03:48 2023, max compression
```

## Comparing `infinitode.py-1.0.4.tar` & `infinitode.py-1.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 14:55:37.199786 infinitode.py-1.0.4/
--rw-rw-rw-   0        0        0     1100 2022-04-19 17:21:19.000000 infinitode.py-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     6169 2023-04-07 14:55:37.198786 infinitode.py-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5883 2022-05-08 16:08:53.000000 infinitode.py-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 14:55:37.177858 infinitode.py-1.0.4/infinitode/
--rw-rw-rw-   0        0        0     1469 2023-04-07 14:53:30.000000 infinitode.py-1.0.4/infinitode/__init__.py
--rw-rw-rw-   0        0        0      883 2022-04-26 14:54:12.000000 infinitode.py-1.0.4/infinitode/badge.py
--rw-rw-rw-   0        0        0    15951 2023-04-07 14:24:32.000000 infinitode.py-1.0.4/infinitode/core.py
--rw-rw-rw-   0        0        0      426 2022-04-28 13:52:01.000000 infinitode.py-1.0.4/infinitode/errors.py
--rw-rw-rw-   0        0        0     6683 2022-04-26 14:53:48.000000 infinitode.py-1.0.4/infinitode/leaderboard.py
--rw-rw-rw-   0        0        0     6544 2022-04-28 13:57:14.000000 infinitode.py-1.0.4/infinitode/player.py
--rw-rw-rw-   0        0        0        0 2022-04-25 15:30:52.000000 infinitode.py-1.0.4/infinitode/py.typed
--rw-rw-rw-   0        0        0     6424 2022-04-28 13:16:02.000000 infinitode.py-1.0.4/infinitode/score.py
--rw-rw-rw-   0        0        0      682 2022-08-20 13:59:13.000000 infinitode.py-1.0.4/infinitode/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-07 14:55:37.195756 infinitode.py-1.0.4/infinitode.py.egg-info/
--rw-rw-rw-   0        0        0     6169 2023-04-07 14:55:37.000000 infinitode.py-1.0.4/infinitode.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-04-07 14:55:37.000000 infinitode.py-1.0.4/infinitode.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 14:55:37.000000 infinitode.py-1.0.4/infinitode.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-07 14:55:37.000000 infinitode.py-1.0.4/infinitode.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-07 14:55:37.000000 infinitode.py-1.0.4/infinitode.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 14:55:37.199786 infinitode.py-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      758 2022-04-28 14:05:57.000000 infinitode.py-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 21:03:48.572318 infinitode.py-1.0.5/
+-rw-rw-rw-   0        0        0     1100 2022-04-19 17:21:19.000000 infinitode.py-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     6254 2023-07-15 21:03:48.571057 infinitode.py-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5968 2023-07-15 20:58:30.000000 infinitode.py-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 21:03:48.543198 infinitode.py-1.0.5/infinitode/
+-rw-rw-rw-   0        0        0     1469 2023-07-15 20:54:51.000000 infinitode.py-1.0.5/infinitode/__init__.py
+-rw-rw-rw-   0        0        0      858 2023-07-15 20:55:02.000000 infinitode.py-1.0.5/infinitode/badge.py
+-rw-rw-rw-   0        0        0    18199 2023-07-15 21:00:13.000000 infinitode.py-1.0.5/infinitode/core.py
+-rw-rw-rw-   0        0        0      432 2023-07-15 20:55:16.000000 infinitode.py-1.0.5/infinitode/errors.py
+-rw-rw-rw-   0        0        0     6821 2023-07-15 20:57:10.000000 infinitode.py-1.0.5/infinitode/leaderboard.py
+-rw-rw-rw-   0        0        0     7530 2023-07-15 20:49:19.000000 infinitode.py-1.0.5/infinitode/player.py
+-rw-rw-rw-   0        0        0        0 2022-04-25 15:30:52.000000 infinitode.py-1.0.5/infinitode/py.typed
+-rw-rw-rw-   0        0        0     6571 2023-07-15 21:00:39.000000 infinitode.py-1.0.5/infinitode/score.py
+-rw-rw-rw-   0        0        0      669 2023-07-15 20:57:01.000000 infinitode.py-1.0.5/infinitode/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-15 21:03:48.568915 infinitode.py-1.0.5/infinitode.py.egg-info/
+-rw-rw-rw-   0        0        0     6254 2023-07-15 21:03:48.000000 infinitode.py-1.0.5/infinitode.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-07-15 21:03:48.000000 infinitode.py-1.0.5/infinitode.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 21:03:48.000000 infinitode.py-1.0.5/infinitode.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-15 21:03:48.000000 infinitode.py-1.0.5/infinitode.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-15 21:03:48.000000 infinitode.py-1.0.5/infinitode.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 21:03:48.572318 infinitode.py-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      758 2022-04-28 14:05:57.000000 infinitode.py-1.0.5/setup.py
```

### Comparing `infinitode.py-1.0.4/LICENSE` & `infinitode.py-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `infinitode.py-1.0.4/PKG-INFO` & `infinitode.py-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infinitode.py
-Version: 1.0.4
+Version: 1.0.5
 Summary: A python wrapper for the Infinitode 2 API.
 Home-page: https://github.com/Sprylos/infinitode.py
 Author: Sprylos
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -112,15 +112,18 @@
         # The last main object is a Player, received only be Session.player()
         # Every Player has the same attributes.
         print(
             player.playerid,
             player.nickname,
             player.level,
             player.xp,
-            player.xp_max,  # xp required per level (always 1000?)
+            player.xp_max,  # xp required per level
+            player.season_level,
+            player.season_xp,
+            player.season_xp_max,
             player.total_score,
             player.total_rank,
             player.total_top,
             player.replays,
             player.issues,
             player.created_at,  # as str
             player.avatar_link  # even when the person has no pfp
```

### Comparing `infinitode.py-1.0.4/README.md` & `infinitode.py-1.0.5/infinitode.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: infinitode.py
+Version: 1.0.5
+Summary: A python wrapper for the Infinitode 2 API.
+Home-page: https://github.com/Sprylos/infinitode.py
+Author: Sprylos
+License: MIT
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Infinitode.py
 
 An asynchronous python wrapper for the Infinitode-2 API using `async`-`await` syntax.
 
 ## Installing
 
 ---
@@ -101,15 +112,18 @@
         # The last main object is a Player, received only be Session.player()
         # Every Player has the same attributes.
         print(
             player.playerid,
             player.nickname,
             player.level,
             player.xp,
-            player.xp_max,  # xp required per level (always 1000?)
+            player.xp_max,  # xp required per level
+            player.season_level,
+            player.season_xp,
+            player.season_xp_max,
             player.total_score,
             player.total_rank,
             player.total_top,
             player.replays,
             player.issues,
             player.created_at,  # as str
             player.avatar_link  # even when the person has no pfp
@@ -143,7 +157,9 @@
 
 async def main():
     async with infinitode.Session() as API:
         await API.leaderboards('6.3')  # just an example
 
 asyncio.run(main())
 ```
+
+
```

### Comparing `infinitode.py-1.0.4/infinitode/__init__.py` & `infinitode.py-1.0.5/infinitode/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 ~~~~~~~~~~~~~~~~~~~
 
 An asynchronous wrapper for the Infinitode API.
 """
 
 __author__ = "Sprylos"
 __title__ = "infinitode.py"
-__version__ = '1.0.4'
+__version__ = "1.0.5"
 __license__ = """MIT License
 
-Copyright (c) 2022 Sprylos
+Copyright (c) 2023 Sprylos
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `infinitode.py-1.0.4/infinitode/badge.py` & `infinitode.py-1.0.5/infinitode/badge.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 from __future__ import annotations
 
-__all__ = ('Badge',)
+__all__ = ("Badge",)
 
 
 class Badge:
     """Represents an in-game pinned badge."""
-    __slots__ = (
-        'icon_img',
-        'icon_color',
-        'overlay_img',
-        'overlay_color'
-    )
 
-    def __init__(self, iconImg: str, iconColor: str, overlayImg: str, overlayColor: str) -> None:
+    __slots__ = ("icon_img", "icon_color", "overlay_img", "overlay_color")
+
+    def __init__(
+        self, iconImg: str, iconColor: str, overlayImg: str, overlayColor: str
+    ) -> None:
         self.icon_img = iconImg
         self.icon_color = iconColor
         self.overlay_img = overlayImg
         self.overlay_color = overlayColor
 
     # magic methods
 
     def __repr__(self) -> str:
         attrs = {
-            'icon_img': self.icon_img,
-            'icon_color': self.icon_color,
-            'overlay_img': self.overlay_img,
-            'overlay_color': self.overlay_color,
+            "icon_img": self.icon_img,
+            "icon_color": self.icon_color,
+            "overlay_img": self.overlay_img,
+            "overlay_color": self.overlay_color,
         }
-        inner = ' '.join(f'{k}={v}' for k, v in attrs.items())
-        return f'<{self.__class__.__name__} {inner}>'
+        inner = " ".join(f"{k}={v}" for k, v in attrs.items())
+        return f"<{self.__class__.__name__} {inner}>"
```

### Comparing `infinitode.py-1.0.4/infinitode/core.py` & `infinitode.py-1.0.5/infinitode/core.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,35 +21,45 @@
 from .errors import APIError, BadArgument
 from .leaderboard import Leaderboard
 from .player import Player
 from .utils import try_int
 from .score import Score
 
 
-__all__ = ('Session',)
+__all__ = ("Session",)
 
 _log = logging.getLogger(__name__)
 
-ID_REGEX = re.compile(r'U-([A-Z0-9]{4}-){2}[A-Z0-9]{6}')
+ID_REGEX = re.compile(r"U-([A-Z0-9]{4}-){2}[A-Z0-9]{6}")
+
+# fmt: off
 LEVELS = (
     '1.1', '1.2', '1.3', '1.4', '1.5', '1.6', '1.7', '1.8', '1.b1',
     '2.1', '2.2', '2.3', '2.4', '2.5', '2.6', '2.7', '2.8', '2.b1',
     '3.1', '3.2', '3.3', '3.4', '3.5', '3.6', '3.7', '3.8', '3.b1',
     '4.1', '4.2', '4.3', '4.4', '4.5', '4.6', '4.7', '4.8', '4.b1',
     '5.1', '5.2', '5.3', '5.4', '5.5', '5.6', '5.7', '5.8', '5.b1', '5.b2',
     '6.1', '6.2', '6.3', '6.4', '6.5', 'rumble', 'dev', 'zecred',
     'DQ1', 'DQ3', 'DQ4', 'DQ5', 'DQ7', 'DQ8', 'DQ9', 'DQ10', 'DQ11', 'DQ12',
 )
+# fmt: on
 
 
 class Session:
     def __init__(self, session: Optional[aiohttp.ClientSession] = None) -> None:
         self._session = session or aiohttp.ClientSession()
-        self._cooldown: Dict[str, Any] = {'DailyQuestInfo': 0.0, 'LatestNews': 0.0, 'DailyQuestLeaderboards': {
-        }, 'SkillPointLeaderboard': 0.0, 'BasicLevelsTopLeaderboards': {}, 'Leaderboards': {}, 'seasonal': 0.0}
+        self._cooldown: Dict[str, Any] = {
+            "DailyQuestInfo": 0.0,
+            "LatestNews": 0.0,
+            "DailyQuestLeaderboards": {},
+            "SkillPointLeaderboard": 0.0,
+            "BasicLevelsTopLeaderboards": {},
+            "Leaderboards": {},
+            "seasonal": 0.0,
+        }
         self._DailyQuestLeaderboards: Dict[str, Leaderboard] = {}
         self._BasicLevelsTopLeaderboards: Dict[str, Leaderboard] = {}
         self._Leaderboards: Dict[str, Leaderboard] = {}
         self._SkillPointLeaderboard: Leaderboard
         self._seasonal: Leaderboard
 
     # async enter and exit allow for the fancy "with" statements
@@ -62,102 +72,172 @@
 
     async def close(self):
         """Closes the internal ClientSession."""
         await self._session.close()
 
     # Rough parameter checking, "*" makes params keyword only
     @staticmethod
-    def _kwarg_check(*, mapname: Optional[str] = None, playerid: Optional[str] = None, mode: Optional[str] = None, difficulty: Optional[str] = None) -> None:
+    def _kwarg_check(
+        *,
+        mapname: Optional[str] = None,
+        playerid: Optional[str] = None,
+        mode: Optional[str] = None,
+        difficulty: Optional[str] = None,
+    ) -> None:
         if mapname is not None and str(mapname) not in LEVELS:
-            raise BadArgument('Invalid map: ' + mapname)
+            raise BadArgument("Invalid map: " + mapname)
         if playerid is not None and not ID_REGEX.match(playerid):
-            raise BadArgument('Invalid playerid: ' + playerid)
-        if mode is not None and not mode in ('score', 'waves'):
+            raise BadArgument("Invalid playerid: " + playerid)
+        if mode is not None and not mode in ("score", "waves"):
             raise BadArgument(
-                "Invalid mode (must be either 'score' or 'waves'): " + mode)
-        if difficulty is not None and not difficulty in ('EASY', 'NORMAL', 'ENDLESS_I'):
+                "Invalid mode (must be either 'score' or 'waves'): " + mode
+            )
+        if difficulty is not None and not difficulty in ("EASY", "NORMAL", "ENDLESS_I"):
             raise BadArgument(
-                "Invalid difficulty (must be one of 'EASY', 'NORMAL', 'ENDLESS_I': " + difficulty)
+                "Invalid difficulty (must be one of 'EASY', 'NORMAL', 'ENDLESS_I': "
+                + difficulty
+            )
 
     # not being more specific with the payload type
     # so the typechecker stops annoying me
-    async def _post(self, arg: str, data: Optional[Dict[str, Any]] = None) -> Dict[str, Any]:
-        '''Internal post method to communicate with Rainy's API'''
-        url = f'https://infinitode.prineside.com/?m=api&a={arg}&apiv=1&g=com.prineside.tdi2&v=282'
-        _log.info('Sending POST request %s with data %s', arg, data)
+    async def _post(
+        self, arg: str, data: Optional[Dict[str, Any]] = None
+    ) -> Dict[str, Any]:
+        """Internal post method to communicate with Rainy's API"""
+        url = f"https://infinitode.prineside.com/?m=api&a={arg}&apiv=1&g=com.prineside.tdi2&v=282"
+        _log.info("Sending POST request %s with data %s", arg, data)
         async with self._session.post(url, data=data) as r:
             try:
                 r.raise_for_status()
             except aiohttp.ClientResponseError:
                 raise APIError("Something went wrong. Try again later")
 
             payload: Dict[str, Any] = await r.json()
-            _log.debug('Response to POST request %s: %s', arg, payload)
+            _log.debug("Response to POST request %s: %s", arg, payload)
 
-            if payload['status'] == 'success':
+            if payload["status"] == "success":
                 return payload
             else:
-                raise APIError(
-                    f'Error response from server: {payload["message"]}')
+                raise APIError(f'Error response from server: {payload["message"]}')
 
     # all the mapnames are Any because any python object can be converted to a str
-    async def leaderboards_rank(self, mapname: Any, playerid: str, mode: str = 'score', difficulty: str = 'NORMAL') -> Score:
+    async def leaderboards_rank(
+        self,
+        mapname: Any,
+        playerid: str,
+        mode: str = "score",
+        difficulty: str = "NORMAL",
+    ) -> Score:
         """
         Retrieves a Score of the given player.
         A valid playerid needs to be specified.
         """
         self._kwarg_check(
-            mapname=mapname, playerid=playerid, mode=mode, difficulty=difficulty)
-        payload = await self._post('getLeaderboardsRank', data={'gamemode': 'BASIC_LEVELS', 'difficulty': difficulty, 'playerid': playerid, 'mapname': str(mapname), 'mode': mode})
-        return Score.from_payload('leaderboards_rank', mapname, mode, difficulty, playerid, payload)
+            mapname=mapname, playerid=playerid, mode=mode, difficulty=difficulty
+        )
+        payload = await self._post(
+            "getLeaderboardsRank",
+            data={
+                "gamemode": "BASIC_LEVELS",
+                "difficulty": difficulty,
+                "playerid": playerid,
+                "mapname": str(mapname),
+                "mode": mode,
+            },
+        )
+        return Score.from_payload(
+            "leaderboards_rank", mapname, mode, difficulty, playerid, payload
+        )
 
-    async def leaderboards(self, mapname: Any, playerid: Optional[str] = None, mode: str = 'score', difficulty: str = 'NORMAL') -> Leaderboard:
+    async def leaderboards(
+        self,
+        mapname: Any,
+        playerid: Optional[str] = None,
+        mode: str = "score",
+        difficulty: str = "NORMAL",
+    ) -> Leaderboard:
         """
         Retrieves a Leaderboard.
         The leaderboard contains the top 200 scores of the specified map.
         """
         self._kwarg_check(
-            mapname=mapname, playerid=playerid, mode=mode, difficulty=difficulty)
-        key = f'{difficulty}{mode}{mapname}'
-        if not playerid and (time.time() < self._cooldown['Leaderboards'].get(key, 0) + 60):
+            mapname=mapname, playerid=playerid, mode=mode, difficulty=difficulty
+        )
+        key = f"{difficulty}{mode}{mapname}"
+        if not playerid and (
+            time.time() < self._cooldown["Leaderboards"].get(key, 0) + 60
+        ):
             return self._Leaderboards[key]
-        payload = await self._post('getLeaderboards', data={'gamemode': 'BASIC_LEVELS', 'difficulty': difficulty, 'playerid': playerid, 'mapname': str(mapname), 'mode': mode})
+        payload = await self._post(
+            "getLeaderboards",
+            data={
+                "gamemode": "BASIC_LEVELS",
+                "difficulty": difficulty,
+                "playerid": playerid,
+                "mapname": str(mapname),
+                "mode": mode,
+            },
+        )
         lb = Leaderboard.from_payload(
-            'leaderboards', mapname, mode, difficulty, playerid, payload)
+            "leaderboards", mapname, mode, difficulty, playerid, payload
+        )
         if lb.player is None:
             self._Leaderboards[key] = lb
-            self._cooldown['Leaderboards'][key] = time.time()
+            self._cooldown["Leaderboards"][key] = time.time()
         return lb
 
-    async def runtime_leaderboards(self, mapname: Any, playerid: str, mode: str = 'score', difficulty: str = 'NORMAL') -> Leaderboard:
+    async def runtime_leaderboards(
+        self,
+        mapname: Any,
+        playerid: str,
+        mode: str = "score",
+        difficulty: str = "NORMAL",
+    ) -> Leaderboard:
         """
         Retrieves a Runtime Leaderboard (The one displayed top right in-game).
         A valid playerid needs to be specified.
         The leaderboard contains the top 200 scores and one Score for each top% of the specified map.
         """
         self._kwarg_check(
-            mapname=mapname, playerid=playerid, mode=mode, difficulty=difficulty)
-        payload = await self._post('getRuntimeLeaderboards', data={'gamemode': 'BASIC_LEVELS', 'difficulty': difficulty, 'playerid': playerid, 'mapname': str(mapname), 'mode': mode})
-        return Leaderboard.from_payload('runtime_leaderboards', mapname, mode, difficulty, playerid, payload)
+            mapname=mapname, playerid=playerid, mode=mode, difficulty=difficulty
+        )
+        payload = await self._post(
+            "getRuntimeLeaderboards",
+            data={
+                "gamemode": "BASIC_LEVELS",
+                "difficulty": difficulty,
+                "playerid": playerid,
+                "mapname": str(mapname),
+                "mode": mode,
+            },
+        )
+        return Leaderboard.from_payload(
+            "runtime_leaderboards", mapname, mode, difficulty, playerid, payload
+        )
 
-    async def skill_point_leaderboard(self, playerid: Optional[str] = None) -> Leaderboard:
+    async def skill_point_leaderboard(
+        self, playerid: Optional[str] = None
+    ) -> Leaderboard:
         """
         Retrieves the Skill Point Leaderboard.
         The leaderboard contains the top 3 skill point owners (looking at you, Eupho!).
         """
         if playerid is not None:
             self._kwarg_check(playerid=playerid)
-        elif time.time() < self._cooldown['SkillPointLeaderboard'] + 60:
+        elif time.time() < self._cooldown["SkillPointLeaderboard"] + 60:
             return self._SkillPointLeaderboard
-        payload = await self._post('getSkillPointLeaderboard', data={'playerid': playerid})
+        payload = await self._post(
+            "getSkillPointLeaderboard", data={"playerid": playerid}
+        )
         lb = Leaderboard.from_payload(
-            'skill_point_leaderboard', 'SP', 'score', 'NORMAL', playerid, payload)
+            "skill_point_leaderboard", "SP", "score", "NORMAL", playerid, payload
+        )
         if lb.player is None:
             self._SkillPointLeaderboard = lb
-            self._cooldown['SkillPointLeaderboard'] = time.time()
+            self._cooldown["SkillPointLeaderboard"] = time.time()
         return lb
 
     async def daily_quest_leaderboards(
         self,
         date: Union[datetime.datetime, str, None] = None,
         playerid: Optional[str] = None,
         warning: bool = True,
@@ -165,151 +245,219 @@
         """
         Retrieves the Daily Quest Leaderboard for the given date.
         If an invalid or no date is provided, the date will be set to the current date.
         You may disable the invalid date warning by setting the warning param to False.
         The leaderboard contains the top 200 DQ players of the given date.
         """
         if date is None:
-            date = datetime.datetime.utcnow().strftime('%Y-%m-%d')
+            date = datetime.datetime.utcnow().strftime("%Y-%m-%d")
         elif isinstance(date, datetime.datetime):
-            date = date.strftime('%Y-%m-%d')
+            date = date.strftime("%Y-%m-%d")
         else:
             try:
-                datetime.datetime.strptime(date, '%Y-%m-%d')
+                datetime.datetime.strptime(date, "%Y-%m-%d")
             except ValueError:
                 if warning == True:
                     _log.warning(
-                        'Invalid date in daily_quest_leaderboards (Use YYYY-MM-DD format): %s', date)
-                date = datetime.datetime.utcnow().strftime('%Y-%m-%d')
-        if not playerid and (time.time() < self._cooldown['DailyQuestLeaderboards'].get(date, 0) + 60):
+                        "Invalid date in daily_quest_leaderboards (Use YYYY-MM-DD format): %s",
+                        date,
+                    )
+                date = datetime.datetime.utcnow().strftime("%Y-%m-%d")
+        if not playerid and (
+            time.time() < self._cooldown["DailyQuestLeaderboards"].get(date, 0) + 60
+        ):
             return self._DailyQuestLeaderboards[date]
         if playerid is not None:
             self._kwarg_check(playerid=playerid)
-        payload = await self._post('getDailyQuestLeaderboards', data={'date': date, 'playerid': playerid})
+        payload = await self._post(
+            "getDailyQuestLeaderboards", data={"date": date, "playerid": playerid}
+        )
         lb = Leaderboard.from_payload(
-            'daily_quest_leaderboards', 'DQ', 'score', 'NORMAL', playerid, payload, date=date)
+            "daily_quest_leaderboards",
+            "DQ",
+            "score",
+            "NORMAL",
+            playerid,
+            payload,
+            date=date,
+        )
         if lb.player is None:
             self._DailyQuestLeaderboards[date] = lb
-            self._cooldown['DailyQuestLeaderboards'][date] = time.time()
+            self._cooldown["DailyQuestLeaderboards"][date] = time.time()
         return lb
 
     async def seasonal_leaderboard(self) -> Leaderboard:
         """
         Retrieves the season Leaderboard.
         The leaderboard contains the top 100 scores in the season.
         This coroutine never takes arguments.
         """
-        if time.time() < self._cooldown['seasonal'] + 60:
+        if time.time() < self._cooldown["seasonal"] + 60:
             return self._seasonal
-        url = 'https://infinitode.prineside.com/xdx/?url=seasonal_leaderboard'
-        _log.info('Sending GET request to %s', url)
+        url = "https://infinitode.prineside.com/xdx/?url=seasonal_leaderboard"
+        _log.info("Sending GET request to %s", url)
         r = await self._session.get(url=url)
         try:
             r.raise_for_status()
         except aiohttp.ClientResponseError:
-            raise APIError('Bad Gateway.')
-        seasonal = bs4.BeautifulSoup(await r.text(), features='lxml')
-        season = int(seasonal.select_one('label[i18n="season_formatted"]')['i18nf'].replace('["', '').replace('"]', ''))  # type: ignore # nopep8
+            raise APIError("Bad Gateway.")
+        seasonal = bs4.BeautifulSoup(await r.text(), features="lxml")
+
+        # fmt: off
+        season = int(seasonal.select_one('label[i18n="season_formatted"]')['i18nf'].replace('["', '').replace('"]', ''))  # type: ignore
         player_count = int(seasonal.select('label[i18n="player_count_formatted"]')[  # type: ignore
             0]['i18nf'].replace('["', '').replace('"]', '').replace(',', ''))  # type: ignore
         lb = Leaderboard.from_payload(
             'seasonal_leaderboard', 'season', 'score', 'NORMAL', None, {
                 'status': 'success',
                 'player': {'total': player_count},
                 'leaderboards': [
                     {
-                        'playerid': seasonal.select('label[color="LIGHT_BLUE:P300"]')[x]['click'].split('id=')[1],  # type: ignore # nopep8
-                        'nickname': seasonal.select('label[color="LIGHT_BLUE:P300"]')[x].text,  # type: ignore # nopep8
-                        'score': seasonal.select('label[nowrap="true"][text-align="right"]')[x].text.replace(',', '')  # type: ignore # nopep8
-                    } for x in range(len(seasonal.select('div[x="90"]')))  # type: ignore
+                        'playerid': seasonal.select('label[color="LIGHT_BLUE:P300"]')[x]['click'].split('id=')[1],  # type: ignore
+                        'nickname': seasonal.select('label[color="LIGHT_BLUE:P300"]')[x].text,
+                        'score': seasonal.select('label[nowrap="true"][text-align="right"]')[x].text.replace(',', '')
+                    } for x in range(len(seasonal.select('div[x="90"]')))
                 ]
             }, season=season
         )
+        # fmt: on
+
         self._seasonal = lb
-        self._cooldown['seasonal'] = time.time()
+        self._cooldown["seasonal"] = time.time()
         return lb
 
     def _parse_player(self, content: str, playerid: str) -> Player:
-        data = bs4.BeautifulSoup(content, features='lxml')
+        data = bs4.BeautifulSoup(content, features="lxml")
         t: Dict[str, Any] = {}
-        t['playerid'] = playerid
-        t['nickname'] = data.select_one('label:not([i18n])').text  # type: ignore # this should never fail # nopep8
-        totals = data.select_one('div[width="522"][height="128"][pad-top="10"][pad-bottom="10"][align="center"]')  # type: ignore # nopep8
+        t["playerid"] = playerid
+        t["nickname"] = data.select_one("label:not([i18n])").text  # type: ignore
+        totals = data.select_one('div[width="522"][height="140"][align="center"]')
         if totals is None:
-            t.update({'total_score': 0, 'total_rank': 0, 'total_top': 0})
+            t.update({"total_score": 0, "total_rank": 0, "total_top": 0})
         else:
-            totals = totals.select('label')  # type: ignore # nopep8
+            totals = totals.select("label")
             if len(totals) >= 4:
-                t['total_score'] = try_int(totals[1].text.replace(',', ''))
-                t['total_rank'] = try_int(totals[2].text.replace(',', ''))
-                t['total_top'] = totals[3].text.replace('- Top ', '')
+                t["total_score"] = try_int(totals[1].text.replace(",", ""))
+                t["total_rank"] = try_int(totals[2].text.replace(",", ""))
+                t["total_top"] = totals[3].text.replace("- Top ", "")
             else:
-                t.update({'total_score': 0, 'total_rank': 0, 'total_top': '0%'})
-        comments = data.findAll(
-            text=lambda text: isinstance(text, bs4.Comment))
+                t.update({"total_score": 0, "total_rank": 0, "total_top": "0%"})
+        comments = data.findAll(text=lambda text: isinstance(text, bs4.Comment))
         for x in comments:
-            if 'Level:' in x:
-                t['level'] = int(x.split('>')[3].split('<')[0])
+            if "Level:" in x:
+                t["level"] = int(x.split(">")[3].split("<")[0])
                 break
         else:
-            t['level'] = 0
-        xp_data = data.select_one('div[width="330"][height="64"]')  # type: ignore # nopep8
+            t["level"] = 0
+        xp_data = data.select_one('div[width="330"][height="64"]')
         if xp_data is None:
-            raise BadArgument('Invalid playerid: ' + playerid)
-        xp_data = xp_data.select_one('label').text.split(' / ')  # type: ignore
-        t['xp'] = int(xp_data[0])
-        t['xp_max'] = int(xp_data[1])
-        t['levels'] = {}
-        for x in data.select('div[width="800"][height="40"]')[1:]:  # type: ignore # nopep8
-            level_data = x.select('label')  # type: ignore
+            raise BadArgument("Invalid playerid: " + playerid)
+        xp_data = xp_data.select_one("label").text.split(" / ")  # type: ignore
+        t["xp"] = int(xp_data[0])
+        t["xp_max"] = int(xp_data[1])
+        season_xp_data = data.select_one(
+            'div[width="530"][align="center"][height="64"][pad-bottom="10"]'
+        )
+        if season_xp_data is None:
+            raise BadArgument("Invalid playerid: " + playerid)
+        season_xp_borders = season_xp_data.select_one("label").text.split(" / ")  # type: ignore
+        t["season_xp"] = int(season_xp_borders[0])
+        t["season_xp_max"] = int(season_xp_borders[1])
+        season_level_data = season_xp_data.select_one(
+            'div[x="466"][width="64"][height="64"]'
+        )
+        if season_level_data is None:
+            raise BadArgument("Invalid playerid: " + playerid)
+        t["season_level"] = season_level_data["data"].split(":")[1]  # type: ignore
+
+        t["levels"] = {}
+        for x in data.select('div[width="800"][height="40"]')[1:]:
+            level_data = x.select("label")
             level = level_data[0].text
-            if not x.select_one('label[i18n="not_ranked"]'):  # type: ignore # nopep8
-                rank = int(level_data[2].text.replace(',', ''))
-                score = int(level_data[1].text.replace(',', ''))
-                total = int(level_data[3].text.replace(
-                    '/ ', '').replace(',', ''))
+            if not x.select_one('label[i18n="not_ranked"]'):
+                rank = int(level_data[2].text.replace(",", ""))
+                score = int(level_data[1].text.replace(",", ""))
+                total = int(level_data[3].text.replace("/ ", "").replace(",", ""))
                 top = level_data[-1].text
             else:
-                rank, score, total, top = 0, 0, 0, '-%'
-            t['levels'][level] = Score(
-                'player', level, 'score', 'NORMAL', playerid,
-                rank=rank, score=score, total=total, top=top,
-                level=t['level'], nickname=t['nickname']
+                rank, score, total, top = 0, 0, 0, "-%"
+            t["levels"][level] = Score(
+                "player",
+                level,
+                "score",
+                "NORMAL",
+                playerid,
+                rank=rank,
+                score=score,
+                total=total,
+                top=top,
+                level=t["level"],
+                nickname=t["nickname"],
             )
-        t['badges'] = {}
-        for x in data.select('div[width="80"][height="80"]'):  # type: ignore # nopep8
-            rar: str = x.select('img')[0]['src'].split('bg-')[1]  # type: ignore # nopep8
-            if rar in ['not-received', 'common', 'rare', 'very-rare', 'epic', 'legendary', 'supreme', 'artifact']:
-                ico: str = x.select('img')[1]['src'].split('icon-')[1]  # type: ignore # nopep8
-                if ico in ['daily-game', 'invited-players', 'killed-enemies', 'mined-resources', 'skillful', 'of-merit', 'beta-tester-season-2'] or ico[:8] == 'season-1':
-                    col: str = x.select('img')[-1]['color']  # type: ignore # nopep8
-                    t['badges'][ico] = (rar, col)
-        labels = data.select('table[width="800"][align="center"]')[-1].select('label')  # type: ignore # nopep8
+        t["badges"] = {}
+        icos = [
+            "daily-game",
+            "invited-players",
+            "killed-enemies",
+            "mined-resources",
+            "skillful",
+            "of-merit",
+            "beta-tester-season-2",
+            f"high-leveled-{t['level'] // 10}",
+        ]
+        for x in data.select('div[width="80"][height="80"]'):
+            rar: str = x.select("img")[0]["src"].split("bg-")[1]  # type: ignore
+            if rar in [
+                "not-received",
+                "common",
+                "rare",
+                "very-rare",
+                "epic",
+                "legendary",
+                "supreme",
+                "artifact",
+            ]:
+                ico: str = x.select("img")[1]["src"].split("icon-")[1]  # type: ignore
+                if (
+                    ico
+                    in icos
+                    + [
+                        "youtube-author-" + rar,
+                        f"season-level-{rar}-2",
+                    ]
+                    or ico[:8] == "season-1"
+                ):
+                    col: str = x.select("img")[-1]["color"]  # type: ignore
+                    t["badges"][ico] = (rar, col)
+        labels = data.select('table[width="800"][align="center"]')[-1].select("label")
         replays = labels[-3].string.split(" ")  # type: ignore
-        t['replays'] = 0 if len(replays) != 4 else int(replays[3])
+        t["replays"] = 0 if len(replays) != 4 else int(replays[3])
         issues = labels[-2].string.split(" ")  # type: ignore
-        t['issues'] = 0 if len(issues) != 6 else int(issues[0][3:])
-        sp = list(labels[-1].string.split("ned ")[1].split(" "))  # type: ignore # nopep8
+        t["issues"] = 0 if len(issues) != 6 else int(issues[0][3:])
+        sp = list(labels[-1].string.split("ned ")[1].split(" "))  # type: ignore
         day = sp[0][:-2] if len(sp[0][:2]) == 2 else "0" + sp[0][:2]
-        t['created_at'] = datetime.datetime.strptime(
-            day + " " + sp[-2] + " " + sp[-1], "%d %B %Y").strftime('%Y-%m-%d')
+        t["created_at"] = datetime.datetime.strptime(
+            day + " " + sp[-2] + " " + sp[-1], "%d %B %Y"
+        ).strftime("%Y-%m-%d")
 
         return Player(**t)
 
     async def player(self, playerid: str) -> Player:
         """
         Retrieves the Player.
         A valid playerid needs to be specified.
         """
         self._kwarg_check(playerid=playerid)
-        url = f'https://infinitode.prineside.com/xdx/index.php?url=profile/view&id={playerid}'
-        _log.info('Sending GET request to %s', url)
+        url = f"https://infinitode.prineside.com/xdx/index.php?url=profile/view&id={playerid}"
+        _log.info("Sending GET request to %s", url)
         r = await self._session.get(url=url)
         try:
             r.raise_for_status()
         except aiohttp.ClientResponseError:
-            raise APIError('Bad Gateway.')
+            raise APIError("Bad Gateway.")
         loop = asyncio.get_event_loop()
         try:
-            return await loop.run_in_executor(None, self._parse_player, await r.text(), playerid)
+            return await loop.run_in_executor(
+                None, self._parse_player, await r.text(), playerid
+            )
         except Exception as exc:
-            raise BadArgument('Invalid playerid: ' + playerid) from exc
+            raise BadArgument("Invalid playerid: " + playerid) from exc
```

### Comparing `infinitode.py-1.0.4/infinitode/leaderboard.py` & `infinitode.py-1.0.5/infinitode/leaderboard.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,68 @@
 from __future__ import annotations
 
 # std
-from typing import (
-    Any,
-    Dict,
-    List,
-    Optional,
-    overload,
-    Union
-)
+from typing import Any, Dict, List, Optional, overload, Union
 
 # local
 from .score import Score
 
 
-__all__ = ('Leaderboard',)
+__all__ = ("Leaderboard",)
 
 
 class Leaderboard_iterator:
     """Iterator class for a Leaderboard."""
-    __slots__ = (
-        '_scores',
-        '_index'
-    )
+
+    __slots__ = ("_scores", "_index")
 
     def __init__(self, scores: List[Score]) -> None:
         self._scores = scores
         self._index: int = 0
 
     def __repr__(self) -> str:
-        return f'<{self.__class__.__name__} scores={len(self._scores)}>'
+        return f"<{self.__class__.__name__} scores={len(self._scores)}>"
 
     def __next__(self) -> Score:
         try:
             score: Score = self._scores[self._index]
         except IndexError:
             raise StopIteration
         self._index += 1
         return score
 
 
 class Leaderboard:
     """Represents an in-game leaderboard."""
-    __slots__ = (
-        '_method',
-        '_mapname',
-        '_mode',
-        '_difficulty',
-        '_total',
-        'raw',
-        '_date',
-        '_season',
-        '_player',
 
-        '_scores',
+    __slots__ = (
+        "_method",
+        "_mapname",
+        "_mode",
+        "_difficulty",
+        "_total",
+        "raw",
+        "_date",
+        "_season",
+        "_player",
+        "_scores",
     )
 
     def __init__(
         self,
         method: str,
         mapname: str,
         mode: str,
         difficulty: str,
         total: Union[int, str],
         *,
         raw: Dict[str, Any],
         date: Optional[str] = None,
         player: Optional[Score] = None,
-        season: Optional[int] = None
+        season: Optional[int] = None,
     ) -> None:
         self._method = method
         self._mapname = mapname
         self._mode = mode
         self._difficulty = difficulty
         self._total = int(total)
         self.raw = raw
@@ -87,29 +78,38 @@
         mapname: str,
         mode: str,
         difficulty: str,
         playerid: Optional[str],
         payload: Dict[str, Any],
         *,
         date: Optional[str] = None,
-        season: Optional[int] = None
+        season: Optional[int] = None,
     ) -> Leaderboard:
-        '''Builds an instance with the given payload.'''
-        player: Dict[str, Any] = payload['player']
-        total: int = player['total']
-        if playerid is not None and (player['score'] and player['rank'] and total):
-            player_score = Score(method, mapname, mode,
-                                 difficulty, playerid, **player)
+        """Builds an instance with the given payload."""
+        player: Dict[str, Any] = payload["player"]
+        total: int = player["total"]
+        if playerid is not None and (player["score"] and player["rank"] and total):
+            player_score = Score(method, mapname, mode, difficulty, playerid, **player)
         else:
             player_score = None
-        instance = cls(method, mapname, mode, difficulty, total,
-                       raw=payload, date=date, player=player_score, season=season)
-        for rank, score in enumerate(payload['leaderboards'], start=1):
-            instance._append(Score(method, mapname, mode,
-                             difficulty, rank=rank, **score))
+        instance = cls(
+            method,
+            mapname,
+            mode,
+            difficulty,
+            total,
+            raw=payload,
+            date=date,
+            player=player_score,
+            season=season,
+        )
+        for rank, score in enumerate(payload["leaderboards"], start=1):
+            instance._append(
+                Score(method, mapname, mode, difficulty, rank=rank, **score)
+            )
         return instance
 
     @property
     def method(self) -> str:
         """The name of the method responsible for creating this leaderboard."""
         return self._method
 
@@ -151,45 +151,45 @@
     @property
     def is_empty(self) -> bool:
         """Whether there are no scores saved in this leaderboard or there are."""
         return not self._scores
 
     def format_scores(self) -> str:
         """Default format used in my Advinas Bot. To format the scores yourself, iterate over this object."""
-        return '\n'.join([i.format_score() for i in self._scores])
+        return "\n".join([i.format_score() for i in self._scores])
 
     def print_scores(self) -> None:
         """Prints out the result of format_scores()."""
         print(self.format_scores())
 
     def get_score(self, attr: str, val: Any) -> Optional[Score]:
         """Returns the score in the leaderboard where the given attribute equals the given value."""
         return next((x for x in self._scores if getattr(x, attr, None) == val), None)
 
     def _append(self, score: Score) -> None:
-        '''Internal append method.'''
+        """Internal append method."""
         self._scores.append(score)
 
     # magic methods
 
     def __repr__(self) -> str:
         attrs = {
-            'method': self._method,
-            'mapname': self._mapname,
-            'mode': self._mode,
-            'difficulty': self._difficulty,
-            'total': self._total,
-            'scores': len(self._scores),
+            "method": self._method,
+            "mapname": self._mapname,
+            "mode": self._mode,
+            "difficulty": self._difficulty,
+            "total": self._total,
+            "scores": len(self._scores),
             # Fine to include these 3, when they are not None.
-            'date': self._date,
-            'season': self._season,
-            'player': True if self._player is not None else None
+            "date": self._date,
+            "season": self._season,
+            "player": True if self._player is not None else None,
         }
-        inner = ' '.join(f'{k}={v}' for k, v in attrs.items() if v is not None)
-        return f'<{self.__class__.__name__} {inner}>'
+        inner = " ".join(f"{k}={v}" for k, v in attrs.items() if v is not None)
+        return f"<{self.__class__.__name__} {inner}>"
 
     def __len__(self) -> int:
         return len(self._scores)
 
     def __contains__(self, item: Any) -> bool:
         return item in self._scores
 
@@ -202,17 +202,24 @@
         ...
 
     def __getitem__(self, key: Any) -> Union[Score, Leaderboard]:
         if isinstance(key, int):
             return self._scores[key]
         elif isinstance(key, slice):
             lb = Leaderboard(
-                self._method, self._mapname, self._mode, self._difficulty, self._total,
-                raw=self.raw, date=self._date, player=self._player, season=self._season
+                self._method,
+                self._mapname,
+                self._mode,
+                self._difficulty,
+                self._total,
+                raw=self.raw,
+                date=self._date,
+                player=self._player,
+                season=self._season,
             )
             lb._scores = self._scores[key]
             return lb
         else:
-            raise KeyError('Only int and slice indexes are allowed.')
+            raise KeyError("Only int and slice indexes are allowed.")
 
     def __iter__(self) -> Leaderboard_iterator:
         return Leaderboard_iterator(self._scores)
```

### Comparing `infinitode.py-1.0.4/infinitode/player.py` & `infinitode.py-1.0.5/infinitode/player.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,77 @@
 from __future__ import annotations
 
 # std
-from typing import (
-    Dict,
-    Optional,
-    Union,
-    Tuple,
-    TYPE_CHECKING
-)
+from typing import Dict, Optional, Union, Tuple, TYPE_CHECKING
 
 # local
 from .score import Score
 from .errors import InfinitodeError
 from .utils import MISSING
 
 if TYPE_CHECKING:
     from .core import Session
 
 
-__all__ = ('Player',)
+__all__ = ("Player",)
 
 
 class Player:
     """Represents an in-game Player."""
-    __slots__ = (
-        '_playerid',
-        '_nickname',
-        '_levels',
-        '_level',
-        '_xp',
-        '_xp_max',
-        '_badges',
-        '_total_score',
-        '_total_rank',
-        '_total_top',
-        '_replays',
-        '_issues',
-        '_created_at',
 
-        '_daily_quest',
-        '_skill_point'
+    __slots__ = (
+        "_playerid",
+        "_nickname",
+        "_levels",
+        "_level",
+        "_xp",
+        "_xp_max",
+        "_season_level",
+        "_season_xp",
+        "_season_xp_max",
+        "_badges",
+        "_total_score",
+        "_total_rank",
+        "_total_top",
+        "_replays",
+        "_issues",
+        "_created_at",
+        "_daily_quest",
+        "_skill_point",
     )
 
     def __init__(
         self,
         playerid: str,
         nickname: str,
         *,
         levels: Dict[str, Score],
         level: int,
         xp: int,
         xp_max: int,
+        season_level: int,
+        season_xp: int,
+        season_xp_max: int,
         badges: Dict[str, Tuple[str, str]],
         total_score: Union[int, str],
         total_rank: Union[int, str],
         total_top: str,
         replays: int,
         issues: int,
         created_at: str,
     ) -> None:
         self._playerid = playerid
         self._nickname = nickname
         self._levels = levels
         self._level = level
         self._xp = xp
         self._xp_max = xp_max
+        self._season_level = season_level
+        self._season_xp = season_xp
+        self._season_xp_max = season_xp_max
         self._badges = badges
         self._total_score = int(total_score)
         self._total_rank = int(total_rank)
         self._total_top = total_top
         self._replays = replays
         self._issues = issues
         self._created_at = created_at
@@ -97,17 +100,32 @@
 
     @property
     def xp_max(self) -> int:
         """The XP required for the player to level up."""
         return self._xp_max
 
     @property
+    def season_level(self) -> int:
+        """The player's season XP level."""
+        return self._season_level
+
+    @property
+    def season_xp(self) -> int:
+        """The player's XP in the current season level."""
+        return self._season_xp
+
+    @property
+    def season_xp_max(self) -> int:
+        """The season XP required for the player to level up."""
+        return self._season_xp_max
+
+    @property
     def badges(self) -> Dict[str, Tuple[str, str]]:
         """
-        The player's badges as a dict in the form: 
+        The player's badges as a dict in the form:
             type: (rarity, colour)
         """
         return self._badges
 
     @property
     def total_score(self) -> int:
         """The player's total (seasonal) score."""
@@ -137,77 +155,97 @@
     def created_at(self) -> str:
         """The player's creation date as a str in the format: '%Y-%m-%d'."""
         return self._created_at
 
     @property
     def avatar_link(self):
         """The link to the player's avatar. Invalid URL if the user doesn't have a pfp."""
-        return f'https://infinitode.prineside.com/img/avatars/{self._playerid}-128.png'
+        return f"https://infinitode.prineside.com/img/avatars/{self._playerid}-128.png"
 
     @property
     def daily_quest(self):
         """Returns the player's daily quest score, or raises InfinitodeError if it wasn't fetched yet."""
         if self._daily_quest is MISSING:
             raise InfinitodeError(
-                'This score has not been fetched yet. Use ~.fetch_daily_quest first.')
+                "This score has not been fetched yet. Use ~.fetch_daily_quest first."
+            )
         else:
             return self._daily_quest
 
     @property
     def skill_point(self):
         """Returns the player's daily quest score, or raises InfinitodeError if it wasn't fetched yet."""
         if self._skill_point is MISSING:
             raise InfinitodeError(
-                'This score has not been fetched yet. Use ~.fetch_skill_point first.')
+                "This score has not been fetched yet. Use ~.fetch_skill_point first."
+            )
         else:
             return self._skill_point
 
     def score(self, mapname: str) -> Score:
         """Returns the player's score on the given map."""
         try:
             return self._levels[mapname]
         except KeyError:
             self._levels[mapname] = Score(
-                'player', mapname, 'score', 'NORMAL', self._playerid,
-                rank=0, score=0, total=0, top='-%')
+                "player",
+                mapname,
+                "score",
+                "NORMAL",
+                self._playerid,
+                rank=0,
+                score=0,
+                total=0,
+                top="-%",
+            )
             return self._levels[mapname]
 
-    async def fetch_daily_quest(self, session: Optional[Session] = None) -> Optional[Score]:
+    async def fetch_daily_quest(
+        self, session: Optional[Session] = None
+    ) -> Optional[Score]:
         """
         Fetches the player's Daily Quest score if it wasn't fetched already.
         Returns None if the player is not ranked.
         """
         if not self._daily_quest:
             if session is None:
                 if self._daily_quest is MISSING:
                     raise InfinitodeError(
-                        'You need to provide a Session to fetch the daily quest score.')
+                        "You need to provide a Session to fetch the daily quest score."
+                    )
                 else:
                     return self._daily_quest
-            self._daily_quest = (await session.daily_quest_leaderboards(playerid=self._playerid)).player
+            self._daily_quest = (
+                await session.daily_quest_leaderboards(playerid=self._playerid)
+            ).player
         return self._daily_quest
 
-    async def fetch_skill_point(self, session: Optional[Session] = None) -> Optional[Score]:
+    async def fetch_skill_point(
+        self, session: Optional[Session] = None
+    ) -> Optional[Score]:
         """
         Fetches the player's Skill Point score if it wasn't fetched already.
         Returns None if the player is not ranked.
         """
         if not self._skill_point:
             if session is None:
                 if self._skill_point is MISSING:
                     raise InfinitodeError(
-                        'You need to provide a Session to fetch the skill point score.')
+                        "You need to provide a Session to fetch the skill point score."
+                    )
                 else:
                     return self._skill_point
-            self._skill_point = (await session.skill_point_leaderboard(playerid=self._playerid)).player
+            self._skill_point = (
+                await session.skill_point_leaderboard(playerid=self._playerid)
+            ).player
         return self._skill_point
 
     # magic methods
 
     def __repr__(self) -> str:
         attrs = {
-            'playerid': self._playerid,
-            'nickname': self._nickname,
-            'total_rank': self._total_rank,
+            "playerid": self._playerid,
+            "nickname": self._nickname,
+            "total_rank": self._total_rank,
         }
-        inner = ' '.join(f'{k}={v}' for k, v in attrs.items())
-        return f'<{self.__class__.__name__} {inner}>'
+        inner = " ".join(f"{k}={v}" for k, v in attrs.items())
+        return f"<{self.__class__.__name__} {inner}>"
```

### Comparing `infinitode.py-1.0.4/infinitode/score.py` & `infinitode.py-1.0.5/infinitode/score.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 from __future__ import annotations
 
 # std
-from typing import (
-    Any,
-    Dict,
-    Optional,
-    Union,
-    TYPE_CHECKING
-)
+from typing import Any, Dict, Optional, Union, TYPE_CHECKING
 
 # local
 from .errors import InfinitodeError
 from .badge import Badge
 
 if TYPE_CHECKING:
     from .core import Session
     from .player import Player
 
-__all__ = ('Score',)
+__all__ = ("Score",)
 
 
 class Score:
     """Represents a single in-game Score."""
+
     __slots__ = (
-        '_method',
-        '_mapname',
-        '_mode',
-        '_difficulty',
-        '_playerid',
-        '_rank',
-        '_score',
-        'raw',
-        '_has_pfp',
-        '_level',
-        '_nickname',
-        '_pinned_badge',
-        '_position',
-        '_top',
-        '_total',
-        '_player',
+        "_method",
+        "_mapname",
+        "_mode",
+        "_difficulty",
+        "_playerid",
+        "_rank",
+        "_score",
+        "raw",
+        "_has_pfp",
+        "_level",
+        "_nickname",
+        "_pinned_badge",
+        "_position",
+        "_top",
+        "_total",
+        "_player",
     )
 
     def __init__(
         self,
         method: str,
         mapname: str,
         mode: str,
@@ -54,28 +49,32 @@
         hasPfp: Optional[bool] = None,
         level: Optional[int] = None,
         nickname: Optional[str] = None,
         pinnedBadge: Optional[Dict[str, str]] = None,
         position: Optional[int] = None,
         top: Optional[str] = None,
         total: Optional[Union[str, int]] = None,
-        player: Optional[Player] = None
+        player: Optional[Player] = None,
     ) -> None:
         self._method = method
         self._mapname = mapname
         self._mode = mode
         self._difficulty = difficulty
         self._playerid = playerid
         self._rank = int(rank)
         self._score = int(score)
         self._has_pfp = hasPfp
         self._level = level
         self._nickname = nickname
-        self._pinned_badge: Optional[Badge] = Badge(**pinnedBadge) if pinnedBadge is not None else None  # nopep8
-        self._position: Optional[int] = int(position) if position is not None else None  # nopep8
+        self._pinned_badge: Optional[Badge] = (
+            Badge(**pinnedBadge) if pinnedBadge is not None else None
+        )  # nopep8
+        self._position: Optional[int] = (
+            int(position) if position is not None else None
+        )  # nopep8
         self._top = top
         # apparently some payloads provide total, but i think it is pointless as a property
         # so i will keep it as a private attribute just in case it will ever be needed
         self._total: Optional[int] = int(total) if total is not None else None
         self._player = player
 
     @classmethod
@@ -83,18 +82,18 @@
         cls,
         # a standalone score payload is only received from the leaderboards rank call
         method: str,
         mapname: str,
         mode: str,
         difficulty: str,
         playerid: str,
-        payload: Dict[str, Any]
+        payload: Dict[str, Any],
     ) -> Score:
-        ''''Builds an instance with the given payload.'''
-        score: Dict[str, Any] = payload['player']
+        """'Builds an instance with the given payload."""
+        score: Dict[str, Any] = payload["player"]
         return cls(method, mapname, mode, difficulty, playerid, **score)
 
     @property
     def method(self) -> str:
         """The name of the method responsible for creating this Score."""
         return self._method
 
@@ -169,36 +168,42 @@
             self._player = await session.player(self._playerid)
         return self._player
 
     def format_score(self):
         """Formats the score the way i use it in my Advinas bot."""
         if self._nickname is None:
             raise InfinitodeError(
-                'The score is not valid for formatting (There is no nickname attached to this score).')
-        return '#{:<5} {:<22} {:>0,}'.format(self._rank, self._nickname if len(self._nickname) < 21 else f"{self._nickname[:19]}...", self._score)
+                "The score is not valid for formatting (There is no nickname attached to this score)."
+            )
+        return "#{:<5} {:<22} {:>0,}".format(
+            self._rank,
+            self._nickname if len(self._nickname) < 21 else f"{self._nickname[:19]}...",
+            self._score,
+        )
 
     def print_score(self):
+        """Prints out the result of format_score()."""
         print(self.format_score())
 
     # magic methods
 
     def __repr__(self) -> str:
         attrs = {
-            'method': self._method,
-            'mapname': self._mapname,
-            'mode': self._mode,
-            'difficulty': self._difficulty,
-            'playerid': self._playerid,
-            'rank': self._rank,
-            'score': self._score,
+            "method": self._method,
+            "mapname": self._mapname,
+            "mode": self._mode,
+            "difficulty": self._difficulty,
+            "playerid": self._playerid,
+            "rank": self._rank,
+            "score": self._score,
             # only include the "important" attributes.
             # 'has_pfp': self._has_pfp,
             # 'level': self._level,
             # 'nickname': self._nickname,
             # 'pinned_badge': self._pinned_badge,
             # 'position': self._position,
             # 'top': self._top,
             # 'total': self._total,
             # 'player': True if self._player is not None else None
         }
-        inner = ' '.join(f'{k}={v}' for k, v in attrs.items())
-        return f'<{self.__class__.__name__} {inner}>'
+        inner = " ".join(f"{k}={v}" for k, v in attrs.items())
+        return f"<{self.__class__.__name__} {inner}>"
```

### Comparing `infinitode.py-1.0.4/infinitode/utils.py` & `infinitode.py-1.0.5/infinitode/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from __future__ import annotations
 
 # std
 from typing import Any
 
-__all__ = (
-    'MISSING',
-    'try_int'
-)
+__all__ = ("MISSING", "try_int")
 
 
 def try_int(string: str, /, *, default: int = 0) -> int:
     try:
         return int(string)
     except ValueError:
         return default
@@ -26,11 +23,11 @@
     def __bool__(self):
         return False
 
     def __hash__(self):
         return 0
 
     def __repr__(self):
-        return '...'
+        return "..."
 
 
 MISSING: Any = _MissingSentinel()
```

### Comparing `infinitode.py-1.0.4/infinitode.py.egg-info/PKG-INFO` & `infinitode.py-1.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: infinitode.py
-Version: 1.0.4
-Summary: A python wrapper for the Infinitode 2 API.
-Home-page: https://github.com/Sprylos/infinitode.py
-Author: Sprylos
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Infinitode.py
 
 An asynchronous python wrapper for the Infinitode-2 API using `async`-`await` syntax.
 
 ## Installing
 
 ---
@@ -112,15 +101,18 @@
         # The last main object is a Player, received only be Session.player()
         # Every Player has the same attributes.
         print(
             player.playerid,
             player.nickname,
             player.level,
             player.xp,
-            player.xp_max,  # xp required per level (always 1000?)
+            player.xp_max,  # xp required per level
+            player.season_level,
+            player.season_xp,
+            player.season_xp_max,
             player.total_score,
             player.total_rank,
             player.total_top,
             player.replays,
             player.issues,
             player.created_at,  # as str
             player.avatar_link  # even when the person has no pfp
@@ -154,9 +146,7 @@
 
 async def main():
     async with infinitode.Session() as API:
         await API.leaderboards('6.3')  # just an example
 
 asyncio.run(main())
 ```
-
-
```

### Comparing `infinitode.py-1.0.4/setup.py` & `infinitode.py-1.0.5/setup.py`

 * *Files identical despite different names*

