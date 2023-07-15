# Comparing `tmp/basketcase-4.0.0.tar.gz` & `tmp/basketcase-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "basketcase-5.0.0.tar", last modified: Sat Jul 15 05:41:04 2023, max compression
```

## Comparing `basketcase-4.0.0.tar` & `basketcase-5.0.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 basketcase-4.0.0/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 basketcase-4.0.0/src/basketcase/__init__.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 basketcase-4.0.0/src/basketcase/__main__.py
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 basketcase-4.0.0/src/basketcase/authenticator.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 basketcase-4.0.0/src/basketcase/basketcase.py
--rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 basketcase-4.0.0/src/basketcase/extractor.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 basketcase-4.0.0/src/basketcase/storage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 basketcase-4.0.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 basketcase-4.0.0/tests/extractor/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 basketcase-4.0.0/tests/extractor/test.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 basketcase-4.0.0/tests/extractor/sample/__init__.py
--rw-r--r--   0        0        0    33804 2020-02-02 00:00:00.000000 basketcase-4.0.0/tests/extractor/sample/api.json
--rw-r--r--   0        0        0   283205 2020-02-02 00:00:00.000000 basketcase-4.0.0/tests/extractor/sample/response.html
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 basketcase-4.0.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 basketcase-4.0.0/LICENSE
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 basketcase-4.0.0/README.md
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 basketcase-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 basketcase-4.0.0/PKG-INFO
+drwxr-xr-x   0 dsilva    (1000) dsilva    (1000)        0 2023-07-15 05:41:04.388985 basketcase-5.0.0/
+-rw-r--r--   0 dsilva    (1000) dsilva    (1000)    35149 2023-06-27 20:26:22.000000 basketcase-5.0.0/LICENSE
+-rw-r--r--   0 dsilva    (1000) dsilva    (1000)    44141 2023-07-15 05:41:04.388985 basketcase-5.0.0/PKG-INFO
+-rw-r--r--   0 dsilva    (1000) dsilva    (1000)     3019 2023-07-15 05:33:45.000000 basketcase-5.0.0/README.md
+-rw-r--r--   0 dsilva    (1000) dsilva    (1000)      780 2023-07-15 05:37:15.000000 basketcase-5.0.0/pyproject.toml
+-rw-r--r--   0 dsilva    (1000) dsilva    (1000)       38 2023-07-15 05:41:04.388985 basketcase-5.0.0/setup.cfg
+drwxr-xr-x   0 dsilva    (1000) dsilva    (1000)        0 2023-07-15 05:41:04.385985 basketcase-5.0.0/src/
+drwxr-xr-x   0 dsilva    (1000) dsilva    (1000)        0 2023-07-15 05:41:04.387985 basketcase-5.0.0/src/basketcase/
+-rw-r--r--   0 dsilva    (1000) dsilva    (1000)        0 2023-06-27 20:26:23.000000 basketcase-5.0.0/src/basketcase/__init__.py
+-rw-r--r--   0 dsilva    (1000) dsilva    (1000)     3681 2023-07-15 04:27:16.000000 basketcase-5.0.0/src/basketcase/__main__.py
+-rw-r--r--   0 dsilva    (1000) dsilva    (1000)     2281 2023-07-15 03:16:24.000000 basketcase-5.0.0/src/basketcase/authenticator.py
+-rw-r--r--   0 dsilva    (1000) dsilva    (1000)     2319 2023-07-15 04:30:50.000000 basketcase-5.0.0/src/basketcase/basketcase.py
+-rw-r--r--   0 dsilva    (1000) dsilva    (1000)     7188 2023-07-15 02:15:39.000000 basketcase-5.0.0/src/basketcase/extractor.py
+-rw-r--r--   0 dsilva    (1000) dsilva    (1000)     2984 2023-07-15 01:38:25.000000 basketcase-5.0.0/src/basketcase/storage.py
+drwxr-xr-x   0 dsilva    (1000) dsilva    (1000)        0 2023-07-15 05:41:04.387985 basketcase-5.0.0/src/basketcase.egg-info/
+-rw-r--r--   0 dsilva    (1000) dsilva    (1000)    44141 2023-07-15 05:41:04.000000 basketcase-5.0.0/src/basketcase.egg-info/PKG-INFO
+-rw-r--r--   0 dsilva    (1000) dsilva    (1000)      431 2023-07-15 05:41:04.000000 basketcase-5.0.0/src/basketcase.egg-info/SOURCES.txt
+-rw-r--r--   0 dsilva    (1000) dsilva    (1000)        1 2023-07-15 05:41:04.000000 basketcase-5.0.0/src/basketcase.egg-info/dependency_links.txt
+-rw-r--r--   0 dsilva    (1000) dsilva    (1000)       56 2023-07-15 05:41:04.000000 basketcase-5.0.0/src/basketcase.egg-info/entry_points.txt
+-rw-r--r--   0 dsilva    (1000) dsilva    (1000)       17 2023-07-15 05:41:04.000000 basketcase-5.0.0/src/basketcase.egg-info/requires.txt
+-rw-r--r--   0 dsilva    (1000) dsilva    (1000)       11 2023-07-15 05:41:04.000000 basketcase-5.0.0/src/basketcase.egg-info/top_level.txt
```

### Comparing `basketcase-4.0.0/src/basketcase/__main__.py` & `basketcase-5.0.0/src/basketcase/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -54,58 +54,76 @@
         '--set-default-session',
         help='Set the specified session as the default then exit',
         metavar='SESSION_ID',
         type=int
     )
     parser.add_argument(
         '--unset-default-session',
-        help='Unset the default session flag then exit',
+        help='Unset the default session then exit',
+        action='store_true'
+    )
+    parser.add_argument(
+        '--no-session',
+        help="Don't use a session",
         action='store_true'
     )
     parser.add_argument(
         '--force',
         help='Ignore failed downloads',
         action='store_true',
         default=False
     )
     args = parser.parse_args()
 
     bc = basketcase.BasketCase(force_flag=args.force)
 
     if args.list_sessions:
