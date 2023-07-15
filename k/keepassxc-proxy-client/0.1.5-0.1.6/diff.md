# Comparing `tmp/keepassxc-proxy-client-0.1.5.tar.gz` & `tmp/keepassxc-proxy-client-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keepassxc-proxy-client-0.1.5.tar", last modified: Mon Feb 27 18:28:15 2023, max compression
+gzip compressed data, was "keepassxc-proxy-client-0.1.6.tar", last modified: Sat Jul 15 12:35:42 2023, max compression
```

## Comparing `keepassxc-proxy-client-0.1.5.tar` & `keepassxc-proxy-client-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2023-02-27 18:28:15.216234 keepassxc-proxy-client-0.1.5/
--rw-r--r--   0 nix       (1000) nix       (1000)       42 2023-02-27 18:25:33.000000 keepassxc-proxy-client-0.1.5/CHANGELOG.md
--rw-r--r--   0 nix       (1000) nix       (1000)      642 2023-02-27 18:25:33.000000 keepassxc-proxy-client-0.1.5/LICENSE
--rw-r--r--   0 nix       (1000) nix       (1000)      106 2023-02-27 18:25:33.000000 keepassxc-proxy-client-0.1.5/MANIFEST.in
--rw-r--r--   0 nix       (1000) nix       (1000)     3165 2023-02-27 18:28:15.216234 keepassxc-proxy-client-0.1.5/PKG-INFO
--rw-r--r--   0 nix       (1000) nix       (1000)     2015 2023-02-27 18:25:33.000000 keepassxc-proxy-client-0.1.5/README.md
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2023-02-27 18:28:15.216234 keepassxc-proxy-client-0.1.5/keepassxc_proxy_client/
--rw-r--r--   0 nix       (1000) nix       (1000)       22 2023-02-27 18:27:37.000000 keepassxc-proxy-client-0.1.5/keepassxc_proxy_client/__init__.py
--rw-r--r--   0 nix       (1000) nix       (1000)     2458 2023-02-27 18:25:33.000000 keepassxc-proxy-client-0.1.5/keepassxc_proxy_client/__main__.py
--rw-r--r--   0 nix       (1000) nix       (1000)     7364 2023-02-27 18:25:33.000000 keepassxc-proxy-client-0.1.5/keepassxc_proxy_client/protocol.py
-drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2023-02-27 18:28:15.216234 keepassxc-proxy-client-0.1.5/keepassxc_proxy_client.egg-info/
--rw-r--r--   0 nix       (1000) nix       (1000)     3165 2023-02-27 18:28:15.000000 keepassxc-proxy-client-0.1.5/keepassxc_proxy_client.egg-info/PKG-INFO
--rw-r--r--   0 nix       (1000) nix       (1000)      492 2023-02-27 18:28:15.000000 keepassxc-proxy-client-0.1.5/keepassxc_proxy_client.egg-info/SOURCES.txt
--rw-r--r--   0 nix       (1000) nix       (1000)        1 2023-02-27 18:28:15.000000 keepassxc-proxy-client-0.1.5/keepassxc_proxy_client.egg-info/dependency_links.txt
--rw-r--r--   0 nix       (1000) nix       (1000)       80 2023-02-27 18:28:15.000000 keepassxc-proxy-client-0.1.5/keepassxc_proxy_client.egg-info/entry_points.txt
--rw-r--r--   0 nix       (1000) nix       (1000)       43 2023-02-27 18:28:15.000000 keepassxc-proxy-client-0.1.5/keepassxc_proxy_client.egg-info/requires.txt
--rw-r--r--   0 nix       (1000) nix       (1000)       23 2023-02-27 18:28:15.000000 keepassxc-proxy-client-0.1.5/keepassxc_proxy_client.egg-info/top_level.txt
--rw-r--r--   0 nix       (1000) nix       (1000)        1 2023-02-27 18:26:46.000000 keepassxc-proxy-client-0.1.5/keepassxc_proxy_client.egg-info/zip-safe
--rw-r--r--   0 nix       (1000) nix       (1000)       39 2023-02-27 18:25:33.000000 keepassxc-proxy-client-0.1.5/requirements.txt
--rw-r--r--   0 nix       (1000) nix       (1000)       38 2023-02-27 18:28:15.216234 keepassxc-proxy-client-0.1.5/setup.cfg
--rw-r--r--   0 nix       (1000) nix       (1000)     1860 2023-02-27 18:25:33.000000 keepassxc-proxy-client-0.1.5/setup.py
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2023-07-15 12:35:42.371925 keepassxc-proxy-client-0.1.6/
+-rw-r--r--   0 nix       (1000) nix       (1000)       42 2023-02-27 18:25:33.000000 keepassxc-proxy-client-0.1.6/CHANGELOG.md
+-rw-r--r--   0 nix       (1000) nix       (1000)      642 2023-02-27 18:25:33.000000 keepassxc-proxy-client-0.1.6/LICENSE
+-rw-r--r--   0 nix       (1000) nix       (1000)      106 2023-02-27 18:25:33.000000 keepassxc-proxy-client-0.1.6/MANIFEST.in
+-rw-r--r--   0 nix       (1000) nix       (1000)     3165 2023-07-15 12:35:42.371925 keepassxc-proxy-client-0.1.6/PKG-INFO
+-rw-r--r--   0 nix       (1000) nix       (1000)     2015 2023-02-27 18:25:33.000000 keepassxc-proxy-client-0.1.6/README.md
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2023-07-15 12:35:42.370925 keepassxc-proxy-client-0.1.6/keepassxc_proxy_client/
+-rw-r--r--   0 nix       (1000) nix       (1000)       22 2023-07-15 12:35:15.000000 keepassxc-proxy-client-0.1.6/keepassxc_proxy_client/__init__.py
+-rw-r--r--   0 nix       (1000) nix       (1000)     3229 2023-07-15 12:33:21.000000 keepassxc-proxy-client-0.1.6/keepassxc_proxy_client/__main__.py
+-rw-r--r--   0 nix       (1000) nix       (1000)     7716 2023-07-15 12:33:21.000000 keepassxc-proxy-client-0.1.6/keepassxc_proxy_client/protocol.py
+drwxr-xr-x   0 nix       (1000) nix       (1000)        0 2023-07-15 12:35:42.370925 keepassxc-proxy-client-0.1.6/keepassxc_proxy_client.egg-info/
+-rw-r--r--   0 nix       (1000) nix       (1000)     3165 2023-07-15 12:35:42.000000 keepassxc-proxy-client-0.1.6/keepassxc_proxy_client.egg-info/PKG-INFO
+-rw-r--r--   0 nix       (1000) nix       (1000)      492 2023-07-15 12:35:42.000000 keepassxc-proxy-client-0.1.6/keepassxc_proxy_client.egg-info/SOURCES.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)        1 2023-07-15 12:35:42.000000 keepassxc-proxy-client-0.1.6/keepassxc_proxy_client.egg-info/dependency_links.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)       80 2023-07-15 12:35:42.000000 keepassxc-proxy-client-0.1.6/keepassxc_proxy_client.egg-info/entry_points.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)       43 2023-07-15 12:35:42.000000 keepassxc-proxy-client-0.1.6/keepassxc_proxy_client.egg-info/requires.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)       23 2023-07-15 12:35:42.000000 keepassxc-proxy-client-0.1.6/keepassxc_proxy_client.egg-info/top_level.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)        1 2023-02-27 18:26:46.000000 keepassxc-proxy-client-0.1.6/keepassxc_proxy_client.egg-info/zip-safe
+-rw-r--r--   0 nix       (1000) nix       (1000)       39 2023-02-27 18:25:33.000000 keepassxc-proxy-client-0.1.6/requirements.txt
+-rw-r--r--   0 nix       (1000) nix       (1000)       38 2023-07-15 12:35:42.371925 keepassxc-proxy-client-0.1.6/setup.cfg
+-rw-r--r--   0 nix       (1000) nix       (1000)     1860 2023-02-27 18:25:33.000000 keepassxc-proxy-client-0.1.6/setup.py
```

### Comparing `keepassxc-proxy-client-0.1.5/LICENSE` & `keepassxc-proxy-client-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `keepassxc-proxy-client-0.1.5/PKG-INFO` & `keepassxc-proxy-client-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keepassxc-proxy-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: A CLI for keepassxc-proxy
 Home-page: https://github.com/hargoniX/keepassxc-proxy-client
 Author: Henrik Boeving
 Author-email: hargonix@gmail.com
 Project-URL: Issue tracker, https://github.com/hargoniX/keepassxc-proxy-client/issues
 Project-URL: Changelog, https://github.com/hargoniX/keepassxc-proxy-client/blob/master/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
```

