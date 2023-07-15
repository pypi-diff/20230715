# Comparing `tmp/st-login-form-0.1.1.tar.gz` & `tmp/st-login-form-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-login-form-0.1.1.tar", last modified: Fri Jul 14 11:40:18 2023, max compression
+gzip compressed data, was "st-login-form-0.2.0.tar", last modified: Sat Jul 15 17:04:19 2023, max compression
```

## Comparing `st-login-form-0.1.1.tar` & `st-login-form-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:40:18.807236 st-login-form-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-14 11:40:10.000000 st-login-form-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 11:40:10.000000 st-login-form-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-14 11:40:18.807236 st-login-form-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-14 11:40:10.000000 st-login-form-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 11:40:18.807236 st-login-form-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-14 11:40:10.000000 st-login-form-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:40:18.807236 st-login-form-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:40:18.807236 st-login-form-0.1.1/src/st_login_form/
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-07-14 11:40:10.000000 st-login-form-0.1.1/src/st_login_form/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:40:18.807236 st-login-form-0.1.1/src/st_login_form.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-14 11:40:18.000000 st-login-form-0.1.1/src/st_login_form.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-14 11:40:18.000000 st-login-form-0.1.1/src/st_login_form.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:40:18.000000 st-login-form-0.1.1/src/st_login_form.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 11:40:18.000000 st-login-form-0.1.1/src/st_login_form.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 11:40:18.000000 st-login-form-0.1.1/src/st_login_form.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:04:19.317008 st-login-form-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-15 17:04:03.000000 st-login-form-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-15 17:04:03.000000 st-login-form-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-15 17:04:19.317008 st-login-form-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-15 17:04:03.000000 st-login-form-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 17:04:19.317008 st-login-form-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-15 17:04:03.000000 st-login-form-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:04:19.317008 st-login-form-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:04:19.317008 st-login-form-0.2.0/src/st_login_form/
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-07-15 17:04:03.000000 st-login-form-0.2.0/src/st_login_form/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:04:19.317008 st-login-form-0.2.0/src/st_login_form.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-15 17:04:19.000000 st-login-form-0.2.0/src/st_login_form.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-15 17:04:19.000000 st-login-form-0.2.0/src/st_login_form.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 17:04:19.000000 st-login-form-0.2.0/src/st_login_form.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-15 17:04:19.000000 st-login-form-0.2.0/src/st_login_form.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-15 17:04:19.000000 st-login-form-0.2.0/src/st_login_form.egg-info/top_level.txt
```

### Comparing `st-login-form-0.1.1/LICENSE` & `st-login-form-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `st-login-form-0.1.1/PKG-INFO` & `st-login-form-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-login-form
-Version: 0.1.1
+Version: 0.2.0
 Summary: A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.
 Author: Siddhant Sadangi
 Author-email: siddhant.sadangi@gmail.com
 Keywords: streamlit,login
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -18,20 +18,20 @@
 
 # :lock: st-login-form
 
 A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.
 
 ![Form screenshot](assets/screenshot.png)
 
-The login form collapses after login to no occupy screen-space.
+The login form collapses after login to free screen-space.
 
 ## :computer: Demo app
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://st-lgn-form.streamlit.app/)
 
-## :construction: Installation instructions 
+## :construction: Installation 
 
 1. Install `st-login-form` 
 ```sh
 pip install st-login-form
 ```
 2. Create a Supabase project as mentioned [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/supabase#sign-in-to-supabase-and-create-a-project)
 3. Create a table to store the usernames and passwords. The table name and column names can be as per your choice.
@@ -64,24 +64,26 @@
       )
     )
   ) tablespace pg_default;
 ```
 4. Follow the rest of the steps from [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/supabase#copy-your-app-secrets-to-the-cloud) to connect your Streamlit app to Supabase
 
 
-## :pen: Usage instructions
+## :pen: Usage
 
 `login_form()` sets `session_state["authenticated"]` to `True` if the login is successful, `session_state["username"]` to the `username` or new or existing user, and to `None` for guest login.
 
+Returns supabase `Client` instance.
+
 ```python
 import streamlit as st
 
 from streamlit_login import login_form
 
-login_form()
+client = login_form()
 
 if st.session_state["authenticated"]:
     if st.session_state["username"]:
         st.success(f"Welcome {st.session_state['username']}")
     else:
         st.success("Welcome guest")
 else:
```

### Comparing `st-login-form-0.1.1/README.md` & `st-login-form-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # :lock: st-login-form
 
 A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.
 
 ![Form screenshot](assets/screenshot.png)
 
-The login form collapses after login to no occupy screen-space.
+The login form collapses after login to free screen-space.
 
 ## :computer: Demo app
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://st-lgn-form.streamlit.app/)
 
-## :construction: Installation instructions 
+## :construction: Installation 
 
 1. Install `st-login-form` 
 ```sh
 pip install st-login-form
 ```
 2. Create a Supabase project as mentioned [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/supabase#sign-in-to-supabase-and-create-a-project)
 3. Create a table to store the usernames and passwords. The table name and column names can be as per your choice.
@@ -46,24 +46,26 @@
       )
     )
   ) tablespace pg_default;
 ```
 4. Follow the rest of the steps from [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/supabase#copy-your-app-secrets-to-the-cloud) to connect your Streamlit app to Supabase
 
 
-## :pen: Usage instructions
+## :pen: Usage
 
 `login_form()` sets `session_state["authenticated"]` to `True` if the login is successful, `session_state["username"]` to the `username` or new or existing user, and to `None` for guest login.
 
+Returns supabase `Client` instance.
+
 ```python
 import streamlit as st
 
 from streamlit_login import login_form
 
