# Comparing `tmp/truecallerpy-0.1.2.tar.gz` & `tmp/truecallerpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truecallerpy-0.1.2.tar", max compression
+gzip compressed data, was "truecallerpy-0.2.0.tar", max compression
```

## Comparing `truecallerpy-0.1.2.tar` & `truecallerpy-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     1076 2022-11-10 15:49:24.252807 truecallerpy-0.1.2/LICENSE
--rw-r--r--   0        0        0     7847 2022-11-10 15:49:24.252807 truecallerpy-0.1.2/README.md
--rw-r--r--   0        0        0     2327 2022-11-16 08:08:47.120405 truecallerpy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1176 2022-11-10 15:49:24.256140 truecallerpy-0.1.2/truecallerpy/__init__.py
--rw-r--r--   0        0        0    12985 2022-11-10 15:49:24.256140 truecallerpy-0.1.2/truecallerpy/app.py
--rw-r--r--   0        0        0     9508 2022-11-10 15:49:24.256140 truecallerpy-0.1.2/truecallerpy/phonesList.py
--rw-r--r--   0        0        0    12163 2022-11-16 08:01:06.633728 truecallerpy-0.1.2/truecallerpy/truecallerLogin.py
--rw-r--r--   0        0        0     1894 2022-11-10 15:49:24.256140 truecallerpy-0.1.2/truecallerpy/version.py
--rw-r--r--   0        0        0        5 2022-11-10 15:49:24.256140 truecallerpy-0.1.2/truecallerpy/version.txt
--rw-r--r--   0        0        0     8981 1970-01-01 00:00:00.000000 truecallerpy-0.1.2/setup.py
--rw-r--r--   0        0        0     8894 1970-01-01 00:00:00.000000 truecallerpy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-15 06:27:59.087737 truecallerpy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     7013 2023-07-15 09:29:51.122736 truecallerpy-0.2.0/README.md
+-rw-r--r--   0        0        0     1662 2023-07-15 09:32:22.571654 truecallerpy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-07-15 06:46:09.912685 truecallerpy-0.2.0/truecallerpy/__init__.py
+-rw-r--r--   0        0        0    11924 2023-07-15 06:53:03.115933 truecallerpy-0.2.0/truecallerpy/cli.py
+-rw-r--r--   0        0        0        0 2023-07-15 06:22:38.263076 truecallerpy-0.2.0/truecallerpy/data/__init__.py
+-rw-r--r--   0        0        0      170 2023-07-15 06:46:37.833038 truecallerpy-0.2.0/truecallerpy/data/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4905 2023-07-15 06:46:37.833038 truecallerpy-0.2.0/truecallerpy/data/__pycache__/phones_list.cpython-311.pyc
+-rw-r--r--   0        0        0     7061 2023-07-15 06:22:38.256409 truecallerpy-0.2.0/truecallerpy/data/phones_list.py
+-rw-r--r--   0        0        0     2276 2023-07-15 06:58:57.402747 truecallerpy-0.2.0/truecallerpy/login.py
+-rw-r--r--   0        0        0     2490 2023-07-15 07:00:54.463843 truecallerpy-0.2.0/truecallerpy/search.py
+-rw-r--r--   0        0        0     6873 2023-07-15 07:14:01.676896 truecallerpy-0.2.0/truecallerpy/typings/truecallerpy.pyi
+-rw-r--r--   0        0        0     1890 2023-07-15 07:01:25.931633 truecallerpy-0.2.0/truecallerpy/verify_otp.py
+-rw-r--r--   0        0        0     8424 1970-01-01 00:00:00.000000 truecallerpy-0.2.0/PKG-INFO
```

### Comparing `truecallerpy-0.1.2/LICENSE` & `truecallerpy-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `truecallerpy-0.1.2/truecallerpy/truecallerLogin.py` & `truecallerpy-0.2.0/truecallerpy/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/python
+
 # ==================================================================================
 # MIT License
 
 # Copyright (c) 2022 Emmadi Sumith Kumar
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
@@ -18,260 +19,324 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ====================================================================================
-
 import os
-import os.path
 import sys
 import json
 import argparse
 import phonenumbers
-from phonenumbers import carrier, timezone, geocoder
-from phonenumbers.phonenumberutil import number_type
-import requests
-import random
-import codecs
-from .phonesList import truecallerpy_get_random_phone
+from phonenumbers import format_number, PhoneNumberFormat
+import questionary
+import colorama
+from colorama import Fore, Style
+from .login import login
+from .verify_otp import verify_otp
+from .search import search_phonenumber, bulk_search
+
+# Initialize colorama
+colorama.init()
+
+homePath = os.path.expanduser("~")
+truecallerpyAuthDirPath = os.path.join(homePath, ".config", "truecallerpy")
+requestFilePath = os.path.join(truecallerpyAuthDirPath, "request.json")
+authKeyFilePath = os.path.join(truecallerpyAuthDirPath, "authkey.json")
 
+if not os.path.exists(truecallerpyAuthDirPath):
+    try:
+        os.makedirs(truecallerpyAuthDirPath, exist_ok=True)
+    except OSError as error:
+        print(error)
+        exit(1)
 
-def getNumber(x):
-    if x[0] == "0":
-        return x[1:].replace(" ", "")
-    else:
-        return x.replace(" ", "")
+# Function to validate phone number
 
 
-def truecallerpy_login(config):
-    if "HOME" in os.environ:
-        config_dir = os.environ['HOME'] + "/.config"
-    else:
-        config_dir = os.environ['HOMEPATH'] + "\.config"
-    # print(config_dir)
-    directory = "truecallerpy"
-    file = "authkey.json"
-    dir_path = os.path.join(config_dir, directory)
-    path = os.path.join(config_dir, directory, file)
-    r_path = os.path.join(config_dir, directory, "request.json")
+def validate_phone_number(input):
     try:
-        os.makedirs(dir_path, exist_ok=True)
-        print("Directory '%s' created successfully" % directory)
-    except OSError as error:
-        raise SystemExit(error)
+        pn = phonenumbers.parse(input, None)
+        if not phonenumbers.is_valid_number(pn):
+            return "Invalid Phone Number"
+        return True
+    except phonenumbers.NumberParseException:
+        return "Enter a valid phone number in International Format"
 
-    print('\x1b[33mLogin\n\n Enter mobile number in International Format\n Example : +919912345678.\x1b[0m\n')
-    number = input('Enter Mobile Number : ')
-    if number[0] != "+":
-        raise SystemExit(
-            '\x1b[31mEnter valid phone number in International Format\x1b[0m')
-    phoneNumber = phonenumbers.parse(number, None)
-
-    # check if a number is valid
-    if phonenumbers.is_valid_number(phoneNumber) == False:
-        raise SystemExit(
-            '\x1b[31mEnter valid phone number in International Format\x1b[0m')
-
-    phoneNumberNational = phonenumbers.format_number(
-        phoneNumber, phonenumbers.PhoneNumberFormat.NATIONAL)
-    print('\x1b[32mSending otp to {} \x1b[0m'.format(getNumber(number)))
-    phoneSpecs = truecallerpy_get_random_phone()
-
-    data = {
-        "countryCode": phonenumbers.region_code_for_number(phoneNumber),
-        "dialingCode": phonenumbers.country_code_for_region(phonenumbers.region_code_for_number(phoneNumber)),
-        "installationDetails": {
-            "app": {
-                "buildVersion": 5,
-                "majorVersion": 11,
-                "minorVersion": 7,
-                "store": "GOOGLE_PLAY"
-            },
-            "device": {
-                "deviceId": ''.join(random.choice('0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrst') for i in range(16)),
-                "language": "en",
-                "manufacturer": "{}".format(phoneSpecs["manufacturer"]),
-                "model": "{}".format(phoneSpecs["model"]),
-                "osName": "Android",
-                "osVersion": "10",
-                "mobileServices": ["GMS"]
-            },
-            "language": "en"
-        },
-        "phoneNumber": getNumber(phoneNumberNational),
-        "region": "region-2",
-        "sequenceNo": 2
-    }
-
-    headers = {
-        "content-type": "application/json; charset=UTF-8",
-        "accept-encoding": "gzip",
-        "user-agent": "Truecaller/11.75.5 (Android;10)",
-        "clientsecret": "lvc22mp3l1sfv6ujg83rd17btt"
-    }
-
-    if os.path.exists(r_path):
-        # print("\n\nPrevious request was found for this mobile number.\n")
-        with open(r_path) as f:
-            req_file = json.load(f)
-        if req_file['status'] == False:
-            try:
-                print("\x1b[31mSomthing when wrong\x1b[0m")
-                os.remove(r_path)
-            except IOError:
-                raise SystemExit(
-                    "Unable to delete file\n Delete '{}' this file and try again".format(r_path))
-        else:
-            if "parsedPhoneNumber" in req_file and '+{}'.format(req_file['parsedPhoneNumber']) == getNumber(number):
-                print("\n\nPrevious request was found for this mobile number.\n")
-                x = input("Do you want to enter previous OTP (y/n): ")
-                x_status = True
-                while x_status:
-                    if x == "y" or x == "yes":
-                        x_status = False
-                        request_data = req_file
-                    elif x == "n" or x == "no":
-                        x_status = False
-                        try:
-                            os.remove(r_path)
-                        except IOError:
-                            raise SystemExit(
-                                "Unable to delete file\n Delete '{}' this file and try again".format(r_path))
-                        try:
-                            postRequest = requests.post(
-                                'https://account-asia-south1.truecaller.com/v2/sendOnboardingOtp', headers=headers, json=data)
-                        except requests.exceptions.RequestException as e:
-                            raise SystemExit(e)
-                        requestFile = open(r_path, "w")
-                        json.dump(postRequest.json(),
-                                  requestFile, indent=3)
-                        requestFile.close()
-                        request_data = postRequest.json()
-                        if request_data['status'] == 1 or request_data['status'] == 9 or request_data['message'] == "Sent":
-                            print('\x1b[32mOtp sent successfully\x1b[0m')
-                    else:
-                        print("\n\nEnter 'y' for yes and 'n' for no\n")
-                        x = input("Do you want to enter previous OTP (y/n): ")
+# Function to validate OTP
 
-            else:
-                try:
-                    postRequest = requests.post(
-                        'https://account-asia-south1.truecaller.com/v2/sendOnboardingOtp', headers=headers, json=data)
-                except requests.exceptions.RequestException as e:
-                    raise SystemExit(e)
-                requestFile = open(r_path, "w")
-                json.dump(postRequest.json(), requestFile, indent=3)
-                requestFile.close()
-                request_data = postRequest.json()
-                if request_data['status'] == 1 or request_data['status'] == 9 or request_data['message'] == "Sent":
-                    print('\x1b[32mOtp sent successfully\x1b[0m')
-    else:
-        try:
-            postRequest = requests.post(
-                'https://account-asia-south1.truecaller.com/v2/sendOnboardingOtp', headers=headers, json=data)
-        except requests.exceptions.RequestException as e:
-            raise SystemExit(e)
-        requestFile = open(r_path, "w")
-        json.dump(postRequest.json(), requestFile, indent=3)
-        requestFile.close()
-        request_data = postRequest.json()
-        if request_data['status'] == 1 or request_data['status'] == 9 or request_data['message'] == "Sent":
-            print('\x1b[32mOtp sent successfully\x1b[0m')
-
-    if request_data['status'] == 1 or request_data['status'] == 9 or request_data['message'] == "Sent":
-        otp = input('Enter Received OTP: ')
-        postData = {
-            "countryCode": phonenumbers.region_code_for_number(phoneNumber),
-            "dialingCode": phonenumbers.country_code_for_region(phonenumbers.region_code_for_number(phoneNumber)),
-            "phoneNumber": getNumber(phoneNumberNational),
-            "requestId": request_data['requestId'],
-            "token": otp
+
+def validate_otp(input):
+    if len(input) != 6 or not input.isdigit():
+        return "Enter a valid 6-digit OTP."
+    return True
+
+
+def check_for_file():
+    if not os.path.isfile(authKeyFilePath):
+        return False
+
+    try:
+        with open(authKeyFilePath) as file:
+            json.load(file)
+        return True
+    except (ValueError, IOError):
+        return False
+
+# Function to perform the login process
+
+
+def loginFuntion():
+    print(
+        f"{Fore.YELLOW}{Style.BRIGHT}Login\n\n Enter mobile number in International Format\n Example : {Fore.MAGENTA}+919912345678{Fore.YELLOW}.\n"
+    )
+
+    questions = [
+        {
+            "type": "text",
+            "name": "phonenumber",
+            "message": "Enter your phone number:",
+            "validate": lambda input: validate_phone_number(input),
         }
+    ]
+    inputNumber = questionary.prompt(questions)
 
-        otpPostRequest = requests.post(
-            'https://account-asia-south1.truecaller.com/v1/verifyOnboardingOtp', headers=headers, json=postData)
-        otp_req_data = otpPostRequest.json()
-        if otp_req_data['status'] == 2 and otp_req_data['suspended'] == False:
-            print('\x1b[33mYour installationId\x1b[0m : \x1b[32m {}\x1b[0m'.format(
-                otp_req_data['installationId']))
-            authKeyFile = open(path, "w")
-            json.dump(otp_req_data, authKeyFile, indent=3)
-            authKeyFile.close()
-            print('\x1b[32mLogged in successfully.\x1b[0m')
-            try:
-                os.remove(r_path)
-            except IOError:
-                raise SystemExit(
-                    "Unable to delete file\n Delete '{}' this file and try again. \nDon't worry about this error your login was successfull".format(r_path))
-        elif otp_req_data['status'] == 11 or otp_req_data['message'] == "Invalid credentials":
-            print('\x1b[31m! Invalid OTP\x1b[0m')
+    try:
+        pn = phonenumbers.parse(inputNumber["phonenumber"], None)
+    except phonenumbers.NumberParseException:
+        print("Enter a valid phone number in International Format")
+        exit(1)
+
+    response = None
+    new_req = True
+
+    if os.path.exists(requestFilePath):
+        with open(requestFilePath, "r") as file:
+            fileData = json.load(file)
+            if (
+                "parsedPhoneNumber" in fileData
+                and f"+{fileData['parsedPhoneNumber']}" == inputNumber["phonenumber"]
+            ):
+                print(
+                    f"{Fore.MAGENTA}\nPrevious request was found for this mobile number.\n"
+                )
+                x = questionary.confirm(
+                    "Do you want to enter previous OTP?").ask()
+
+                if x:
+                    new_req = False
+                    response = fileData
+
+    if new_req:
+        response = login(str(inputNumber["phonenumber"]))
+        print(
+            f"{Fore.YELLOW}Sending OTP to {Fore.GREEN}{inputNumber['phonenumber']}{Fore.YELLOW}."
+        )
+
+    if (
+        response["status"] == 1
+        or response["status"] == 9
+        or response["message"] == "Sent"
+    ):
+        with open(requestFilePath, "w") as file:
+            json.dump(response, file, indent=4)
+
+        if new_req:
+            print(f"{Fore.GREEN}OTP sent successfully.")
+
+        questions1 = [
+            {
+                "type": "text",
+                "name": "otp",
+                "message": "Enter Received OTP:",
+                "validate": lambda input: validate_otp(input),
+            }
+        ]
+
+        token = questionary.prompt(questions1)
+
+        response1 = verify_otp(
+            str(inputNumber["phonenumber"]),
+            response,
+            token["otp"],
+        )
+
+        # print(response1)
+
+        if "status" in response1 and response1["status"] == 2 and "suspended" in response1 and not response1["suspended"]:
+            print(
+                f"{Fore.YELLOW}{Style.BRIGHT}Your installationId: {Fore.GREEN}{response1['installationId']}"
+            )
+
+            with open(authKeyFilePath, "w") as file:
+                json.dump(response1, file, indent=3)
+
+            print(f"{Fore.GREEN}Logged in successfully.")
+            os.remove(requestFilePath)
+        elif "status" in response1 and response1["status"] == 11 or response1["status"] == 40101:
+            print(f"{Fore.RED}! Invalid OTP")
+            print(
+                f"OTP not valid. Enter the 6-digit OTP received on {inputNumber['phonenumber']}."
+            )
+        elif "status" in response1 and response1["status"] == 7:
+            print(f"{Fore.RED}Retries limit exceeded")
+            print(
+                f"Retries on secret code reached for {inputNumber['phonenumber']}."
+            )
+        elif "suspended" in response1 and response1["suspended"] == True:
+            print(f"{Fore.RED}Oops... Your account is suspended.")
+            print("Your account has been suspended by Truecaller.")
+        elif "message" in response1:
+            print(f"{Fore.RED}{response1['message']}")
         else:
-            print(otp_req_data['message'])
-
-    elif (request_data['status'] == 6 or request_data['status'] == 5):
-        print('\x1b[31mYou have exceeded the limit of verification attempts.\nPlease try again after some time.\x1b[0m')
-        try:
-            os.remove(r_path)
-        except IOError:
-            raise SystemExit(
-                "Unable to delete file\n Delete '{}' this file and try again".format(r_path))
+            print(json.dumps(response1, indent=4))
+    elif "status" in response and response["status"] == 6 or response["status"] == 5:
+        if os.path.exists(requestFilePath):
+            os.remove(requestFilePath)
+        print(
+            f"{Fore.RED}You have exceeded the limit of verification attempts.\nPlease try again after some time."
+        )
     else:
-        print('\x1b[31m {} \x1b[0m'.format(request_data['message']))
+        print(f"{Fore.RED}{response['message']}")
 
 
-def truecallerpy_login_with_file(config):
-    if "HOME" in os.environ:
-        config_dir = os.environ['HOME'] + "/.config"
-    else:
-        config_dir = os.environ['HOMEPATH'] + "\.config"
+def searcFunction(args):
+    if not check_for_file():
+        print(Fore.MAGENTA + Style.BRIGHT +
+              "Please login to your account." + Style.RESET_ALL)
+        sys.exit()
 
-    directory = "truecallerpy"
-    file = "authkey.json"
-    dir_path = os.path.join(config_dir, directory)
-    path = os.path.join(config_dir, directory, file)
     try:
-        os.makedirs(dir_path, exist_ok=True)
-    except OSError as error:
-        raise SystemExit(
-            "Login failed! \nDirectory '%s' can not be created" % directory)
-    if os.path.exists(config['file']) == False:
-        raise SystemExit(
-            "FileNotFoundError: [Errno 2] No such file or directory: {}".format(config['file']))
+        with open(authKeyFilePath, "r") as auth_key_file:
+            data = auth_key_file.read()
+            json_auth_key = json.loads(data)
+            country_code = json_auth_key["phones"][0]["countryCode"]
+            installation_id = json_auth_key["installationId"]
+
+        # Perform the search operation
+        search_result = search_phonenumber(
+            args.search, country_code, installation_id)
+
+        if args.name and not args.email:
+            try:
+                name = search_result['data'][0]['name']
+            except (AttributeError, IndexError, KeyError):
+                name = "Unknown Name"
+
+            print(
+                name if args.raw else f"{Fore.BLUE + Style.BRIGHT}Name: {Fore.GREEN}{name}{Style.RESET_ALL}")
+
+        elif not args.name and args.email:
+            try:
+                data = search_result.get("data")
+                if data and len(data) > 0:
+                    internet_addresses = data[0].get("internetAddresses")
+                    if internet_addresses and len(internet_addresses) > 0:
+                        email = internet_addresses[0].get("id")
+                    else:
+                        email = "Unknown Email"
+                else:
+                    email = "Unknown Email"
+
+            except (AttributeError, IndexError, KeyError):
+                email = "Unknown Email"
+
+            print(
+                email if args.raw else f"{Fore.BLUE + Style.BRIGHT}Email: {Fore.GREEN}{email}{Style.RESET_ALL}")
+        else:
+            print(search_result if args.raw else json.dumps(
+                search_result, indent=2))
+    except Exception as error:
+        print(Fore.RED + str(error) + Style.RESET_ALL)
+
+
+def bulkSearchFunction(args):
+    if not check_for_file():
+        print(Fore.MAGENTA + Style.BRIGHT +
+              "Please login to your account." + Style.RESET_ALL)
+        sys.exit()
     try:
-        with open(config['file']) as loginJsonFile:
-            jsonFileData = json.load(loginJsonFile)
+        with open(authKeyFilePath, "r") as auth_key_file:
+            data = auth_key_file.read()
+            json_auth_key = json.loads(data)
+
+            countryCode = json_auth_key["phones"][0]["countryCode"]
+            installationId = json_auth_key["installationId"]
+
+        # Perform bulk search operation
+        search_result = bulk_search(
+            str(args.bs), countryCode, installationId)
+
+        print(json.dumps(search_result)
+              if args.raw else json.dumps(search_result, indent=2))
+
+    except Exception as error:
+        print(error)
+        sys.exit(1)
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        usage="\n%(prog)s login (Login to Truecaller).\n%(prog)s -s [number] (command to search a number)."
+    )
+
+    subparsers = parser.add_subparsers(dest="command")
+    subparsers.add_parser("login", help="Login to Truecaller")
+
+    parser.add_argument("-s", "--search", metavar="NUMBER",
+                        help="Phone number to search")
+
+    parser.add_argument(
+        "-r", "--raw", help="Print raw output", action="store_true")
+    parser.add_argument("--bs", "--bulksearch", metavar="NUMBERS",
+                        help="Make a bulk number search")
+    parser.add_argument(
+        "-e", "--email", help="Print email assigned to the phone number", action="store_true")
+    parser.add_argument(
+        "-n", "--name", help="Print name assigned to the phone number", action="store_true")
+
+    parser.add_argument("-i", "--installationid",
+                        help="Show your InstallationId", action="store_true")
+    parser.add_argument("-v", "--verbose",
+                        help="Show additional information", action="count")
+
+    args = parser.parse_args()
+    # print(parser.print_help())
+    if args.command == "login":
+        # Logic for login command
+        loginFuntion()
+    elif args.search:
+        # Logic for search command
+        searcFunction(args)
+    elif args.bs:
+        bulkSearchFunction(args)
+        # print("bs")
+    elif args.installationid:
+        if not check_for_file():
+            print(Fore.MAGENTA + Style.BRIGHT +
+                  "Please login to your account." + Style.RESET_ALL)
+            sys.exit()
+
+        try:
+            with open(authKeyFilePath, "r") as auth_key_file:
+                data = auth_key_file.read()
+                json_auth_key = json.loads(data)
+
+                installationId = json_auth_key["installationId"]
+
+                if args.raw:
+                    print(installationId)
+                else:
+                    print(Fore.BLUE + Style.BRIGHT + "Your InstallationId: " +
+                          Style.RESET_ALL + Fore.GREEN + installationId + Style.RESET_ALL)
+
+        except Exception as error:
+            print(Fore.RED + "An error occurred." + Style.RESET_ALL)
+            print(error)
+            sys.exit(1)
+    else:
+        parser.print_help()
 
-        installationIdJSON = {
-            "status": 2,
-            "message": "Verified",
-            "installationId": "{}".format(jsonFileData["account"]["installations"][0]["installation"]["id"]),
-            "ttl": 123456,
-            "userId": "{}".format(jsonFileData["account"]["userId"]),
-            "suspended": False,
-            "phones": [
-                {
-                    "phoneNumber": "{}".format(jsonFileData["profile"]["personalData"]["phoneNumbers"][0]["number"]),
-                    "countryCode": "{}".format(jsonFileData["profile"]["personalData"]["phoneNumbers"][0]["countryCode"]),
-                    "priority": 1
-                }
-            ]
-        }
 
-        print('\x1b[33mYour installationId\x1b[0m : \x1b[32m {}\x1b[0m'.format(
-            jsonFileData["account"]["installations"][0]["installation"]["id"]))
-        authKeyFile = open(path, "w")
-        json.dump(installationIdJSON, authKeyFile, indent=3)
-        authKeyFile.close()
-        print('\x1b[32mLogged in successfully.\x1b[0m')
-
-    except IOError:
-        raise SystemExit(
-            "Login failed!\n" + config['file'] + " the file is not accessible or fail to create " + path)
-    finally:
-        loginJsonFile.close()
-
-
-# if __name__ == '__main__':
-#     truecallerpy_login(config)
-#     truecallerpy_login_with_file(config)
+if __name__ == "__main__":
+    main()
```