-        bc.authenticator.list_sessions()
+        sessions = bc.authenticator.get_sessions()
+
+        for session in sessions:
+            print(f'{session["rowid"]!s}: {session["description"]}')
+
         return 0
-    elif args.set_default_session:
+
+    if args.set_default_session:
         bc.authenticator.set_default_session(args.set_default_session)
         print(f'Session marked as default: {args.set_default_session}')
         return 0
-    elif args.unset_default_session:
+
+    if args.unset_default_session:
         bc.authenticator.unset_default_session()
-        print(f'Default session flag removed')
+        print(f'Default session mark removed')
         return 0
-    elif args.forget_session:
-        bc.authenticator.delete_session(args.forget_session)
+
+    if args.forget_session:
+        bc.authenticator.forget_session(args.forget_session)
         print(f'Removed session id: {args.forget_session}')
         return 0
-    elif args.cookie:
-        description = ''
+
+    if args.cookie:
+        session = {
+            'description': '',
+            'cookie_id': args.cookie,
+            'is_default': 0
+        }
 
         if args.cookie_name:
-            description = args.cookie_name
+            session['description'] = args.cookie_name
         else:
-            description = input('Provide a short name to identify this cookie: ')
+            session['description'] = input('Provide a short name to identify this cookie: ')
 
-        session_id = bc.authenticator.new_session(args.cookie, description, False)
+        session_id = bc.authenticator.new_session(session)
         print(f'Added session id: {session_id}')
         return 0
 
-    if args.session:
-        bc.authenticator.load_session(args.session)
-    else:
-        bc.authenticator.load_default_session()
+    if not args.no_session:
+        if args.session:
+            bc.authenticator.load_session(args.session)
+        else:
+            bc.authenticator.load_default()
 
     urls = set()
 
     if args.file:
         for line in args.file:
             line = line.rstrip()
 
@@ -117,8 +135,9 @@
         raise RuntimeError('Use at least one of the arguments: --url, --input-file')
 
     bc.fetch(urls)
     return 0
 
 
 if __name__ == '__main__':
-    sys.exit(main())
+    exit_code = main()
+    sys.exit(exit_code)
```

### Comparing `basketcase-4.0.0/src/basketcase/authenticator.py` & `basketcase-5.0.0/src/basketcase/authenticator.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,83 +7,76 @@
 
 class Authenticator:
     def __init__(
         self,
         http_client: 'requests.Session',
         storage_manager: 'storage.Storage'
     ):
-        self._http_client = http_client
-        self._storage = storage_manager
+        self.http_client = http_client
+        self.storage = storage_manager
 