### Comparing `keepassxc-proxy-client-0.1.5/README.md` & `keepassxc-proxy-client-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `keepassxc-proxy-client-0.1.5/keepassxc_proxy_client/__main__.py` & `keepassxc-proxy-client-0.1.6/keepassxc_proxy_client/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 secret and can allow anyone with access to your local machine access to all
 passwords that are related to a URL, thus it should be stored safely.
 
 keepassxc_proxy_client get <file> <url>: Reads a keepassxc association from
 <file> and attempts to get the first password for <url>. Will exit with 1 if the
 assocation is not valid for the running keepassxc instance or the no logins are
 found for the given URL.
+
+keepassxc_proxy_client unlock <file>: Causes a running KeepassXC instance
+to launch a dialogue window to allow the user to unlock a locked database.
+If the database is already unlocked it has no effect.
 """
 
 
 def main():
     if len(sys.argv) < 2 or sys.argv[1] in ["-h", "--help","help", "h"]:
         print(USAGE)
         sys.exit(0)
@@ -68,10 +72,29 @@
         logins = connection.get_logins(url)
         if not logins:
             print("No logins found for the given URL")
             sys.exit(1)
 
         print(logins[0]["password"])
         sys.exit(0)
+    elif command == "unlock":
+        if len(sys.argv) < 3:
+            print("Too few arguments provided, see --help for usage")
+            sys.exit(1)
+
+        associate_file = sys.argv[2]
+        association = json.load(open(associate_file, "r"))
+
+        connection = keepassxc_proxy_client.protocol.Connection()
+        connection.connect()
+
+        connection.load_associate(
+            association["name"],
+            base64.b64decode(association["public_key"].encode("utf-8"))
+        )
+
+        print(connection.test_associate(True))
+
+        sys.exit(0)
     else:
         print("Unkown subcommand, see --help for usage")
         sys.exit(1)
```

### Comparing `keepassxc-proxy-client-0.1.5/keepassxc_proxy_client/protocol.py` & `keepassxc-proxy-client-0.1.6/keepassxc_proxy_client/protocol.py`

 * *Files 14% similar despite different names*

```diff
@@ -81,14 +81,17 @@
         self.box = Box(self.private_key, PublicKey(base64.b64decode(response["publicKey"])))
         self.nonce = (int.from_bytes(self.nonce, "big") + 1).to_bytes(24, "big")
 
     def get_socket_path():
         server_name = "org.keepassxc.KeePassXC.BrowserServer"
         system = platform.system()
         if system == "Linux" and "XDG_RUNTIME_DIR" in os.environ:
+            flatpak_socket_path = os.path.join(os.environ["XDG_RUNTIME_DIR"], "app/org.keepassxc.KeePassXC", server_name)
+            if os.path.exists(flatpak_socket_path):
+                return flatpak_socket_path
             return os.path.join(os.environ["XDG_RUNTIME_DIR"], server_name)
         elif system == "Darwin" and "TMPDIR" in os.environ:
             return os.path.join(os.getenv("TMPDIR"), server_name)
         elif system == "Windows":
             pathWin = "org.keepassxc.KeePassXC.BrowserServer_"  + getpass.getuser()
             return pathWin
         else:
@@ -126,22 +129,22 @@
     def load_associate(self, name, public_key):
         self.associate_id = name
         self.id_public_key = PublicKey(public_key)
 
     def dump_associate(self):
         return (self.associate_id, self.id_public_key._public_key)
 
-    def test_associate(self):
+    def test_associate(self, trigger_unlock = False):
         msg = {
             "action": "test-associate",
             "id": self.associate_id,
             "key": base64.b64encode(self.id_public_key._public_key).decode("utf-8")
         }
 
-        self.send_encrypted_message(msg)
+        self.send_encrypted_message(msg, trigger_unlock)
         self.get_encrypted_response()
         return True
 
     def get_logins(self, url):
         msg = {
             "action": "get-logins",
             "url": url,
@@ -197,17 +200,19 @@
         server_nonce = base64.b64decode(raw_response["nonce"])
         decrypted = self.box.decrypt(base64.b64decode(raw_response["message"]), server_nonce)
         response = json.loads(decrypted)
         if not response["success"]:
             raise ResponseUnsuccesfulException(raw_response)
         return response
 
-    def send_encrypted_message(self, msg):
+    def send_encrypted_message(self, msg, trigger_unlock = False):
         encrypted = base64.b64encode(self.box.encrypt(json.dumps(msg).encode("utf-8"), nonce=self.nonce).ciphertext)
         msg = {
             "action": msg["action"],
             "message": encrypted.decode("utf-8"),
             "nonce": base64.b64encode(self.nonce).decode("utf-8"),
             "clientID": self.client_id
         }
+        if (trigger_unlock):
+            msg['triggerUnlock'] = 'true'
         self.socket.sendall(json.dumps(msg).encode("utf-8"))
         self.nonce = (int.from_bytes(self.nonce, "big") + 1).to_bytes(24, "big")
```

### Comparing `keepassxc-proxy-client-0.1.5/keepassxc_proxy_client.egg-info/PKG-INFO` & `keepassxc-proxy-client-0.1.6/keepassxc_proxy_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keepassxc-proxy-client
-Version: 0.1.5
+Version: 0.1.6
 Summary: A CLI for keepassxc-proxy
 Home-page: https://github.com/hargoniX/keepassxc-proxy-client
 Author: Henrik Boeving
 Author-email: hargonix@gmail.com
 Project-URL: Issue tracker, https://github.com/hargoniX/keepassxc-proxy-client/issues
 Project-URL: Changelog, https://github.com/hargoniX/keepassxc-proxy-client/blob/master/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
```

### Comparing `keepassxc-proxy-client-0.1.5/setup.py` & `keepassxc-proxy-client-0.1.6/setup.py`

 * *Files identical despite different names*

