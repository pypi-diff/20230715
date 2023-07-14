# Comparing `tmp/RelayMe-0.0.5.tar.gz` & `tmp/RelayMe-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RelayMe-0.0.5.tar", last modified: Fri Jul 14 16:54:10 2023, max compression
+gzip compressed data, was "RelayMe-0.0.6.tar", last modified: Fri Jul 14 23:24:53 2023, max compression
```

## Comparing `RelayMe-0.0.5.tar` & `RelayMe-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 16:54:10.430789 RelayMe-0.0.5/
--rw-rw-rw-   0        0        0      432 2023-07-14 16:53:05.000000 RelayMe-0.0.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-07-13 14:27:01.000000 RelayMe-0.0.5/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-07-13 14:09:08.000000 RelayMe-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2527 2023-07-14 16:54:10.430789 RelayMe-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1551 2023-07-14 16:52:16.000000 RelayMe-0.0.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-14 16:54:10.408259 RelayMe-0.0.5/RelayMe/
--rw-rw-rw-   0        0        0     1380 2023-07-14 16:53:31.000000 RelayMe-0.0.5/RelayMe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 16:54:10.428207 RelayMe-0.0.5/RelayMe.egg-info/
--rw-rw-rw-   0        0        0     2527 2023-07-14 16:54:10.000000 RelayMe-0.0.5/RelayMe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-07-14 16:54:10.000000 RelayMe-0.0.5/RelayMe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 16:54:10.000000 RelayMe-0.0.5/RelayMe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-14 16:54:10.000000 RelayMe-0.0.5/RelayMe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 16:54:10.431789 RelayMe-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      779 2023-07-14 16:52:24.000000 RelayMe-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 23:24:53.504353 RelayMe-0.0.6/
+-rw-rw-rw-   0        0        0      518 2023-07-14 23:22:37.000000 RelayMe-0.0.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-07-13 14:27:01.000000 RelayMe-0.0.6/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-07-13 14:09:08.000000 RelayMe-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2806 2023-07-14 23:24:53.503355 RelayMe-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1744 2023-07-14 23:20:53.000000 RelayMe-0.0.6/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 23:24:53.473919 RelayMe-0.0.6/RelayMe/
+-rw-rw-rw-   0        0        0     1603 2023-07-14 23:21:04.000000 RelayMe-0.0.6/RelayMe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-14 23:24:53.501358 RelayMe-0.0.6/RelayMe.egg-info/
+-rw-rw-rw-   0        0        0     2806 2023-07-14 23:24:53.000000 RelayMe-0.0.6/RelayMe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-07-14 23:24:53.000000 RelayMe-0.0.6/RelayMe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 23:24:53.000000 RelayMe-0.0.6/RelayMe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-14 23:24:53.000000 RelayMe-0.0.6/RelayMe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-14 23:24:53.504353 RelayMe-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      779 2023-07-14 23:21:16.000000 RelayMe-0.0.6/setup.py
```

### Comparing `RelayMe-0.0.5/LICENCE.txt` & `RelayMe-0.0.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `RelayMe-0.0.5/PKG-INFO` & `RelayMe-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RelayMe
-Version: 0.0.5
+Version: 0.0.6
 Summary: Sends emails with chosen email relay service
 Home-page: 
 Author: Elijah Phifer
 Author-email: elijahphifer9@gmail.com
 License: MIT
 Keywords: mail,email,relay,relayservice
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENCE.txt
 
 RelayMe
 =======
 
-0.0.5
+0.0.6
 -----
 
 This module is geared towards emailing using email relay services.
 
 Prerequisites
 -------------
 
@@ -36,51 +36,63 @@
 The `SenderConfig` instance needs a config file key to be passed in, which should contain the following keys:
 
 - `server`
 - `port`
 - `sender`
 - `username`
 - `password`
+- `subject`
+- `header`
+- `footer`
 
 (Case doesn't matter, but spelling is important. The keys could also be named 'Server', 'PORT', 'UserName', etc.)
 
+(The order doesn't matter either. The keys can be in any order you like.)
+
 (Also the 'username' and 'password' keys are optional if your relay service doesn't require a user name and pass word to authenticate.)
 
 Here is an example config key:
 
 .. code-block:: python
 
-   'EmailSender': {
+   'EmailConfig': {
        'server': 'smtp.example.com',
        'port': 123,
        'sender': 'sender@example.com',
        'username': 'username',
-       'password': 'password'
+       'password': 'password',
+       'subject": "Hello from the SenderConfig module!",
+       'header": "This is the header",
+       'footer': "This is the footer"
    }
 
 Usage
 -----
 
 Here's an example of how to use this module in your code:
 
 .. code-block:: python
 
    from RelayMe import SenderConfig
 
-   sender = SenderConfig(config['EmailSender'])
-   subject = "Hello from the SenderConfig module!"
+   sender = SenderConfig(config["EmailConfig"])
+
    body = "This is the body of the email."
    recipient = "John.Doe@mail.com"  # (or it can come from a config file where you could list multiple emails)
 
-   sender.send_email(subject, body, recipient)
+   sender.send_email(body, recipient)
 
 
 Change Log
 =============
 
+0.0.6 (07/14/2023)
+-------------------
+-Added more variables to the config file.
+
 0.0.5 (07/14/2023)
 -------------------
 -Fixed spelling and grammer in README file
 
 0.0.4 (07/14/2023)
 -------------------
 -Added more details about usage to the README file
```

### Comparing `RelayMe-0.0.5/README.txt` & `RelayMe-0.0.6/README.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 RelayMe
 =======
 
-0.0.5
+0.0.6
 -----
 
 This module is geared towards emailing using email relay services.
 
 Prerequisites
 -------------
 