-login_form()
+client = login_form()
 
 if st.session_state["authenticated"]:
     if st.session_state["username"]:
         st.success(f"Welcome {st.session_state['username']}")
     else:
         st.success("Welcome guest")
 else:
```

### Comparing `st-login-form-0.1.1/setup.py` & `st-login-form-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="st-login-form",
-    version="0.1.1",
+    version="0.2.0",
     author="Siddhant Sadangi",
     author_email="siddhant.sadangi@gmail.com",
     description="A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
@@ -23,9 +23,9 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: User Interfaces",
     ],
     keywords=["streamlit", "login"],
     python_requires=">=3.8",
-    install_requires=["streamlit>=1.2", "jinja2"],
+    install_requires=["streamlit>=1.2", "jinja2", "supabase"],
 )
```

### Comparing `st-login-form-0.1.1/src/st_login_form/__init__.py` & `st-login-form-0.2.0/src/st_login_form/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,24 +37,27 @@
     login_password_label: str = "Enter your password",
     login_password_placeholder: str = None,
     login_password_help: str = None,
     login_submit_label: str = "Login",
     login_success_message: str = "Login succeeded :tada:",
     login_error_message: str = "Wrong username/password :x: ",
     guest_submit_label: str = "Guest login",
-) -> None:
+) -> Client:
     """Creates a user login form in Streamlit apps.
 
     Connects to a Supabase DB using `SUPABASE_URL` and `SUPABASE_KEY` Streamlit secrets.
     Sets `session_state["authenticated"]` to True if the login is successful.
     Sets `session_state["username"]` to provided username or new or existing user, and to `None` for guest login.
+
+    Returns:
+    Supabase client instance
     """
 
     # Initialize supabase connection
-    supabase = init_connection()
+    client = init_connection()
 
     # User Authentication
     if "authenticated" not in st.session_state:
         st.session_state["authenticated"] = False
 
     if "username" not in st.session_state:
         st.session_state["username"] = None
@@ -97,15 +100,15 @@
                 if st.form_submit_button(
                     label=create_submit_label,
                     type="primary",
                     disabled=st.session_state["authenticated"],
                 ):
                     try:
                         data, _ = (
-                            supabase.table(user_tablename)
+                            client.table(user_tablename)
                             .insert({username_col: username, password_col: password})
                             .execute()
                         )
                     except Exception as e:
                         st.error(e.message)
                     else:
                         login_success(create_success_message, username)
@@ -130,15 +133,15 @@
 
                 if st.form_submit_button(
                     label=login_submit_label,
                     disabled=st.session_state["authenticated"],
                     type="primary",
                 ):
                     data, _ = (
-                        supabase.table(user_tablename)
+                        client.table(user_tablename)
                         .select(f"{username_col}, {password_col}")
                         .eq(username_col, username)
                         .eq(password_col, password)
                         .execute()
                     )
 
                     if len(data[-1]) > 0:
@@ -152,14 +155,16 @@
                 if st.button(
                     label=guest_submit_label,
                     type="primary",
                     disabled=st.session_state["authenticated"],
                 ):
                     st.session_state["authenticated"] = True
 
+        return client
+
 
 def main() -> None:
     login_form(
         create_username_placeholder="Username will be visible in the global leaderboard.",
         create_password_placeholder="⚠️ Password will be stored as plain text. You won't be able to recover it if you forget.",
         guest_submit_label="Play as a guest ⚠️ Scores won't be saved",
     )
```

### Comparing `st-login-form-0.1.1/src/st_login_form.egg-info/PKG-INFO` & `st-login-form-0.2.0/src/st_login_form.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-login-form
-Version: 0.1.1
+Version: 0.2.0
 Summary: A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.
 Author: Siddhant Sadangi
 Author-email: siddhant.sadangi@gmail.com
 Keywords: streamlit,login
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -18,20 +18,20 @@
 
 # :lock: st-login-form
 
 A streamlit component that creates a user login form connected to a Supabase DB. It lets users create a new username and password, login to an existing account, or login as an anonymous guest.
 
 ![Form screenshot](assets/screenshot.png)
 
-The login form collapses after login to no occupy screen-space.
+The login form collapses after login to free screen-space.
 
 ## :computer: Demo app
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://st-lgn-form.streamlit.app/)
 
-## :construction: Installation instructions 
+## :construction: Installation 
 
 1. Install `st-login-form` 
 ```sh
 pip install st-login-form
 ```
 2. Create a Supabase project as mentioned [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/supabase#sign-in-to-supabase-and-create-a-project)
 3. Create a table to store the usernames and passwords. The table name and column names can be as per your choice.
@@ -64,24 +64,26 @@
       )
     )
   ) tablespace pg_default;
 ```
 4. Follow the rest of the steps from [here](https://docs.streamlit.io/knowledge-base/tutorials/databases/supabase#copy-your-app-secrets-to-the-cloud) to connect your Streamlit app to Supabase
 
 
-## :pen: Usage instructions
+## :pen: Usage
 
 `login_form()` sets `session_state["authenticated"]` to `True` if the login is successful, `session_state["username"]` to the `username` or new or existing user, and to `None` for guest login.
 
+Returns supabase `Client` instance.
+
 ```python
 import streamlit as st
 
 from streamlit_login import login_form
 
-login_form()
+client = login_form()
 
 if st.session_state["authenticated"]:
     if st.session_state["username"]:
         st.success(f"Welcome {st.session_state['username']}")
     else:
         st.success("Welcome guest")
 else:
```

