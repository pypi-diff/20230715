# Comparing `tmp/barladb-0.1.2.tar.gz` & `tmp/barladb-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barladb-0.1.2.tar", last modified: Sat Jul 15 14:25:30 2023, max compression
+gzip compressed data, was "barladb-0.1.4.tar", last modified: Sat Jul 15 14:32:44 2023, max compression
```

## Comparing `barladb-0.1.2.tar` & `barladb-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 14:25:30.709229 barladb-0.1.2/
--rw-rw-rw-   0        0        0     3122 2023-07-15 14:25:30.709229 barladb-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-15 14:25:30.704196 barladb-0.1.2/barladb/
--rw-rw-rw-   0        0        0      342 2023-07-15 11:58:29.000000 barladb-0.1.2/barladb/classes.py
--rw-rw-rw-   0        0        0       13 2023-07-15 10:58:22.000000 barladb-0.1.2/barladb/config.py
--rw-rw-rw-   0        0        0     2056 2023-07-15 13:51:16.000000 barladb-0.1.2/barladb/db.py
-drwxrwxrwx   0        0        0        0 2023-07-15 14:25:30.708218 barladb-0.1.2/barladb.egg-info/
--rw-rw-rw-   0        0        0     3122 2023-07-15 14:25:30.000000 barladb-0.1.2/barladb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-07-15 14:25:30.000000 barladb-0.1.2/barladb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 14:25:30.000000 barladb-0.1.2/barladb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-15 14:25:30.000000 barladb-0.1.2/barladb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-07-15 14:25:30.000000 barladb-0.1.2/barladb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 14:25:30.710295 barladb-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     3257 2023-07-15 14:25:22.000000 barladb-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 14:32:44.579240 barladb-0.1.4/
+-rw-rw-rw-   0        0        0     3312 2023-07-15 14:32:44.580542 barladb-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-15 14:32:44.575151 barladb-0.1.4/barladb/
+-rw-rw-rw-   0        0        0      342 2023-07-15 11:58:29.000000 barladb-0.1.4/barladb/classes.py
+-rw-rw-rw-   0        0        0       13 2023-07-15 10:58:22.000000 barladb-0.1.4/barladb/config.py
+-rw-rw-rw-   0        0        0     2057 2023-07-15 14:30:46.000000 barladb-0.1.4/barladb/db.py
+drwxrwxrwx   0        0        0        0 2023-07-15 14:32:44.579240 barladb-0.1.4/barladb.egg-info/
+-rw-rw-rw-   0        0        0     3312 2023-07-15 14:32:44.000000 barladb-0.1.4/barladb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-07-15 14:32:44.000000 barladb-0.1.4/barladb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 14:32:44.000000 barladb-0.1.4/barladb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-15 14:32:44.000000 barladb-0.1.4/barladb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-07-15 14:32:44.000000 barladb-0.1.4/barladb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 14:32:44.580542 barladb-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     3447 2023-07-15 14:32:21.000000 barladb-0.1.4/setup.py
```

### Comparing `barladb-0.1.2/PKG-INFO` & `barladb-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: barladb
-Version: 0.1.2
+Version: 0.1.4
 Summary: A very easy local database based on JSON
 Author: barlin41k
 Author-email: sasaigrypocta@gmail.com
 Description-Content-Type: text/markdown
 
 
+# Изменения:
+- В классе `Json` я указал неправильную функцию в файле `db.py`. `db.create` будет работать корректно!
+
 # Что такое barlaDB?
 - `barlaDB` - это легкая, простая библиотека для небольших проектов на `Python`, которая имеет очень лёгкий интерфейс. С ней смогут познакомиться даже чайники в `Python`!
 
 # Лёгкий пример использования
 ```python
 from barladb import db #Импортирование функций БД
 from barladb import config #Импортируем конфиг для того чтобы подключить логирование действий
```

### Comparing `barladb-0.1.2/barladb/db.py` & `barladb-0.1.4/barladb/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             print("BarlaDB: " + Fore.YELLOW + "Переменная с данными пуста." + Style.RESET_ALL)
         else:
             return
     except:
         print("BarlaDB: " + Fore.RED + f"Базы данных {filepath} не существует!" + Style.RESET_ALL)
         return
 def create(filename: str):
-    Json.set(filename, data)
+    Json.save(filename, data)
     if config.debug:
         print("BarlaDB: " + Fore.GREEN + f"База данных {filepath} была успешно создана!" + Style.RESET_ALL)
 def delete(filename: str):
   try:
     os.remove(f"{filename}.json")
     if config.debug:
       print("BarlaDB: " + Fore.GREEN + f"База данных {filepath} была успешно удалена!" + Style.RESET_ALL)
```

### Comparing `barladb-0.1.2/barladb.egg-info/PKG-INFO` & `barladb-0.1.4/barladb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: barladb
-Version: 0.1.2
+Version: 0.1.4
 Summary: A very easy local database based on JSON
 Author: barlin41k
 Author-email: sasaigrypocta@gmail.com
 Description-Content-Type: text/markdown
 
 
+# Изменения:
+- В классе `Json` я указал неправильную функцию в файле `db.py`. `db.create` будет работать корректно!
+
 # Что такое barlaDB?
 - `barlaDB` - это легкая, простая библиотека для небольших проектов на `Python`, которая имеет очень лёгкий интерфейс. С ней смогут познакомиться даже чайники в `Python`!
 
 # Лёгкий пример использования
 ```python
 from barladb import db #Импортирование функций БД
 from barladb import config #Импортируем конфиг для того чтобы подключить логирование действий
```

### Comparing `barladb-0.1.2/setup.py` & `barladb-0.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from setuptools import setup
 
 setup(
     name='barladb',
-    version='0.1.2',
+    version='0.1.4',
     description='A very easy local database based on JSON',
     packages=['barladb'],
     author_email='sasaigrypocta@gmail.com',
     author="barlin41k",
     zip_safe=False,
     long_description='''
+# Изменения:
+- В классе `Json` я указал неправильную функцию в файле `db.py`. `db.create` будет работать корректно!
+
 # Что такое barlaDB?
 - `barlaDB` - это легкая, простая библиотека для небольших проектов на `Python`, которая имеет очень лёгкий интерфейс. С ней смогут познакомиться даже чайники в `Python`!
 
 # Лёгкий пример использования
 ```python
 from barladb import db #Импортирование функций БД
 from barladb import config #Импортируем конфиг для того чтобы подключить логирование действий
```