-    def new_session(
-            self,
-            cookie_id: str,
-            description: str,
-            is_default: bool
-    ) -> int:
-        session_id = self._storage.insert(description, cookie_id, is_default)
-        return session_id
-    
-    def list_sessions(self):
-        sessions = self._storage.get_all()
-
-        for session in sessions:
-            description = session['first_used']
-
-            if session['description']:
-                description = session['description']
-            
-            if session['is_default']:
-                description += ' (default)'
-
-            print(f'{session["rowid"]!s}: {description}')
-
-    def delete_session(self, id: int):
-        session = self._storage.get_one_by_id(id)
+    def load_session(self, session_id: int):
+        session = self.storage.get_one_by_id(session_id)
 
         if not session:
-            raise RuntimeError(f'Session not found')
-        
-        self._storage.delete(session)
+            raise RuntimeError('Session not found')
 
-    def load_session(self, id: int):
-        session = self._storage.get_one_by_id(id)
+        self.http_client.cookies.set('sessionid', session['cookie_id'])
 
-        if session:
-            self._http_client.cookies.set('sessionid', session['cookie_id'])
+    def load_default(self):
+        """Load the default session, if one exists"""
 
-    def load_default_session(self):
-        sessions = self._storage.get_all()
+        sessions = self.storage.get_all()
 
         if len(sessions) == 1:
             # A single session is treated as the default
-            self._http_client.cookies.set('sessionid', sessions[0]['cookie_id'])
+            self.http_client.cookies.set('sessionid', sessions[0]['cookie_id'])
         else:
             for session in sessions:
                 if not session['is_default']:
                     continue
 
-                self._http_client.cookies.set('sessionid', session['cookie_id'])
+                self.http_client.cookies.set('sessionid', session['cookie_id'])
 
-    def set_default_session(self, id: int):
-        session = self._storage.get_one_by_id(id)
+    def get_sessions(self) -> list:
+        sessions = list()
+
+        for session in self.storage.get_all():
+            description = session['first_used']
+
+            if session['description']:
+                description = session['description']
+
+            if session['is_default']:
+                description += ' (default)'
+
+            session['description'] = description
+            sessions.append(session)
+
+        return sessions
+
+    def set_default_session(self, session_id: int):
+        session = self.storage.get_one_by_id(session_id)
 
         if not session:
-            raise RuntimeError(f'Session not found')
+            raise RuntimeError('Session not found')
 
         if session['is_default']:
             raise RuntimeError('Session is already default')
 
-        self._storage.reset_default()
+        session['is_default'] = 1
+        self.storage.update(session)
 
-        session_dict = {
-            'rowid': session['rowid'],
-            'description': session['description'],
-            'cookie_id': session['cookie_id'],
-            'is_default': session['is_default'],
-        }
-
-        session_dict['is_default'] = 1
-        self._storage.update(session_dict)
-    
     def unset_default_session(self):
-        self._storage.reset_default()
+        self.storage.reset_default()
+
+    def forget_session(self, session_id: int):
+        session = self.storage.get_one_by_id(session_id)
+
+        if not session:
+            raise RuntimeError('Session not found')
+
+        self.storage.delete(session)
+
+    def new_session(self, session: dict):
+        session_id = self.storage.insert(session)
+        return session_id
```

### Comparing `basketcase-4.0.0/src/basketcase/basketcase.py` & `basketcase-5.0.0/src/basketcase/basketcase.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,65 @@
-from __future__ import unicode_literals
-import yt_dlp
-
-from PIL import Image
-from io import BytesIO
+import stat
 from pathlib import Path
 from datetime import datetime
 import requests
 
 from . import extractor
-from . import storage
 from . import authenticator
+from . import storage
 
 
 class BasketCase:
-    def __init__(self, force_flag = False):
+    def __init__(
+        self,
+        force_flag: bool = False
+    ):
         # Create application data directory
-        self._data_directory = f'{Path.home()!s}/.basketcase'
-        Path(self._data_directory).mkdir(parents=True, exist_ok=True)
-
-        # Set output path
-        self._output_base = f'{Path.cwd()!s}/basketcase_{datetime.now()!s}'
-        self._output_images = self._output_base + '/images'
-        self._output_videos = self._output_base + '/videos'
+        self.data_dir = f'{Path.home()!s}/.basketcase'
+        Path(self.data_dir).mkdir(parents=True, exist_ok=True)
+        Path(self.data_dir).chmod(stat.S_IRWXU)
+
+        # Set output directory
+        output_name = f'basketcase_downloads/{datetime.now()!s}'
+        self.output_dir = f'{Path.cwd()!s}/{output_name}'
 
         # Initialize dependencies