@@ -20,39 +20,47 @@
 The `SenderConfig` instance needs a config file key to be passed in, which should contain the following keys:
 
 - `server`
 - `port`
 - `sender`
 - `username`
 - `password`
+- `subject`
+- `header`
+- `footer`
 
 (Case doesn't matter, but spelling is important. The keys could also be named 'Server', 'PORT', 'UserName', etc.)
 
+(The order doesn't matter either. The keys can be in any order you like.)
+
 (Also the 'username' and 'password' keys are optional if your relay service doesn't require a user name and pass word to authenticate.)
 
 Here is an example config key:
 
 .. code-block:: python
 
-   'EmailSender': {
+   'EmailConfig': {
        'server': 'smtp.example.com',
        'port': 123,
        'sender': 'sender@example.com',
        'username': 'username',
-       'password': 'password'
+       'password': 'password',
+       'subject": "Hello from the SenderConfig module!",
+       'header": "This is the header",
+       'footer': "This is the footer"
    }
 
 Usage
 -----
 
 Here's an example of how to use this module in your code:
 
 .. code-block:: python
 
    from RelayMe import SenderConfig
 
-   sender = SenderConfig(config['EmailSender'])
-   subject = "Hello from the SenderConfig module!"
+   sender = SenderConfig(config["EmailConfig"])
+
    body = "This is the body of the email."
    recipient = "John.Doe@mail.com"  # (or it can come from a config file where you could list multiple emails)
 
-   sender.send_email(subject, body, recipient)
+   sender.send_email(body, recipient)
```

### Comparing `RelayMe-0.0.5/RelayMe/__init__.py` & `RelayMe-0.0.6/RelayMe/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,20 +12,23 @@
             '%(asctime)s - %(name)s - %(levelname)s - %(message)s')
         console_handler = logging.StreamHandler()
         console_handler.setLevel(logging.INFO)
 
         console_handler.setFormatter(formatter)
         self.logger.addHandler(console_handler)
 
-    def send_email(self, subject, body, recipient, sender=None):
+    def send_email(self, body, recipients, subject=None, header=None, footer=None, sender=None):
         email = EmailMessage()
-        email['Subject'] = subject
+        email['Subject'] = subject or self.config['subject']
         email['From'] = sender or self.config['sender']
-        email['To'] = recipient
-        email.set_content(body)
+        email['To'] = recipients
+        head = (header or self.config['header']) + "\n\n"
+        foot = "\n\n" + (footer or self.config['footer'])
+        message = str(head + body + foot)
+        email.set_content(message)
 
         try:
             with smtplib.SMTP(self.config['server'], self.config['port']) as smtp:
                 if self.config.get('username') and self.config.get('password'):
                     smtp.login(self.config['username'],
                                self.config['password'])
                 smtp.send_message(email)
```

### Comparing `RelayMe-0.0.5/RelayMe.egg-info/PKG-INFO` & `RelayMe-0.0.6/RelayMe.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RelayMe
-Version: 0.0.5
+Version: 0.0.6
 Summary: Sends emails with chosen email relay service
 Home-page: 
 Author: Elijah Phifer
 Author-email: elijahphifer9@gmail.com
 License: MIT
 Keywords: mail,email,relay,relayservice
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENCE.txt
 
 RelayMe
 =======
 
-0.0.5
+0.0.6
 -----
 
 This module is geared towards emailing using email relay services.
 
 Prerequisites
 -------------
 
@@ -36,51 +36,63 @@
 The `SenderConfig` instance needs a config file key to be passed in, which should contain the following keys:
 
 - `server`
 - `port`
 - `sender`
 - `username`
 - `password`
+- `subject`
+- `header`
+- `footer`
 
 (Case doesn't matter, but spelling is important. The keys could also be named 'Server', 'PORT', 'UserName', etc.)
 
+(The order doesn't matter either. The keys can be in any order you like.)
+
 (Also the 'username' and 'password' keys are optional if your relay service doesn't require a user name and pass word to authenticate.)
 
 Here is an example config key:
 
 .. code-block:: python
 
-   'EmailSender': {
+   'EmailConfig': {
        'server': 'smtp.example.com',
        'port': 123,
        'sender': 'sender@example.com',
        'username': 'username',
-       'password': 'password'
+       'password': 'password',
+       'subject": "Hello from the SenderConfig module!",
+       'header": "This is the header",
+       'footer': "This is the footer"
    }
 
 Usage
 -----
 
 Here's an example of how to use this module in your code:
 
 .. code-block:: python
 
    from RelayMe import SenderConfig
 
-   sender = SenderConfig(config['EmailSender'])
-   subject = "Hello from the SenderConfig module!"
+   sender = SenderConfig(config["EmailConfig"])
+
    body = "This is the body of the email."
    recipient = "John.Doe@mail.com"  # (or it can come from a config file where you could list multiple emails)
 
-   sender.send_email(subject, body, recipient)
+   sender.send_email(body, recipient)
 
 
 Change Log
 =============
 
+0.0.6 (07/14/2023)
+-------------------
+-Added more variables to the config file.
+
 0.0.5 (07/14/2023)
 -------------------
 -Fixed spelling and grammer in README file
 
 0.0.4 (07/14/2023)
 -------------------
 -Added more details about usage to the README file
```

### Comparing `RelayMe-0.0.5/setup.py` & `RelayMe-0.0.6/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='RelayMe',
-    version='0.0.5',
+    version='0.0.6',
     description='Sends emails with chosen email relay service',
     long_description=open('README.txt').read() + '\n\n' +
     open('CHANGELOG.txt').read(),
     url='',
     author='Elijah Phifer',
     author_email='elijahphifer9@gmail.com',
     license='MIT',
```