-        self._storage = storage.Storage(self._data_directory)
-        self._http_client = requests.Session()
-        self.authenticator = authenticator.Authenticator(self._http_client, self._storage)
-        self.extractor = extractor.Extractor(http_client=self._http_client, force=force_flag)
+        self.http_client = requests.Session()
+        self.storage = storage.Storage(self.data_dir)
+        self.authenticator = authenticator.Authenticator(self.http_client, self.storage)
+        self.extractor = extractor.Extractor(http_client=self.http_client, force=force_flag)
 
-    def fetch(self, target_urls):
+    def fetch(self, target_urls: set):
         resources = self.extractor.scan(target_urls)
 
         if resources['images'] or resources['videos']:
-            # Create media output directories
-            Path(self._output_images).mkdir(parents=True, exist_ok=True)
-            Path(self._output_videos).mkdir(parents=True, exist_ok=True)
-
             for index, resource in resources['images'].items():
-                self._get_image(resource)
-            
-            self._get_videos(resources['videos'])
+                self.get_image(resource)
+
+            for index, resource in resources['videos'].items():
+                self.get_video(resource)
         else:
             print('Nothing to download.')
 
-    def _get_image(self, resource):
-        print(f'Downloading image: {resource["url"]}')
+    def get_image(self, resource: dict):
+        user_dir = f'{self.output_dir}/{resource["username"]}'
+        Path(user_dir).mkdir(parents=True, exist_ok=True)
+
+        print(f'Downloading image: {resource["username"]}/{resource["id"]}')
 
-        image = None
+        with self.http_client.get(resource['url'], timeout=10) as response:
+            response.raise_for_status()
 
-        with self._http_client.get(resource['url'], timeout=10) as request:
-            # Build image from binary response data
-            image = Image.open(BytesIO(request.content))
+            with open(f'{user_dir}/{resource["id"]}.jpg', mode='w+b') as file:
+                file.write(response.content)
 
-        image.save(f'{self._output_images}/{resource["id"]}.jpg', format='JPEG')
+    def get_video(self, resource: dict):
+        user_dir = f'{self.output_dir}/{resource["username"]}'
+        Path(user_dir).mkdir(parents=True, exist_ok=True)
 
-    def _get_videos(self, urls):
-        if self._http_client.cookies.get('sessionid'):
-            # Add the session cookie
-            yt_dlp.utils.std_headers.update({'Cookie': 'sessionid=' + self._http_client.cookies.get('sessionid')})
+        print(f'Downloading video: {resource["username"]}/{resource["id"]}')
 
-        ydl_opts = {
-            'outtmpl': self._output_videos + '/%(title)s.%(ext)s'  # Set output directory
-        }
+        with self.http_client.get(resource['url'], timeout=10) as response:
+            response.raise_for_status()
 
-        with yt_dlp.YoutubeDL(ydl_opts) as ydl:
-            ydl.download(urls)
+            with open(file=f'{user_dir}/{resource["id"]}.mp4', mode='w+b') as file:
+                file.write(response.content)
```

### Comparing `basketcase-4.0.0/src/basketcase/storage.py` & `basketcase-5.0.0/src/basketcase/storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,115 +1,120 @@
 import sqlite3
 
 
+def dict_factory(cursor, row):
+    fields = [column[0] for column in cursor.description]
+    return {key: value for key, value in zip(fields, row)}
+
+
 class Storage:
-    """Database handler for internal program data."""
+    """Database handler for internal program data"""
 
-    def __init__(self, base_directory):
-        self._connection = sqlite3.connect(f'{base_directory}/data.db')
-        self._connection.row_factory = sqlite3.Row
-        self._initialize()
+    def __init__(self, base_dir: str):
+        self.connection = sqlite3.connect(f'{base_dir}/data.db')
+        self.connection.row_factory = dict_factory
+        self.initialize()
 
-    def _initialize(self):
-        cursor = self._connection.cursor()
+    def initialize(self):
+        cursor = self.connection.cursor()
 
         cursor.execute('''
             CREATE TABLE IF NOT EXISTS session (
                 description TEXT,
                 cookie_id TEXT,
                 is_default INTEGER,
                 first_used TEXT
-            );
+            )
         ''')
 
-        self._connection.commit()
-    
-    def insert(self, description, cookie_id, is_default = False):
-        cursor = self._connection.cursor()
+        self.connection.commit()
+
+    def get_one_by_id(self, rowid: int) -> dict | None:
+        cursor = self.connection.cursor()
 
         cursor.execute('''
-            INSERT INTO session (
-                description,
-                cookie_id,
-                is_default,
-                first_used
-            ) VALUES (
-                :description,
-                :cookie_id,
-                :is_default,
-                datetime()
-            );
+            SELECT rowid, * FROM session
+            WHERE rowid = :rowid
         ''', {
-            'description': description,
-            'cookie_id': cookie_id,
-            'is_default': int(is_default)
+            'rowid': rowid
         })
 
-        self._connection.commit()
+        session = cursor.fetchone()
 
-        return cursor.lastrowid
-    
-    def update(self, session):
-        cursor = self._connection.cursor()
+        if not session:
+            return None
+
+        return session
+
+    def get_all(self) -> list:
+        cursor = self.connection.cursor()
+
+        cursor.execute('''
+            SELECT rowid, * FROM session
+        ''')
+
+        return cursor.fetchall()
+
+    def update(self, session: dict):
+        cursor = self.connection.cursor()
 
         cursor.execute('''
             UPDATE session SET
                 description = :description,
                 cookie_id = :cookie_id,
                 is_default = :is_default
-            WHERE rowid = :id
+            WHERE rowid = :rowid
         ''', {
-            'id': session['rowid'],
+            'rowid': session['rowid'],
             'description': session['description'],
             'cookie_id': session['cookie_id'],
             'is_default': session['is_default']
         })
 
-        self._connection.commit()
+        self.connection.commit()
+
+    def insert(self, session: dict) -> int:
+        cursor = self.connection.cursor()
+
+        cursor.execute('''
+            INSERT INTO session (
+                description,
+                cookie_id,
+                is_default,
+                first_used
+            ) VALUES (
+                :description,
+                :cookie_id,
+                :is_default,
+                datetime()
+            )
+        ''', {
+            'description': session['description'],
+            'cookie_id': session['cookie_id'],
+            'is_default': session['is_default']
+        })
+
+        self.connection.commit()
+
+        return cursor.lastrowid
 
     def reset_default(self):
-        cursor = self._connection.cursor()
+        cursor = self.connection.cursor()
 
         cursor.execute('''
             UPDATE session SET
                 is_default = 0
         ''')
 
-        self._connection.commit()
+        self.connection.commit()
 
-    def delete(self, session):
-        cursor = self._connection.cursor()
+    def delete(self, session: dict):
+        cursor = self.connection.cursor()
 
         cursor.execute('''
             DELETE FROM session
-            WHERE rowid = :id
-        ''', {
-            'id': session['rowid']
-        })
-
-        self._connection.commit()
-    
-    def get_one_by_id(self, id):
-        cursor = self._connection.cursor()
-
-        cursor.execute('''
-            SELECT rowid, * FROM session
-            WHERE rowid = :id
+            WHERE rowid = :rowid
         ''', {
-            'id': id
+            'rowid': session['rowid']
         })
 
-        session = cursor.fetchone()
-
-        if not session:
-            return None
-    
-        return session
-
-    def get_all(self):
-        cursor = self._connection.cursor()
-
-        cursor.execute('''
-            SELECT rowid, * FROM session
-        ''')
-
-        return cursor.fetchall()
+        self.connection.commit()
```

### Comparing `basketcase-4.0.0/README.md` & `basketcase-5.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,77 @@
 # BasketCase
 Download images and videos from Instagram.
 
+Notable features:
+- Stories can be downloaded without triggering the "seen" flag.
+- Downloads a high quality version of a profile picture.
+
 ## Installation
 Install it from [PyPI](https://pypi.org/project/basketcase/).
 
 ```sh
-pip install basketcase
+pip install --user basketcase
 ```
 
-> This will put the executable `basketcase` on your PATH.
+> This should put the executable `basketcase` on your PATH.
 
-## Usage
+## Command-line usage
 ```sh
 basketcase -u "https://instagram.com/p/<post_id>"
 ```
 
-> Downloaded resources will be stored in the current working directory (i.e. `$PWD/basketcase_{timestamp}/`).
+> Downloaded resources will be stored in the current working directory (i.e. `$PWD/basketcase_downloads`).
 
-To download from multiple URLs, create a text file (e.g. `basketcase.txt`) and populate it with resource URLs
+To download from multiple URLs, create a text file (e.g. `urls.txt`)
+and populate it with resource URLs:
 
 ```
 https://instagram.com/p/<post_id>
 https://instagram.com/reel/<reel_id>
 https://instagram.com/<username>
 ```
 
 ```sh
-basketcase -f ./basketcase.txt
+basketcase -f ./urls.txt
 ```
 
 ### Supported URLs
-| Supported URL | Description |
-| --- | --- |
-| `https://instagram.com/<username>` | User profile. Downloads stories from the past 24 hours. |
-| `https://instagram.com/p/<post_id>` | Standard publication. |
-| `https://instagram.com/reel/<reel_id>` | Reels movie |
-| `https://www.instagram.com/stories/highlights/<highlight_id>/` | A collection of stories, or "highlights" |
-| `https://www.instagram.com/s/<random_characters>` | A shorter type of URL |
+| Supported URL                                                  | Description                                                                      |
+|----------------------------------------------------------------|----------------------------------------------------------------------------------|
+| `https://instagram.com/<username>`                             | User profile. Downloads stories from the past 24 hours, and the profile picture. |
+| `https://instagram.com/p/<post_id>`                            | Standard publication.                                                            |
+| `https://instagram.com/reel/<reel_id>`                         | Reels movie                                                                      |
+| `https://www.instagram.com/stories/highlights/<highlight_id>/` | A collection of stories, or "highlights"                                         |
+| `https://www.instagram.com/s/<random_characters>`              | A shorter type of URL                                                            |
 
 ### Authentication
 1. Add a session cookie
 
 ```sh
-basketcase --cookie <session_cookie_id> --cookie-name "my session cookie"
+basketcase --cookie <session_cookie_id> --cookie-name "my session"
 # Added session id: 1
 ```
 
 2. Specify its identifier when downloading
 
 ```sh
 basketcase -s 1
 ```
 
-> List all available sessions with `basketcase -l`
+> List all available sessions with `basketcase -l`.
+> To disable sessions, use `--no-session`.
+> If only one exists, it is treated as the default.
 
 ## User data
-Cookies and other application data are kept in `~/.basketcase`.
+Cookies and other application data are kept in your home directory (i.e. `~/.basketcase`).
 
 ## Development setup
-1. `cd` to the project root and create a virtual environment in a directory named `venv`, which is conveniently ignored in version control.
+1. `cd` to the project root and create a virtual environment
+in a directory named `venv`, which is conveniently ignored in
+version control.
 2. Install the dependencies.
 
 ```sh
 pip install -r requirements.txt
 ```
 
 3. Install this package in editable mode.
@@ -78,15 +87,15 @@
 pip freeze --exclude-editable > requirements.txt
 ```
 
 2. Increment the version on `pyproject.toml`.
 3. Build the package.
 
 ```sh
-hatch build
+python -m build
 ```
 
 4. Commit and push the changes (and a new version tag) to the git repository.
 5. Publish it.
 ```sh
-hatch publish
+python -m twine upload dist/*
 ```
```

### Comparing `basketcase-4.0.0/pyproject.toml` & `basketcase-5.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "basketcase"
-version = "4.0.0"
+version = "5.0.0"
 authors = [
-  { name="Douglas Silva", email="doug.hs@protonmail.ch" },
+  { name="Douglas Silva", email="douglas-h-silva@proton.me" },
 ]
 description = "Download images and videos from Instagram"
 readme = "README.md"
-license = { file="LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
 ]
+license = {file = "LICENSE"}
+keywords = ["instagram", "story", "stories"]
 dependencies = [
   "requests~=2.28.2",
-  "yt-dlp==2023.1.6",
-  "Pillow~=9.4.0",
 ]
 
 [project.scripts]
 "basketcase" = "basketcase.__main__:main"
 
 [project.urls]
 "Homepage" = "https://gitlab.com/crimson.king/basketcase"
-"Bug Tracker" = "https://gitlab.com/crimson.king/basketcase/-/issues"
+"Bug Tracker" = "https://gitlab.com/crimson.king/basketcase/-/issues"
```

