# Comparing `tmp/python-mbedtls-2.7.0.tar.gz` & `tmp/python-mbedtls-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-mbedtls-2.7.0.tar", last modified: Sat May 27 19:44:02 2023, max compression
+gzip compressed data, was "python-mbedtls-2.7.1.tar", last modified: Sat Jul 15 09:44:52 2023, max compression
```

## Comparing `python-mbedtls-2.7.0.tar` & `python-mbedtls-2.7.1.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.977504 python-mbedtls-2.7.0/
--rw-rw-rw-   0        0        0     2310 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    13721 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/ChangeLog
--rw-rw-rw-   0        0        0     1112 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/LICENSE.txt
--rw-rw-rw-   0        0        0      458 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/MANIFEST.in
--rw-rw-rw-   0        0        0    14078 2023-05-27 19:44:02.977504 python-mbedtls-2.7.0/PKG-INFO
--rw-rw-rw-   0        0        0    13185 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.915009 python-mbedtls-2.7.0/docs/
-drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.915009 python-mbedtls-2.7.0/docs/source/
--rw-rw-rw-   0        0        0     2082 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/docs/source/apicipher.rst
--rw-rw-rw-   0        0        0      299 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/docs/source/apimd.rst
--rw-rw-rw-   0        0        0       93 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/docs/source/apimpi.rst
--rw-rw-rw-   0        0        0      125 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/docs/source/apipk.rst
--rw-rw-rw-   0        0        0       97 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/docs/source/apisecrets.rst
--rw-rw-rw-   0        0        0       93 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/docs/source/apitls.rst
--rw-rw-rw-   0        0        0       96 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/docs/source/apix509.rst
--rw-rw-rw-   0        0        0      520 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/docs/source/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.930631 python-mbedtls-2.7.0/programs/
--rw-rw-rw-   0        0        0     5770 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/programs/client.py
--rw-rw-rw-   0        0        0     6024 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/programs/server.py
--rw-rw-rw-   0        0        0     2221 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.930631 python-mbedtls-2.7.0/requirements/
--rw-rw-rw-   0        0        0       99 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements/build.in
--rw-rw-rw-   0        0        0      525 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements/build.txt
--rw-rw-rw-   0        0        0       26 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements/docs.in
--rw-rw-rw-   0        0        0      767 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements/docs.txt
--rw-rw-rw-   0        0        0      182 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements/tests.in
--rw-rw-rw-   0        0        0      992 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements/tests.txt
--rw-rw-rw-   0        0        0       25 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements/typing.in
--rw-rw-rw-   0        0        0      273 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements/typing.txt
--rw-rw-rw-   0        0        0      209 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.930631 python-mbedtls-2.7.0/scripts/
--rw-rw-rw-   0        0        0      700 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/build-wheel.sh
--rw-rw-rw-   0        0        0      167 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/check-future-annotations.sh
--rw-rw-rw-   0        0        0      151 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/check-license-header.sh
--rw-rw-rw-   0        0        0      169 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/deploy.sh
--rw-rw-rw-   0        0        0      503 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/download-mbedtls.sh
--rw-rw-rw-   0        0        0      483 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/install-mbedtls.sh
--rw-rw-rw-   0        0        0     1038 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/install-pymbedtls.sh
--rw-rw-rw-   0        0        0      256 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/run-tests.sh
--rw-rw-rw-   0        0        0      732 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/start-devpi.sh
--rw-rw-rw-   0        0        0       45 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/stop-devpi.sh
--rw-rw-rw-   0        0        0      277 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/scripts/update-reqs.sh
--rw-rw-rw-   0        0        0       42 2023-05-27 19:44:02.977504 python-mbedtls-2.7.0/setup.cfg
--rw-rw-rw-   0        0        0     6131 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.915009 python-mbedtls-2.7.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.961879 python-mbedtls-2.7.0/src/mbedtls/
--rw-rw-rw-   0        0        0      819 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/__init__.py
--rw-rw-rw-   0        0        0      495 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_asn1.pxd
--rw-rw-rw-   0        0        0      168 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_debug.pxd
--rw-rw-rw-   0        0        0     1617 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_dhm.pxd
--rw-rw-rw-   0        0        0     2287 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_ecdh.pxd
--rw-rw-rw-   0        0        0     1036 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_ecdsa.pxd
--rw-rw-rw-   0        0        0     4499 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_ecp.pxd
--rw-rw-rw-   0        0        0     2092 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_md.pxd
--rw-rw-rw-   0        0        0     1209 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_md.pyi
--rw-rw-rw-   0        0        0     8152 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_md.pyx
--rw-rw-rw-   0        0        0      183 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_platform.pxd
--rw-rw-rw-   0        0        0      151 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_platform.pyi
--rw-rw-rw-   0        0        0      262 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_platform.pyx
--rw-rw-rw-   0        0        0     2844 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_random.pxd
--rw-rw-rw-   0        0        0      925 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_random.pyi
--rw-rw-rw-   0        0        0     4892 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_random.pyx
--rw-rw-rw-   0        0        0      922 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_ringbuf.pxd
--rw-rw-rw-   0        0        0     5607 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_ringbuf.pyx
--rw-rw-rw-   0        0        0     1260 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_rsa.pxd
--rw-rw-rw-   0        0        0      825 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_timing.pxd
--rw-rw-rw-   0        0        0    14971 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_tls.pxd
--rw-rw-rw-   0        0        0     4259 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_tls.pyi
--rw-rw-rw-   0        0        0    43292 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_tls.pyx
--rw-rw-rw-   0        0        0    17041 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/_tlsi.py
-drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.961879 python-mbedtls-2.7.0/src/mbedtls/cipher/
--rw-rw-rw-   0        0        0     2810 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/AES.py
--rw-rw-rw-   0        0        0     1494 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/ARC4.py
--rw-rw-rw-   0        0        0     2095 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/ARIA.py
--rw-rw-rw-   0        0        0     1747 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/Blowfish.py
--rw-rw-rw-   0        0        0     2317 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/CHACHA20.py
--rw-rw-rw-   0        0        0     1838 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/Camellia.py
--rw-rw-rw-   0        0        0     1635 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/DES.py
--rw-rw-rw-   0        0        0     1725 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/DES3.py
--rw-rw-rw-   0        0        0     1718 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/DES3dbl.py
--rw-rw-rw-   0        0        0     2474 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/__init__.py
--rw-rw-rw-   0        0        0     5241 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/_cipher.pxd
--rw-rw-rw-   0        0        0     1651 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/_cipher.pyi
--rw-rw-rw-   0        0        0     9518 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/cipher/_cipher.pyx
--rw-rw-rw-   0        0        0      183 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/exceptions.pxd
--rw-rw-rw-   0        0        0      329 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/exceptions.pyi
--rw-rw-rw-   0        0        0     1494 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/exceptions.pyx
--rw-rw-rw-   0        0        0     2734 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/hashlib.py
--rw-rw-rw-   0        0        0      862 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/hkdf.pxd
--rw-rw-rw-   0        0        0      586 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/hkdf.pyi
--rw-rw-rw-   0        0        0     5118 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/hkdf.pyx
--rw-rw-rw-   0        0        0     2987 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/hmac.py
--rw-rw-rw-   0        0        0     3238 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/mpi.pxd
--rw-rw-rw-   0        0        0     3625 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/mpi.pyi
--rw-rw-rw-   0        0        0    11411 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/mpi.pyx
--rw-rw-rw-   0        0        0     4408 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/pk.pxd
--rw-rw-rw-   0        0        0     8158 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/pk.pyi
--rw-rw-rw-   0        0        0    36634 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/pk.pyx
--rw-rw-rw-   0        0        0        0 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/py.typed
--rw-rw-rw-   0        0        0     1723 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/secrets.py
--rw-rw-rw-   0        0        0    15543 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/tls.py
--rw-rw-rw-   0        0        0      333 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/version.pxd
--rw-rw-rw-   0        0        0      457 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/version.pyi
--rw-rw-rw-   0        0        0     1665 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/version.pyx
--rw-rw-rw-   0        0        0     9497 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/x509.pxd
--rw-rw-rw-   0        0        0     5740 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/x509.pyi
--rw-rw-rw-   0        0        0    32201 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/src/mbedtls/x509.pyx
-drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.961879 python-mbedtls-2.7.0/src/python_mbedtls.egg-info/
--rw-rw-rw-   0        0        0    14078 2023-05-27 19:44:02.000000 python-mbedtls-2.7.0/src/python_mbedtls.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2758 2023-05-27 19:44:02.000000 python-mbedtls-2.7.0/src/python_mbedtls.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 19:44:02.000000 python-mbedtls-2.7.0/src/python_mbedtls.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-05-27 19:44:02.000000 python-mbedtls-2.7.0/src/python_mbedtls.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-27 19:44:02.000000 python-mbedtls-2.7.0/src/python_mbedtls.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 19:44:02.977504 python-mbedtls-2.7.0/tests/
--rw-rw-rw-   0        0        0     1928 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/conftest.py
--rw-rw-rw-   0        0        0     1375 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_assertion_rewriting.py
--rw-rw-rw-   0        0        0    13296 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_cipher.py
--rw-rw-rw-   0        0        0      673 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_error.py
--rw-rw-rw-   0        0        0    11093 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_hkdf.py
--rw-rw-rw-   0        0        0     6915 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_md.py
--rw-rw-rw-   0        0        0     7640 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_mpi.py
--rw-rw-rw-   0        0        0    19072 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_pk.py
--rw-rw-rw-   0        0        0      317 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_platform.py
--rw-rw-rw-   0        0        0     4128 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_random.py
--rw-rw-rw-   0        0        0      715 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_readme.py
--rw-rw-rw-   0        0        0     8157 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_ringbuf.py
--rw-rw-rw-   0        0        0     1637 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_secrets.py
--rw-rw-rw-   0        0        0    38946 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_tls.py
--rw-rw-rw-   0        0        0      879 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_version.py
--rw-rw-rw-   0        0        0    10426 2023-05-27 19:43:37.000000 python-mbedtls-2.7.0/tests/test_x509.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-15 09:44:52.681643 python-mbedtls-2.7.1/
+-rw-r--r--   0 runner     (501) staff       (20)     2244 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/CONTRIBUTING.md
+-rw-r--r--   0 runner     (501) staff       (20)    13338 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/ChangeLog
+-rw-r--r--   0 runner     (501) staff       (20)     1091 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/LICENSE.txt
+-rw-r--r--   0 runner     (501) staff       (20)      441 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)    13629 2023-07-15 09:44:52.681125 python-mbedtls-2.7.1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    12757 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/README.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-15 09:44:52.623808 python-mbedtls-2.7.1/docs/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-15 09:44:52.632735 python-mbedtls-2.7.1/docs/source/
+-rw-r--r--   0 runner     (501) staff       (20)     1981 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/docs/source/apicipher.rst
+-rw-r--r--   0 runner     (501) staff       (20)      283 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/docs/source/apimd.rst
+-rw-r--r--   0 runner     (501) staff       (20)       89 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/docs/source/apimpi.rst
+-rw-r--r--   0 runner     (501) staff       (20)      119 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/docs/source/apipk.rst
+-rw-r--r--   0 runner     (501) staff       (20)       93 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/docs/source/apisecrets.rst
+-rw-r--r--   0 runner     (501) staff       (20)       89 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/docs/source/apitls.rst
+-rw-r--r--   0 runner     (501) staff       (20)       92 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/docs/source/apix509.rst
+-rw-r--r--   0 runner     (501) staff       (20)      492 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/docs/source/index.rst
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-15 09:44:52.633576 python-mbedtls-2.7.1/programs/
+-rwxr-xr-x   0 runner     (501) staff       (20)     5488 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/programs/client.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     5732 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/programs/server.py
+-rw-r--r--   0 runner     (501) staff       (20)     2118 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/pyproject.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-15 09:44:52.637390 python-mbedtls-2.7.1/requirements/
+-rw-r--r--   0 runner     (501) staff       (20)       94 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/requirements/build.in
+-rw-r--r--   0 runner     (501) staff       (20)      487 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/requirements/build.txt
+-rw-r--r--   0 runner     (501) staff       (20)       24 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/requirements/docs.in
+-rw-r--r--   0 runner     (501) staff       (20)      733 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/requirements/docs.txt
+-rw-r--r--   0 runner     (501) staff       (20)      165 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/requirements/tests.in
+-rw-r--r--   0 runner     (501) staff       (20)      911 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/requirements/tests.txt
+-rw-r--r--   0 runner     (501) staff       (20)       23 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/requirements/typing.in
+-rw-r--r--   0 runner     (501) staff       (20)      269 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/requirements/typing.txt
+-rw-r--r--   0 runner     (501) staff       (20)      201 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-15 09:44:52.642576 python-mbedtls-2.7.1/scripts/
+-rwxr-xr-x   0 runner     (501) staff       (20)      660 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/scripts/build-wheel.sh
+-rwxr-xr-x   0 runner     (501) staff       (20)      160 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/scripts/check-future-annotations.sh
+-rwxr-xr-x   0 runner     (501) staff       (20)      144 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/scripts/check-license-header.sh
+-rwxr-xr-x   0 runner     (501) staff       (20)      158 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/scripts/deploy.sh
+-rwxr-xr-x   0 runner     (501) staff       (20)      471 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/scripts/download-mbedtls.sh
+-rwxr-xr-x   0 runner     (501) staff       (20)      456 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/scripts/install-mbedtls.sh
+-rwxr-xr-x   0 runner     (501) staff       (20)      991 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/scripts/install-pymbedtls.sh
+-rwxr-xr-x   0 runner     (501) staff       (20)      245 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/scripts/run-tests.sh
+-rwxr-xr-x   0 runner     (501) staff       (20)      691 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/scripts/start-devpi.sh
+-rwxr-xr-x   0 runner     (501) staff       (20)       40 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/scripts/stop-devpi.sh
+-rwxr-xr-x   0 runner     (501) staff       (20)      263 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/scripts/update-reqs.sh
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-07-15 09:44:52.681756 python-mbedtls-2.7.1/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     5921 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-15 09:44:52.625279 python-mbedtls-2.7.1/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-15 09:44:52.664981 python-mbedtls-2.7.1/src/mbedtls/
+-rw-r--r--   0 runner     (501) staff       (20)      781 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      479 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_asn1.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      163 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_debug.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     1568 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_dhm.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     2221 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_ecdh.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     1002 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_ecdsa.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     4356 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_ecp.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     2021 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_md.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     1161 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_md.pyi
+-rw-r--r--   0 runner     (501) staff       (20)     7888 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_md.pyx
+-rw-r--r--   0 runner     (501) staff       (20)      177 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_platform.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      145 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_platform.pyi
+-rw-r--r--   0 runner     (501) staff       (20)      249 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_platform.pyx
+-rw-r--r--   0 runner     (501) staff       (20)     2762 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_random.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      897 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_random.pyi
+-rw-r--r--   0 runner     (501) staff       (20)     4732 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_random.pyx
+-rw-r--r--   0 runner     (501) staff       (20)      889 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_ringbuf.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     5392 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_ringbuf.pyx
+-rw-r--r--   0 runner     (501) staff       (20)     1224 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_rsa.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_timing.pxd
+-rw-r--r--   0 runner     (501) staff       (20)    14515 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_tls.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     4126 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_tls.pyi
+-rw-r--r--   0 runner     (501) staff       (20)    42074 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_tls.pyx
+-rw-r--r--   0 runner     (501) staff       (20)    16526 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/_tlsi.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-15 09:44:52.670891 python-mbedtls-2.7.1/src/mbedtls/cipher/
+-rw-r--r--   0 runner     (501) staff       (20)     2585 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/cipher/AES.py
+-rw-r--r--   0 runner     (501) staff       (20)     1322 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/cipher/ARC4.py
+-rw-r--r--   0 runner     (501) staff       (20)     1907 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/cipher/ARIA.py
+-rw-r--r--   0 runner     (501) staff       (20)     1572 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/cipher/Blowfish.py
+-rw-r--r--   0 runner     (501) staff       (20)     2115 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/cipher/CHACHA20.py
+-rw-r--r--   0 runner     (501) staff       (20)     1658 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/cipher/Camellia.py
+-rw-r--r--   0 runner     (501) staff       (20)     1461 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/cipher/DES.py
+-rw-r--r--   0 runner     (501) staff       (20)     1548 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/cipher/DES3.py
+-rw-r--r--   0 runner     (501) staff       (20)     1539 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/cipher/DES3dbl.py
+-rw-r--r--   0 runner     (501) staff       (20)     2218 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/cipher/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5077 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/cipher/_cipher.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     1585 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/cipher/_cipher.pyi
+-rw-r--r--   0 runner     (501) staff       (20)     9255 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/cipher/_cipher.pyx
+-rw-r--r--   0 runner     (501) staff       (20)      178 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/exceptions.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      317 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/exceptions.pyi
+-rw-r--r--   0 runner     (501) staff       (20)     1438 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/exceptions.pyx
+-rw-r--r--   0 runner     (501) staff       (20)     2524 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/hashlib.py
+-rw-r--r--   0 runner     (501) staff       (20)      834 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/hkdf.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      559 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/hkdf.pyi
+-rw-r--r--   0 runner     (501) staff       (20)     4939 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/hkdf.pyx
+-rw-r--r--   0 runner     (501) staff       (20)     2773 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/hmac.py
+-rw-r--r--   0 runner     (501) staff       (20)     3117 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/mpi.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     3535 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/mpi.pyi
+-rw-r--r--   0 runner     (501) staff       (20)    11039 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/mpi.pyx
+-rw-r--r--   0 runner     (501) staff       (20)     4277 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/pk.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     7893 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/pk.pyi
+-rw-r--r--   0 runner     (501) staff       (20)    35486 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/pk.pyx
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/py.typed
+-rw-r--r--   0 runner     (501) staff       (20)     1544 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/secrets.py
+-rw-r--r--   0 runner     (501) staff       (20)    15317 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/tls.py
+-rw-r--r--   0 runner     (501) staff       (20)      325 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/version.pxd
+-rw-r--r--   0 runner     (501) staff       (20)      435 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/version.pyi
+-rw-r--r--   0 runner     (501) staff       (20)     1603 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/version.pyx
+-rw-r--r--   0 runner     (501) staff       (20)     9188 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/x509.pxd
+-rw-r--r--   0 runner     (501) staff       (20)     5543 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/x509.pyi
+-rw-r--r--   0 runner     (501) staff       (20)    31159 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/src/mbedtls/x509.pyx
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-15 09:44:52.673133 python-mbedtls-2.7.1/src/python_mbedtls.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    13629 2023-07-15 09:44:52.000000 python-mbedtls-2.7.1/src/python_mbedtls.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2758 2023-07-15 09:44:52.000000 python-mbedtls-2.7.1/src/python_mbedtls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-15 09:44:52.000000 python-mbedtls-2.7.1/src/python_mbedtls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       26 2023-07-15 09:44:52.000000 python-mbedtls-2.7.1/src/python_mbedtls.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        8 2023-07-15 09:44:52.000000 python-mbedtls-2.7.1/src/python_mbedtls.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-15 09:44:52.680552 python-mbedtls-2.7.1/tests/
+-rw-r--r--   0 runner     (501) staff       (20)     1857 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/tests/conftest.py
+-rw-r--r--   0 runner     (501) staff       (20)     1333 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/tests/test_assertion_rewriting.py
+-rw-r--r--   0 runner     (501) staff       (20)    12864 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/tests/test_cipher.py
+-rw-r--r--   0 runner     (501) staff       (20)      647 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/tests/test_error.py
+-rw-r--r--   0 runner     (501) staff       (20)    10757 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/tests/test_hkdf.py
+-rw-r--r--   0 runner     (501) staff       (20)     6564 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/tests/test_md.py
+-rw-r--r--   0 runner     (501) staff       (20)     7286 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/tests/test_mpi.py
+-rw-r--r--   0 runner     (501) staff       (20)    18305 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/tests/test_pk.py
+-rw-r--r--   0 runner     (501) staff       (20)      302 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/tests/test_platform.py
+-rw-r--r--   0 runner     (501) staff       (20)     4004 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/tests/test_random.py
+-rw-r--r--   0 runner     (501) staff       (20)      689 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/tests/test_readme.py
+-rw-r--r--   0 runner     (501) staff       (20)     7869 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/tests/test_ringbuf.py
+-rw-r--r--   0 runner     (501) staff       (20)     1577 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/tests/test_secrets.py
+-rw-r--r--   0 runner     (501) staff       (20)    37589 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/tests/test_tls.py
+-rw-r--r--   0 runner     (501) staff       (20)      840 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/tests/test_version.py
+-rw-r--r--   0 runner     (501) staff       (20)     9929 2023-07-15 09:44:48.000000 python-mbedtls-2.7.1/tests/test_x509.py
```

### Comparing `python-mbedtls-2.7.0/CONTRIBUTING.md` & `python-mbedtls-2.7.1/CONTRIBUTING.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-
-# Contributing to `python-mbedtls`
-
-## Code of conduct
-
-Simply be a nice person in all communications.
-
-
-## Coding guidelines
-
-### Coding style
-
-Both Cython and Python code must follow the [PEP 8 -- Style guide for
-Python code](https://www.python.org/dev/peps/pep-0008/).  This includes
-the tests.  Although [black](https://github.com/ambv/black) does not yet
-support Cython, new code should resemble its output.
-
-### Tests
-
-`python-mbedtls` uses [pytest](https://docs.pytest.org/en/latest/) and
-makes extensive use of fixtures.  New tests should follow the already
-existing style.
-
-In general, every new method must be called at least once by a test and
-these tests must be short.
-[Parametrize](https://docs.pytest.org/en/latest/parametrize.html) tests
-and fixtures to check edge cases, etc.
-
-Demonstrate common use cases with extra tests for new features.
-
-Also see [tests/test_hkdf.py](tests/test_hkdf.py) for examples
-of test vectors.
-
-*NOTE: PRs without tests will no be merged!*
-
-### Documentation
-
-Document every new class and public method using [Google-style
-docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/).
-Adapting the documentation from `libmbedtls` is acceptable in most
-cases.  See also [PEP 257 -- Docstring
-Conventions](https://www.python.org/dev/peps/pep-0257/).
-
-For new features, an example usage should be added to the README.
-
-Finally, you should summarize your contribution with a one-liner in the
-ChangeLog.  Have your name or handle here as well.
-
-## Commit guidelines
-
-`python-mbedtls` follows a linear workflow where every feature is
-fast-forward merged onto the master branch.
-
-The rule for the size of a commit is one feature per commit and one
-commit per feature.  In particular, do not mix bug fixes and new
-features in one commit but open several pull requests instead.
-
-The commit messages start with the file/feature modified or added,
-followed by colon and a space, followed by a short title.  This first
-line should not exceed 50 characters.  It may be followed by an empty
-line and a long description.  Lines on the long description should fit
-within 72 characters and markdown formatting is allowed.
-
-See also:
- * [Pro Git](https://git-scm.com/book/en/v2).
- * `git log` for examples.
+
+# Contributing to `python-mbedtls`
+
+## Code of conduct
+
+Simply be a nice person in all communications.
+
+
+## Coding guidelines
+
+### Coding style
+
+Both Cython and Python code must follow the [PEP 8 -- Style guide for
+Python code](https://www.python.org/dev/peps/pep-0008/).  This includes
+the tests.  Although [black](https://github.com/ambv/black) does not yet
+support Cython, new code should resemble its output.
+
+### Tests
+
+`python-mbedtls` uses [pytest](https://docs.pytest.org/en/latest/) and
+makes extensive use of fixtures.  New tests should follow the already
+existing style.
+
+In general, every new method must be called at least once by a test and
+these tests must be short.
+[Parametrize](https://docs.pytest.org/en/latest/parametrize.html) tests
+and fixtures to check edge cases, etc.
+
+Demonstrate common use cases with extra tests for new features.
+
+Also see [tests/test_hkdf.py](tests/test_hkdf.py) for examples
+of test vectors.
+
+*NOTE: PRs without tests will no be merged!*
+
+### Documentation
+
+Document every new class and public method using [Google-style
+docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/).
+Adapting the documentation from `libmbedtls` is acceptable in most
+cases.  See also [PEP 257 -- Docstring
+Conventions](https://www.python.org/dev/peps/pep-0257/).
+
+For new features, an example usage should be added to the README.
+
+Finally, you should summarize your contribution with a one-liner in the
+ChangeLog.  Have your name or handle here as well.
+
+## Commit guidelines
+
+`python-mbedtls` follows a linear workflow where every feature is
+fast-forward merged onto the master branch.
+
+The rule for the size of a commit is one feature per commit and one
+commit per feature.  In particular, do not mix bug fixes and new
+features in one commit but open several pull requests instead.
+
+The commit messages start with the file/feature modified or added,
+followed by colon and a space, followed by a short title.  This first
+line should not exceed 50 characters.  It may be followed by an empty
+line and a long description.  Lines on the long description should fit
+within 72 characters and markdown formatting is allowed.
+
+See also:
+ * [Pro Git](https://git-scm.com/book/en/v2).
+ * `git log` for examples.
```

### Comparing `python-mbedtls-2.7.0/ChangeLog` & `python-mbedtls-2.7.1/ChangeLog`

 * *Files 23% similar despite different names*

```diff
@@ -1,468 +1,473 @@
-[2.7.0] - 2023-05-27
-
-* ci: Update wheels to mbedtls 2.28.3.
-* tls: Add `setmtu`, for the maximum transport unit, and an
-optional `max_fragmentation_length` configuration.
-
-[2.6.1] - 2023-02-15
-
-* cipher: Fix encryption and decryption of 0-length strings.
-
-[2.6.0] - 2023-01-15
-
-* ci: Update wheels to mbedtls 2.28.2.
-* md: Fixup cases where "algorithms_available" would return actually
-unavailable algorithms.
-* pk: Remove trailing null bytes from PEM format.  (Issue #75)
-* cipher: `get_supported_ciphers()` now returns a sequence (consistent
-with the md "available_*" functions).
-
-[2.5.1] - 2022-09-07
-
-* Add missing pyi file to wheel.
-
-[2.5.0] - 2022-09-02
-
-* Add Python 3.11 build.
-* Add musllinux build.
-
-[2.4.0] - 2022-08-07
-
-* typing: Complete typing.
-* tls: Improve support for connectionless DTLS.
-* tls: Implement and fix type of `TLSWrappedSocket.recv_into()`.
-* tls: Fix type of `TLSWrappedSocket.recvfrom_into()`.
-
-[2.3.1] - 2022-07-29
-
-* tls: Fix argument to `_enable_debug_output()`.  The function
-now takes a configured context instead of a MbedTLSConfiguration.
-* typing: Add type annotations to more modules.
-
-[2.3.0] - 2022-07-20
-
-* tls: Improve typing and remove base class to TLSConfiguration
-and DTLSConfiguration.
-* Update wheels to mbedtls 2.28.1
-
-[2.2.0] - 2022-06-18
-
-* pk: Fix choice of the curve in ECC (PR 63).  Before this, the
-curve chosen was ignored and the `ECC.generate()` would always
-use the same one.
-
-* pk: Improve handling of CURVE25519 and CURVE448 in ECC (PR 63).
-* pk: ECDHClient and ECDHServer take an ECC key in `__init__()`.
-* pk: Remove `to_ECDH_{client,server}` methods from ECC.
-* pk: Make key accessors public (and remove the private ones).
-
-* docs: Resurrect gh-pages.
-
-* *: Add typing information.  The typing information is in an alpha
-stage, incomplete, and subject to change.  We also welcome pull requests.
-
-[2.1.0] - 2022-04-28
-
-* tls: Add TLS 1.3 support.
-* tls: TLSWrappedBuffer.shutdown() does not raise anymore when
-the connection is already closed.
-* tls: Make TLSWrappedBuffer picklable in the limited cases documented
-under `mbedtls_ssl_context_load` and `mbedtls_ssl_context_save` in
-the backend.
-* mpi: Remove is_prime() method.
-
-[2.0.1] - 2022-04-12
-
-* tls: Fix check of arguments to TLSWrappedSocket.sendto().
-
-[2.0.0] - 2022-04-07
-
-* tls: Context and TLSWrappedBuffer are now entirely separated.
-** The contexts are now picklable.
-** The contexts do not support TLSWrappedBuffer API anymore.
-* tls: TLSSession currently *unsupported*!
-* tls: Improved handshake logic with more appropriate signaling
-over WantReadError and WantWriteError.
-* Update wheels to mbedtls 2.28.0 (current LTS).
-
-[1.7.0] - 2022-03-23
-
-* cipher: CBC does not use PKCS7 padding by default and now requires a full
-block.  Encoding will raise ValueError otherwise.
-* tls: Add support for session caching.
-* tls: Implement `context.getpeercert()`.
-* tls: Add context manager to `TLSWrappedSocket`
-* programs: Add example DTLS and TLS client and server.
-* ci: Drop CircleCI.
-* Update wheels to mbedtls 2.16.12
-* Add support for Python 3.10.
-* Drop Python 3.6 (EOL).
-
-[1.6.0] - 2021-10-03
-
-* tls: Fix arguments of TLSWrappedSocket.sendto() method.
-* *: Add MacOS support and tests on GitHub.
-* *: Add Windows support and tests on GitHub.
-* *: Remove Travis-CI job: The main CI is moved to GitHub
-Actions because of the less FOSS-friendly policy by Travis CI.
-* *: Implement the pickling protocol (PEP 307).
-RingBuffer, ciphers, TLSConfiguration and DTLSConfiguration,
-and x509 certificates are copyable.  The other Cython classes
-are non-copyable.
-* tls: Fix missing DTLS-only parameters in DTLSConfiguration
-`__repr__()` and `__eq__()`.  Equality, especially, could
-have returned True for two configuration differing only on
-some parameters.
-* tls: Fix handling of min and max handshake timeout
-when set independently.
-* tls: Fix exception raised when unwrapping a
-`TLSWrappedSocket` before opening it.
-* tls: Augment size of the accept buffer for DTLS (nicho2).
-* Update wheels to mbedtls 2.16.11.
-
-[1.5.1] - 2020-12-30
-
-* doc: Do not document Python 2.7-3.5 as documented ;p
-
-[1.5.0] - 2020-12-30
-
-* ci: Drop Python < 3.6.
-* hashlib: Drop hash alias to hashlib.
-* cipher,tls,x509: Unsupported ciphers now consistently
-raise NotImplementedError.
-* upstream: The size of the IV in ECB mode is consistently 0.
-* Update wheels to mbedtls 2.16.9.
-* cython: Get rid of compilation warnings.
-
-[1.4.1] - 2020-11-30
-
-* *: The '*.pyx' files were missing from the archive
-on pypi.
-
-[1.4.0] - 2020-10-17
-
-* tls: Add accessors to min/max timeout DTLS handshake.
-* ci: Support Python 3.9 final.
-* ci: update wheels to mbedtls 2.16.8.
-* ci: Prepare experimental support for Python 3.10.
-
-[1.3.1] - 2020-07-23
-
-* *: Add support for Python 3.9.
-* update wheels to mbedtls 2.16.7.
-
-[1.3.0] - 2020-06-04
-
-* hash -> hashlib: Importing from `hash` is now deprecated.
-Import from `mbedtls.hashlib` now instead.
-* tls: fix bug (typo) in `tls.recvfrom_into()` that would make
-the method crash.
-
-[1.2.1]
-
-* update wheels to mbedtls 2.16.6
-
-[1.2.0] - 2020-03-10
-
-* ci: Partial support to Python 3.9
-* ci: Upgrade manylinux from 1 to 2010.
-* *: Drop Python 3.4
-
-[1.1.0] - 2020-02-22
-
-* tls: Add support to PSK for (D)TLS
-* tls: Fixup `access()` method for DTLS on Python 2.7 and 3.4.
-* tls: Ensure that the `ciphers` parameter is a tuple and let
-`ciphers` accessors return tuples.
-* update wheels to mbedtls 2.16.5
-
-[1.0.0] - 2020-01-05
-
-* ci: Add support to Python 3.8.
-* md: Support MD2 and MD4 algo.
-* ci: Update dependencies.
-
-[0.18.3]
-
-* setup.py: Refuse to build if mbedtls is too old.
-
-[0.18.2]
-
-* cipher: Increase test coverage and fix minor bugs.
-* tests: Do not assume that havege is missing as it could be included
-in some configurations.
-* tests: Make error reporting with memoryviews closer to pytest
-reporting for bytes.
-
-[0.18.1]
-
-* update wheels with 2.16.3.
-* version: Make `has_feature()` public.
-* tests: Skip tests to features that are not compiled in.
-* tests: Improve error reporting with memoryviews.
-
-[0.18.0] - 2019-05-11
-
-* secrets: Add PEP-506 conform secrets module for generating secrets.
-* cipher/hash/hmac: These modules and packages are now pure-Python.
-* mpi: Add bitwise operations.
-
-API Changes
-
-* pk.ECDHNaive: `generate()` returns the public key as an ECPoint and
-`import_peers_public()` now takes an ECPoint.  `import_peer_public(MPI)`
-is deprecated and will be removed in a future release.  Further note
-the `s` in `import_peers_public()`.
-* pk: Make `ECDH*.{public_key,private_key,peers_public_key}` public.  The
-private equivalents with a `_*` prefix are deprecated and will be removed in a
-future release.  Further note the `s` in `peers_public_key`.
-* _random: Privatize `Entropy` and refactor `Random` class.
-
-Bugfixes
-
-* mpi: Fix bug in `mpi.to_bytes()`.
-
-Misc.
-
-* *: Format Python files with `black`
-* ci: Check that the docs build in CI.
-* ci: Repair test coverage measurements on coveralls.
-* mpi: Simplify code for comparisons.
-* mpi: Add tests and better exceptions for `__pow__()`.
-
-
-[0.17.1] - 2019-04-16
-
-This is a bugfix release fixing several TLS issues.
-
-Misc.
-
-* Split download and install scripts.
-
-Bugfixes
-
-* tls: Split input and output buffers for TLS/TCP.
-* tls: Fixes issue with TLSv1 by reading greedily from the buffer.
-
-
-[0.17.0] - 2019-04-12
-
-* Add support to HKDF (HMAC key derivation function).
-
-Misc.
-
-* Change branching model to fast-forward merge on the master branch.
-* Change directive `language_level` from 2 to 3 for Cython.
-
-Bugfixes
-
-* *: Fixup handling of empty and `None` buffers (#20: Roman (inpos)).
-* hmac: Hmac now accepts the empty key (b"").
-
-
-[0.16.0] - 2019-04-04
-
-Add Chacha20/Poly1305 support (Stephen.Y).
-
-* cipher: Add support for the ARIA family.
-* cipher: Add OFB, XFB, and CHACHA/POLY modes and support for
-AEAD ciphers (Stephen.Y).
-* Update wheels with mbedtls 2.16.1.
-
-[0.15.0] - 2019-03-15
-
-Add DTLS support.  Both client side and server side are implemented.
-Setting the cookie on the server side is *not* optional in `python-mbedtls`.
-
-* pk: Add support for curves 448 and 25519 (Stephen.Y).
-
-Misc.
-
-* Update wheels with mbedtls 2.14.1.
-* version: Add accessors to the version of mbed TLS in use.
-* tls: Allow configuration of libmbedtls debug level.
-
-[0.14.1] - 2019-01-10
-
-Update wheels with mbedtls 2.7.9.
-
-[0.14.0] - 2019-01-08
-
-* Build and test on `manylinux1` (PEP 513) to distribute linux
-wheels with Mbed TLS.  It is not necessary anymore to install
-mbed TLS separately.
-* x509/CRL: Add support for upstream Mbed TLS version 2.7.2 and above.
-Note that this did not require changes in the library but only
-in the tests.
-* The library now internally uses a single global `Random` instance.
-This instance is not accessible from Python.
-* pk/DHServer, pk/DHClient: Increase test entropy to avoid
-flakey tests.
-
-API Changes
-
-* random: `Random()` now takes an optional `entropy` object
-as argument.
-* random: `Random.reseed()` now takes optional data that can be used
-to increase entropy.
-
-Bugfixes
-
-* mpi: Let MPI built from an empty byte (b"") be 0 as regular ints.
-
-[0.13.0] - 2018-10-25
-
-Add TLS support.  Both client side and server side are implemented.
-SSLv3 is not supported.  Session management and SNI callbacks are
-not implemented.
-
-API Changes
-
-* x509: `ca` and `max_path_length` basic constraints are now
-grouped into a `BasicConstraints` namedtuple.  It is possible
-to leave the basic constraints unset by passing None
-to `CRT.new(..., basic_constraints=None)`.
-* random: `random` module renamed `_random`.
-
-Bugfixes
-
-* mpi: GC now actually overwrites keys with random data.
-
-Misc.
-
-* pk: Improved error handling.
-* Declare mbedtls functions nogil.
-* The install script uses cmake to install mbedtls.
-
-[0.12.2] - 2018-09-10
-
-Misc.
-
-* New `property` syntax from Cython 0.24.
-* Fixup rendering on Pypi.
-* Update required deps.
-
-[0.12.1] - 2018-08-27
-
-Update version in `setup.py`.  No change in the code.
-
-[0.12.0] - 2018-08-27
-
-* x509: Add accessors to most fields of CRT, CSR, and CRL.
-The `x509` module can now be used to inspect existing certificates.
-* x509: The module now offers basic signing and
-verification capabilities.
-
-API Changes
-
-* pk: `from_{PEM,DER,buffer}` are now `classmethod`s to
-comply with PEP 543.
-* x509: `Certificate` class renamed `CRT`.
-* x509: `start` and `end` arguments renamed `not_before` and
-`not_after`; `md_alg` argument is now `digestmod`.
-* x509: Re-order the arguments of the `new()` methods.
-* exceptions: Rename `MbedTLSError` -> `TLSError` to comply
-with PEP 543.
-
-Misc
-
-* pk: `__eq__()` now also accepts DER (bytes) or PEM (str) formats.
-* x509: `__bytes__()` returns the certificates in the DER format.
-* x509: `__str__()` now returns a human-readable string.
-
-
-[0.11.1] - 2018-07-04
-
-Update changelog.  No changes in the code.
-
-
-[0.11.0] - 2018-07-01
-
-* Support Diffie-Hellman-Merkle key exchange.
-* MPIs (multi-precision integers) now implement the full
-`numbers.Integral` API.
-* MPIs are erased from memory upon garbage collection.
-* The `mpi` library is now public (renamed `_mpi` -> `mpi`).
-
-API Changes
-
-* pk: Methods that were previously returning a long integer now
-return an MPI.
-* exceptions: Rename `_ErrorBase` -> `MbedTLSError`.  It is now
-the only new exception.
-* exceptions: `mbedtls_strerror()` generates the error message.
-
-
-[0.10.0] - 2018-05-07
-
-Support elliptic curve cryptography
-
-* pk/ECC: Elliptic curve digital signature algorithm.
-* pk/ECDHServer, pk/ECDHClient: Elliptic curve Diffie-Hellman.
-The two classes together support ECDHE (ephemeral) as well.
-
-API Changes
-
-* pk/RSA: generate() returns the private key.
-* pk/RSA: to_DER() and to_PEM() are obsolete and will be removed.
-Users should call export_key() and export_public_key() instead.
-* pk/RSA: has_public() and has_private() are now private.
-Test if export_key() and export_public_key() are truthy
-or falsy instead.
-* pk/RSA: __str__() now returns the private key in PEM format.
-* pk/RSA: to_bytes() and __bytes__() now return the private key
-in DER format.
-
-Bugfix
-
-* pk: Increase the size of the buffer for sign, encrypt, decrypt
-
-Misc.
-
-* Use const memoryviews supported by Cython 0.28.0.
-* pk: pk is now a module instead of a package.
-
-[0.9.0] - 2018-03-14
-
-Misc.
-
-* Switch to semantic versioning.
-* Add pxd files to source distribution.
-
-
-[0.9] - 2018-03-13
-
-API Changes
-
-* x509/Certificate: next() returns the next certificate in a chain.
-* md: Implement block_size property.
-
-Misc.
-
-* Clean up imports.
-* Fix tests and packaging.
-* Change git merge policy to fast-forward on develop.
-
-
-[0.8 withdrawn] - 2018-02-24
-
-Support X.509 Certificates
-
-* x509/Certificate: X.509 certificate writer and parser.
-* x509/CSR: X.509 certificate signing request writer and parser.
-* x509/CRL: X.509 certificate revocation list and validation.
-
-API Changes
-
-* CipherBase/RSA: import_() method renamed from_buffer() for PEP 543.
-* CipherBase/RSA: export(format="PEM") method renamed to_PEM()
-* CipherBase/RSA: export(format="DER") method renamed to_DER()
-* CipherBase/RSA: from_DER(), from_PEM() to import from DER or PEM.
-* CipherBase/RSA: to_bytes() alias to_DER()
-
-
-[0.7] - 2018-02-04
-
-* Add support for Python 2.7, 3.5, and 3.6.
-* Tests ported from nosetest to pytest.
-* Setup continuous integration.
+[2.7.1] - 2023-07-15
+
+* tls: Fix missing close notify alert.
+* ci: Drop Python 3.7.
+
+[2.7.0] - 2023-05-27
+
+* ci: Update wheels to mbedtls 2.28.3.
+* tls: Add `setmtu`, for the maximum transport unit, and an
+optional `max_fragmentation_length` configuration.
+
+[2.6.1] - 2023-02-15
+
+* cipher: Fix encryption and decryption of 0-length strings.
+
+[2.6.0] - 2023-01-15
+
+* ci: Update wheels to mbedtls 2.28.2.
+* md: Fixup cases where "algorithms_available" would return actually
+unavailable algorithms.
+* pk: Remove trailing null bytes from PEM format.  (Issue #75)
+* cipher: `get_supported_ciphers()` now returns a sequence (consistent
+with the md "available_*" functions).
+
+[2.5.1] - 2022-09-07
+
+* Add missing pyi file to wheel.
+
+[2.5.0] - 2022-09-02
+
+* Add Python 3.11 build.
+* Add musllinux build.
+
+[2.4.0] - 2022-08-07
+
+* typing: Complete typing.
+* tls: Improve support for connectionless DTLS.
+* tls: Implement and fix type of `TLSWrappedSocket.recv_into()`.
+* tls: Fix type of `TLSWrappedSocket.recvfrom_into()`.
+
+[2.3.1] - 2022-07-29
+
+* tls: Fix argument to `_enable_debug_output()`.  The function
+now takes a configured context instead of a MbedTLSConfiguration.
+* typing: Add type annotations to more modules.
+
+[2.3.0] - 2022-07-20
+
+* tls: Improve typing and remove base class to TLSConfiguration
+and DTLSConfiguration.
+* Update wheels to mbedtls 2.28.1
+
+[2.2.0] - 2022-06-18
+
+* pk: Fix choice of the curve in ECC (PR 63).  Before this, the
+curve chosen was ignored and the `ECC.generate()` would always
+use the same one.
+
+* pk: Improve handling of CURVE25519 and CURVE448 in ECC (PR 63).
+* pk: ECDHClient and ECDHServer take an ECC key in `__init__()`.
+* pk: Remove `to_ECDH_{client,server}` methods from ECC.
+* pk: Make key accessors public (and remove the private ones).
+
+* docs: Resurrect gh-pages.
+
+* *: Add typing information.  The typing information is in an alpha
+stage, incomplete, and subject to change.  We also welcome pull requests.
+
+[2.1.0] - 2022-04-28
+
+* tls: Add TLS 1.3 support.
+* tls: TLSWrappedBuffer.shutdown() does not raise anymore when
+the connection is already closed.
+* tls: Make TLSWrappedBuffer picklable in the limited cases documented
+under `mbedtls_ssl_context_load` and `mbedtls_ssl_context_save` in
+the backend.
+* mpi: Remove is_prime() method.
+
+[2.0.1] - 2022-04-12
+
+* tls: Fix check of arguments to TLSWrappedSocket.sendto().
+
+[2.0.0] - 2022-04-07
+
+* tls: Context and TLSWrappedBuffer are now entirely separated.
+** The contexts are now picklable.
+** The contexts do not support TLSWrappedBuffer API anymore.
+* tls: TLSSession currently *unsupported*!
+* tls: Improved handshake logic with more appropriate signaling
+over WantReadError and WantWriteError.
+* Update wheels to mbedtls 2.28.0 (current LTS).
+
+[1.7.0] - 2022-03-23
+
+* cipher: CBC does not use PKCS7 padding by default and now requires a full
+block.  Encoding will raise ValueError otherwise.
+* tls: Add support for session caching.
+* tls: Implement `context.getpeercert()`.
+* tls: Add context manager to `TLSWrappedSocket`
+* programs: Add example DTLS and TLS client and server.
+* ci: Drop CircleCI.
+* Update wheels to mbedtls 2.16.12
+* Add support for Python 3.10.
+* Drop Python 3.6 (EOL).
+
+[1.6.0] - 2021-10-03
+
+* tls: Fix arguments of TLSWrappedSocket.sendto() method.
+* *: Add MacOS support and tests on GitHub.
+* *: Add Windows support and tests on GitHub.
+* *: Remove Travis-CI job: The main CI is moved to GitHub
+Actions because of the less FOSS-friendly policy by Travis CI.
+* *: Implement the pickling protocol (PEP 307).
+RingBuffer, ciphers, TLSConfiguration and DTLSConfiguration,
+and x509 certificates are copyable.  The other Cython classes
+are non-copyable.
+* tls: Fix missing DTLS-only parameters in DTLSConfiguration
+`__repr__()` and `__eq__()`.  Equality, especially, could
+have returned True for two configuration differing only on
+some parameters.
+* tls: Fix handling of min and max handshake timeout
+when set independently.
+* tls: Fix exception raised when unwrapping a
+`TLSWrappedSocket` before opening it.
+* tls: Augment size of the accept buffer for DTLS (nicho2).
+* Update wheels to mbedtls 2.16.11.
+
+[1.5.1] - 2020-12-30
+
+* doc: Do not document Python 2.7-3.5 as documented ;p
+
+[1.5.0] - 2020-12-30
+
+* ci: Drop Python < 3.6.
+* hashlib: Drop hash alias to hashlib.
+* cipher,tls,x509: Unsupported ciphers now consistently
+raise NotImplementedError.
+* upstream: The size of the IV in ECB mode is consistently 0.
+* Update wheels to mbedtls 2.16.9.
+* cython: Get rid of compilation warnings.
+
+[1.4.1] - 2020-11-30
+
+* *: The '*.pyx' files were missing from the archive
+on pypi.
+
+[1.4.0] - 2020-10-17
+
+* tls: Add accessors to min/max timeout DTLS handshake.
+* ci: Support Python 3.9 final.
+* ci: update wheels to mbedtls 2.16.8.
+* ci: Prepare experimental support for Python 3.10.
+
+[1.3.1] - 2020-07-23
+
+* *: Add support for Python 3.9.
+* update wheels to mbedtls 2.16.7.
+
+[1.3.0] - 2020-06-04
+
+* hash -> hashlib: Importing from `hash` is now deprecated.
+Import from `mbedtls.hashlib` now instead.
+* tls: fix bug (typo) in `tls.recvfrom_into()` that would make
+the method crash.
+
+[1.2.1]
+
+* update wheels to mbedtls 2.16.6
+
+[1.2.0] - 2020-03-10
+
+* ci: Partial support to Python 3.9
+* ci: Upgrade manylinux from 1 to 2010.
+* *: Drop Python 3.4
+
+[1.1.0] - 2020-02-22
+
+* tls: Add support to PSK for (D)TLS
+* tls: Fixup `access()` method for DTLS on Python 2.7 and 3.4.
+* tls: Ensure that the `ciphers` parameter is a tuple and let
+`ciphers` accessors return tuples.
+* update wheels to mbedtls 2.16.5
+
+[1.0.0] - 2020-01-05
+
+* ci: Add support to Python 3.8.
+* md: Support MD2 and MD4 algo.
+* ci: Update dependencies.
+
+[0.18.3]
+
+* setup.py: Refuse to build if mbedtls is too old.
+
+[0.18.2]
+
+* cipher: Increase test coverage and fix minor bugs.
+* tests: Do not assume that havege is missing as it could be included
+in some configurations.
+* tests: Make error reporting with memoryviews closer to pytest
+reporting for bytes.
+
+[0.18.1]
+
+* update wheels with 2.16.3.
+* version: Make `has_feature()` public.
+* tests: Skip tests to features that are not compiled in.
+* tests: Improve error reporting with memoryviews.
+
+[0.18.0] - 2019-05-11
+
+* secrets: Add PEP-506 conform secrets module for generating secrets.
+* cipher/hash/hmac: These modules and packages are now pure-Python.
+* mpi: Add bitwise operations.
+
+API Changes
+
+* pk.ECDHNaive: `generate()` returns the public key as an ECPoint and
+`import_peers_public()` now takes an ECPoint.  `import_peer_public(MPI)`
+is deprecated and will be removed in a future release.  Further note
+the `s` in `import_peers_public()`.
+* pk: Make `ECDH*.{public_key,private_key,peers_public_key}` public.  The
+private equivalents with a `_*` prefix are deprecated and will be removed in a
+future release.  Further note the `s` in `peers_public_key`.
+* _random: Privatize `Entropy` and refactor `Random` class.
+
+Bugfixes
+
+* mpi: Fix bug in `mpi.to_bytes()`.
+
+Misc.
+
+* *: Format Python files with `black`
+* ci: Check that the docs build in CI.
+* ci: Repair test coverage measurements on coveralls.
+* mpi: Simplify code for comparisons.
+* mpi: Add tests and better exceptions for `__pow__()`.
+
+
+[0.17.1] - 2019-04-16
+
+This is a bugfix release fixing several TLS issues.
+
+Misc.
+
+* Split download and install scripts.
+
+Bugfixes
+
+* tls: Split input and output buffers for TLS/TCP.
+* tls: Fixes issue with TLSv1 by reading greedily from the buffer.
+
+
+[0.17.0] - 2019-04-12
+
+* Add support to HKDF (HMAC key derivation function).
+
+Misc.
+
+* Change branching model to fast-forward merge on the master branch.
+* Change directive `language_level` from 2 to 3 for Cython.
+
+Bugfixes
+
+* *: Fixup handling of empty and `None` buffers (#20: Roman (inpos)).
+* hmac: Hmac now accepts the empty key (b"").
+
+
+[0.16.0] - 2019-04-04
+
+Add Chacha20/Poly1305 support (Stephen.Y).
+
+* cipher: Add support for the ARIA family.
+* cipher: Add OFB, XFB, and CHACHA/POLY modes and support for
+AEAD ciphers (Stephen.Y).
+* Update wheels with mbedtls 2.16.1.
+
+[0.15.0] - 2019-03-15
+
+Add DTLS support.  Both client side and server side are implemented.
+Setting the cookie on the server side is *not* optional in `python-mbedtls`.
+
+* pk: Add support for curves 448 and 25519 (Stephen.Y).
+
+Misc.
+
+* Update wheels with mbedtls 2.14.1.
+* version: Add accessors to the version of mbed TLS in use.
+* tls: Allow configuration of libmbedtls debug level.
+
+[0.14.1] - 2019-01-10
+
+Update wheels with mbedtls 2.7.9.
+
+[0.14.0] - 2019-01-08
+
+* Build and test on `manylinux1` (PEP 513) to distribute linux
+wheels with Mbed TLS.  It is not necessary anymore to install
+mbed TLS separately.
+* x509/CRL: Add support for upstream Mbed TLS version 2.7.2 and above.
+Note that this did not require changes in the library but only
+in the tests.
+* The library now internally uses a single global `Random` instance.
+This instance is not accessible from Python.
+* pk/DHServer, pk/DHClient: Increase test entropy to avoid
+flakey tests.
+
+API Changes
+
+* random: `Random()` now takes an optional `entropy` object
+as argument.
+* random: `Random.reseed()` now takes optional data that can be used
+to increase entropy.
+
+Bugfixes
+
+* mpi: Let MPI built from an empty byte (b"") be 0 as regular ints.
+
+[0.13.0] - 2018-10-25
+
+Add TLS support.  Both client side and server side are implemented.
+SSLv3 is not supported.  Session management and SNI callbacks are
+not implemented.
+
+API Changes
+
+* x509: `ca` and `max_path_length` basic constraints are now
+grouped into a `BasicConstraints` namedtuple.  It is possible
+to leave the basic constraints unset by passing None
+to `CRT.new(..., basic_constraints=None)`.
+* random: `random` module renamed `_random`.
+
+Bugfixes
+
+* mpi: GC now actually overwrites keys with random data.
+
+Misc.
+
+* pk: Improved error handling.
+* Declare mbedtls functions nogil.
+* The install script uses cmake to install mbedtls.
+
+[0.12.2] - 2018-09-10
+
+Misc.
+
+* New `property` syntax from Cython 0.24.
+* Fixup rendering on Pypi.
+* Update required deps.
+
+[0.12.1] - 2018-08-27
+
+Update version in `setup.py`.  No change in the code.
+
+[0.12.0] - 2018-08-27
+
+* x509: Add accessors to most fields of CRT, CSR, and CRL.
+The `x509` module can now be used to inspect existing certificates.
+* x509: The module now offers basic signing and
+verification capabilities.
+
+API Changes
+
+* pk: `from_{PEM,DER,buffer}` are now `classmethod`s to
+comply with PEP 543.
+* x509: `Certificate` class renamed `CRT`.
+* x509: `start` and `end` arguments renamed `not_before` and
+`not_after`; `md_alg` argument is now `digestmod`.
+* x509: Re-order the arguments of the `new()` methods.
+* exceptions: Rename `MbedTLSError` -> `TLSError` to comply
+with PEP 543.
+
+Misc
+
+* pk: `__eq__()` now also accepts DER (bytes) or PEM (str) formats.
+* x509: `__bytes__()` returns the certificates in the DER format.
+* x509: `__str__()` now returns a human-readable string.
+
+
+[0.11.1] - 2018-07-04
+
+Update changelog.  No changes in the code.
+
+
+[0.11.0] - 2018-07-01
+
+* Support Diffie-Hellman-Merkle key exchange.
+* MPIs (multi-precision integers) now implement the full
+`numbers.Integral` API.
+* MPIs are erased from memory upon garbage collection.
+* The `mpi` library is now public (renamed `_mpi` -> `mpi`).
+
+API Changes
+
+* pk: Methods that were previously returning a long integer now
+return an MPI.
+* exceptions: Rename `_ErrorBase` -> `MbedTLSError`.  It is now
+the only new exception.
+* exceptions: `mbedtls_strerror()` generates the error message.
+
+
+[0.10.0] - 2018-05-07
+
+Support elliptic curve cryptography
+
+* pk/ECC: Elliptic curve digital signature algorithm.
+* pk/ECDHServer, pk/ECDHClient: Elliptic curve Diffie-Hellman.
+The two classes together support ECDHE (ephemeral) as well.
+
+API Changes
+
+* pk/RSA: generate() returns the private key.
+* pk/RSA: to_DER() and to_PEM() are obsolete and will be removed.
+Users should call export_key() and export_public_key() instead.
+* pk/RSA: has_public() and has_private() are now private.
+Test if export_key() and export_public_key() are truthy
+or falsy instead.
+* pk/RSA: __str__() now returns the private key in PEM format.
+* pk/RSA: to_bytes() and __bytes__() now return the private key
+in DER format.
+
+Bugfix
+
+* pk: Increase the size of the buffer for sign, encrypt, decrypt
+
+Misc.
+
+* Use const memoryviews supported by Cython 0.28.0.
+* pk: pk is now a module instead of a package.
+
+[0.9.0] - 2018-03-14
+
+Misc.
+
+* Switch to semantic versioning.
+* Add pxd files to source distribution.
+
+
+[0.9] - 2018-03-13
+
+API Changes
+
+* x509/Certificate: next() returns the next certificate in a chain.
+* md: Implement block_size property.
+
+Misc.
+
+* Clean up imports.
+* Fix tests and packaging.
+* Change git merge policy to fast-forward on develop.
+
+
+[0.8 withdrawn] - 2018-02-24
+
+Support X.509 Certificates
+
+* x509/Certificate: X.509 certificate writer and parser.
+* x509/CSR: X.509 certificate signing request writer and parser.
+* x509/CRL: X.509 certificate revocation list and validation.
+
+API Changes
+
+* CipherBase/RSA: import_() method renamed from_buffer() for PEP 543.
+* CipherBase/RSA: export(format="PEM") method renamed to_PEM()
+* CipherBase/RSA: export(format="DER") method renamed to_DER()
+* CipherBase/RSA: from_DER(), from_PEM() to import from DER or PEM.
+* CipherBase/RSA: to_bytes() alias to_DER()
+
+
+[0.7] - 2018-02-04
+
+* Add support for Python 2.7, 3.5, and 3.6.
+* Tests ported from nosetest to pytest.
+* Setup continuous integration.
```

### Comparing `python-mbedtls-2.7.0/LICENSE.txt` & `python-mbedtls-2.7.1/LICENSE.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) 2015 Elaborated Networks GmbH
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
+The MIT License (MIT)
+
+Copyright (c) 2015 Elaborated Networks GmbH
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

### Comparing `python-mbedtls-2.7.0/PKG-INFO` & `python-mbedtls-2.7.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,444 +1,444 @@
-Metadata-Version: 2.1
-Name: python-mbedtls
-Version: 2.7.0
-Summary: hash, hmac, RSA, ECC, X.509, TLS, DTLS, handshakes, and secrets with an mbed TLS back end
-Home-page: https://github.com/Synss/python-mbedtls
-Download-URL: https://github.com/Synss/python-mbedtls/tarball/2.7.0
-Author: Mathias Laurin
-Author-email: Mathias.Laurin@github.com
-License: MIT License
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Security :: Cryptography
-Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-
-.. vim:tw=72
-
-=======================================================
-Cryptographic library for Python with Mbed TLS back end
-=======================================================
-
-.. image:: https://results.pre-commit.ci/badge/github/Synss/python-mbedtls/master.svg
-   :target: https://results.pre-commit.ci/latest/github/Synss/python-mbedtls/master
-   :alt: pre-commit.ci status
-
-.. image::
-   https://github.com/Synss/python-mbedtls/actions/workflows/main.yml/badge.svg?branch=master
-   :target: https://github.com/Synss/python-mbedtls/actions/
-
-.. image::
-   https://coveralls.io/repos/github/Synss/python-mbedtls/badge.svg?branch=master
-   :target: https://coveralls.io/github/Synss/python-mbedtls?branch=master
-
-
-`python-mbedtls`_ is a free cryptographic library for Python that uses
-`mbed TLS`_ for back end.
-
-   mbed TLS (formerly known as PolarSSL) makes it trivially easy for
-   developers to include cryptographic and SSL/TLS capabilities in their
-   (embedded) products, facilitating this functionality with a minimal
-   coding footprint.
-
-*python-mbedtls* API follows the recommendations from:
-
-* `PEP 272`_ -- API for Block Encryption Algorithms v1.0
-* `PEP 452`_ -- API for Cryptographic Hash Functions v2.0
-* `PEP 506`_ -- Adding a Secret Module to the Standard Library
-* `PEP 543`_ -- A Unified TLS API for Python (`completed and modernized`_)
-
-and therefore plays well with the `cryptographic services`_ from the
-Python standard library and many other cryptography libraries as well.
-
-.. _python-mbedtls: https://synss.github.io/python-mbedtls
-.. _mbed TLS: https://tls.mbed.org
-.. _PEP 272: https://www.python.org/dev/peps/pep-0272/
-.. _PEP 452: https://www.python.org/dev/peps/pep-0452/
-.. _PEP 506: https://www.python.org/dev/peps/pep-0506/
-.. _PEP 543: https://www.python.org/dev/peps/pep-0543/
-.. _cryptographic services: https://docs.python.org/3/library/crypto.html
-.. _PyCrypto: https://www.dlitz.net/software/pycrypto/
-.. _hashlib: https://docs.python.org/3.6/library/hashlib.html
-.. _hmac: https://docs.python.org/3.6/library/hmac.html
-.. _completed and modernized: https://github.com/Synss/python-mbedtls/blob/master/src/mbedtls/_tlsi.py
-
-
-License
-=======
-
-*python-mbedtls* is licensed under the MIT License (see LICENSE.txt).
-This enables the use of *python-mbedtls* in both open source and closed
-source projects.  The MIT License is compatible with both GPL and Apache
-2.0 license under which mbed TLS is distributed.
-
-
-API documentation
-=================
-
-https://synss.github.io/python-mbedtls/
-
-
-Installation
-============
-
-The bindings are tested with mbedTLS 2.28.3 for Python 3.7,
-3.8, 3.9, 3.10, and 3.11 on Linux, macOS, and Windows.
-
-`manylinux`_ wheels are available for 64-bit Linux systems.  Install
-with ``pip install python-mbedtls``.
-
-.. _manylinux: https://www.python.org/dev/peps/pep-0513/
-
-
-Usage and examples
-==================
-
-Now, let us see examples using the various parts of the library.
-
-
-Check which version of mbed TLS is being used by python-mbedtls
----------------------------------------------------------------
-
-The *mbedtls.version* module shows the run-time version
-information to mbed TLS.
-
->>> from mbedtls import version
->>> _ = version.version  # "mbed TLS 2.28.3"
->>> _ = version.version_info  # (2, 28, 3)
-
-
-Message digest
---------------
-
-The *mbedtls.hashlib* module supports MD2, MD4, MD5, SHA-1, SHA-2
-(in 224, 256, 384, and 512-bits), and RIPEMD-160 secure hashes
-and message digests.  Note that MD2 and MD4 are not included
-by default and are only present if they are compiled in mbedtls.
-
-Here are the examples from (standard) *hashlib* ported
-to *python-mbedtls*:
-
->>> from mbedtls import hashlib
->>> m = hashlib.md5()
->>> m.update(b"Nobody inspects")
->>> m.update(b" the spammish repetition")
->>> m.digest()
-b'\xbbd\x9c\x83\xdd\x1e\xa5\xc9\xd9\xde\xc9\xa1\x8d\xf0\xff\xe9'
->>> m.digest_size
-16
->>> m.block_size
-64
-
-More condensed:
-
->>> hashlib.sha224(b"Nobody inspects the spammish repetition").hexdigest()
-'a4337bc45a8fc544c03f52dc550cd6e1e87021bc896588bd79e901e2'
-
-Using ``new()``:
-
->>> h = hashlib.new('ripemd160')
->>> h.update(b"Nobody inspects the spammish repetition")
->>> h.hexdigest()
-'cc4a5ce1b3df48aec5d22d1f16b894a0b894eccc'
-
-
-HMAC algorithm
---------------
-
-The *mbedtls.hmac* module computes HMAC.
-
-Example:
-
->>> from mbedtls import hmac
->>> m = hmac.new(b"This is my secret key", digestmod="md5")
->>> m.update(b"Nobody inspects")
->>> m.update(b" the spammish repetition")
->>> m.digest()
-b'\x9d-/rj\\\x98\x80\xb1rG\x87\x0f\xe9\xe4\xeb'
-
-Warning:
-
-The message is cleared after calculation of the digest.  Only call
-``mbedtls.hmac.Hmac.digest()`` or ``mbedtls.hmac.Hmac.hexdigest()``
-once per message.
-
-
-HMAC-based key derivation function (HKDF)
------------------------------------------
-
-The *mbedtls.hkdf* module exposes extract-and-expand key derivation
-functions.  The main function is ``hkdf()`` but ``extract()`` and
-``expand()`` may be used as well.
-
-Example:
-
->>> from mbedtls import hkdf
->>> hkdf.hkdf(
-...     b"my secret key",
-...     length=42,
-...     info=b"my cool app",
-...     salt=b"and pepper",
-...     digestmod=hmac.sha256
-... )
-b'v,\xef\x90\xccU\x1d\x1b\xd7\\a\xaf\x92\xac\n\x90\xf9q\xf4)\xcd"\xf7\x1a\x94p\x03.\xa8e\x1e\xfb\x92\xe8l\x0cc\xf8e\rvj'
-
-where *info*, *salt*, and *digestmod* are optional, although providing
-(at least) *info* is highly recommended.
-
-
-Symmetric cipher
-----------------
-
-The *mbedtls.cipher* module provides symmetric encryption.  The API
-follows the recommendations from PEP 272 so that it can be used as a
-drop-in replacement to other libraries.
-
-*python-mbedtls* provides the following algorithms:
-
-- AES encryption/decryption (128, 192, and 256 bits) in ECB, CBC, CFB128,
-  CTR, OFB, or XTS mode;
-- AES AEAD (128, 192, and 256 bits) in GCM or CCM mode;
-- ARC4 encryption/decryption;
-- ARIA encryption/decryption (128, 192, and 256 bits) in ECB, CBC,
-  CTR, or GCM modes;
-- Blowfish encryption/decryption in ECB, CBC, CFB64, or CTR mode;
-- Camellia encryption/decryption (128, 192, and 256 bits) in ECB, CBC,
-  CFB128, CTR, or GCM mode;
-- DES, DES3, and double DES3 encryption/decryption in ECB or CBC mode;
-- CHACHA20 and CHACHA20/POLY1305 encryption/decryption.
-
-Example:
-
->>> from mbedtls import cipher
->>> c = cipher.AES.new(b"My 16-bytes key.", cipher.MODE_CBC, b"CBC needs an IV.")
->>> enc = c.encrypt(b"This is a super-secret message!!")
->>> enc
-b"*`k6\x98\x97=[\xdf\x7f\x88\x96\xf5\t\x19J\xf62h\xf4n\xca\xe8\xfe\xf5\xd7X'\xb1\x8c\xc9\x85"
->>> c.decrypt(enc)
-b'This is a super-secret message!!'
-
-
-RSA public key
---------------
-
-The *mbedtls.pk* module provides the RSA cryptosystem.  This includes:
-
-- Public-private key generation and key import/export in PEM and DER
-  formats;
-- asymmetric encryption and decryption;
-- message signature and verification.
-
-Key generation, the default size is 2048 bits:
-
->>> from mbedtls import pk
->>> rsa = pk.RSA()
->>> prv = rsa.generate()
->>> rsa.key_size
-256
-
-Message encryption and decryption:
-
->>> enc = rsa.encrypt(b"secret message")
->>> rsa.decrypt(enc)
-b'secret message'
-
-Message signature and verification:
-
->>> sig = rsa.sign(b"Please sign here.")
->>> rsa.verify(b"Please sign here.", sig)
-True
->>> rsa.verify(b"Sorry, wrong message.", sig)
-False
->>> pub = rsa.export_public_key(format="DER")
->>> other = pk.RSA.from_buffer(pub)
->>> other.verify(b"Please sign here.", sig)
-True
-
-
-Static and ephemeral elliptic curve Diffie-Hellman
---------------------------------------------------
-
-The *mbedtls.pk* module provides the ECC cryptosystem.  This includes:
-
-- Public-private key generation and key import/export in the PEM and DER
-  formats;
-- asymmetric encrypt and decryption;
-- message signature and verification;
-- ephemeral ECDH key exchange.
-
-``get_supported_curves()`` returns the list of supported curves.
-
-The API of the ECC class is the same as the API of the RSA class
-but ciphering (``encrypt()`` and ``decrypt()`` is not supported by
-Mbed TLS).
-
-Message signature and verification using elliptic a curve digital
-signature algorithm (ECDSA):
-
->>> from mbedtls import pk
->>> ecdsa = pk.ECC()
->>> prv = ecdsa.generate()
->>> sig = ecdsa.sign(b"Please sign here.")
->>> ecdsa.verify(b"Please sign here.", sig)
-True
->>> ecdsa.verify(b"Sorry, wrong message.", sig)
-False
->>> pub = ecdsa.export_public_key(format="DER")
->>> other = pk.ECC.from_buffer(pub)
->>> other.verify(b"Please sign here.", sig)
-True
-
-The classes ``ECDHServer`` and ``ECDHClient`` may be used for ephemeral
-ECDH.  The key exchange is as follows:
-
->>> ecdh_key = pk.ECC()
->>> ecdh_key.generate()
->>> ecdh_srv = pk.ECDHServer(ecdh_key)
->>> ecdh_cli = pk.ECDHClient(ecdh_key)
-
-The server generates the ServerKeyExchange encrypted payload and
-passes it to the client:
-
->>> ske = ecdh_srv.generate()
->>> ecdh_cli.import_SKE(ske)
-
-then the client generates the ClientKeyExchange encrypted payload and
-passes it back to the server:
-
->>> cke = ecdh_cli.generate()
->>> ecdh_srv.import_CKE(cke)
-
-Now, client and server may generate their shared secret:
-
->>> secret = ecdh_srv.generate_secret()
->>> ecdh_cli.generate_secret() == secret
-True
->>> ecdh_srv.shared_secret == ecdh_cli.shared_secret
-True
-
-
-Diffie-Hellman-Merkle key exchange
-----------------------------------
-
-The classes ``DHServer`` and ``DHClient`` may be used for DH Key
-exchange.  The classes have the same API as ``ECDHServer``
-and ``ECDHClient``, respectively.
-
-The key exchange is as follow:
-
->>> from mbedtls.mpi import MPI
->>> from mbedtls import pk
->>> dh_srv = pk.DHServer(MPI.prime(128), MPI.prime(96))
->>> dh_cli = pk.DHClient(MPI.prime(128), MPI.prime(96))
-
-The 128-bytes prime and the 96-bytes prime are the modulus ``P``
-and the generator ``G``.
-
-The server generates the ServerKeyExchange payload:
-
->>> ske = dh_srv.generate()
->>> dh_cli.import_SKE(ske)
-
-The payload ends with ``G^X mod P`` where ``X`` is the secret value of
-the server.
-
->>> cke = dh_cli.generate()
->>> dh_srv.import_CKE(cke)
-
-``cke`` is ``G^Y mod P`` (with ``Y`` the secret value from the client)
-returned as its representation in bytes so that it can be readily
-transported over the network.
-
-As in ECDH, client and server may now generate their shared secret:
-
->>> secret = dh_srv.generate_secret()
->>> dh_cli.generate_secret() == secret
-True
->>> dh_srv.shared_secret == dh_cli.shared_secret
-True
-
-
-X.509 certificate writing and parsing
--------------------------------------
-
-The *mbedtls.x509* module can be used to parse X.509 certificates
-or create and verify a certificate chain.
-
-Here, the trusted root is a self-signed CA certificate
-``ca0_crt`` signed by ``ca0_key``.
-
->>> import datetime as dt
->>>
->>> from mbedtls import hashlib
->>> from mbedtls import pk
->>> from mbedtls import x509
->>>
->>> now = dt.datetime.utcnow()
->>> ca0_key = pk.RSA()
->>> _ = ca0_key.generate()
->>> ca0_csr = x509.CSR.new(ca0_key, "CN=Trusted CA", hashlib.sha256())
->>> ca0_crt = x509.CRT.selfsign(
-...     ca0_csr, ca0_key,
-...     not_before=now, not_after=now + dt.timedelta(days=90),
-...     serial_number=0x123456,
-...     basic_constraints=x509.BasicConstraints(True, 1))
-...
-
-An intermediate then issues a Certificate Singing Request (CSR) that the
-root CA signs:
-
->>> ca1_key = pk.ECC()
->>> _ = ca1_key.generate()
->>> ca1_csr = x509.CSR.new(ca1_key, "CN=Intermediate CA", hashlib.sha256())
->>>
->>> ca1_crt = ca0_crt.sign(
-...     ca1_csr, ca0_key, now, now + dt.timedelta(days=90), 0x123456,
-...     basic_constraints=x509.BasicConstraints(ca=True, max_path_length=3))
-...
-
-And finally, the intermediate CA signs a certificate for the
-End Entity on the basis of a new CSR:
-
->>> ee0_key = pk.ECC()
->>> _ = ee0_key.generate()
->>> ee0_csr = x509.CSR.new(ee0_key, "CN=End Entity", hashlib.sha256())
->>>
->>> ee0_crt = ca1_crt.sign(
-...     ee0_csr, ca1_key, now, now + dt.timedelta(days=90), 0x987654)
-...
-
-The emitting certificate can be used to verify the next certificate in
-the chain:
-
->>> ca1_crt.verify(ee0_crt)
-True
->>> ca0_crt.verify(ca1_crt)
-True
-
-Note, however, that this verification is only one step in a private key
-infrastructure and does not take CRLs, path length, etc. into account.
-
-
-TLS and DTLS client and server
-------------------------------
-
-The *mbedtls.tls* module provides TLS clients and servers.  The API
-follows the recommendations of `PEP 543`_.  Note, however, that the
-Python standard SSL library does not follow the PEP so that this
-library may not be a drop-in replacement.
-
-.. _PEP 543: https://www.python.org/dev/peps/pep-0543/
-
-Connectionless DTLS is supported as well.
-
-See examples in the `programs/`_ directory of the repository
-and `tests/test_tls.py`_.
-
-.. _programs/: https://github.com/Synss/python-mbedtls/tree/master/programs
-.. _tests/test_tls.py: https://github.com/Synss/python-mbedtls/blob/master/tests/test_tls.py
+Metadata-Version: 2.1
+Name: python-mbedtls
+Version: 2.7.1
+Summary: hash, hmac, RSA, ECC, X.509, TLS, DTLS, handshakes, and secrets with an mbed TLS back end
+Home-page: https://github.com/Synss/python-mbedtls
+Download-URL: https://github.com/Synss/python-mbedtls/tarball/2.7.1
+Author: Mathias Laurin
+Author-email: Mathias.Laurin@github.com
+License: MIT License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Cython
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Security :: Cryptography
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+.. vim:tw=72
+
+=======================================================
+Cryptographic library for Python with Mbed TLS back end
+=======================================================
+
+.. image:: https://results.pre-commit.ci/badge/github/Synss/python-mbedtls/master.svg
+   :target: https://results.pre-commit.ci/latest/github/Synss/python-mbedtls/master
+   :alt: pre-commit.ci status
+
+.. image::
+   https://github.com/Synss/python-mbedtls/actions/workflows/main.yml/badge.svg?branch=master
+   :target: https://github.com/Synss/python-mbedtls/actions/
+
+.. image::
+   https://coveralls.io/repos/github/Synss/python-mbedtls/badge.svg?branch=master
+   :target: https://coveralls.io/github/Synss/python-mbedtls?branch=master
+
+
+`python-mbedtls`_ is a free cryptographic library for Python that uses
+`mbed TLS`_ for back end.
+
+   mbed TLS (formerly known as PolarSSL) makes it trivially easy for
+   developers to include cryptographic and SSL/TLS capabilities in their
+   (embedded) products, facilitating this functionality with a minimal
+   coding footprint.
+
+*python-mbedtls* API follows the recommendations from:
+
+* `PEP 272`_ -- API for Block Encryption Algorithms v1.0
+* `PEP 452`_ -- API for Cryptographic Hash Functions v2.0
+* `PEP 506`_ -- Adding a Secret Module to the Standard Library
+* `PEP 543`_ -- A Unified TLS API for Python (`completed and modernized`_)
+
+and therefore plays well with the `cryptographic services`_ from the
+Python standard library and many other cryptography libraries as well.
+
+.. _python-mbedtls: https://synss.github.io/python-mbedtls
+.. _mbed TLS: https://tls.mbed.org
+.. _PEP 272: https://www.python.org/dev/peps/pep-0272/
+.. _PEP 452: https://www.python.org/dev/peps/pep-0452/
+.. _PEP 506: https://www.python.org/dev/peps/pep-0506/
+.. _PEP 543: https://www.python.org/dev/peps/pep-0543/
+.. _cryptographic services: https://docs.python.org/3/library/crypto.html
+.. _PyCrypto: https://www.dlitz.net/software/pycrypto/
+.. _hashlib: https://docs.python.org/3.6/library/hashlib.html
+.. _hmac: https://docs.python.org/3.6/library/hmac.html
+.. _completed and modernized: https://github.com/Synss/python-mbedtls/blob/master/src/mbedtls/_tlsi.py
+
+
+License
+=======
+
+*python-mbedtls* is licensed under the MIT License (see LICENSE.txt).
+This enables the use of *python-mbedtls* in both open source and closed
+source projects.  The MIT License is compatible with both GPL and Apache
+2.0 license under which mbed TLS is distributed.
+
+
+API documentation
+=================
+
+https://synss.github.io/python-mbedtls/
+
+
+Installation
+============
+
+The bindings are tested with mbedTLS 2.28.3 for Python 3.8,
+3.9, 3.10, and 3.11 on Linux, macOS, and Windows.
+
+`manylinux`_ wheels are available for 64-bit Linux systems.  Install
+with ``pip install python-mbedtls``.
+
+.. _manylinux: https://www.python.org/dev/peps/pep-0513/
+
+
+Usage and examples
+==================
+
+Now, let us see examples using the various parts of the library.
+
+
+Check which version of mbed TLS is being used by python-mbedtls
+---------------------------------------------------------------
+
+The *mbedtls.version* module shows the run-time version
+information to mbed TLS.
+
+>>> from mbedtls import version
+>>> _ = version.version  # "mbed TLS 2.28.3"
+>>> _ = version.version_info  # (2, 28, 3)
+
+
+Message digest
+--------------
+
+The *mbedtls.hashlib* module supports MD2, MD4, MD5, SHA-1, SHA-2
+(in 224, 256, 384, and 512-bits), and RIPEMD-160 secure hashes
+and message digests.  Note that MD2 and MD4 are not included
+by default and are only present if they are compiled in mbedtls.
+
+Here are the examples from (standard) *hashlib* ported
+to *python-mbedtls*:
+
+>>> from mbedtls import hashlib
+>>> m = hashlib.md5()
+>>> m.update(b"Nobody inspects")
+>>> m.update(b" the spammish repetition")
+>>> m.digest()
+b'\xbbd\x9c\x83\xdd\x1e\xa5\xc9\xd9\xde\xc9\xa1\x8d\xf0\xff\xe9'
+>>> m.digest_size
+16
+>>> m.block_size
+64
+
+More condensed:
+
+>>> hashlib.sha224(b"Nobody inspects the spammish repetition").hexdigest()
+'a4337bc45a8fc544c03f52dc550cd6e1e87021bc896588bd79e901e2'
+
+Using ``new()``:
+
+>>> h = hashlib.new('ripemd160')
+>>> h.update(b"Nobody inspects the spammish repetition")
+>>> h.hexdigest()
+'cc4a5ce1b3df48aec5d22d1f16b894a0b894eccc'
+
+
+HMAC algorithm
+--------------
+
+The *mbedtls.hmac* module computes HMAC.
+
+Example:
+
+>>> from mbedtls import hmac
+>>> m = hmac.new(b"This is my secret key", digestmod="md5")
+>>> m.update(b"Nobody inspects")
+>>> m.update(b" the spammish repetition")
+>>> m.digest()
+b'\x9d-/rj\\\x98\x80\xb1rG\x87\x0f\xe9\xe4\xeb'
+
+Warning:
+
+The message is cleared after calculation of the digest.  Only call
+``mbedtls.hmac.Hmac.digest()`` or ``mbedtls.hmac.Hmac.hexdigest()``
+once per message.
+
+
+HMAC-based key derivation function (HKDF)
+-----------------------------------------
+
+The *mbedtls.hkdf* module exposes extract-and-expand key derivation
+functions.  The main function is ``hkdf()`` but ``extract()`` and
+``expand()`` may be used as well.
+
+Example:
+
+>>> from mbedtls import hkdf
+>>> hkdf.hkdf(
+...     b"my secret key",
+...     length=42,
+...     info=b"my cool app",
+...     salt=b"and pepper",
+...     digestmod=hmac.sha256
+... )
+b'v,\xef\x90\xccU\x1d\x1b\xd7\\a\xaf\x92\xac\n\x90\xf9q\xf4)\xcd"\xf7\x1a\x94p\x03.\xa8e\x1e\xfb\x92\xe8l\x0cc\xf8e\rvj'
+
+where *info*, *salt*, and *digestmod* are optional, although providing
+(at least) *info* is highly recommended.
+
+
+Symmetric cipher
+----------------
+
+The *mbedtls.cipher* module provides symmetric encryption.  The API
+follows the recommendations from PEP 272 so that it can be used as a
+drop-in replacement to other libraries.
+
+*python-mbedtls* provides the following algorithms:
+
+- AES encryption/decryption (128, 192, and 256 bits) in ECB, CBC, CFB128,
+  CTR, OFB, or XTS mode;
+- AES AEAD (128, 192, and 256 bits) in GCM or CCM mode;
+- ARC4 encryption/decryption;
+- ARIA encryption/decryption (128, 192, and 256 bits) in ECB, CBC,
+  CTR, or GCM modes;
+- Blowfish encryption/decryption in ECB, CBC, CFB64, or CTR mode;
+- Camellia encryption/decryption (128, 192, and 256 bits) in ECB, CBC,
+  CFB128, CTR, or GCM mode;
+- DES, DES3, and double DES3 encryption/decryption in ECB or CBC mode;
+- CHACHA20 and CHACHA20/POLY1305 encryption/decryption.
+
+Example:
+
+>>> from mbedtls import cipher
+>>> c = cipher.AES.new(b"My 16-bytes key.", cipher.MODE_CBC, b"CBC needs an IV.")
+>>> enc = c.encrypt(b"This is a super-secret message!!")
+>>> enc
+b"*`k6\x98\x97=[\xdf\x7f\x88\x96\xf5\t\x19J\xf62h\xf4n\xca\xe8\xfe\xf5\xd7X'\xb1\x8c\xc9\x85"
+>>> c.decrypt(enc)
+b'This is a super-secret message!!'
+
+
+RSA public key
+--------------
+
+The *mbedtls.pk* module provides the RSA cryptosystem.  This includes:
+
+- Public-private key generation and key import/export in PEM and DER
+  formats;
+- asymmetric encryption and decryption;
+- message signature and verification.
+
+Key generation, the default size is 2048 bits:
+
+>>> from mbedtls import pk
+>>> rsa = pk.RSA()
+>>> prv = rsa.generate()
+>>> rsa.key_size
+256
+
+Message encryption and decryption:
+
+>>> enc = rsa.encrypt(b"secret message")
+>>> rsa.decrypt(enc)
+b'secret message'
+
+Message signature and verification:
+
+>>> sig = rsa.sign(b"Please sign here.")
+>>> rsa.verify(b"Please sign here.", sig)
+True
+>>> rsa.verify(b"Sorry, wrong message.", sig)
+False
+>>> pub = rsa.export_public_key(format="DER")
+>>> other = pk.RSA.from_buffer(pub)
+>>> other.verify(b"Please sign here.", sig)
+True
+
+
+Static and ephemeral elliptic curve Diffie-Hellman
+--------------------------------------------------
+
+The *mbedtls.pk* module provides the ECC cryptosystem.  This includes:
+
+- Public-private key generation and key import/export in the PEM and DER
+  formats;
+- asymmetric encrypt and decryption;
+- message signature and verification;
+- ephemeral ECDH key exchange.
+
+``get_supported_curves()`` returns the list of supported curves.
+
+The API of the ECC class is the same as the API of the RSA class
+but ciphering (``encrypt()`` and ``decrypt()`` is not supported by
+Mbed TLS).
+
+Message signature and verification using elliptic a curve digital
+signature algorithm (ECDSA):
+
+>>> from mbedtls import pk
+>>> ecdsa = pk.ECC()
+>>> prv = ecdsa.generate()
+>>> sig = ecdsa.sign(b"Please sign here.")
+>>> ecdsa.verify(b"Please sign here.", sig)
+True
+>>> ecdsa.verify(b"Sorry, wrong message.", sig)
+False
+>>> pub = ecdsa.export_public_key(format="DER")
+>>> other = pk.ECC.from_buffer(pub)
+>>> other.verify(b"Please sign here.", sig)
+True
+
+The classes ``ECDHServer`` and ``ECDHClient`` may be used for ephemeral
+ECDH.  The key exchange is as follows:
+
+>>> ecdh_key = pk.ECC()
+>>> ecdh_key.generate()
+>>> ecdh_srv = pk.ECDHServer(ecdh_key)
+>>> ecdh_cli = pk.ECDHClient(ecdh_key)
+
+The server generates the ServerKeyExchange encrypted payload and
+passes it to the client:
+
+>>> ske = ecdh_srv.generate()
+>>> ecdh_cli.import_SKE(ske)
+
+then the client generates the ClientKeyExchange encrypted payload and
+passes it back to the server:
+
+>>> cke = ecdh_cli.generate()
+>>> ecdh_srv.import_CKE(cke)
+
+Now, client and server may generate their shared secret:
+
+>>> secret = ecdh_srv.generate_secret()
+>>> ecdh_cli.generate_secret() == secret
+True
+>>> ecdh_srv.shared_secret == ecdh_cli.shared_secret
+True
+
+
+Diffie-Hellman-Merkle key exchange
+----------------------------------
+
+The classes ``DHServer`` and ``DHClient`` may be used for DH Key
+exchange.  The classes have the same API as ``ECDHServer``
+and ``ECDHClient``, respectively.
+
+The key exchange is as follow:
+
+>>> from mbedtls.mpi import MPI
+>>> from mbedtls import pk
+>>> dh_srv = pk.DHServer(MPI.prime(128), MPI.prime(96))
+>>> dh_cli = pk.DHClient(MPI.prime(128), MPI.prime(96))
+
+The 128-bytes prime and the 96-bytes prime are the modulus ``P``
+and the generator ``G``.
+
+The server generates the ServerKeyExchange payload:
+
+>>> ske = dh_srv.generate()
+>>> dh_cli.import_SKE(ske)
+
+The payload ends with ``G^X mod P`` where ``X`` is the secret value of
+the server.
+
+>>> cke = dh_cli.generate()
+>>> dh_srv.import_CKE(cke)
+
+``cke`` is ``G^Y mod P`` (with ``Y`` the secret value from the client)
+returned as its representation in bytes so that it can be readily
+transported over the network.
+
+As in ECDH, client and server may now generate their shared secret:
+
+>>> secret = dh_srv.generate_secret()
+>>> dh_cli.generate_secret() == secret
+True
+>>> dh_srv.shared_secret == dh_cli.shared_secret
+True
+
+
+X.509 certificate writing and parsing
+-------------------------------------
+
+The *mbedtls.x509* module can be used to parse X.509 certificates
+or create and verify a certificate chain.
+
+Here, the trusted root is a self-signed CA certificate
+``ca0_crt`` signed by ``ca0_key``.
+
+>>> import datetime as dt
+>>>
+>>> from mbedtls import hashlib
+>>> from mbedtls import pk
+>>> from mbedtls import x509
+>>>
+>>> now = dt.datetime.utcnow()
+>>> ca0_key = pk.RSA()
+>>> _ = ca0_key.generate()
+>>> ca0_csr = x509.CSR.new(ca0_key, "CN=Trusted CA", hashlib.sha256())
+>>> ca0_crt = x509.CRT.selfsign(
+...     ca0_csr, ca0_key,
+...     not_before=now, not_after=now + dt.timedelta(days=90),
+...     serial_number=0x123456,
+...     basic_constraints=x509.BasicConstraints(True, 1))
+...
+
+An intermediate then issues a Certificate Singing Request (CSR) that the
+root CA signs:
+
+>>> ca1_key = pk.ECC()
+>>> _ = ca1_key.generate()
+>>> ca1_csr = x509.CSR.new(ca1_key, "CN=Intermediate CA", hashlib.sha256())
+>>>
+>>> ca1_crt = ca0_crt.sign(
+...     ca1_csr, ca0_key, now, now + dt.timedelta(days=90), 0x123456,
+...     basic_constraints=x509.BasicConstraints(ca=True, max_path_length=3))
+...
+
+And finally, the intermediate CA signs a certificate for the
+End Entity on the basis of a new CSR:
+
+>>> ee0_key = pk.ECC()
+>>> _ = ee0_key.generate()
+>>> ee0_csr = x509.CSR.new(ee0_key, "CN=End Entity", hashlib.sha256())
+>>>
+>>> ee0_crt = ca1_crt.sign(
+...     ee0_csr, ca1_key, now, now + dt.timedelta(days=90), 0x987654)
+...
+
+The emitting certificate can be used to verify the next certificate in
+the chain:
+
+>>> ca1_crt.verify(ee0_crt)
+True
+>>> ca0_crt.verify(ca1_crt)
+True
+
+Note, however, that this verification is only one step in a private key
+infrastructure and does not take CRLs, path length, etc. into account.
+
+
+TLS and DTLS client and server
+------------------------------
+
+The *mbedtls.tls* module provides TLS clients and servers.  The API
+follows the recommendations of `PEP 543`_.  Note, however, that the
+Python standard SSL library does not follow the PEP so that this
+library may not be a drop-in replacement.
+
+.. _PEP 543: https://www.python.org/dev/peps/pep-0543/
+
+Connectionless DTLS is supported as well.
+
+See examples in the `programs/`_ directory of the repository
+and `tests/test_tls.py`_.
+
+.. _programs/: https://github.com/Synss/python-mbedtls/tree/master/programs
+.. _tests/test_tls.py: https://github.com/Synss/python-mbedtls/blob/master/tests/test_tls.py
```

### Comparing `python-mbedtls-2.7.0/README.rst` & `python-mbedtls-2.7.1/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,423 +1,423 @@
-.. vim:tw=72
-
-=======================================================
-Cryptographic library for Python with Mbed TLS back end
-=======================================================
-
-.. image:: https://results.pre-commit.ci/badge/github/Synss/python-mbedtls/master.svg
-   :target: https://results.pre-commit.ci/latest/github/Synss/python-mbedtls/master
-   :alt: pre-commit.ci status
-
-.. image::
-   https://github.com/Synss/python-mbedtls/actions/workflows/main.yml/badge.svg?branch=master
-   :target: https://github.com/Synss/python-mbedtls/actions/
-
-.. image::
-   https://coveralls.io/repos/github/Synss/python-mbedtls/badge.svg?branch=master
-   :target: https://coveralls.io/github/Synss/python-mbedtls?branch=master
-
-
-`python-mbedtls`_ is a free cryptographic library for Python that uses
-`mbed TLS`_ for back end.
-
-   mbed TLS (formerly known as PolarSSL) makes it trivially easy for
-   developers to include cryptographic and SSL/TLS capabilities in their
-   (embedded) products, facilitating this functionality with a minimal
-   coding footprint.
-
-*python-mbedtls* API follows the recommendations from:
-
-* `PEP 272`_ -- API for Block Encryption Algorithms v1.0
-* `PEP 452`_ -- API for Cryptographic Hash Functions v2.0
-* `PEP 506`_ -- Adding a Secret Module to the Standard Library
-* `PEP 543`_ -- A Unified TLS API for Python (`completed and modernized`_)
-
-and therefore plays well with the `cryptographic services`_ from the
-Python standard library and many other cryptography libraries as well.
-
-.. _python-mbedtls: https://synss.github.io/python-mbedtls
-.. _mbed TLS: https://tls.mbed.org
-.. _PEP 272: https://www.python.org/dev/peps/pep-0272/
-.. _PEP 452: https://www.python.org/dev/peps/pep-0452/
-.. _PEP 506: https://www.python.org/dev/peps/pep-0506/
-.. _PEP 543: https://www.python.org/dev/peps/pep-0543/
-.. _cryptographic services: https://docs.python.org/3/library/crypto.html
-.. _PyCrypto: https://www.dlitz.net/software/pycrypto/
-.. _hashlib: https://docs.python.org/3.6/library/hashlib.html
-.. _hmac: https://docs.python.org/3.6/library/hmac.html
-.. _completed and modernized: https://github.com/Synss/python-mbedtls/blob/master/src/mbedtls/_tlsi.py
-
-
-License
-=======
-
-*python-mbedtls* is licensed under the MIT License (see LICENSE.txt).
-This enables the use of *python-mbedtls* in both open source and closed
-source projects.  The MIT License is compatible with both GPL and Apache
-2.0 license under which mbed TLS is distributed.
-
-
-API documentation
-=================
-
-https://synss.github.io/python-mbedtls/
-
-
-Installation
-============
-
-The bindings are tested with mbedTLS 2.28.3 for Python 3.7,
-3.8, 3.9, 3.10, and 3.11 on Linux, macOS, and Windows.
-
-`manylinux`_ wheels are available for 64-bit Linux systems.  Install
-with ``pip install python-mbedtls``.
-
-.. _manylinux: https://www.python.org/dev/peps/pep-0513/
-
-
-Usage and examples
-==================
-
-Now, let us see examples using the various parts of the library.
-
-
-Check which version of mbed TLS is being used by python-mbedtls
----------------------------------------------------------------
-
-The *mbedtls.version* module shows the run-time version
-information to mbed TLS.
-
->>> from mbedtls import version
->>> _ = version.version  # "mbed TLS 2.28.3"
->>> _ = version.version_info  # (2, 28, 3)
-
-
-Message digest
---------------
-
-The *mbedtls.hashlib* module supports MD2, MD4, MD5, SHA-1, SHA-2
-(in 224, 256, 384, and 512-bits), and RIPEMD-160 secure hashes
-and message digests.  Note that MD2 and MD4 are not included
-by default and are only present if they are compiled in mbedtls.
-
-Here are the examples from (standard) *hashlib* ported
-to *python-mbedtls*:
-
->>> from mbedtls import hashlib
->>> m = hashlib.md5()
->>> m.update(b"Nobody inspects")
->>> m.update(b" the spammish repetition")
->>> m.digest()
-b'\xbbd\x9c\x83\xdd\x1e\xa5\xc9\xd9\xde\xc9\xa1\x8d\xf0\xff\xe9'
->>> m.digest_size
-16
->>> m.block_size
-64
-
-More condensed:
-
->>> hashlib.sha224(b"Nobody inspects the spammish repetition").hexdigest()
-'a4337bc45a8fc544c03f52dc550cd6e1e87021bc896588bd79e901e2'
-
-Using ``new()``:
-
->>> h = hashlib.new('ripemd160')
->>> h.update(b"Nobody inspects the spammish repetition")
->>> h.hexdigest()
-'cc4a5ce1b3df48aec5d22d1f16b894a0b894eccc'
-
-
-HMAC algorithm
---------------
-
-The *mbedtls.hmac* module computes HMAC.
-
-Example:
-
->>> from mbedtls import hmac
->>> m = hmac.new(b"This is my secret key", digestmod="md5")
->>> m.update(b"Nobody inspects")
->>> m.update(b" the spammish repetition")
->>> m.digest()
-b'\x9d-/rj\\\x98\x80\xb1rG\x87\x0f\xe9\xe4\xeb'
-
-Warning:
-
-The message is cleared after calculation of the digest.  Only call
-``mbedtls.hmac.Hmac.digest()`` or ``mbedtls.hmac.Hmac.hexdigest()``
-once per message.
-
-
-HMAC-based key derivation function (HKDF)
------------------------------------------
-
-The *mbedtls.hkdf* module exposes extract-and-expand key derivation
-functions.  The main function is ``hkdf()`` but ``extract()`` and
-``expand()`` may be used as well.
-
-Example:
-
->>> from mbedtls import hkdf
->>> hkdf.hkdf(
-...     b"my secret key",
-...     length=42,
-...     info=b"my cool app",
-...     salt=b"and pepper",
-...     digestmod=hmac.sha256
-... )
-b'v,\xef\x90\xccU\x1d\x1b\xd7\\a\xaf\x92\xac\n\x90\xf9q\xf4)\xcd"\xf7\x1a\x94p\x03.\xa8e\x1e\xfb\x92\xe8l\x0cc\xf8e\rvj'
-
-where *info*, *salt*, and *digestmod* are optional, although providing
-(at least) *info* is highly recommended.
-
-
-Symmetric cipher
-----------------
-
-The *mbedtls.cipher* module provides symmetric encryption.  The API
-follows the recommendations from PEP 272 so that it can be used as a
-drop-in replacement to other libraries.
-
-*python-mbedtls* provides the following algorithms:
-
-- AES encryption/decryption (128, 192, and 256 bits) in ECB, CBC, CFB128,
-  CTR, OFB, or XTS mode;
-- AES AEAD (128, 192, and 256 bits) in GCM or CCM mode;
-- ARC4 encryption/decryption;
-- ARIA encryption/decryption (128, 192, and 256 bits) in ECB, CBC,
-  CTR, or GCM modes;
-- Blowfish encryption/decryption in ECB, CBC, CFB64, or CTR mode;
-- Camellia encryption/decryption (128, 192, and 256 bits) in ECB, CBC,
-  CFB128, CTR, or GCM mode;
-- DES, DES3, and double DES3 encryption/decryption in ECB or CBC mode;
-- CHACHA20 and CHACHA20/POLY1305 encryption/decryption.
-
-Example:
-
->>> from mbedtls import cipher
->>> c = cipher.AES.new(b"My 16-bytes key.", cipher.MODE_CBC, b"CBC needs an IV.")
->>> enc = c.encrypt(b"This is a super-secret message!!")
->>> enc
-b"*`k6\x98\x97=[\xdf\x7f\x88\x96\xf5\t\x19J\xf62h\xf4n\xca\xe8\xfe\xf5\xd7X'\xb1\x8c\xc9\x85"
->>> c.decrypt(enc)
-b'This is a super-secret message!!'
-
-
-RSA public key
---------------
-
-The *mbedtls.pk* module provides the RSA cryptosystem.  This includes:
-
-- Public-private key generation and key import/export in PEM and DER
-  formats;
-- asymmetric encryption and decryption;
-- message signature and verification.
-
-Key generation, the default size is 2048 bits:
-
->>> from mbedtls import pk
->>> rsa = pk.RSA()
->>> prv = rsa.generate()
->>> rsa.key_size
-256
-
-Message encryption and decryption:
-
->>> enc = rsa.encrypt(b"secret message")
->>> rsa.decrypt(enc)
-b'secret message'
-
-Message signature and verification:
-
->>> sig = rsa.sign(b"Please sign here.")
->>> rsa.verify(b"Please sign here.", sig)
-True
->>> rsa.verify(b"Sorry, wrong message.", sig)
-False
->>> pub = rsa.export_public_key(format="DER")
->>> other = pk.RSA.from_buffer(pub)
->>> other.verify(b"Please sign here.", sig)
-True
-
-
-Static and ephemeral elliptic curve Diffie-Hellman
---------------------------------------------------
-
-The *mbedtls.pk* module provides the ECC cryptosystem.  This includes:
-
-- Public-private key generation and key import/export in the PEM and DER
-  formats;
-- asymmetric encrypt and decryption;
-- message signature and verification;
-- ephemeral ECDH key exchange.
-
-``get_supported_curves()`` returns the list of supported curves.
-
-The API of the ECC class is the same as the API of the RSA class
-but ciphering (``encrypt()`` and ``decrypt()`` is not supported by
-Mbed TLS).
-
-Message signature and verification using elliptic a curve digital
-signature algorithm (ECDSA):
-
->>> from mbedtls import pk
->>> ecdsa = pk.ECC()
->>> prv = ecdsa.generate()
->>> sig = ecdsa.sign(b"Please sign here.")
->>> ecdsa.verify(b"Please sign here.", sig)
-True
->>> ecdsa.verify(b"Sorry, wrong message.", sig)
-False
->>> pub = ecdsa.export_public_key(format="DER")
->>> other = pk.ECC.from_buffer(pub)
->>> other.verify(b"Please sign here.", sig)
-True
-
-The classes ``ECDHServer`` and ``ECDHClient`` may be used for ephemeral
-ECDH.  The key exchange is as follows:
-
->>> ecdh_key = pk.ECC()
->>> ecdh_key.generate()
->>> ecdh_srv = pk.ECDHServer(ecdh_key)
->>> ecdh_cli = pk.ECDHClient(ecdh_key)
-
-The server generates the ServerKeyExchange encrypted payload and
-passes it to the client:
-
->>> ske = ecdh_srv.generate()
->>> ecdh_cli.import_SKE(ske)
-
-then the client generates the ClientKeyExchange encrypted payload and
-passes it back to the server:
-
->>> cke = ecdh_cli.generate()
->>> ecdh_srv.import_CKE(cke)
-
-Now, client and server may generate their shared secret:
-
->>> secret = ecdh_srv.generate_secret()
->>> ecdh_cli.generate_secret() == secret
-True
->>> ecdh_srv.shared_secret == ecdh_cli.shared_secret
-True
-
-
-Diffie-Hellman-Merkle key exchange
-----------------------------------
-
-The classes ``DHServer`` and ``DHClient`` may be used for DH Key
-exchange.  The classes have the same API as ``ECDHServer``
-and ``ECDHClient``, respectively.
-
-The key exchange is as follow:
-
->>> from mbedtls.mpi import MPI
->>> from mbedtls import pk
->>> dh_srv = pk.DHServer(MPI.prime(128), MPI.prime(96))
->>> dh_cli = pk.DHClient(MPI.prime(128), MPI.prime(96))
-
-The 128-bytes prime and the 96-bytes prime are the modulus ``P``
-and the generator ``G``.
-
-The server generates the ServerKeyExchange payload:
-
->>> ske = dh_srv.generate()
->>> dh_cli.import_SKE(ske)
-
-The payload ends with ``G^X mod P`` where ``X`` is the secret value of
-the server.
-
->>> cke = dh_cli.generate()
->>> dh_srv.import_CKE(cke)
-
-``cke`` is ``G^Y mod P`` (with ``Y`` the secret value from the client)
-returned as its representation in bytes so that it can be readily
-transported over the network.
-
-As in ECDH, client and server may now generate their shared secret:
-
->>> secret = dh_srv.generate_secret()
->>> dh_cli.generate_secret() == secret
-True
->>> dh_srv.shared_secret == dh_cli.shared_secret
-True
-
-
-X.509 certificate writing and parsing
--------------------------------------
-
-The *mbedtls.x509* module can be used to parse X.509 certificates
-or create and verify a certificate chain.
-
-Here, the trusted root is a self-signed CA certificate
-``ca0_crt`` signed by ``ca0_key``.
-
->>> import datetime as dt
->>>
->>> from mbedtls import hashlib
->>> from mbedtls import pk
->>> from mbedtls import x509
->>>
->>> now = dt.datetime.utcnow()
->>> ca0_key = pk.RSA()
->>> _ = ca0_key.generate()
->>> ca0_csr = x509.CSR.new(ca0_key, "CN=Trusted CA", hashlib.sha256())
->>> ca0_crt = x509.CRT.selfsign(
-...     ca0_csr, ca0_key,
-...     not_before=now, not_after=now + dt.timedelta(days=90),
-...     serial_number=0x123456,
-...     basic_constraints=x509.BasicConstraints(True, 1))
-...
-
-An intermediate then issues a Certificate Singing Request (CSR) that the
-root CA signs:
-
->>> ca1_key = pk.ECC()
->>> _ = ca1_key.generate()
->>> ca1_csr = x509.CSR.new(ca1_key, "CN=Intermediate CA", hashlib.sha256())
->>>
->>> ca1_crt = ca0_crt.sign(
-...     ca1_csr, ca0_key, now, now + dt.timedelta(days=90), 0x123456,
-...     basic_constraints=x509.BasicConstraints(ca=True, max_path_length=3))
-...
-
-And finally, the intermediate CA signs a certificate for the
-End Entity on the basis of a new CSR:
-
->>> ee0_key = pk.ECC()
->>> _ = ee0_key.generate()
->>> ee0_csr = x509.CSR.new(ee0_key, "CN=End Entity", hashlib.sha256())
->>>
->>> ee0_crt = ca1_crt.sign(
-...     ee0_csr, ca1_key, now, now + dt.timedelta(days=90), 0x987654)
-...
-
-The emitting certificate can be used to verify the next certificate in
-the chain:
-
->>> ca1_crt.verify(ee0_crt)
-True
->>> ca0_crt.verify(ca1_crt)
-True
-
-Note, however, that this verification is only one step in a private key
-infrastructure and does not take CRLs, path length, etc. into account.
-
-
-TLS and DTLS client and server
-------------------------------
-
-The *mbedtls.tls* module provides TLS clients and servers.  The API
-follows the recommendations of `PEP 543`_.  Note, however, that the
-Python standard SSL library does not follow the PEP so that this
-library may not be a drop-in replacement.
-
-.. _PEP 543: https://www.python.org/dev/peps/pep-0543/
-
-Connectionless DTLS is supported as well.
-
-See examples in the `programs/`_ directory of the repository
-and `tests/test_tls.py`_.
-
-.. _programs/: https://github.com/Synss/python-mbedtls/tree/master/programs
-.. _tests/test_tls.py: https://github.com/Synss/python-mbedtls/blob/master/tests/test_tls.py
+.. vim:tw=72
+
+=======================================================
+Cryptographic library for Python with Mbed TLS back end
+=======================================================
+
+.. image:: https://results.pre-commit.ci/badge/github/Synss/python-mbedtls/master.svg
+   :target: https://results.pre-commit.ci/latest/github/Synss/python-mbedtls/master
+   :alt: pre-commit.ci status
+
+.. image::
+   https://github.com/Synss/python-mbedtls/actions/workflows/main.yml/badge.svg?branch=master
+   :target: https://github.com/Synss/python-mbedtls/actions/
+
+.. image::
+   https://coveralls.io/repos/github/Synss/python-mbedtls/badge.svg?branch=master
+   :target: https://coveralls.io/github/Synss/python-mbedtls?branch=master
+
+
+`python-mbedtls`_ is a free cryptographic library for Python that uses
+`mbed TLS`_ for back end.
+
+   mbed TLS (formerly known as PolarSSL) makes it trivially easy for
+   developers to include cryptographic and SSL/TLS capabilities in their
+   (embedded) products, facilitating this functionality with a minimal
+   coding footprint.
+
+*python-mbedtls* API follows the recommendations from:
+
+* `PEP 272`_ -- API for Block Encryption Algorithms v1.0
+* `PEP 452`_ -- API for Cryptographic Hash Functions v2.0
+* `PEP 506`_ -- Adding a Secret Module to the Standard Library
+* `PEP 543`_ -- A Unified TLS API for Python (`completed and modernized`_)
+
+and therefore plays well with the `cryptographic services`_ from the
+Python standard library and many other cryptography libraries as well.
+
+.. _python-mbedtls: https://synss.github.io/python-mbedtls
+.. _mbed TLS: https://tls.mbed.org
+.. _PEP 272: https://www.python.org/dev/peps/pep-0272/
+.. _PEP 452: https://www.python.org/dev/peps/pep-0452/
+.. _PEP 506: https://www.python.org/dev/peps/pep-0506/
+.. _PEP 543: https://www.python.org/dev/peps/pep-0543/
+.. _cryptographic services: https://docs.python.org/3/library/crypto.html
+.. _PyCrypto: https://www.dlitz.net/software/pycrypto/
+.. _hashlib: https://docs.python.org/3.6/library/hashlib.html
+.. _hmac: https://docs.python.org/3.6/library/hmac.html
+.. _completed and modernized: https://github.com/Synss/python-mbedtls/blob/master/src/mbedtls/_tlsi.py
+
+
+License
+=======
+
+*python-mbedtls* is licensed under the MIT License (see LICENSE.txt).
+This enables the use of *python-mbedtls* in both open source and closed
+source projects.  The MIT License is compatible with both GPL and Apache
+2.0 license under which mbed TLS is distributed.
+
+
+API documentation
+=================
+
+https://synss.github.io/python-mbedtls/
+
+
+Installation
+============
+
+The bindings are tested with mbedTLS 2.28.3 for Python 3.8,
+3.9, 3.10, and 3.11 on Linux, macOS, and Windows.
+
+`manylinux`_ wheels are available for 64-bit Linux systems.  Install
+with ``pip install python-mbedtls``.
+
+.. _manylinux: https://www.python.org/dev/peps/pep-0513/
+
+
+Usage and examples
+==================
+
+Now, let us see examples using the various parts of the library.
+
+
+Check which version of mbed TLS is being used by python-mbedtls
+---------------------------------------------------------------
+
+The *mbedtls.version* module shows the run-time version
+information to mbed TLS.
+
+>>> from mbedtls import version
+>>> _ = version.version  # "mbed TLS 2.28.3"
+>>> _ = version.version_info  # (2, 28, 3)
+
+
+Message digest
+--------------
+
+The *mbedtls.hashlib* module supports MD2, MD4, MD5, SHA-1, SHA-2
+(in 224, 256, 384, and 512-bits), and RIPEMD-160 secure hashes
+and message digests.  Note that MD2 and MD4 are not included
+by default and are only present if they are compiled in mbedtls.
+
+Here are the examples from (standard) *hashlib* ported
+to *python-mbedtls*:
+
+>>> from mbedtls import hashlib
+>>> m = hashlib.md5()
+>>> m.update(b"Nobody inspects")
+>>> m.update(b" the spammish repetition")
+>>> m.digest()
+b'\xbbd\x9c\x83\xdd\x1e\xa5\xc9\xd9\xde\xc9\xa1\x8d\xf0\xff\xe9'
+>>> m.digest_size
+16
+>>> m.block_size
+64
+
+More condensed:
+
+>>> hashlib.sha224(b"Nobody inspects the spammish repetition").hexdigest()
+'a4337bc45a8fc544c03f52dc550cd6e1e87021bc896588bd79e901e2'
+
+Using ``new()``:
+
+>>> h = hashlib.new('ripemd160')
+>>> h.update(b"Nobody inspects the spammish repetition")
+>>> h.hexdigest()
+'cc4a5ce1b3df48aec5d22d1f16b894a0b894eccc'
+
+
+HMAC algorithm
+--------------
+
+The *mbedtls.hmac* module computes HMAC.
+
+Example:
+
+>>> from mbedtls import hmac
+>>> m = hmac.new(b"This is my secret key", digestmod="md5")
+>>> m.update(b"Nobody inspects")
+>>> m.update(b" the spammish repetition")
+>>> m.digest()
+b'\x9d-/rj\\\x98\x80\xb1rG\x87\x0f\xe9\xe4\xeb'
+
+Warning:
+
+The message is cleared after calculation of the digest.  Only call
+``mbedtls.hmac.Hmac.digest()`` or ``mbedtls.hmac.Hmac.hexdigest()``
+once per message.
+
+
+HMAC-based key derivation function (HKDF)
+-----------------------------------------
+
+The *mbedtls.hkdf* module exposes extract-and-expand key derivation
+functions.  The main function is ``hkdf()`` but ``extract()`` and
+``expand()`` may be used as well.
+
+Example:
+
+>>> from mbedtls import hkdf
+>>> hkdf.hkdf(
+...     b"my secret key",
+...     length=42,
+...     info=b"my cool app",
+...     salt=b"and pepper",
+...     digestmod=hmac.sha256
+... )
+b'v,\xef\x90\xccU\x1d\x1b\xd7\\a\xaf\x92\xac\n\x90\xf9q\xf4)\xcd"\xf7\x1a\x94p\x03.\xa8e\x1e\xfb\x92\xe8l\x0cc\xf8e\rvj'
+
+where *info*, *salt*, and *digestmod* are optional, although providing
+(at least) *info* is highly recommended.
+
+
+Symmetric cipher
+----------------
+
+The *mbedtls.cipher* module provides symmetric encryption.  The API
+follows the recommendations from PEP 272 so that it can be used as a
+drop-in replacement to other libraries.
+
+*python-mbedtls* provides the following algorithms:
+
+- AES encryption/decryption (128, 192, and 256 bits) in ECB, CBC, CFB128,
+  CTR, OFB, or XTS mode;
+- AES AEAD (128, 192, and 256 bits) in GCM or CCM mode;
+- ARC4 encryption/decryption;
+- ARIA encryption/decryption (128, 192, and 256 bits) in ECB, CBC,
+  CTR, or GCM modes;
+- Blowfish encryption/decryption in ECB, CBC, CFB64, or CTR mode;
+- Camellia encryption/decryption (128, 192, and 256 bits) in ECB, CBC,
+  CFB128, CTR, or GCM mode;
+- DES, DES3, and double DES3 encryption/decryption in ECB or CBC mode;
+- CHACHA20 and CHACHA20/POLY1305 encryption/decryption.
+
+Example:
+
+>>> from mbedtls import cipher
+>>> c = cipher.AES.new(b"My 16-bytes key.", cipher.MODE_CBC, b"CBC needs an IV.")
+>>> enc = c.encrypt(b"This is a super-secret message!!")
+>>> enc
+b"*`k6\x98\x97=[\xdf\x7f\x88\x96\xf5\t\x19J\xf62h\xf4n\xca\xe8\xfe\xf5\xd7X'\xb1\x8c\xc9\x85"
+>>> c.decrypt(enc)
+b'This is a super-secret message!!'
+
+
+RSA public key
+--------------
+
+The *mbedtls.pk* module provides the RSA cryptosystem.  This includes:
+
+- Public-private key generation and key import/export in PEM and DER
+  formats;
+- asymmetric encryption and decryption;
+- message signature and verification.
+
+Key generation, the default size is 2048 bits:
+
+>>> from mbedtls import pk
+>>> rsa = pk.RSA()
+>>> prv = rsa.generate()
+>>> rsa.key_size
+256
+
+Message encryption and decryption:
+
+>>> enc = rsa.encrypt(b"secret message")
+>>> rsa.decrypt(enc)
+b'secret message'
+
+Message signature and verification:
+
+>>> sig = rsa.sign(b"Please sign here.")
+>>> rsa.verify(b"Please sign here.", sig)
+True
+>>> rsa.verify(b"Sorry, wrong message.", sig)
+False
+>>> pub = rsa.export_public_key(format="DER")
+>>> other = pk.RSA.from_buffer(pub)
+>>> other.verify(b"Please sign here.", sig)
+True
+
+
+Static and ephemeral elliptic curve Diffie-Hellman
+--------------------------------------------------
+
+The *mbedtls.pk* module provides the ECC cryptosystem.  This includes:
+
+- Public-private key generation and key import/export in the PEM and DER
+  formats;
+- asymmetric encrypt and decryption;
+- message signature and verification;
+- ephemeral ECDH key exchange.
+
+``get_supported_curves()`` returns the list of supported curves.
+
+The API of the ECC class is the same as the API of the RSA class
+but ciphering (``encrypt()`` and ``decrypt()`` is not supported by
+Mbed TLS).
+
+Message signature and verification using elliptic a curve digital
+signature algorithm (ECDSA):
+
+>>> from mbedtls import pk
+>>> ecdsa = pk.ECC()
+>>> prv = ecdsa.generate()
+>>> sig = ecdsa.sign(b"Please sign here.")
+>>> ecdsa.verify(b"Please sign here.", sig)
+True
+>>> ecdsa.verify(b"Sorry, wrong message.", sig)
+False
+>>> pub = ecdsa.export_public_key(format="DER")
+>>> other = pk.ECC.from_buffer(pub)
+>>> other.verify(b"Please sign here.", sig)
+True
+
+The classes ``ECDHServer`` and ``ECDHClient`` may be used for ephemeral
+ECDH.  The key exchange is as follows:
+
+>>> ecdh_key = pk.ECC()
+>>> ecdh_key.generate()
+>>> ecdh_srv = pk.ECDHServer(ecdh_key)
+>>> ecdh_cli = pk.ECDHClient(ecdh_key)
+
+The server generates the ServerKeyExchange encrypted payload and
+passes it to the client:
+
+>>> ske = ecdh_srv.generate()
+>>> ecdh_cli.import_SKE(ske)
+
+then the client generates the ClientKeyExchange encrypted payload and
+passes it back to the server:
+
+>>> cke = ecdh_cli.generate()
+>>> ecdh_srv.import_CKE(cke)
+
+Now, client and server may generate their shared secret:
+
+>>> secret = ecdh_srv.generate_secret()
+>>> ecdh_cli.generate_secret() == secret
+True
+>>> ecdh_srv.shared_secret == ecdh_cli.shared_secret
+True
+
+
+Diffie-Hellman-Merkle key exchange
+----------------------------------
+
+The classes ``DHServer`` and ``DHClient`` may be used for DH Key
+exchange.  The classes have the same API as ``ECDHServer``
+and ``ECDHClient``, respectively.
+
+The key exchange is as follow:
+
+>>> from mbedtls.mpi import MPI
+>>> from mbedtls import pk
+>>> dh_srv = pk.DHServer(MPI.prime(128), MPI.prime(96))
+>>> dh_cli = pk.DHClient(MPI.prime(128), MPI.prime(96))
+
+The 128-bytes prime and the 96-bytes prime are the modulus ``P``
+and the generator ``G``.
+
+The server generates the ServerKeyExchange payload:
+
+>>> ske = dh_srv.generate()
+>>> dh_cli.import_SKE(ske)
+
+The payload ends with ``G^X mod P`` where ``X`` is the secret value of
+the server.
+
+>>> cke = dh_cli.generate()
+>>> dh_srv.import_CKE(cke)
+
+``cke`` is ``G^Y mod P`` (with ``Y`` the secret value from the client)
+returned as its representation in bytes so that it can be readily
+transported over the network.
+
+As in ECDH, client and server may now generate their shared secret:
+
+>>> secret = dh_srv.generate_secret()
+>>> dh_cli.generate_secret() == secret
+True
+>>> dh_srv.shared_secret == dh_cli.shared_secret
+True
+
+
+X.509 certificate writing and parsing
+-------------------------------------
+
+The *mbedtls.x509* module can be used to parse X.509 certificates
+or create and verify a certificate chain.
+
+Here, the trusted root is a self-signed CA certificate
+``ca0_crt`` signed by ``ca0_key``.
+
+>>> import datetime as dt
+>>>
+>>> from mbedtls import hashlib
+>>> from mbedtls import pk
+>>> from mbedtls import x509
+>>>
+>>> now = dt.datetime.utcnow()
+>>> ca0_key = pk.RSA()
+>>> _ = ca0_key.generate()
+>>> ca0_csr = x509.CSR.new(ca0_key, "CN=Trusted CA", hashlib.sha256())
+>>> ca0_crt = x509.CRT.selfsign(
+...     ca0_csr, ca0_key,
+...     not_before=now, not_after=now + dt.timedelta(days=90),
+...     serial_number=0x123456,
+...     basic_constraints=x509.BasicConstraints(True, 1))
+...
+
+An intermediate then issues a Certificate Singing Request (CSR) that the
+root CA signs:
+
+>>> ca1_key = pk.ECC()
+>>> _ = ca1_key.generate()
+>>> ca1_csr = x509.CSR.new(ca1_key, "CN=Intermediate CA", hashlib.sha256())
+>>>
+>>> ca1_crt = ca0_crt.sign(
+...     ca1_csr, ca0_key, now, now + dt.timedelta(days=90), 0x123456,
+...     basic_constraints=x509.BasicConstraints(ca=True, max_path_length=3))
+...
+
+And finally, the intermediate CA signs a certificate for the
+End Entity on the basis of a new CSR:
+
+>>> ee0_key = pk.ECC()
+>>> _ = ee0_key.generate()
+>>> ee0_csr = x509.CSR.new(ee0_key, "CN=End Entity", hashlib.sha256())
+>>>
+>>> ee0_crt = ca1_crt.sign(
+...     ee0_csr, ca1_key, now, now + dt.timedelta(days=90), 0x987654)
+...
+
+The emitting certificate can be used to verify the next certificate in
+the chain:
+
+>>> ca1_crt.verify(ee0_crt)
+True
+>>> ca0_crt.verify(ca1_crt)
+True
+
+Note, however, that this verification is only one step in a private key
+infrastructure and does not take CRLs, path length, etc. into account.
+
+
+TLS and DTLS client and server
+------------------------------
+
+The *mbedtls.tls* module provides TLS clients and servers.  The API
+follows the recommendations of `PEP 543`_.  Note, however, that the
+Python standard SSL library does not follow the PEP so that this
+library may not be a drop-in replacement.
+
+.. _PEP 543: https://www.python.org/dev/peps/pep-0543/
+
+Connectionless DTLS is supported as well.
+
+See examples in the `programs/`_ directory of the repository
+and `tests/test_tls.py`_.
+
+.. _programs/: https://github.com/Synss/python-mbedtls/tree/master/programs
+.. _tests/test_tls.py: https://github.com/Synss/python-mbedtls/blob/master/tests/test_tls.py
```

### Comparing `python-mbedtls-2.7.0/programs/client.py` & `python-mbedtls-2.7.1/programs/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,201 +1,207 @@
-#!/usr/bin/env python
-# SPDX-License-Identifier: MIT
-"""An example DTLS/TLS client.
-
-Run ./programs/client.py --help.
-
-"""
-
-from __future__ import annotations
-
-import argparse
-import socket
-import sys
-import time
-from contextlib import suppress
-from typing import Any, Optional, Tuple, Union
-
-from mbedtls._tls import _enable_debug_output, _set_debug_level  # type: ignore
-from mbedtls.exceptions import TLSError
-from mbedtls.tls import (
-    ClientContext,
-    DTLSConfiguration,
-    TLSConfiguration,
-    TLSWrappedSocket,
-)
-
-if sys.version_info < (3, 10):
-    from typing_extensions import TypeAlias
-else:
-    from typing import TypeAlias
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Final
-else:
-    from typing import Final
-
-
-__all__ = ["Client"]
-
-_Address: TypeAlias = Union[Tuple[Any, ...], str]
-
-
-def _echo_tls(sock: TLSWrappedSocket, buffer: bytes, chunksize: int) -> bytes:
-    view = memoryview(buffer)
-    received = bytearray()
-    for idx in range(0, len(view), chunksize):
-        part = view[idx : idx + chunksize]
-        sock.send(part)
-        received += sock.recv(chunksize)
-    return received
-
-
-def _echo_dtls(sock: TLSWrappedSocket, buffer: bytes, chunksize: int) -> bytes:
-    view = memoryview(buffer)
-    received = bytearray()
-    while len(received) != len(buffer):
-        part = view[len(received) : len(received) + chunksize]
-        sock.send(part)
-        data, _addr = sock.recvfrom(chunksize)
-        received += data
-        if not data:
-            # Avoid tight loop.
-            time.sleep(0.01)
-    return received
-
-
-class Client:
-    def __init__(
-        self,
-        cli_conf: Union[TLSConfiguration, DTLSConfiguration],
-        proto: socket.SocketKind,
-        srv_address: _Address,
-        srv_hostname: Optional[str],
-    ) -> None:
-        super().__init__()
-        self.cli_conf: Final = cli_conf
-        self.proto: Final = proto
-        self.srv_address: Final = srv_address
-        self.srv_hostname: Final = srv_hostname
-        self._sock: Optional[TLSWrappedSocket] = None
-        self._echo: Final = {
-            socket.SOCK_STREAM: _echo_tls,
-            socket.SOCK_DGRAM: _echo_dtls,
-        }[self.proto]
-
-    def __enter__(self) -> Client:
-        self.start()
-        return self
-
-    def __exit__(self, *exc_info: object) -> None:
-        self.stop()
-
-    def __del__(self) -> None:
-        self.stop()
-
-    @property
-    def context(self) -> Optional[ClientContext]:
-        if self._sock is None:
-            return None
-        assert isinstance(self._sock.context, ClientContext)
-        return self._sock.context
-
-    def do_handshake(self) -> None:
-        if not self._sock:
-            return
-
-        self._sock.do_handshake()
-
-    def echo(self, buffer: bytes, chunksize: int) -> bytes:
-        if not self._sock:
-            return b""
-
-        return bytes(self._echo(self._sock, buffer, chunksize))
-
-    def start(self) -> None:
-        if self._sock:
-            self.stop()
-
-        self._sock = ClientContext(self.cli_conf).wrap_socket(
-            socket.socket(socket.AF_INET, self.proto),
-            server_hostname=self.srv_hostname,
-        )
-        self._sock.connect(self.srv_address)
-
-    def stop(self) -> None:
-        if not self._sock:
-            return
-
-        with suppress(TLSError, OSError):
-            self._sock.close()
-        self._sock = None
-
-    def restart(self) -> None:
-        self.stop()
-        self.start()
-
-
-def parse_args() -> argparse.Namespace:
-    class PSKArg(argparse.Action):
-        def __call__(
-            self,
-            parser: object,
-            namespace: argparse.Namespace,
-            values: Any,
-            option_string: Optional[str] = None,
-        ) -> None:
-            def entry(kv: bytes) -> Tuple[str, bytes]:
-                k, v = kv.split(b"=")
-                return k.decode("utf-8"), v
-
-            setattr(namespace, self.dest, entry(values))
-
-    parser = argparse.ArgumentParser(description="client")
-    group = parser.add_mutually_exclusive_group(required=True)
-    group.add_argument(
-        "--tls", dest="proto", action="store_const", const=socket.SOCK_STREAM
-    )
-    group.add_argument(
-        "--dtls", dest="proto", action="store_const", const=socket.SOCK_DGRAM
-    )
-    parser.add_argument("--address", default="127.0.0.1")
-    parser.add_argument("--port", default=4433, type=int)
-    parser.add_argument("--debug", type=int)
-    parser.add_argument("--server-name", default="localhost")
-    parser.add_argument(
-        "--psk",
-        type=lambda x: x.encode("latin1"),
-        action=PSKArg,
-        metavar="CLI=SECRET",
-    )
-    parser.add_argument("message", default="hello")
-    return parser.parse_args()
-
-
-def main(args: argparse.Namespace) -> None:
-    conf: Union[TLSConfiguration, DTLSConfiguration]
-    if args.proto is socket.SOCK_STREAM:
-        conf = TLSConfiguration(
-            pre_shared_key=args.psk, validate_certificates=False
-        )
-    elif args.proto is socket.SOCK_DGRAM:
-        conf = DTLSConfiguration(
-            pre_shared_key=args.psk, validate_certificates=False
-        )
-    else:
-        raise NotImplementedError(args.proto)
-
-    with Client(
-        conf, args.proto, (args.address, args.port), args.server_name
-    ) as cli:
-        if args.debug is not None:
-            _enable_debug_output(cli.context)
-            _set_debug_level(args.debug)
-
-        cli.do_handshake()
-        received = cli.echo(args.message.encode("utf-8"), 1024)
-    print(received.decode("utf-8"))
-
-
-if __name__ == "__main__":
-    main(parse_args())
+#!/usr/bin/env python
+# SPDX-License-Identifier: MIT
+"""An example DTLS/TLS server.
+
+Run ./programs/server.py --help.
+
+"""
+
+from __future__ import annotations
+
+import argparse
+import socket
+import sys
+import time
+from contextlib import suppress
+from functools import partial
+from typing import Any, Callable, NoReturn, Optional, Tuple, Union
+
+from mbedtls._tls import _enable_debug_output, _set_debug_level  # type: ignore
+from mbedtls.tls import (
+    DTLSConfiguration,
+    HelloVerifyRequest,
+    ServerContext,
+    TLSConfiguration,
+    TLSWrappedSocket,
+)
+
+if sys.version_info < (3, 10):
+    from typing_extensions import TypeAlias
+else:
+    from typing import TypeAlias
+
+from typing import Final
+
+__all__ = ["Server"]
+
+_Address: TypeAlias = Union[Tuple[Any, ...], str]
+
+
+def _make_tls_connection(sock: TLSWrappedSocket) -> TLSWrappedSocket:
+    assert sock
+    conn, _addr = sock.accept()
+    conn.do_handshake()
+    return conn
+
+
+def _make_dtls_connection(sock: TLSWrappedSocket) -> TLSWrappedSocket:
+    assert sock
+    conn, addr = sock.accept()
+    conn.setcookieparam(addr[0].encode("ascii"))
+    with suppress(HelloVerifyRequest):
+        conn.do_handshake()
+
+    _, (conn, addr) = conn, conn.accept()
+    _.close()
+    conn.setcookieparam(addr[0].encode("ascii"))
+    conn.do_handshake()
+    return conn
+
+
+class Server:
+    def __init__(
+        self,
+        srv_conf: Union[TLSConfiguration, DTLSConfiguration],
+        proto: socket.SocketKind,
+        address: _Address,
+    ) -> None:
+        super().__init__()
+        self.srv_conf: Final = srv_conf
+        self.proto: Final = proto
+        self.address: Final = address
+        self._make_connection: Final = {
+            socket.SOCK_STREAM: _make_tls_connection,
+            socket.SOCK_DGRAM: _make_dtls_connection,
+        }[self.proto]
+        self._sock: Optional[TLSWrappedSocket] = None
+
+    def __enter__(self) -> Server:
+        self.start()
+        return self
+
+    def __exit__(self, *exc_info: object) -> None:
+        self.stop()
+
+    def __del__(self) -> None:
+        self.stop()
+
+    @property
+    def context(self) -> Optional[ServerContext]:
+        if self._sock is None:
+            return None
+        assert isinstance(self._sock.context, ServerContext)
+        return self._sock.context
+
+    def start(self) -> None:
+        if self._sock:
+            self.stop()
+
+        self._sock = ServerContext(self.srv_conf).wrap_socket(
+            socket.socket(socket.AF_INET, self.proto)
+        )
+        self._sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        self._sock.bind(self.address)
+        if self.proto is socket.SOCK_STREAM:
+            self._sock.listen(1)
+
+    def stop(self) -> None:
+        if not self._sock:
+            return
+
+        self._sock.close()
+        self._sock = None
+
+    def run(
+        self, conn_handler: Callable[[TLSWrappedSocket], None]
+    ) -> NoReturn:
+        if not self._sock:
+            raise ConnectionRefusedError("server not started")
+
+        while True:
+            self._run(conn_handler)
+
+    def _run(self, conn_handler: Callable[[TLSWrappedSocket], None]) -> None:
+        assert self._sock is not None
+        with self._make_connection(self._sock) as conn:
+            conn_handler(conn)
+
+
+def echo_handler(conn: TLSWrappedSocket, *, packet_size: int) -> None:
+    while True:
+        data = conn.recv(packet_size)
+        if data:
+            break
+        # Avoid tight loop.
+        time.sleep(0.01)
+    sent = 0
+    view = memoryview(data)
+    while sent != len(data):
+        sent += conn.send(view[sent:])
+
+
+def parse_args() -> argparse.Namespace:
+    class PSKStoreArg(argparse.Action):
+        def __call__(
+            self,
+            parser: object,
+            namespace: argparse.Namespace,
+            values: Any,
+            option_string: Optional[str] = None,
+        ) -> None:
+            def entry(kv: bytes) -> Tuple[str, bytes]:
+                k, v = kv.split(b"=")
+                return k.decode("utf-8"), v
+
+            setattr(
+                namespace,
+                self.dest,
+                dict(entry(kv) for kv in values.split(b",")),
+            )
+
+    parser = argparse.ArgumentParser(description="server")
+    group = parser.add_mutually_exclusive_group(required=True)
+    group.add_argument(
+        "--tls", dest="proto", action="store_const", const=socket.SOCK_STREAM
+    )
+    group.add_argument(
+        "--dtls", dest="proto", action="store_const", const=socket.SOCK_DGRAM
+    )
+    parser.add_argument("--address", default="0.0.0.0")
+    parser.add_argument("--port", default=4433, type=int)
+    parser.add_argument("--debug", type=int)
+    parser.add_argument(
+        "--psk-store",
+        type=lambda x: x.encode("latin1"),
+        action=PSKStoreArg,
+        metavar="CLI1=SECRET1,CLI2=SECRET2...",
+    )
+    return parser.parse_args()
+
+
+def main(args: argparse.Namespace) -> NoReturn:
+    conf: Union[TLSConfiguration, DTLSConfiguration]
+    if args.proto is socket.SOCK_STREAM:
+        conf = TLSConfiguration(
+            pre_shared_key_store=args.psk_store, validate_certificates=False
+        )
+    elif args.proto is socket.SOCK_DGRAM:
+        conf = DTLSConfiguration(
+            pre_shared_key_store=args.psk_store, validate_certificates=False
+        )
+    else:
+        raise NotImplementedError(args.proto)
+
+    with Server(conf, args.proto, (args.address, args.port)) as srv:
+        if args.debug is not None:
+            _enable_debug_output(srv.context)
+            _set_debug_level(args.debug)
+
+        srv.run(partial(echo_handler, packet_size=4069))
+
+
+if __name__ == "__main__":
+    import faulthandler
+
+    faulthandler.enable()
+    with suppress(KeyboardInterrupt):
+        main(parse_args())
```

### Comparing `python-mbedtls-2.7.0/pyproject.toml` & `python-mbedtls-2.7.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-[tool.black]
-line-length = 79
-target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
-
-[tool.cibuildwheel]
-skip = "*-manylinux_i686 *-win32"
-test-requires = "-rrequirements/tests.txt"
-test-command = "pytest {project}/tests"
-
-[tool.cibuildwheel.linux]
-before-all = '''
-./scripts/download-mbedtls.sh $VERSION ~/.local/src \
-&& ./scripts/install-mbedtls.sh ~/.local/src
-'''
-
-[tool.cibuildwheel.macos]
-before-all = '''
-./scripts/download-mbedtls.sh $VERSION ~/.local/src \
-&& ./scripts/install-mbedtls.sh ~/.local/src \
-&& cp /usr/local/lib/libmbed*dylib .
-'''
-
-[tool.cibuildwheel.windows]
-before-all = """
-powershell -Command Get-Host \
-&& powershell Get-Location \
-&& powershell New-Item -Path . -Name _lib -ItemType directory \
-&& powershell %CD%\\scripts\\download-mbedtls.ps1 %VERSION% _lib\\mbedtls \
-&& powershell %CD%\\scripts\\install-mbedtls.ps1 -ConfigurationType StaticLibrary _lib\\mbedtls \
-&& powershell %CD%\\scripts\\install-mbedtls.ps1 -ConfigurationType DynamicLibrary _lib\\mbedtls \
-&& dir %LIB%
-"""
-
-[tool.coverage.report]
-exclude_lines = [
-  '\.\.\.',
-  'assert 0',
-  'def __repr__',
-  'free\(\w+\)',
-  'from typing import ',
-  'from typing_extensions import ',
-  'if sys\.version_info',
-  'pragma: no cover',
-  'raise MemoryError',
-  'raise NotImplementedError',
-]
-include = ['src/*']
-
-[tool.coverage.run]
-plugins = ['Cython.Coverage']
-
-[tool.isort]
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-use_parentheses = true
-line_length = 79
-
-[tool.mypy]
-show_error_codes = true
-strict = true
-
-[tool.pylint.master]
-extension-pkg-whitelist='mbedtls'
-load-plugins=[
-  "pylint_per_file_ignores",
-]
-disable=[
-  "missing-class-docstring",
-  "missing-function-docstring",
-  "missing-module-docstring",
-]
-
-[tool.pylint-per-file-ignores]
-"src/mbedtls/"="""
-C0209,
-R0801,
-import-error,
-useless-import-alias,
-"""
-"tests/"="redefined-outer-name"
-
-[tool.pylint.messages_control]
-disable = "C0103"
-
-[tool.pylint.similarities]
-ignore-comments = "yes"
-ignore-docstrings = "yes"
-min-similarity-lines = "8"
-
-[tool.pytest.ini_options]
-markers = "e2e: end-to-end tests"
-
-[tool.ruff]
-ignore = ["E701"]
+[tool.black]
+line-length = 79
+target-version = ['py38', 'py39', 'py310', 'py311']
+
+[tool.cibuildwheel]
+skip = "*-manylinux_i686 *-win32"
+test-requires = "-rrequirements/tests.txt"
+test-command = "pytest {project}/tests"
+
+[tool.cibuildwheel.linux]
+before-all = '''
+./scripts/download-mbedtls.sh $VERSION ~/.local/src \
+&& ./scripts/install-mbedtls.sh ~/.local/src
+'''
+
+[tool.cibuildwheel.macos]
+before-all = '''
+./scripts/download-mbedtls.sh $VERSION ~/.local/src \
+&& ./scripts/install-mbedtls.sh ~/.local/src \
+&& cp /usr/local/lib/libmbed*dylib .
+'''
+
+[tool.cibuildwheel.windows]
+before-all = """
+powershell -Command Get-Host \
+&& powershell Get-Location \
+&& powershell New-Item -Path . -Name _lib -ItemType directory \
+&& powershell %CD%\\scripts\\download-mbedtls.ps1 %VERSION% _lib\\mbedtls \
+&& powershell %CD%\\scripts\\install-mbedtls.ps1 -ConfigurationType StaticLibrary _lib\\mbedtls \
+&& powershell %CD%\\scripts\\install-mbedtls.ps1 -ConfigurationType DynamicLibrary _lib\\mbedtls \
+&& dir %LIB%
+"""
+
+[tool.coverage.report]
+exclude_lines = [
+  '\.\.\.',
+  'assert 0',
+  'def __repr__',
+  'free\(\w+\)',
+  'from typing import ',
+  'from typing_extensions import ',
+  'if sys\.version_info',
+  'pragma: no cover',
+  'raise MemoryError',
+  'raise NotImplementedError',
+]
+include = ['src/*']
+
+[tool.coverage.run]
+plugins = ['Cython.Coverage']
+
+[tool.isort]
+multi_line_output = 3
+include_trailing_comma = true
+force_grid_wrap = 0
+use_parentheses = true
+line_length = 79
+
+[tool.mypy]
+show_error_codes = true
+strict = true
+
+[tool.pylint.master]
+extension-pkg-whitelist='mbedtls'
+load-plugins=[
+  "pylint_per_file_ignores",
+]
+disable=[
+  "missing-class-docstring",
+  "missing-function-docstring",
+  "missing-module-docstring",
+]
+
+[tool.pylint-per-file-ignores]
+"src/mbedtls/"="""
+C0209,
+R0801,
+import-error,
+useless-import-alias,
+"""
+"tests/"="redefined-outer-name"
+
+[tool.pylint.messages_control]
+disable = "C0103"
+
+[tool.pylint.similarities]
+ignore-comments = "yes"
+ignore-docstrings = "yes"
+min-similarity-lines = "8"
+
+[tool.pytest.ini_options]
+markers = "e2e: end-to-end tests"
+
+[tool.ruff]
+ignore = ["E701"]
```

### Comparing `python-mbedtls-2.7.0/scripts/build-wheel.sh` & `python-mbedtls-2.7.1/scripts/build-wheel.sh`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-#!/bin/bash
-
-set -ex
-
-function get_abi_tag {
-	local python="${1:?}"
-	echo $($python -c 'from wheel import bdist_wheel as w; print(w.get_abi_tag())')
-}
-
-function build {
-	local python="${1:?}"
-	$python --version
-	$python setup.py bdist_wheel 1> /dev/null
-	rm -r .eggs* build*
-}
-
-function audit_linux {
-	auditwheel repair "${1:?}"
-}
-
-function audit_macos {
-	delocate-wheel -w wheelhouse -v "${1:?}"
-}
-
-function main {
-	local python="${1:-python}"
-	local system="${2:-linux}"  # "[linux|macos]"
-
-	build $python
-	whl=$(ls ./dist/*$(get_abi_tag $python)*.whl)
-	ls $whl
-
-	if [ "$system" = "macos" ]; then
-		audit_macos $whl
-	else
-		audit_linux $whl
-	fi
-}
-
-main "$@"
+#!/bin/bash
+
+set -ex
+
+function get_abi_tag {
+	local python="${1:?}"
+	echo $($python -c 'from wheel import bdist_wheel as w; print(w.get_abi_tag())')
+}
+
+function build {
+	local python="${1:?}"
+	$python --version
+	$python setup.py bdist_wheel 1> /dev/null
+	rm -r .eggs* build*
+}
+
+function audit_linux {
+	auditwheel repair "${1:?}"
+}
+
+function audit_macos {
+	delocate-wheel -w wheelhouse -v "${1:?}"
+}
+
+function main {
+	local python="${1:-python}"
+	local system="${2:-linux}"  # "[linux|macos]"
+
+	build $python
+	whl=$(ls ./dist/*$(get_abi_tag $python)*.whl)
+	ls $whl
+
+	if [ "$system" = "macos" ]; then
+		audit_macos $whl
+	else
+		audit_linux $whl
+	fi
+}
+
+main "$@"
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/_dhm.pxd` & `python-mbedtls-2.7.1/src/mbedtls/_dhm.pxd`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2016, Elaborated Networks GmbH
-# Copyright (c) 2018, Mathias Laurin
-
-cimport mbedtls.mpi as _mpi
-
-
-cdef extern from "mbedtls/dhm.h" nogil:
-    ctypedef struct mbedtls_dhm_context:
-        _mpi.mbedtls_mpi P
-        _mpi.mbedtls_mpi G
-        _mpi.mbedtls_mpi X
-        _mpi.mbedtls_mpi GX
-        _mpi.mbedtls_mpi GY
-        _mpi.mbedtls_mpi K
-
-    void mbedtls_dhm_init(mbedtls_dhm_context *ctx)
-    void mbedtls_dhm_free(mbedtls_dhm_context *ctx)
-
-    int mbedtls_dhm_make_params(
-        mbedtls_dhm_context *ctx,
-        int x_size,
-        unsigned char *output, size_t *olen,
-        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng)
-    int mbedtls_dhm_make_public(
-        mbedtls_dhm_context *ctx,
-        int x_size,
-        unsigned char *output, size_t olen,
-        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng)
-
-    int mbedtls_dhm_read_params(
-        mbedtls_dhm_context *ctx,
-        unsigned char **p,
-        const unsigned char *end)
-    int mbedtls_dhm_read_public(
-        mbedtls_dhm_context *ctx,
-        const unsigned char *input, size_t ilen)
-
-    int mbedtls_dhm_calc_secret(
-        mbedtls_dhm_context *ctx,
-        unsigned char *output, size_t output_size, size_t *olen,
-        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng)
-
-    # int mbedtls_dhm_parse_dhm(
-    #     mbedtls_dhm_context *dhm,
-    #     const unsigned char *dhmin, size_t dhminlen)
-    # int mbedtls_dhm_parse_dhmfile(
-    #     mbedtls_dhm_context *dhm,
-    #     const char *path)
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2016, Elaborated Networks GmbH
+# Copyright (c) 2018, Mathias Laurin
+
+cimport mbedtls.mpi as _mpi
+
+
+cdef extern from "mbedtls/dhm.h" nogil:
+    ctypedef struct mbedtls_dhm_context:
+        _mpi.mbedtls_mpi P
+        _mpi.mbedtls_mpi G
+        _mpi.mbedtls_mpi X
+        _mpi.mbedtls_mpi GX
+        _mpi.mbedtls_mpi GY
+        _mpi.mbedtls_mpi K
+
+    void mbedtls_dhm_init(mbedtls_dhm_context *ctx)
+    void mbedtls_dhm_free(mbedtls_dhm_context *ctx)
+
+    int mbedtls_dhm_make_params(
+        mbedtls_dhm_context *ctx,
+        int x_size,
+        unsigned char *output, size_t *olen,
+        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng)
+    int mbedtls_dhm_make_public(
+        mbedtls_dhm_context *ctx,
+        int x_size,
+        unsigned char *output, size_t olen,
+        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng)
+
+    int mbedtls_dhm_read_params(
+        mbedtls_dhm_context *ctx,
+        unsigned char **p,
+        const unsigned char *end)
+    int mbedtls_dhm_read_public(
+        mbedtls_dhm_context *ctx,
+        const unsigned char *input, size_t ilen)
+
+    int mbedtls_dhm_calc_secret(
+        mbedtls_dhm_context *ctx,
+        unsigned char *output, size_t output_size, size_t *olen,
+        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng)
+
+    # int mbedtls_dhm_parse_dhm(
+    #     mbedtls_dhm_context *dhm,
+    #     const unsigned char *dhmin, size_t dhminlen)
+    # int mbedtls_dhm_parse_dhmfile(
+    #     mbedtls_dhm_context *dhm,
+    #     const char *path)
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/_ecdsa.pxd` & `python-mbedtls-2.7.1/src/mbedtls/_ecdsa.pxd`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2016, Elaborated Networks GmbH
-# Copyright (c) 2018, Mathias Laurin
-
-cdef extern from "mbedtls/ecdsa.h" nogil:
-    ctypedef struct mbedtls_ecdsa_context:
-        mbedtls_ecp_group grp
-        _mpi.mbedtls_mpi d
-        mbedtls_ecp_point Q
-
-    int MBEDTLS_ECDSA_MAX_LEN
-
-    # mbedtls_ecp_group
-    # -----------------
-    # mbedtls_ecdsa_sign
-    # mbedtls_ecdsa_sign_det
-    # mbedtls_ecdsa_verify
-
-    # mbedtls_ecdsa_context
-    # ---------------------
-    void mbedtls_ecdsa_init(mbedtls_ecdsa_context *ctx)
-    void mbedtls_ecdsa_free(mbedtls_ecdsa_context *ctx)
-
-    int mbedtls_ecdsa_from_keypair(
-        mbedtls_ecdsa_context *ctx,
-        const mbedtls_ecp_keypair *key)
-
-    # mbedtls_ecdsa_write_signature
-    # mbedtls_ecdsa_write_signature_det
-    # mbedtls_ecdsa_read_signature
-
-    int mbedtls_ecdsa_genkey(
-        mbedtls_ecdsa_context *ctx, mbedtls_ecp_group_id gid,
-        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng)
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2016, Elaborated Networks GmbH
+# Copyright (c) 2018, Mathias Laurin
+
+cdef extern from "mbedtls/ecdsa.h" nogil:
+    ctypedef struct mbedtls_ecdsa_context:
+        mbedtls_ecp_group grp
+        _mpi.mbedtls_mpi d
+        mbedtls_ecp_point Q
+
+    int MBEDTLS_ECDSA_MAX_LEN
+
+    # mbedtls_ecp_group
+    # -----------------
+    # mbedtls_ecdsa_sign
+    # mbedtls_ecdsa_sign_det
+    # mbedtls_ecdsa_verify
+
+    # mbedtls_ecdsa_context
+    # ---------------------
+    void mbedtls_ecdsa_init(mbedtls_ecdsa_context *ctx)
+    void mbedtls_ecdsa_free(mbedtls_ecdsa_context *ctx)
+
+    int mbedtls_ecdsa_from_keypair(
+        mbedtls_ecdsa_context *ctx,
+        const mbedtls_ecp_keypair *key)
+
+    # mbedtls_ecdsa_write_signature
+    # mbedtls_ecdsa_write_signature_det
+    # mbedtls_ecdsa_read_signature
+
+    int mbedtls_ecdsa_genkey(
+        mbedtls_ecdsa_context *ctx, mbedtls_ecp_group_id gid,
+        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng)
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/_ecp.pxd` & `python-mbedtls-2.7.1/src/mbedtls/_ecp.pxd`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2016, Elaborated Networks GmbH
-# Copyright (c) 2018, Mathias Laurin
-
-cimport mbedtls.mpi as _mpi
-
-
-cdef extern from "mbedtls/ecp.h" nogil:
-    ctypedef enum mbedtls_ecp_group_id:
-        MBEDTLS_ECP_DP_NONE = 0,
-        MBEDTLS_ECP_DP_SECP192R1
-        MBEDTLS_ECP_DP_SECP224R1
-        MBEDTLS_ECP_DP_SECP256R1
-        MBEDTLS_ECP_DP_SECP384R1
-        MBEDTLS_ECP_DP_SECP521R1
-        MBEDTLS_ECP_DP_BP256R1
-        MBEDTLS_ECP_DP_BP384R1
-        MBEDTLS_ECP_DP_BP512R1
-        MBEDTLS_ECP_DP_CURVE25519
-        MBEDTLS_ECP_DP_SECP192K1
-        MBEDTLS_ECP_DP_SECP224K1
-        MBEDTLS_ECP_DP_SECP256K1
-        MBEDTLS_ECP_DP_CURVE448
-
-    ctypedef enum mbedtls_ecp_curve_type:
-        MBEDTLS_ECP_TYPE_NONE = 0
-        MBEDTLS_ECP_TYPE_SHORT_WEIERSTRASS
-        MBEDTLS_ECP_TYPE_MONTGOMERY
-
-    ctypedef struct mbedtls_ecp_curve_info:
-        mbedtls_ecp_group_id grp_id
-        int bit_size
-        const char *name
-
-    ctypedef struct mbedtls_ecp_point:
-        _mpi.mbedtls_mpi X
-        _mpi.mbedtls_mpi Y
-        _mpi.mbedtls_mpi Z
-
-    ctypedef struct mbedtls_ecp_group:
-        mbedtls_ecp_group_id id
-        _mpi.mbedtls_mpi P
-        _mpi.mbedtls_mpi A
-        _mpi.mbedtls_mpi B
-        mbedtls_ecp_point G
-        _mpi.mbedtls_mpi N
-        size_t pbits
-        size_t nbits
-        unsigned int h
-        int (*modp)(_mpi.mbedtls_mpi *)
-        int (*t_pre)(mbedtls_ecp_point *, void *)
-        int (*t_post)(mbedtls_ecp_point *, void *)
-        void *t_data
-        mbedtls_ecp_point *T
-        size_t T_size
-
-    ctypedef struct mbedtls_ecp_keypair:
-        mbedtls_ecp_group grp
-        _mpi.mbedtls_mpi d
-        mbedtls_ecp_point Q
-
-    int MBEDTLS_ECP_MAX_BYTES
-    int MBEDTLS_ECP_PF_UNCOMPRESSED
-
-    # Free functions
-    # --------------
-    const mbedtls_ecp_curve_info* mbedtls_ecp_curve_list()
-    # mbedtls_ecp_grp_id_list
-    # mbedtls_ecp_curve_info_from_grp_id
-    # mbedtls_ecp_curve_info_from_tls_id
-    # mbedtls_ecp_curve_info_from_name
-    mbedtls_ecp_curve_type mbedtls_ecp_get_type(
-        const mbedtls_ecp_group *grp
-    )
-
-    # mbedtls_ecp_point
-    # -----------------
-    void mbedtls_ecp_point_init(mbedtls_ecp_point *pt)
-    void mbedtls_ecp_point_free(mbedtls_ecp_point *pt)
-    int mbedtls_ecp_copy(
-        mbedtls_ecp_point *P,
-        const mbedtls_ecp_point *Q)
-    # mbedtls_ecp_set_zero
-    int mbedtls_ecp_is_zero(mbedtls_ecp_point *pt)
-    int mbedtls_ecp_point_cmp(
-        const mbedtls_ecp_point *P,
-        const mbedtls_ecp_point *Q)
-    # mbedtls_ecp_point_read_string
-
-    # mbedtls_ecp_group
-    # -----------------
-    void mbedtls_ecp_group_init(mbedtls_ecp_group *grp)
-    void mbedtls_ecp_group_free(mbedtls_ecp_group *grp)
-    int mbedtls_ecp_group_copy(
-        mbedtls_ecp_group *dst,
-        const mbedtls_ecp_group *src)
-
-    int mbedtls_ecp_point_write_binary(
-        const mbedtls_ecp_group *grp,
-        const mbedtls_ecp_point *P,
-        int format, size_t *olen, unsigned char *buf, size_t buflen)
-    int mbedtls_ecp_point_read_binary(
-        const mbedtls_ecp_group *grp,
-        mbedtls_ecp_point *P,
-        const unsigned char *buf, size_t ilen)
-
-    # mbedtls_ecp_tls_read_point
-    # mbedtls_ecp_tls_write_point
-
-    int mbedtls_ecp_group_load(
-        mbedtls_ecp_group *grp,
-        mbedtls_ecp_group_id index)
-
-    # mbedtls_ecp_tls_read_group
-    # mbedtls_ecp_tls_write_group
-    int mbedtls_ecp_mul(
-        mbedtls_ecp_group *grp,
-        mbedtls_ecp_point *R,
-        const _mpi.mbedtls_mpi *m,
-        const mbedtls_ecp_point *P,
-        int (*f_rng)(void *, unsigned char *, size_t),
-        void *p_rng)
-    # mbedtls_ecp_muladd
-    # mbedtls_ecp_check_pubkey
-    # mbedtls_ecp_check_privkey
-
-    # mbedtls_ecp_keypair
-    # -------------------
-    void mbedtls_ecp_keypair_init(mbedtls_ecp_keypair *key)
-    void mbedtls_ecp_keypair_free(mbedtls_ecp_keypair *key)
-    # mbedtls_ecp_gen_keypair_base
-    int mbedtls_ecp_gen_keypair(
-        mbedtls_ecp_group *grp,
-        _mpi.mbedtls_mpi *d,
-        mbedtls_ecp_point *Q,
-        int (*f_rng)(void *, unsigned char *, size_t),
-        void *p_rng)
-    # mbedtls_ecp_check_pub_priv
-    int mbedtls_ecp_gen_key(
-        mbedtls_ecp_group_id grp_id,
-        mbedtls_ecp_keypair *key,
-        int (*f_rng)(void *, unsigned char *, size_t),
-        void *p_rng)
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2016, Elaborated Networks GmbH
+# Copyright (c) 2018, Mathias Laurin
+
+cimport mbedtls.mpi as _mpi
+
+
+cdef extern from "mbedtls/ecp.h" nogil:
+    ctypedef enum mbedtls_ecp_group_id:
+        MBEDTLS_ECP_DP_NONE = 0,
+        MBEDTLS_ECP_DP_SECP192R1
+        MBEDTLS_ECP_DP_SECP224R1
+        MBEDTLS_ECP_DP_SECP256R1
+        MBEDTLS_ECP_DP_SECP384R1
+        MBEDTLS_ECP_DP_SECP521R1
+        MBEDTLS_ECP_DP_BP256R1
+        MBEDTLS_ECP_DP_BP384R1
+        MBEDTLS_ECP_DP_BP512R1
+        MBEDTLS_ECP_DP_CURVE25519
+        MBEDTLS_ECP_DP_SECP192K1
+        MBEDTLS_ECP_DP_SECP224K1
+        MBEDTLS_ECP_DP_SECP256K1
+        MBEDTLS_ECP_DP_CURVE448
+
+    ctypedef enum mbedtls_ecp_curve_type:
+        MBEDTLS_ECP_TYPE_NONE = 0
+        MBEDTLS_ECP_TYPE_SHORT_WEIERSTRASS
+        MBEDTLS_ECP_TYPE_MONTGOMERY
+
+    ctypedef struct mbedtls_ecp_curve_info:
+        mbedtls_ecp_group_id grp_id
+        int bit_size
+        const char *name
+
+    ctypedef struct mbedtls_ecp_point:
+        _mpi.mbedtls_mpi X
+        _mpi.mbedtls_mpi Y
+        _mpi.mbedtls_mpi Z
+
+    ctypedef struct mbedtls_ecp_group:
+        mbedtls_ecp_group_id id
+        _mpi.mbedtls_mpi P
+        _mpi.mbedtls_mpi A
+        _mpi.mbedtls_mpi B
+        mbedtls_ecp_point G
+        _mpi.mbedtls_mpi N
+        size_t pbits
+        size_t nbits
+        unsigned int h
+        int (*modp)(_mpi.mbedtls_mpi *)
+        int (*t_pre)(mbedtls_ecp_point *, void *)
+        int (*t_post)(mbedtls_ecp_point *, void *)
+        void *t_data
+        mbedtls_ecp_point *T
+        size_t T_size
+
+    ctypedef struct mbedtls_ecp_keypair:
+        mbedtls_ecp_group grp
+        _mpi.mbedtls_mpi d
+        mbedtls_ecp_point Q
+
+    int MBEDTLS_ECP_MAX_BYTES
+    int MBEDTLS_ECP_PF_UNCOMPRESSED
+
+    # Free functions
+    # --------------
+    const mbedtls_ecp_curve_info* mbedtls_ecp_curve_list()
+    # mbedtls_ecp_grp_id_list
+    # mbedtls_ecp_curve_info_from_grp_id
+    # mbedtls_ecp_curve_info_from_tls_id
+    # mbedtls_ecp_curve_info_from_name
+    mbedtls_ecp_curve_type mbedtls_ecp_get_type(
+        const mbedtls_ecp_group *grp
+    )
+
+    # mbedtls_ecp_point
+    # -----------------
+    void mbedtls_ecp_point_init(mbedtls_ecp_point *pt)
+    void mbedtls_ecp_point_free(mbedtls_ecp_point *pt)
+    int mbedtls_ecp_copy(
+        mbedtls_ecp_point *P,
+        const mbedtls_ecp_point *Q)
+    # mbedtls_ecp_set_zero
+    int mbedtls_ecp_is_zero(mbedtls_ecp_point *pt)
+    int mbedtls_ecp_point_cmp(
+        const mbedtls_ecp_point *P,
+        const mbedtls_ecp_point *Q)
+    # mbedtls_ecp_point_read_string
+
+    # mbedtls_ecp_group
+    # -----------------
+    void mbedtls_ecp_group_init(mbedtls_ecp_group *grp)
+    void mbedtls_ecp_group_free(mbedtls_ecp_group *grp)
+    int mbedtls_ecp_group_copy(
+        mbedtls_ecp_group *dst,
+        const mbedtls_ecp_group *src)
+
+    int mbedtls_ecp_point_write_binary(
+        const mbedtls_ecp_group *grp,
+        const mbedtls_ecp_point *P,
+        int format, size_t *olen, unsigned char *buf, size_t buflen)
+    int mbedtls_ecp_point_read_binary(
+        const mbedtls_ecp_group *grp,
+        mbedtls_ecp_point *P,
+        const unsigned char *buf, size_t ilen)
+
+    # mbedtls_ecp_tls_read_point
+    # mbedtls_ecp_tls_write_point
+
+    int mbedtls_ecp_group_load(
+        mbedtls_ecp_group *grp,
+        mbedtls_ecp_group_id index)
+
+    # mbedtls_ecp_tls_read_group
+    # mbedtls_ecp_tls_write_group
+    int mbedtls_ecp_mul(
+        mbedtls_ecp_group *grp,
+        mbedtls_ecp_point *R,
+        const _mpi.mbedtls_mpi *m,
+        const mbedtls_ecp_point *P,
+        int (*f_rng)(void *, unsigned char *, size_t),
+        void *p_rng)
+    # mbedtls_ecp_muladd
+    # mbedtls_ecp_check_pubkey
+    # mbedtls_ecp_check_privkey
+
+    # mbedtls_ecp_keypair
+    # -------------------
+    void mbedtls_ecp_keypair_init(mbedtls_ecp_keypair *key)
+    void mbedtls_ecp_keypair_free(mbedtls_ecp_keypair *key)
+    # mbedtls_ecp_gen_keypair_base
+    int mbedtls_ecp_gen_keypair(
+        mbedtls_ecp_group *grp,
+        _mpi.mbedtls_mpi *d,
+        mbedtls_ecp_point *Q,
+        int (*f_rng)(void *, unsigned char *, size_t),
+        void *p_rng)
+    # mbedtls_ecp_check_pub_priv
+    int mbedtls_ecp_gen_key(
+        mbedtls_ecp_group_id grp_id,
+        mbedtls_ecp_keypair *key,
+        int (*f_rng)(void *, unsigned char *, size_t),
+        void *p_rng)
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/_md.pyi` & `python-mbedtls-2.7.1/src/mbedtls/cipher/_cipher.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,66 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2022, Mathias Laurin
-
-from __future__ import annotations
-
-from typing import Optional, Sequence
-
-algorithms_guaranteed: Sequence[str]
-algorithms_available: Sequence[str]
-
-class Hash:
-    def __init__(
-        self,
-        name: str,
-        buffer: Optional[bytes] = None,
-        *,
-        block_size: int = ...,
-    ) -> None: ...
-    @property
-    def digest_size(self) -> int: ...
-    @property
-    def block_size(self) -> int: ...
-    @property
-    def name(self) -> str: ...
-    def update(self, buffer: bytes) -> None: ...
-    def digest(self) -> bytes: ...
-    def hexdigest(self) -> str: ...
-    def copy(self) -> Hash: ...
-
-class Hmac:
-    def __init__(
-        self,
-        key: bytes,
-        name: str,
-        buffer: Optional[bytes] = None,
-        *,
-        block_size: int,
-    ) -> None: ...
-    @property
-    def digest_size(self) -> int: ...
-    @property
-    def block_size(self) -> int: ...
-    @property
-    def name(self) -> str: ...
-    def update(self, buffer: bytes) -> None: ...
-    def digest(self) -> bytes: ...
-    def hexdigest(self) -> str: ...
-    def copy(self) -> Hmac: ...
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2022, Mathias Laurin
+
+from __future__ import annotations
+
+import enum
+from typing import Sequence, Optional, Tuple
+
+def get_supported_ciphers() -> Sequence[bytes]: ...
+
+class Mode(enum.Enum):
+    ECB: int
+    CBC: int
+    CFB: int
+    OFB: int
+    CTR: int
+    GCM: int
+    STREAM: int
+    CCM: int
+    XTS: int
+    CHACHAPOLY: int
+
+class Cipher:
+    def __init__(
+        self, cipher_name: bytes, key: bytes, mode: Mode, iv: Optional[bytes]
+    ) -> None: ...
+    def __str__(self) -> str: ...
+    @property
+    def block_size(self) -> int: ...
+    @property
+    def mode(self) -> Mode: ...
+    @property
+    def iv_size(self) -> int: ...
+    @property
+    def _type(self) -> bytes: ...
+    @property
+    def name(self) -> bytes: ...
+    @property
+    def key_size(self) -> int: ...
+    def encrypt(self, message: bytes) -> bytes: ...
+    def decrypt(self, message: bytes) -> bytes: ...
+
+class AEADCipher:
+    def __init__(
+        self,
+        cipher_name: bytes,
+        key: bytes,
+        mode: Mode,
+        iv: Optional[bytes],
+        ad: Optional[bytes],
+    ) -> None: ...
+    def __str__(self) -> str: ...
+    @property
+    def block_size(self) -> int: ...
+    @property
+    def mode(self) -> Mode: ...
+    @property
+    def iv_size(self) -> int: ...
+    @property
+    def _type(self) -> bytes: ...
+    @property
+    def name(self) -> bytes: ...
+    @property
+    def key_size(self) -> int: ...
+    def encrypt(self, message: bytes) -> Tuple[bytes, bytes]: ...
+    def decrypt(self, message: bytes, tag: bytes) -> bytes: ...
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/_random.pyi` & `python-mbedtls-2.7.1/src/mbedtls/_random.pyi`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2022, Mathias Laurin
-
-from __future__ import annotations
-
-from typing import NoReturn, Optional, Sequence, TypeVar
-
-T_co = TypeVar("T_co", covariant=True)
-
-class _Entropy:
-    def __init__(self) -> None: ...
-    def __getstate__(self) -> NoReturn: ...
-    def gather(self) -> None: ...
-    def retrieve(self, __length: int) -> bytes: ...
-    def update(self, __data: bytes) -> None: ...
-
-class Random:
-    _entropy: _Entropy
-    def __init__(self) -> None: ...
-    def __getstate__(self) -> NoReturn: ...
-    def _reseed(self, __data: Optional[bytes] = None) -> None: ...
-    def urandom(self, __length: int) -> None: ...
-    def randbelow(self, upper_bound: int) -> int: ...
-    def random(self) -> float: ...
-    def getrandbits(self, __k: int) -> int: ...
-    def choice(self, __seq: Sequence[T_co]) -> T_co: ...
-
-def default_rng() -> Random: ...
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2022, Mathias Laurin
+
+from __future__ import annotations
+
+from typing import NoReturn, Optional, Sequence, TypeVar
+
+T_co = TypeVar("T_co", covariant=True)
+
+class _Entropy:
+    def __init__(self) -> None: ...
+    def __getstate__(self) -> NoReturn: ...
+    def gather(self) -> None: ...
+    def retrieve(self, __length: int) -> bytes: ...
+    def update(self, __data: bytes) -> None: ...
+
+class Random:
+    _entropy: _Entropy
+    def __init__(self) -> None: ...
+    def __getstate__(self) -> NoReturn: ...
+    def _reseed(self, __data: Optional[bytes] = None) -> None: ...
+    def urandom(self, __length: int) -> None: ...
+    def randbelow(self, upper_bound: int) -> int: ...
+    def random(self) -> float: ...
+    def getrandbits(self, __k: int) -> int: ...
+    def choice(self, __seq: Sequence[T_co]) -> T_co: ...
+
+def default_rng() -> Random: ...
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/_random.pyx` & `python-mbedtls-2.7.1/src/mbedtls/_random.pyx`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,160 +1,160 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2016, Elaborated Networks GmbH
-# Copyright (c) 2019, Mathias Laurin
-
-"""Random number generator (RNG) wrapper."""
-
-
-from libc.stdlib cimport free, malloc
-
-cimport mbedtls._platform as _plt
-cimport mbedtls._random as _rnd
-
-import numbers as _numbers
-
-import mbedtls.mpi as _mpi
-from mbedtls.exceptions import check_error
-
-BPF = 53  # Number of bits in a float
-RECIP_BPF = 2**-BPF
-
-
-cdef class _Entropy:
-    def __cinit__(self):
-        """Initialize the context."""
-        _rnd.mbedtls_entropy_init(&self._ctx)
-
-    def __dealloc__(self):
-        """Free and clear the context."""
-        _rnd.mbedtls_entropy_free(&self._ctx)
-
-    def __getstate__(self):
-        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
-
-    def gather(self):
-        """Trigger an extra gather poll for the accumulator."""
-        _rnd.mbedtls_entropy_gather(&self._ctx)
-
-    def retrieve(self, size_t length):
-        """Retrieve entropy from the accumulator."""
-        cdef unsigned char *output = <unsigned char *> malloc(
-            length * sizeof(unsigned char)
-        )
-        if not output:
-            raise MemoryError()
-        try:
-            check_error(_rnd.mbedtls_entropy_func(&self._ctx, output, length))
-            return output[:length]
-        finally:
-            free(output)
-
-    def update(self, const unsigned char[:] data):
-        """Add data to the accumulator manually."""
-        check_error(
-            _rnd.mbedtls_entropy_update_manual(
-                &self._ctx, &data[0], data.shape[0]
-            )
-        )
-
-
-cdef class Random:
-    def __init__(self):
-        self._entropy = _Entropy()
-        check_error(
-            _rnd.mbedtls_ctr_drbg_seed(
-                &self._ctx,
-                &_rnd.mbedtls_entropy_func,
-                &self._entropy._ctx,
-                NULL, 0
-            )
-        )
-
-    def __cinit__(self):
-        """Initialize the context."""
-        _rnd.mbedtls_ctr_drbg_init(&self._ctx)
-
-    def __dealloc__(self):
-        """Free and clear the context."""
-        _rnd.mbedtls_ctr_drbg_free(&self._ctx)
-
-    def __getstate__(self):
-        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
-
-    @property
-    def _entropy(self):
-        return self._entropy
-
-    def _reseed(self, const unsigned char[:] data=None):
-        """Reseed the RNG."""
-        if data is None:
-            check_error(_rnd.mbedtls_ctr_drbg_reseed(&self._ctx, NULL, 0))
-        else:
-            check_error(
-                _rnd.mbedtls_ctr_drbg_reseed(&self._ctx, &data[0], data.size)
-            )
-
-    def urandom(self, size_t length):
-        """Returns `length` random bytes."""
-        cdef unsigned char *output = <unsigned char *> malloc(
-            length * sizeof(unsigned char)
-        )
-        if not output:
-            raise MemoryError()
-        try:
-            check_error(
-                _rnd.mbedtls_ctr_drbg_random(&self._ctx, output, length)
-            )
-            ret = output[:length]
-            _plt.mbedtls_platform_zeroize(output, length)
-            return ret
-        finally:
-            free(output)
-
-    def randbelow(self, upper_bound):
-        """Return a random int in the range [0, n).
-
-        Raises ValueError if n <= 0.
-
-        """
-        if upper_bound <= 0:
-            raise ValueError("Upper bound must be positive.")
-        kk = upper_bound.bit_length()
-        rr = self.getrandbits(kk)
-        while rr >= upper_bound:
-            rr = self.getrandbits(kk)
-        return rr
-
-    def random(self):
-        """Return the next random floating point number."""
-        # Algorithm taken from Python's secrets and random libraries.
-        return float(
-            _mpi.MPI.from_bytes(self.urandom(7), "big") >> 3
-        ) * RECIP_BPF
-
-    def getrandbits(self, k):
-        """Generate an int with `k` random bits."""
-        # Algorithm adapted from Python's secrets and random libraries.
-        if k <= 0:
-            raise ValueError("number of bits must be greater than zero")
-        if not isinstance(k, _numbers.Integral):
-            raise TypeError("number of bits should be an integer")
-        numbytes = (k + 7) // 8
-        value = _mpi.MPI.from_bytes(self.urandom(numbytes), "big")
-        # Trim excess bits:
-        extra_bits = value.bit_length() - k
-        return value >> (0 if extra_bits <= 0 else extra_bits)
-
-    def choice(self, seq):
-        """Return a random element from `seq`."""
-        try:
-            ii = self.randbelow(len(seq))
-        except ValueError:
-            raise IndexError("Cannot choose from an empty sequence")
-        return seq[ii]
-
-
-cdef Random __rng = Random()
-
-
-cpdef Random default_rng():
-    return __rng
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2016, Elaborated Networks GmbH
+# Copyright (c) 2019, Mathias Laurin
+
+"""Random number generator (RNG) wrapper."""
+
+
+from libc.stdlib cimport free, malloc
+
+cimport mbedtls._platform as _plt
+cimport mbedtls._random as _rnd
+
+import numbers as _numbers
+
+import mbedtls.mpi as _mpi
+from mbedtls.exceptions import check_error
+
+BPF = 53  # Number of bits in a float
+RECIP_BPF = 2**-BPF
+
+
+cdef class _Entropy:
+    def __cinit__(self):
+        """Initialize the context."""
+        _rnd.mbedtls_entropy_init(&self._ctx)
+
+    def __dealloc__(self):
+        """Free and clear the context."""
+        _rnd.mbedtls_entropy_free(&self._ctx)
+
+    def __getstate__(self):
+        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
+
+    def gather(self):
+        """Trigger an extra gather poll for the accumulator."""
+        _rnd.mbedtls_entropy_gather(&self._ctx)
+
+    def retrieve(self, size_t length):
+        """Retrieve entropy from the accumulator."""
+        cdef unsigned char *output = <unsigned char *> malloc(
+            length * sizeof(unsigned char)
+        )
+        if not output:
+            raise MemoryError()
+        try:
+            check_error(_rnd.mbedtls_entropy_func(&self._ctx, output, length))
+            return output[:length]
+        finally:
+            free(output)
+
+    def update(self, const unsigned char[:] data):
+        """Add data to the accumulator manually."""
+        check_error(
+            _rnd.mbedtls_entropy_update_manual(
+                &self._ctx, &data[0], data.shape[0]
+            )
+        )
+
+
+cdef class Random:
+    def __init__(self):
+        self._entropy = _Entropy()
+        check_error(
+            _rnd.mbedtls_ctr_drbg_seed(
+                &self._ctx,
+                &_rnd.mbedtls_entropy_func,
+                &self._entropy._ctx,
+                NULL, 0
+            )
+        )
+
+    def __cinit__(self):
+        """Initialize the context."""
+        _rnd.mbedtls_ctr_drbg_init(&self._ctx)
+
+    def __dealloc__(self):
+        """Free and clear the context."""
+        _rnd.mbedtls_ctr_drbg_free(&self._ctx)
+
+    def __getstate__(self):
+        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
+
+    @property
+    def _entropy(self):
+        return self._entropy
+
+    def _reseed(self, const unsigned char[:] data=None):
+        """Reseed the RNG."""
+        if data is None:
+            check_error(_rnd.mbedtls_ctr_drbg_reseed(&self._ctx, NULL, 0))
+        else:
+            check_error(
+                _rnd.mbedtls_ctr_drbg_reseed(&self._ctx, &data[0], data.size)
+            )
+
+    def urandom(self, size_t length):
+        """Returns `length` random bytes."""
+        cdef unsigned char *output = <unsigned char *> malloc(
+            length * sizeof(unsigned char)
+        )
+        if not output:
+            raise MemoryError()
+        try:
+            check_error(
+                _rnd.mbedtls_ctr_drbg_random(&self._ctx, output, length)
+            )
+            ret = output[:length]
+            _plt.mbedtls_platform_zeroize(output, length)
+            return ret
+        finally:
+            free(output)
+
+    def randbelow(self, upper_bound):
+        """Return a random int in the range [0, n).
+
+        Raises ValueError if n <= 0.
+
+        """
+        if upper_bound <= 0:
+            raise ValueError("Upper bound must be positive.")
+        kk = upper_bound.bit_length()
+        rr = self.getrandbits(kk)
+        while rr >= upper_bound:
+            rr = self.getrandbits(kk)
+        return rr
+
+    def random(self):
+        """Return the next random floating point number."""
+        # Algorithm taken from Python's secrets and random libraries.
+        return float(
+            _mpi.MPI.from_bytes(self.urandom(7), "big") >> 3
+        ) * RECIP_BPF
+
+    def getrandbits(self, k):
+        """Generate an int with `k` random bits."""
+        # Algorithm adapted from Python's secrets and random libraries.
+        if k <= 0:
+            raise ValueError("number of bits must be greater than zero")
+        if not isinstance(k, _numbers.Integral):
+            raise TypeError("number of bits should be an integer")
+        numbytes = (k + 7) // 8
+        value = _mpi.MPI.from_bytes(self.urandom(numbytes), "big")
+        # Trim excess bits:
+        extra_bits = value.bit_length() - k
+        return value >> (0 if extra_bits <= 0 else extra_bits)
+
+    def choice(self, seq):
+        """Return a random element from `seq`."""
+        try:
+            ii = self.randbelow(len(seq))
+        except ValueError:
+            raise IndexError("Cannot choose from an empty sequence")
+        return seq[ii]
+
+
+cdef Random __rng = Random()
+
+
+cpdef Random default_rng():
+    return __rng
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/_ringbuf.pxd` & `python-mbedtls-2.7.1/src/mbedtls/_ringbuf.pxd`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2018, Mathias Laurin
-
-"""A ring buffer.
-
-See Also:
-    https://github.com/dhess/c-ringbuf/
-
-"""
-
-
-cdef struct ring_buffer_ctx:
-    unsigned char *buf
-    unsigned char *head
-    unsigned char *tail
-    size_t _size
-
-
-cdef c_init(ring_buffer_ctx *, size_t)
-cdef void c_free(ring_buffer_ctx *) nogil
-cdef void c_clear(ring_buffer_ctx *) nogil
-cdef size_t c_capacity(ring_buffer_ctx *) nogil
-cdef size_t c_len(ring_buffer_ctx *) nogil
-cdef c_peek(ring_buffer_ctx *, size_t)
-cdef size_t c_peekinto(ring_buffer_ctx *, unsigned char *, size_t) nogil
-cdef c_read(ring_buffer_ctx *, size_t)
-cdef size_t c_readinto(ring_buffer_ctx *, unsigned char *, size_t) nogil
-cdef size_t c_consume(ring_buffer_ctx *, size_t) nogil
-cdef size_t c_write(ring_buffer_ctx *, const unsigned char *, size_t) nogil
-
-
-cdef class RingBuffer:
-    cdef ring_buffer_ctx _ctx
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2018, Mathias Laurin
+
+"""A ring buffer.
+
+See Also:
+    https://github.com/dhess/c-ringbuf/
+
+"""
+
+
+cdef struct ring_buffer_ctx:
+    unsigned char *buf
+    unsigned char *head
+    unsigned char *tail
+    size_t _size
+
+
+cdef c_init(ring_buffer_ctx *, size_t)
+cdef void c_free(ring_buffer_ctx *) nogil
+cdef void c_clear(ring_buffer_ctx *) nogil
+cdef size_t c_capacity(ring_buffer_ctx *) nogil
+cdef size_t c_len(ring_buffer_ctx *) nogil
+cdef c_peek(ring_buffer_ctx *, size_t)
+cdef size_t c_peekinto(ring_buffer_ctx *, unsigned char *, size_t) nogil
+cdef c_read(ring_buffer_ctx *, size_t)
+cdef size_t c_readinto(ring_buffer_ctx *, unsigned char *, size_t) nogil
+cdef size_t c_consume(ring_buffer_ctx *, size_t) nogil
+cdef size_t c_write(ring_buffer_ctx *, const unsigned char *, size_t) nogil
+
+
+cdef class RingBuffer:
+    cdef ring_buffer_ctx _ctx
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/_ringbuf.pyx` & `python-mbedtls-2.7.1/src/mbedtls/_ringbuf.pyx`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,215 +1,215 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2018, Mathias Laurin
-
-"""A ring buffer.
-
-See Also:
-    https://github.com/dhess/c-ringbuf/ Drew Hess' ring
-    buffer C implementation was a great help in the
-    development of this module.
-
-"""
-
-
-from libc.stdlib cimport free, malloc
-from libc.string cimport memcpy
-
-cimport mbedtls._ringbuf as _rb
-
-import cython
-
-
-cdef c_init(_rb.ring_buffer_ctx *ctx, size_t maxlen):
-    # ringbuf_new()
-    ctx._size = maxlen + 1
-    ctx.buf = <unsigned char *>malloc(ctx._size * sizeof(unsigned char))
-    if not ctx.buf:
-        raise MemoryError()
-    ctx.head = ctx.tail = ctx.buf
-
-
-cdef void c_free(_rb.ring_buffer_ctx *ctx) nogil:
-    # ringbuf_free()
-    free(ctx.buf)
-    ctx.head = ctx.tail = NULL
-
-
-cdef void c_clear(_rb.ring_buffer_ctx *ctx) nogil:
-    # ringbuf_reset()
-    ctx.head = ctx.tail
-
-
-cdef size_t c_capacity(_rb.ring_buffer_ctx *ctx) nogil:
-    # ringbuf_capacity()
-    return ctx._size - 1
-
-
-cdef unsigned char * c_end(ring_buffer_ctx * ctx) nogil:
-    # ringbuf_end()
-    return &ctx.buf[ctx._size]
-
-
-cdef size_t c_len(ring_buffer_ctx *ctx) nogil:
-    # ringbuf_bytes_used()
-    if ctx.head >= ctx.tail:
-        return ctx.head - ctx.tail
-    else:
-        return c_capacity(ctx) - (ctx.tail - ctx.head - 1)
-
-
-cdef c_peek(ring_buffer_ctx *ctx, size_t amt):
-    cdef unsigned char *dst = <unsigned char *>malloc(
-        min(amt, c_len(ctx) * sizeof(unsigned char)))
-    if not dst:
-        raise MemoryError()
-    try:
-        nread = c_peekinto(ctx, dst, amt)
-        return bytes(dst[:nread])
-    finally:
-        free(dst)
-
-
-@cython.boundscheck(False)
-cdef size_t c_peekinto(
-        ring_buffer_ctx *ctx, unsigned char *dst, size_t amt) nogil:
-    cdef size_t size = min(amt, c_len(ctx))
-    cdef size_t nread = 0
-    cdef unsigned char * index = ctx.tail
-    while nread != size:
-        if index == c_end(ctx):
-            index = ctx.buf
-
-        amt = min(<size_t>(c_end(ctx) - index), size - nread)
-        memcpy(&dst[nread], index, amt)
-        index += amt
-        nread += amt
-
-    return nread
-
-
-cdef c_read(ring_buffer_ctx *ctx, size_t amt):
-    cdef unsigned char *dst = <unsigned char *>malloc(
-        min(amt, c_len(ctx)) * sizeof(unsigned char))
-    if not dst:
-        raise MemoryError()
-    try:
-        nread = c_readinto(ctx, dst, amt)
-        return bytes(dst[:nread])
-    finally:
-        free(dst)
-
-
-@cython.boundscheck(False)
-cdef size_t c_readinto(
-        ring_buffer_ctx *ctx, unsigned char *dst, size_t amt) nogil:
-    # ringbuf_memcpy_from()
-    cdef size_t size = min(amt, c_len(ctx))
-    cdef size_t nread = 0
-    while nread != size:
-        if ctx.tail == c_end(ctx):
-            ctx.tail = ctx.buf
-
-        amt = min(<size_t>(c_end(ctx) - ctx.tail), size - nread)
-        memcpy(&dst[nread], ctx.tail, amt)
-        ctx.tail += amt
-        nread += amt
-
-    return nread
-
-
-cdef size_t c_consume(ring_buffer_ctx *ctx, size_t amt) nogil:
-    cdef size_t size = min(amt, c_len(ctx))
-    cdef size_t nconsumed = 0
-    while nconsumed != size:
-        if ctx.tail == c_end(ctx):
-            ctx.tail = ctx.buf
-
-        amt = min(<size_t>(c_end(ctx) - ctx.tail), size - nconsumed)
-        ctx.tail += amt
-        nconsumed += amt
-
-    return nconsumed
-
-
-@cython.boundscheck(False)
-cdef size_t c_write(
-        ring_buffer_ctx *ctx, const unsigned char *src, size_t amt) nogil:
-    # ringbuf_memcpy_into()
-    cdef size_t size = amt
-    # if size > c_capacity(ctx) - c_len(ctx):
-    #     raise BufferError("Buffer overflow")
-
-    cdef size_t nwritten = 0
-    while nwritten != size:
-        if ctx.head == c_end(ctx):
-            ctx.head = ctx.buf
-
-        amt = min(<size_t>(c_end(ctx) - ctx.head), size - nwritten)
-        memcpy(ctx.head, &src[nwritten], amt)
-        ctx.head += amt
-        nwritten += amt
-
-    return nwritten
-
-
-cdef class RingBuffer:
-    def __init__(self, size_t maxlen, content=b""):
-        self.write(content)
-
-    def __cinit__(self, size_t maxlen, content=b""):
-        c_init(&self._ctx, maxlen)
-
-    def __dealloc__(self):
-        c_free(&self._ctx)
-
-    def __reduce__(self):
-        return type(self), (self.maxlen, self.__bytes__())
-
-    @property
-    def maxlen(self):
-        return c_capacity(&self._ctx)
-
-    def __eq__(self, other):
-        # Call `__bytes__()` directly for Python 2.7.
-        try:
-            return self.__bytes__() == other.__bytes__()
-        except AttributeError:
-            return self.__bytes__() == bytes(other)
-
-    def __len__(self):
-        return c_len(&self._ctx)
-
-    def __bool__(self):
-        return not self.empty()
-
-    def __bytes__(self):
-        return self.peek(len(self))
-
-    def clear(self):
-        c_clear(&self._ctx)
-
-    def full(self):
-        return len(self) == self.maxlen
-
-    def empty(self):
-        return len(self) == 0
-
-    def peek(self, size_t amt):
-        return c_peek(&self._ctx, amt)
-
-    def read(self, size_t amt):
-        return c_read(&self._ctx, amt)
-
-    def consume(self, size_t amt):
-        return c_consume(&self._ctx, amt)
-
-    def write(self, const unsigned char[:] src not None, amt=None):
-        if src.size == 0:
-            return 0
-        if amt is None:
-            amt = src.size
-        else:
-            amt = min(src.size, amt)
-        if amt > self.maxlen - len(self):
-            raise BufferError("Buffer overflow")
-        return c_write(&self._ctx, &src[0], amt)
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2018, Mathias Laurin
+
+"""A ring buffer.
+
+See Also:
+    https://github.com/dhess/c-ringbuf/ Drew Hess' ring
+    buffer C implementation was a great help in the
+    development of this module.
+
+"""
+
+
+from libc.stdlib cimport free, malloc
+from libc.string cimport memcpy
+
+cimport mbedtls._ringbuf as _rb
+
+import cython
+
+
+cdef c_init(_rb.ring_buffer_ctx *ctx, size_t maxlen):
+    # ringbuf_new()
+    ctx._size = maxlen + 1
+    ctx.buf = <unsigned char *>malloc(ctx._size * sizeof(unsigned char))
+    if not ctx.buf:
+        raise MemoryError()
+    ctx.head = ctx.tail = ctx.buf
+
+
+cdef void c_free(_rb.ring_buffer_ctx *ctx) nogil:
+    # ringbuf_free()
+    free(ctx.buf)
+    ctx.head = ctx.tail = NULL
+
+
+cdef void c_clear(_rb.ring_buffer_ctx *ctx) nogil:
+    # ringbuf_reset()
+    ctx.head = ctx.tail
+
+
+cdef size_t c_capacity(_rb.ring_buffer_ctx *ctx) nogil:
+    # ringbuf_capacity()
+    return ctx._size - 1
+
+
+cdef unsigned char * c_end(ring_buffer_ctx * ctx) nogil:
+    # ringbuf_end()
+    return &ctx.buf[ctx._size]
+
+
+cdef size_t c_len(ring_buffer_ctx *ctx) nogil:
+    # ringbuf_bytes_used()
+    if ctx.head >= ctx.tail:
+        return ctx.head - ctx.tail
+    else:
+        return c_capacity(ctx) - (ctx.tail - ctx.head - 1)
+
+
+cdef c_peek(ring_buffer_ctx *ctx, size_t amt):
+    cdef unsigned char *dst = <unsigned char *>malloc(
+        min(amt, c_len(ctx) * sizeof(unsigned char)))
+    if not dst:
+        raise MemoryError()
+    try:
+        nread = c_peekinto(ctx, dst, amt)
+        return bytes(dst[:nread])
+    finally:
+        free(dst)
+
+
+@cython.boundscheck(False)
+cdef size_t c_peekinto(
+        ring_buffer_ctx *ctx, unsigned char *dst, size_t amt) nogil:
+    cdef size_t size = min(amt, c_len(ctx))
+    cdef size_t nread = 0
+    cdef unsigned char * index = ctx.tail
+    while nread != size:
+        if index == c_end(ctx):
+            index = ctx.buf
+
+        amt = min(<size_t>(c_end(ctx) - index), size - nread)
+        memcpy(&dst[nread], index, amt)
+        index += amt
+        nread += amt
+
+    return nread
+
+
+cdef c_read(ring_buffer_ctx *ctx, size_t amt):
+    cdef unsigned char *dst = <unsigned char *>malloc(
+        min(amt, c_len(ctx)) * sizeof(unsigned char))
+    if not dst:
+        raise MemoryError()
+    try:
+        nread = c_readinto(ctx, dst, amt)
+        return bytes(dst[:nread])
+    finally:
+        free(dst)
+
+
+@cython.boundscheck(False)
+cdef size_t c_readinto(
+        ring_buffer_ctx *ctx, unsigned char *dst, size_t amt) nogil:
+    # ringbuf_memcpy_from()
+    cdef size_t size = min(amt, c_len(ctx))
+    cdef size_t nread = 0
+    while nread != size:
+        if ctx.tail == c_end(ctx):
+            ctx.tail = ctx.buf
+
+        amt = min(<size_t>(c_end(ctx) - ctx.tail), size - nread)
+        memcpy(&dst[nread], ctx.tail, amt)
+        ctx.tail += amt
+        nread += amt
+
+    return nread
+
+
+cdef size_t c_consume(ring_buffer_ctx *ctx, size_t amt) nogil:
+    cdef size_t size = min(amt, c_len(ctx))
+    cdef size_t nconsumed = 0
+    while nconsumed != size:
+        if ctx.tail == c_end(ctx):
+            ctx.tail = ctx.buf
+
+        amt = min(<size_t>(c_end(ctx) - ctx.tail), size - nconsumed)
+        ctx.tail += amt
+        nconsumed += amt
+
+    return nconsumed
+
+
+@cython.boundscheck(False)
+cdef size_t c_write(
+        ring_buffer_ctx *ctx, const unsigned char *src, size_t amt) nogil:
+    # ringbuf_memcpy_into()
+    cdef size_t size = amt
+    # if size > c_capacity(ctx) - c_len(ctx):
+    #     raise BufferError("Buffer overflow")
+
+    cdef size_t nwritten = 0
+    while nwritten != size:
+        if ctx.head == c_end(ctx):
+            ctx.head = ctx.buf
+
+        amt = min(<size_t>(c_end(ctx) - ctx.head), size - nwritten)
+        memcpy(ctx.head, &src[nwritten], amt)
+        ctx.head += amt
+        nwritten += amt
+
+    return nwritten
+
+
+cdef class RingBuffer:
+    def __init__(self, size_t maxlen, content=b""):
+        self.write(content)
+
+    def __cinit__(self, size_t maxlen, content=b""):
+        c_init(&self._ctx, maxlen)
+
+    def __dealloc__(self):
+        c_free(&self._ctx)
+
+    def __reduce__(self):
+        return type(self), (self.maxlen, self.__bytes__())
+
+    @property
+    def maxlen(self):
+        return c_capacity(&self._ctx)
+
+    def __eq__(self, other):
+        # Call `__bytes__()` directly for Python 2.7.
+        try:
+            return self.__bytes__() == other.__bytes__()
+        except AttributeError:
+            return self.__bytes__() == bytes(other)
+
+    def __len__(self):
+        return c_len(&self._ctx)
+
+    def __bool__(self):
+        return not self.empty()
+
+    def __bytes__(self):
+        return self.peek(len(self))
+
+    def clear(self):
+        c_clear(&self._ctx)
+
+    def full(self):
+        return len(self) == self.maxlen
+
+    def empty(self):
+        return len(self) == 0
+
+    def peek(self, size_t amt):
+        return c_peek(&self._ctx, amt)
+
+    def read(self, size_t amt):
+        return c_read(&self._ctx, amt)
+
+    def consume(self, size_t amt):
+        return c_consume(&self._ctx, amt)
+
+    def write(self, const unsigned char[:] src not None, amt=None):
+        if src.size == 0:
+            return 0
+        if amt is None:
+            amt = src.size
+        else:
+            amt = min(src.size, amt)
+        if amt > self.maxlen - len(self):
+            raise BufferError("Buffer overflow")
+        return c_write(&self._ctx, &src[0], amt)
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/_rsa.pxd` & `python-mbedtls-2.7.1/src/mbedtls/_rsa.pxd`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2016, Elaborated Networks GmbH
-# Copyright (c) 2018, Mathias Laurin
-
-cdef extern from "mbedtls/rsa.h" nogil:
-    ctypedef struct mbedtls_rsa_context:
-        pass
-
-    # mbedtls_rsa_context
-    # -------------------
-    # mbedtls_rsa_init
-    # mbedtls_rsa_set_padding
-    int mbedtls_rsa_gen_key(
-        mbedtls_rsa_context *ctx,
-        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng,
-        unsigned int nbits, int exponent)
-    int mbedtls_rsa_check_pubkey(const mbedtls_rsa_context *ctx)
-    int mbedtls_rsa_check_privkey(const mbedtls_rsa_context *ctx)
-    # mbedtls_rsa_check_pub_priv
-    # mbedtls_rsa_public
-    # mbedtls_rsa_private
-    # mbedtls_rsa_pkcs1_encrypt
-    # mbedtls_rsa_rsaes_pkcs1_v15_encrypt
-    # mbedtls_rsa_rsaes_oaep_encrypt
-    # mbedtls_rsa_pkcs1_decrypt
-    # mbedtls_rsa_rsaes_pkcs1_v15_decrypt
-    # mbedtls_rsa_rsaes_oaep_decrypt
-    # mbedtls_rsa_pkcs1_sign
-    # mbedtls_rsa_rsassa_pkcs1_v15_sign
-    # mbedtls_rsa_rsassa_pss_sign
-    # mbedtls_rsa_pkcs1_verify
-    # mbedtls_rsa_rsassa_pkcs1_v15_verify
-    # mbedtls_rsa_rsassa_pss_verify
-    # mbedtls_rsa_rsassa_pss_verify_ext
-    # mbedtls_rsa_copy
-    # mbedtls_rsa_free
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2016, Elaborated Networks GmbH
+# Copyright (c) 2018, Mathias Laurin
+
+cdef extern from "mbedtls/rsa.h" nogil:
+    ctypedef struct mbedtls_rsa_context:
+        pass
+
+    # mbedtls_rsa_context
+    # -------------------
+    # mbedtls_rsa_init
+    # mbedtls_rsa_set_padding
+    int mbedtls_rsa_gen_key(
+        mbedtls_rsa_context *ctx,
+        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng,
+        unsigned int nbits, int exponent)
+    int mbedtls_rsa_check_pubkey(const mbedtls_rsa_context *ctx)
+    int mbedtls_rsa_check_privkey(const mbedtls_rsa_context *ctx)
+    # mbedtls_rsa_check_pub_priv
+    # mbedtls_rsa_public
+    # mbedtls_rsa_private
+    # mbedtls_rsa_pkcs1_encrypt
+    # mbedtls_rsa_rsaes_pkcs1_v15_encrypt
+    # mbedtls_rsa_rsaes_oaep_encrypt
+    # mbedtls_rsa_pkcs1_decrypt
+    # mbedtls_rsa_rsaes_pkcs1_v15_decrypt
+    # mbedtls_rsa_rsaes_oaep_decrypt
+    # mbedtls_rsa_pkcs1_sign
+    # mbedtls_rsa_rsassa_pkcs1_v15_sign
+    # mbedtls_rsa_rsassa_pss_sign
+    # mbedtls_rsa_pkcs1_verify
+    # mbedtls_rsa_rsassa_pkcs1_v15_verify
+    # mbedtls_rsa_rsassa_pss_verify
+    # mbedtls_rsa_rsassa_pss_verify_ext
+    # mbedtls_rsa_copy
+    # mbedtls_rsa_free
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/_timing.pxd` & `python-mbedtls-2.7.1/src/mbedtls/_timing.pxd`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2018, Mathias Laurin
-
-cdef extern from "mbedtls/timing.h" nogil:
-    # This provides callbacks for DTLS with blocking IO.
-
-    ctypedef struct mbedtls_timing_hr_time:
-        pass
-
-    ctypedef struct mbedtls_timing_delay_context:
-        mbedtls_timing_hr_time timer
-        int int_ms
-        int fin_ms
-
-    # extern volatile int mbedtls_timing_alarmed
-
-    # unsigned long mbedtls_timing_hardclock()
-    # unsigned long mbedtls_timing_get_timer(
-    #     mbedtls_timing_hr_time *,
-    #     int reset,
-    # )
-    # void mbedtls_set_alarm(int seconds)
-
-    # mbedtls_ssl_set_timer_t callback
-    void mbedtls_timing_set_delay(void *data, int int_ms, int fin_ms)
-    # mbedtls_ssl_get_timer_t callback
-    int mbedtls_timing_get_delay(void *data)
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2018, Mathias Laurin
+
+cdef extern from "mbedtls/timing.h" nogil:
+    # This provides callbacks for DTLS with blocking IO.
+
+    ctypedef struct mbedtls_timing_hr_time:
+        pass
+
+    ctypedef struct mbedtls_timing_delay_context:
+        mbedtls_timing_hr_time timer
+        int int_ms
+        int fin_ms
+
+    # extern volatile int mbedtls_timing_alarmed
+
+    # unsigned long mbedtls_timing_hardclock()
+    # unsigned long mbedtls_timing_get_timer(
+    #     mbedtls_timing_hr_time *,
+    #     int reset,
+    # )
+    # void mbedtls_set_alarm(int seconds)
+
+    # mbedtls_ssl_set_timer_t callback
+    void mbedtls_timing_set_delay(void *data, int int_ms, int fin_ms)
+    # mbedtls_ssl_get_timer_t callback
+    int mbedtls_timing_get_delay(void *data)
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/_tls.pxd` & `python-mbedtls-2.7.1/src/mbedtls/_tls.pxd`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,456 +1,456 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2018, Mathias Laurin
-
-from libc.stdint cimport uint16_t
-
-cimport mbedtls._ecdh as _ecdh
-cimport mbedtls._ringbuf as _rb
-cimport mbedtls._timing as _timing
-cimport mbedtls.pk as _pk
-cimport mbedtls.x509 as _x509
-
-cdef:
-    enum:
-        MBEDTLS_SSL_TRANSPORT_STREAM = 0
-        MBEDTLS_SSL_TRANSPORT_DATAGRAM = 1
-
-    enum:
-        MBEDTLS_SSL_PRESET_DEFAULT = 0
-        MBEDTLS_SSL_PRESET_SUITEB = 2
-
-    enum:
-        MBEDTLS_SSL_VERIFY_NONE = 0
-        MBEDTLS_SSL_VERIFY_OPTIONAL = 1
-        MBEDTLS_SSL_VERIFY_REQUIRED = 2
-
-    enum:
-        MBEDTLS_SSL_ANTI_REPLAY_DISABLED = 0
-        MBEDTLS_SSL_ANTI_REPLAY_ENABLED = 1
-
-    enum:
-        # Message type
-        MBEDTLS_SSL_MSG_CHANGE_CIPHER_SPEC = 20  # 0x14
-        MBEDTLS_SSL_MSG_ALERT = 21      # 0x15
-        MBEDTLS_SSL_MSG_HANDSHAKE = 22  # 0x16
-        MBEDTLS_SSL_MSG_APPLICATION_DATA = 23  # 0x17
-
-    enum:
-        MBEDTLS_SSL_HELLO_REQUEST
-        MBEDTLS_SSL_CLIENT_HELLO
-        MBEDTLS_SSL_SERVER_HELLO
-        MBEDTLS_SSL_SERVER_CERTIFICATE
-        MBEDTLS_SSL_SERVER_KEY_EXCHANGE
-        MBEDTLS_SSL_CERTIFICATE_REQUEST
-        MBEDTLS_SSL_SERVER_HELLO_DONE
-        MBEDTLS_SSL_CLIENT_CERTIFICATE
-        MBEDTLS_SSL_CLIENT_KEY_EXCHANGE
-        MBEDTLS_SSL_CERTIFICATE_VERIFY
-        MBEDTLS_SSL_CLIENT_CHANGE_CIPHER_SPEC
-        MBEDTLS_SSL_CLIENT_FINISHED
-        MBEDTLS_SSL_SERVER_CHANGE_CIPHER_SPEC
-        MBEDTLS_SSL_SERVER_FINISHED
-        MBEDTLS_SSL_FLUSH_BUFFERS
-        MBEDTLS_SSL_HANDSHAKE_WRAPUP
-        MBEDTLS_SSL_HANDSHAKE_OVER
-        MBEDTLS_SSL_SERVER_NEW_SESSION_TICKET
-        MBEDTLS_SSL_SERVER_HELLO_VERIFY_REQUEST_SENT
-
-    enum:
-        MBEDTLS_SSL_IS_CLIENT
-        MBEDTLS_SSL_IS_SERVER
-
-    enum:
-        MBEDTLS_ERR_NET_CONN_RESET = -0x0050
-        MBEDTLS_ERR_SSL_WANT_READ = -0x6900
-        MBEDTLS_ERR_SSL_WANT_WRITE = -0x6880
-        MBEDTLS_ERR_SSL_CLIENT_RECONNECT = -0x6780
-        MBEDTLS_ERR_SSL_PEER_CLOSE_NOTIFY = -0x7880
-        MBEDTLS_ERR_SSL_BUFFER_TOO_SMALL = -0x6a00
-        MBEDTLS_ERR_SSL_HELLO_VERIFY_REQUIRED = -0x6a80
-        MBEDTLS_ERR_SSL_BAD_INPUT_DATA = -0x7100
-
-
-cdef extern from "mbedtls/ssl_internal.h" nogil:
-    ctypedef struct mbedtls_ssl_transform:
-        pass
-
-    ctypedef struct mbedtls_ssl_handshake_params:
-        int sig_alg
-        int verify_sig_alg
-        # Diffie-Hellman key exchange:
-        # mbedtls_dhm_context dhm_ctx
-        _ecdh.mbedtls_ecdh_context ecdh_ctx
-        # EC-J-Pake (not very much used anymore)
-        # mbedtls_ecjpake_context ecjpake_ctx
-        mbedtls_ssl_key_cert *key_cert
-
-    ctypedef struct mbedtls_ssl_key_cert:
-        _x509.mbedtls_x509_crt *cert
-        _pk.mbedtls_pk_context *key
-        mbedtls_ssl_key_cert *next
-
-
-cdef extern from "mbedtls/ssl.h" nogil:
-    # Defined here
-    # ------------
-    # ctypedef enum mbedtls_ssl_states: pass
-
-    ctypedef struct mbedtls_ssl_session:
-        pass
-
-    ctypedef struct mbedtls_ssl_config:
-        # set_certificate_chain
-        mbedtls_ssl_key_cert *key_cert
-        # set_ciphers
-        const int *ciphersuite_list[4]
-        # set_inner_protocols
-        const char **alpn_list
-        # set_lowest_supported_version/set_highest_supported_version
-        unsigned char max_major_ver
-        unsigned char max_minor_ver
-        unsigned char min_major_ver
-        unsigned char min_minor_ver
-        # set_anti_replay
-        unsigned int anti_replay
-        # set_handshake_timeout
-        unsigned int hs_timeout_min
-        unsigned int hs_timeout_max
-
-        unsigned int endpoint
-        unsigned int transport
-        # set_validate_certificates
-        unsigned int authmode
-
-        # set_trust_store
-        _x509.mbedtls_x509_crt *ca_chain
-        _x509.mbedtls_x509_crt *ca_crl
-        # set_sni_callback
-        # f_sni / p_sni
-        # for mbedtls_ssl_conf_psk_cb
-        void *p_psk
-        unsigned char *psk
-        size_t psk_len
-        unsigned char *psk_identity
-        size_t psk_identity_len
-
-    ctypedef struct mbedtls_ssl_context:
-        const mbedtls_ssl_config *conf
-        int state
-        char *hostname
-        unsigned char *cli_id
-        size_t cli_id_len
-
-    # Callback types
-    # --------------
-    ctypedef int(*mbedtls_ssl_send_p)(void*, const unsigned char*, size_t)
-    ctypedef int(*mbedtls_ssl_recv_p)(void*, unsigned char*, size_t)
-    ctypedef int(*mbedtls_ssl_recv_timeout_p)(
-        void*, unsigned char*, size_t, int)
-
-    ctypedef void(*mbedtls_ssl_set_timer_t)(void *ctx, int int_ms, int fin_ms)
-    ctypedef int(*mbedtls_ssl_get_timer_t)(void *ctx)
-    ctypedef int(*mbedtls_ssl_cookie_write_t)(
-        void *ctx,
-        unsigned char **p, unsigned char *end,
-        const unsigned char *info, size_t ilen)
-    ctypedef int(*mbedtls_ssl_cookie_check_t)(
-        void *ctx,
-        const unsigned char *cookie, size_t clen,
-        const unsigned char *info, size_t ilen)
-    # mbedtls_ssl_ticket_write_t
-    # mbedtls_ssl_ticket_parse_t
-    # mbedtls_ssl_export_keys_t
-
-    # Free functions
-    # --------------
-    const int* mbedtls_ssl_list_ciphersuites()
-    const char* mbedtls_ssl_get_ciphersuite_name(const int ciphersuite_id)
-    int mbedtls_ssl_get_ciphersuite_id(const char *ciphersuite_name)
-
-    # mbedtls_ssl_config
-    # ------------------
-    void mbedtls_ssl_conf_endpoint(mbedtls_ssl_config *conf, int endpoint)
-    # void mbedtls_ssl_conf_transport(mbedtls_ssl_config *conf, int transport)
-
-    void mbedtls_ssl_conf_authmode(mbedtls_ssl_config *conf, int authmode)
-    void mbedtls_ssl_conf_ciphersuites(
-        mbedtls_ssl_config *conf,
-        const int* ciphersuites)
-
-    # DTLS only
-    # ---------
-    void mbedtls_ssl_conf_dtls_anti_replay(
-        mbedtls_ssl_config *conf,
-        char mode)
-    # mbedtls_ssl_conf_dtls_badmac_limit
-    void mbedtls_ssl_conf_handshake_timeout(
-        mbedtls_ssl_config *conf,
-        int min, int max)
-    # mbedtls_ssl_conf_ciphersuites_for_version
-    # mbedtls_ssl_conf_cert_profile
-
-    # TLS + DTLS
-    # ----------
-    void mbedtls_ssl_conf_ca_chain(
-        mbedtls_ssl_config *conf,
-        _x509.mbedtls_x509_crt *ca_chain,
-        _x509.mbedtls_x509_crl *ca_crl)
-    int mbedtls_ssl_conf_own_cert(
-        mbedtls_ssl_config *conf,
-        _x509.mbedtls_x509_crt *own_cert,
-        _pk.mbedtls_pk_context *pk_key)
-
-    int mbedtls_ssl_conf_psk(
-        mbedtls_ssl_config *conf,
-        const unsigned char *psk,
-        size_t psk_len,
-        const unsigned char *psk_identity,
-        size_t psk_identity_len)
-    # mbedtls_ssl_conf_dh_param
-    # mbedtls_ssl_conf_dh_param_ctx
-    # mbedtls_ssl_conf_dhm_min_bitlen
-    # mbedtls_ssl_conf_curves
-    # mbedtls_ssl_conf_sig_hashes
-    int mbedtls_ssl_conf_alpn_protocols(
-        mbedtls_ssl_config *conf,
-        const char **protos)
-    int mbedtls_ssl_context_save(
-        mbedtls_ssl_context *ssl,
-        unsigned char *buf,
-        size_t buf_len,
-        size_t *olen,
-    )
-    int mbedtls_ssl_context_load(
-        mbedtls_ssl_context *ssl,
-        const unsigned char *buf,
-        size_t len,
-    )
-    void mbedtls_ssl_config_init(mbedtls_ssl_config *conf)
-    int mbedtls_ssl_config_defaults(
-        mbedtls_ssl_config *conf,
-        int endpoint,
-        int transport,
-        int preset)
-    void mbedtls_ssl_config_free(mbedtls_ssl_config *conf)
-
-    # mbedtls_ssl_config: set callbacks
-    # ---------------------------------
-    # mbedtls_ssl_conf_verify  // optional
-
-    void mbedtls_ssl_conf_rng(
-        mbedtls_ssl_config *conf,
-        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng
-    )
-    void mbedtls_ssl_conf_dbg(
-        mbedtls_ssl_config *conf,
-        void (*f_dbg)(void *, int, const char *, int, const char *),
-        void *p_dbg
-    )
-
-    # mbedtls_ssl_conf_read_timeout
-    # mbedtls_ssl_conf_session_tickets_cb
-    # mbedtls_ssl_conf_export_keys_cb
-
-    void mbedtls_ssl_conf_dtls_cookies(
-        mbedtls_ssl_config *conf,
-        mbedtls_ssl_cookie_write_t f_cookie_write,
-        mbedtls_ssl_cookie_check_t f_cookie_check,
-        void *p_cookie,
-    )
-
-    # mbedtls_ssl_conf_session_cache
-    void mbedtls_ssl_conf_psk_cb(
-        mbedtls_ssl_config *conf,
-        int (*f_psk)(
-            void *,
-            mbedtls_ssl_context *,
-            const unsigned char *,
-            size_t
-        ),
-        void *psk_store)
-    void mbedtls_ssl_conf_sni(
-        mbedtls_ssl_config *conf,
-        int (*f_sni)(void *, mbedtls_ssl_context *, const unsigned char*,
-                     size_t),
-        void* p_sni)
-    void mbedtls_ssl_conf_max_version(
-        mbedtls_ssl_config *conf,
-        int major,
-        int minor)
-    void mbedtls_ssl_conf_min_version(
-        mbedtls_ssl_config *conf,
-        int major,
-        int minor)
-    # mbedtls_ssl_conf_fallback
-    # mbedtls_ssl_conf_encrypt_then_mac
-    # mbedtls_ssl_conf_extended_master_secret
-    # mbedtls_ssl_conf_arc4_support
-
-    int mbedtls_ssl_conf_max_frag_len(
-        mbedtls_ssl_config *conf,
-        unsigned char mgl_code,
-    )
-
-    # mbedtls_ssl_conf_truncated_hmac
-    # mbedtls_ssl_conf_cbc_record_splitting
-    # mbedtls_ssl_conf_session_tickets
-    void mbedtls_ssl_conf_renegotiation(
-        mbedtls_ssl_config *conf,
-        int renegotiation)
-    # mbedtls_ssl_conf_legacy_renegotiation
-    # mbedtls_ssl_conf_renegotiation_enforced
-    # mbedtls_ssl_conf_renegotiation_period
-
-    # mbedtls_ssl_context
-    # -------------------
-    void mbedtls_ssl_init(mbedtls_ssl_context *ctx)
-    int mbedtls_ssl_setup(
-        mbedtls_ssl_context *ctx,
-        const mbedtls_ssl_config *conf)
-    int mbedtls_ssl_session_reset(mbedtls_ssl_context *ctx)
-    void mbedtls_ssl_set_bio(
-        mbedtls_ssl_context *ssl,
-        void *p_bio,
-        mbedtls_ssl_send_p f_send,
-        mbedtls_ssl_recv_p f_recv,
-        mbedtls_ssl_recv_timeout_p f_recv_timeout)
-
-    void mbedtls_ssl_set_mtu(
-        mbedtls_ssl_context *ssl,
-        uint16_t mtu,
-    )
-
-    void mbedtls_ssl_set_timer_cb(
-        # DTLS
-        mbedtls_ssl_context *ssl,
-        void *p_timer,
-        mbedtls_ssl_set_timer_t f_set_timer,
-        mbedtls_ssl_get_timer_t f_get_timer)
-    int mbedtls_ssl_set_client_transport_id(
-        # DTLS
-        mbedtls_ssl_context *ssl,
-        const unsigned char *info,
-        size_t ilen)
-    int mbedtls_ssl_set_session(
-        const mbedtls_ssl_context *ssl,
-        mbedtls_ssl_session *session)
-    int mbedtls_ssl_set_hs_psk(
-        mbedtls_ssl_context *ssl,
-        const unsigned char *psk,
-        size_t psk_len)
-    int mbedtls_ssl_set_hostname(
-        mbedtls_ssl_context *ssl,
-        const char *hostname)
-    # mbedtls_ssl_set_hs_ecjpake_password
-    # mbedtls_ssl_set_hs_own_cert
-    # mbedtls_ssl_set_hs_ca_chain
-    # mbedtls_ssl_set_hs_authmode
-    const char* mbedtls_ssl_get_alpn_protocol(const mbedtls_ssl_context *ctx)
-    size_t mbedtls_ssl_get_bytes_avail(const mbedtls_ssl_context *ctx)
-    int mbedtls_ssl_get_verify_result(const mbedtls_ssl_context *ssl)
-    const char* mbedtls_ssl_get_ciphersuite(const mbedtls_ssl_context *ssl)
-    const char* mbedtls_ssl_get_version(const mbedtls_ssl_context *ssl)
-    # mbedtls_ssl_get_record_expansion
-    size_t mbedtls_ssl_get_max_frag_len(const mbedtls_ssl_context *ssl)
-    const _x509.mbedtls_x509_crt *mbedtls_ssl_get_peer_cert(
-        const mbedtls_ssl_context *ctx)
-    int mbedtls_ssl_get_session(
-        const mbedtls_ssl_context *ssl,
-        mbedtls_ssl_session *session)
-    int mbedtls_ssl_handshake(mbedtls_ssl_context *ctx)
-    int mbedtls_ssl_handshake_step(mbedtls_ssl_context *ssl)
-    int mbedtls_ssl_renegotiate(mbedtls_ssl_context *ssl)
-    int mbedtls_ssl_read(
-        mbedtls_ssl_context *ctx,
-        unsigned char *buf,
-        size_t len)
-    int mbedtls_ssl_write(
-        mbedtls_ssl_context *ctx,
-        const unsigned char *buf,
-        size_t len)
-    # mbedtls_ssl_send_alert_message
-    int mbedtls_ssl_close_notify(mbedtls_ssl_context *ssl)
-    void mbedtls_ssl_free(mbedtls_ssl_context *ctx)
-
-    # mbedtls_ssl_session
-    # -------------------
-    void mbedtls_ssl_session_init(mbedtls_ssl_session *session)
-    void mbedtls_ssl_session_free(mbedtls_ssl_session *session)
-
-
-cdef extern from "mbedtls/ssl_cookie.h" nogil:
-    # This provides callbacks for DTLS.
-
-    ctypedef struct mbedtls_ssl_cookie_ctx:
-        # mbedtls_md_context_t hmac_ctx
-        unsigned long timeout
-        # mbedtls_threading_mutex_t mutex
-
-    void mbedtls_ssl_cookie_init(mbedtls_ssl_cookie_ctx *ctx)
-    int mbedtls_ssl_cookie_setup(
-        mbedtls_ssl_cookie_ctx *ctx,
-        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng,
-    )
-    void mbedtls_ssl_cookie_set_timeout(
-        mbedtls_ssl_cookie_ctx *ctx,
-        unsigned long delay,
-    )
-    void mbedtls_ssl_cookie_free(mbedtls_ssl_cookie_ctx *ctx)
-    mbedtls_ssl_cookie_write_t mbedtls_ssl_cookie_write
-    mbedtls_ssl_cookie_check_t mbedtls_ssl_cookie_check
-
-
-cdef class _DTLSCookie:
-    cdef mbedtls_ssl_cookie_ctx _ctx
-
-
-cdef class _PSKSToreProxy:
-    cdef object _mapping
-
-
-cdef class MbedTLSConfiguration:
-    cdef mbedtls_ssl_config _ctx
-    cdef _chain
-    cdef int *_ciphers
-    cdef const char **_protos
-    cdef _PSKSToreProxy _store
-    cdef _DTLSCookie _cookie
-    cdef object _max_fragmentation_length
-    # cdef'd because we aim at a non-writable structure.
-    cdef _set_validate_certificates(self, validate)
-    cdef _set_certificate_chain(self, chain)
-    cdef _set_ciphers(self, ciphers)
-    cdef _set_inner_protocols(self, protocols)
-    cdef _set_lowest_supported_version(self, version)
-    cdef _set_highest_supported_version(self, version)
-    cdef _set_trust_store(self, object store)
-    cdef _set_max_fragmentation_length(self, object mfl)
-    cdef _set_anti_replay(self, mode)
-    cdef _set_handshake_timeout(self, minimum, maximum)
-    cdef _set_cookie(self, _DTLSCookie cookie)
-    cdef _set_sni_callback(self, callback)
-    cdef _set_pre_shared_key(self, psk)
-    cdef _set_pre_shared_key_store(self, psk_store)
-
-
-cdef class TLSSession:
-    cdef mbedtls_ssl_session _ctx
-
-
-cdef struct _C_Buffers:
-    _rb.ring_buffer_ctx *out_ctx
-    _rb.ring_buffer_ctx *in_ctx
-
-
-cdef class _BaseContext:
-    cdef MbedTLSConfiguration _conf
-
-
-cdef class MbedTLSBuffer:
-    cdef _BaseContext _context
-    cdef mbedtls_ssl_context _ctx
-    cdef _rb.RingBuffer _c_output_buffer
-    cdef _rb.RingBuffer _c_input_buffer
-    cdef _C_Buffers _c_buffers
-    # DTLS only:
-    cdef _timing.mbedtls_timing_delay_context _timer
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2018, Mathias Laurin
+
+from libc.stdint cimport uint16_t
+
+cimport mbedtls._ecdh as _ecdh
+cimport mbedtls._ringbuf as _rb
+cimport mbedtls._timing as _timing
+cimport mbedtls.pk as _pk
+cimport mbedtls.x509 as _x509
+
+cdef:
+    enum:
+        MBEDTLS_SSL_TRANSPORT_STREAM = 0
+        MBEDTLS_SSL_TRANSPORT_DATAGRAM = 1
+
+    enum:
+        MBEDTLS_SSL_PRESET_DEFAULT = 0
+        MBEDTLS_SSL_PRESET_SUITEB = 2
+
+    enum:
+        MBEDTLS_SSL_VERIFY_NONE = 0
+        MBEDTLS_SSL_VERIFY_OPTIONAL = 1
+        MBEDTLS_SSL_VERIFY_REQUIRED = 2
+
+    enum:
+        MBEDTLS_SSL_ANTI_REPLAY_DISABLED = 0
+        MBEDTLS_SSL_ANTI_REPLAY_ENABLED = 1
+
+    enum:
+        # Message type
+        MBEDTLS_SSL_MSG_CHANGE_CIPHER_SPEC = 20  # 0x14
+        MBEDTLS_SSL_MSG_ALERT = 21      # 0x15
+        MBEDTLS_SSL_MSG_HANDSHAKE = 22  # 0x16
+        MBEDTLS_SSL_MSG_APPLICATION_DATA = 23  # 0x17
+
+    enum:
+        MBEDTLS_SSL_HELLO_REQUEST
+        MBEDTLS_SSL_CLIENT_HELLO
+        MBEDTLS_SSL_SERVER_HELLO
+        MBEDTLS_SSL_SERVER_CERTIFICATE
+        MBEDTLS_SSL_SERVER_KEY_EXCHANGE
+        MBEDTLS_SSL_CERTIFICATE_REQUEST
+        MBEDTLS_SSL_SERVER_HELLO_DONE
+        MBEDTLS_SSL_CLIENT_CERTIFICATE
+        MBEDTLS_SSL_CLIENT_KEY_EXCHANGE
+        MBEDTLS_SSL_CERTIFICATE_VERIFY
+        MBEDTLS_SSL_CLIENT_CHANGE_CIPHER_SPEC
+        MBEDTLS_SSL_CLIENT_FINISHED
+        MBEDTLS_SSL_SERVER_CHANGE_CIPHER_SPEC
+        MBEDTLS_SSL_SERVER_FINISHED
+        MBEDTLS_SSL_FLUSH_BUFFERS
+        MBEDTLS_SSL_HANDSHAKE_WRAPUP
+        MBEDTLS_SSL_HANDSHAKE_OVER
+        MBEDTLS_SSL_SERVER_NEW_SESSION_TICKET
+        MBEDTLS_SSL_SERVER_HELLO_VERIFY_REQUEST_SENT
+
+    enum:
+        MBEDTLS_SSL_IS_CLIENT
+        MBEDTLS_SSL_IS_SERVER
+
+    enum:
+        MBEDTLS_ERR_NET_CONN_RESET = -0x0050
+        MBEDTLS_ERR_SSL_WANT_READ = -0x6900
+        MBEDTLS_ERR_SSL_WANT_WRITE = -0x6880
+        MBEDTLS_ERR_SSL_CLIENT_RECONNECT = -0x6780
+        MBEDTLS_ERR_SSL_PEER_CLOSE_NOTIFY = -0x7880
+        MBEDTLS_ERR_SSL_BUFFER_TOO_SMALL = -0x6a00
+        MBEDTLS_ERR_SSL_HELLO_VERIFY_REQUIRED = -0x6a80
+        MBEDTLS_ERR_SSL_BAD_INPUT_DATA = -0x7100
+
+
+cdef extern from "mbedtls/ssl_internal.h" nogil:
+    ctypedef struct mbedtls_ssl_transform:
+        pass
+
+    ctypedef struct mbedtls_ssl_handshake_params:
+        int sig_alg
+        int verify_sig_alg
+        # Diffie-Hellman key exchange:
+        # mbedtls_dhm_context dhm_ctx
+        _ecdh.mbedtls_ecdh_context ecdh_ctx
+        # EC-J-Pake (not very much used anymore)
+        # mbedtls_ecjpake_context ecjpake_ctx
+        mbedtls_ssl_key_cert *key_cert
+
+    ctypedef struct mbedtls_ssl_key_cert:
+        _x509.mbedtls_x509_crt *cert
+        _pk.mbedtls_pk_context *key
+        mbedtls_ssl_key_cert *next
+
+
+cdef extern from "mbedtls/ssl.h" nogil:
+    # Defined here
+    # ------------
+    # ctypedef enum mbedtls_ssl_states: pass
+
+    ctypedef struct mbedtls_ssl_session:
+        pass
+
+    ctypedef struct mbedtls_ssl_config:
+        # set_certificate_chain
+        mbedtls_ssl_key_cert *key_cert
+        # set_ciphers
+        const int *ciphersuite_list[4]
+        # set_inner_protocols
+        const char **alpn_list
+        # set_lowest_supported_version/set_highest_supported_version
+        unsigned char max_major_ver
+        unsigned char max_minor_ver
+        unsigned char min_major_ver
+        unsigned char min_minor_ver
+        # set_anti_replay
+        unsigned int anti_replay
+        # set_handshake_timeout
+        unsigned int hs_timeout_min
+        unsigned int hs_timeout_max
+
+        unsigned int endpoint
+        unsigned int transport
+        # set_validate_certificates
+        unsigned int authmode
+
+        # set_trust_store
+        _x509.mbedtls_x509_crt *ca_chain
+        _x509.mbedtls_x509_crt *ca_crl
+        # set_sni_callback
+        # f_sni / p_sni
+        # for mbedtls_ssl_conf_psk_cb
+        void *p_psk
+        unsigned char *psk
+        size_t psk_len
+        unsigned char *psk_identity
+        size_t psk_identity_len
+
+    ctypedef struct mbedtls_ssl_context:
+        const mbedtls_ssl_config *conf
+        int state
+        char *hostname
+        unsigned char *cli_id
+        size_t cli_id_len
+
+    # Callback types
+    # --------------
+    ctypedef int(*mbedtls_ssl_send_p)(void*, const unsigned char*, size_t)
+    ctypedef int(*mbedtls_ssl_recv_p)(void*, unsigned char*, size_t)
+    ctypedef int(*mbedtls_ssl_recv_timeout_p)(
+        void*, unsigned char*, size_t, int)
+
+    ctypedef void(*mbedtls_ssl_set_timer_t)(void *ctx, int int_ms, int fin_ms)
+    ctypedef int(*mbedtls_ssl_get_timer_t)(void *ctx)
+    ctypedef int(*mbedtls_ssl_cookie_write_t)(
+        void *ctx,
+        unsigned char **p, unsigned char *end,
+        const unsigned char *info, size_t ilen)
+    ctypedef int(*mbedtls_ssl_cookie_check_t)(
+        void *ctx,
+        const unsigned char *cookie, size_t clen,
+        const unsigned char *info, size_t ilen)
+    # mbedtls_ssl_ticket_write_t
+    # mbedtls_ssl_ticket_parse_t
+    # mbedtls_ssl_export_keys_t
+
+    # Free functions
+    # --------------
+    const int* mbedtls_ssl_list_ciphersuites()
+    const char* mbedtls_ssl_get_ciphersuite_name(const int ciphersuite_id)
+    int mbedtls_ssl_get_ciphersuite_id(const char *ciphersuite_name)
+
+    # mbedtls_ssl_config
+    # ------------------
+    void mbedtls_ssl_conf_endpoint(mbedtls_ssl_config *conf, int endpoint)
+    # void mbedtls_ssl_conf_transport(mbedtls_ssl_config *conf, int transport)
+
+    void mbedtls_ssl_conf_authmode(mbedtls_ssl_config *conf, int authmode)
+    void mbedtls_ssl_conf_ciphersuites(
+        mbedtls_ssl_config *conf,
+        const int* ciphersuites)
+
+    # DTLS only
+    # ---------
+    void mbedtls_ssl_conf_dtls_anti_replay(
+        mbedtls_ssl_config *conf,
+        char mode)
+    # mbedtls_ssl_conf_dtls_badmac_limit
+    void mbedtls_ssl_conf_handshake_timeout(
+        mbedtls_ssl_config *conf,
+        int min, int max)
+    # mbedtls_ssl_conf_ciphersuites_for_version
+    # mbedtls_ssl_conf_cert_profile
+
+    # TLS + DTLS
+    # ----------
+    void mbedtls_ssl_conf_ca_chain(
+        mbedtls_ssl_config *conf,
+        _x509.mbedtls_x509_crt *ca_chain,
+        _x509.mbedtls_x509_crl *ca_crl)
+    int mbedtls_ssl_conf_own_cert(
+        mbedtls_ssl_config *conf,
+        _x509.mbedtls_x509_crt *own_cert,
+        _pk.mbedtls_pk_context *pk_key)
+
+    int mbedtls_ssl_conf_psk(
+        mbedtls_ssl_config *conf,
+        const unsigned char *psk,
+        size_t psk_len,
+        const unsigned char *psk_identity,
+        size_t psk_identity_len)
+    # mbedtls_ssl_conf_dh_param
+    # mbedtls_ssl_conf_dh_param_ctx
+    # mbedtls_ssl_conf_dhm_min_bitlen
+    # mbedtls_ssl_conf_curves
+    # mbedtls_ssl_conf_sig_hashes
+    int mbedtls_ssl_conf_alpn_protocols(
+        mbedtls_ssl_config *conf,
+        const char **protos)
+    int mbedtls_ssl_context_save(
+        mbedtls_ssl_context *ssl,
+        unsigned char *buf,
+        size_t buf_len,
+        size_t *olen,
+    )
+    int mbedtls_ssl_context_load(
+        mbedtls_ssl_context *ssl,
+        const unsigned char *buf,
+        size_t len,
+    )
+    void mbedtls_ssl_config_init(mbedtls_ssl_config *conf)
+    int mbedtls_ssl_config_defaults(
+        mbedtls_ssl_config *conf,
+        int endpoint,
+        int transport,
+        int preset)
+    void mbedtls_ssl_config_free(mbedtls_ssl_config *conf)
+
+    # mbedtls_ssl_config: set callbacks
+    # ---------------------------------
+    # mbedtls_ssl_conf_verify  // optional
+
+    void mbedtls_ssl_conf_rng(
+        mbedtls_ssl_config *conf,
+        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng
+    )
+    void mbedtls_ssl_conf_dbg(
+        mbedtls_ssl_config *conf,
+        void (*f_dbg)(void *, int, const char *, int, const char *),
+        void *p_dbg
+    )
+
+    # mbedtls_ssl_conf_read_timeout
+    # mbedtls_ssl_conf_session_tickets_cb
+    # mbedtls_ssl_conf_export_keys_cb
+
+    void mbedtls_ssl_conf_dtls_cookies(
+        mbedtls_ssl_config *conf,
+        mbedtls_ssl_cookie_write_t f_cookie_write,
+        mbedtls_ssl_cookie_check_t f_cookie_check,
+        void *p_cookie,
+    )
+
+    # mbedtls_ssl_conf_session_cache
+    void mbedtls_ssl_conf_psk_cb(
+        mbedtls_ssl_config *conf,
+        int (*f_psk)(
+            void *,
+            mbedtls_ssl_context *,
+            const unsigned char *,
+            size_t
+        ),
+        void *psk_store)
+    void mbedtls_ssl_conf_sni(
+        mbedtls_ssl_config *conf,
+        int (*f_sni)(void *, mbedtls_ssl_context *, const unsigned char*,
+                     size_t),
+        void* p_sni)
+    void mbedtls_ssl_conf_max_version(
+        mbedtls_ssl_config *conf,
+        int major,
+        int minor)
+    void mbedtls_ssl_conf_min_version(
+        mbedtls_ssl_config *conf,
+        int major,
+        int minor)
+    # mbedtls_ssl_conf_fallback
+    # mbedtls_ssl_conf_encrypt_then_mac
+    # mbedtls_ssl_conf_extended_master_secret
+    # mbedtls_ssl_conf_arc4_support
+
+    int mbedtls_ssl_conf_max_frag_len(
+        mbedtls_ssl_config *conf,
+        unsigned char mgl_code,
+    )
+
+    # mbedtls_ssl_conf_truncated_hmac
+    # mbedtls_ssl_conf_cbc_record_splitting
+    # mbedtls_ssl_conf_session_tickets
+    void mbedtls_ssl_conf_renegotiation(
+        mbedtls_ssl_config *conf,
+        int renegotiation)
+    # mbedtls_ssl_conf_legacy_renegotiation
+    # mbedtls_ssl_conf_renegotiation_enforced
+    # mbedtls_ssl_conf_renegotiation_period
+
+    # mbedtls_ssl_context
+    # -------------------
+    void mbedtls_ssl_init(mbedtls_ssl_context *ctx)
+    int mbedtls_ssl_setup(
+        mbedtls_ssl_context *ctx,
+        const mbedtls_ssl_config *conf)
+    int mbedtls_ssl_session_reset(mbedtls_ssl_context *ctx)
+    void mbedtls_ssl_set_bio(
+        mbedtls_ssl_context *ssl,
+        void *p_bio,
+        mbedtls_ssl_send_p f_send,
+        mbedtls_ssl_recv_p f_recv,
+        mbedtls_ssl_recv_timeout_p f_recv_timeout)
+
+    void mbedtls_ssl_set_mtu(
+        mbedtls_ssl_context *ssl,
+        uint16_t mtu,
+    )
+
+    void mbedtls_ssl_set_timer_cb(
+        # DTLS
+        mbedtls_ssl_context *ssl,
+        void *p_timer,
+        mbedtls_ssl_set_timer_t f_set_timer,
+        mbedtls_ssl_get_timer_t f_get_timer)
+    int mbedtls_ssl_set_client_transport_id(
+        # DTLS
+        mbedtls_ssl_context *ssl,
+        const unsigned char *info,
+        size_t ilen)
+    int mbedtls_ssl_set_session(
+        const mbedtls_ssl_context *ssl,
+        mbedtls_ssl_session *session)
+    int mbedtls_ssl_set_hs_psk(
+        mbedtls_ssl_context *ssl,
+        const unsigned char *psk,
+        size_t psk_len)
+    int mbedtls_ssl_set_hostname(
+        mbedtls_ssl_context *ssl,
+        const char *hostname)
+    # mbedtls_ssl_set_hs_ecjpake_password
+    # mbedtls_ssl_set_hs_own_cert
+    # mbedtls_ssl_set_hs_ca_chain
+    # mbedtls_ssl_set_hs_authmode
+    const char* mbedtls_ssl_get_alpn_protocol(const mbedtls_ssl_context *ctx)
+    size_t mbedtls_ssl_get_bytes_avail(const mbedtls_ssl_context *ctx)
+    int mbedtls_ssl_get_verify_result(const mbedtls_ssl_context *ssl)
+    const char* mbedtls_ssl_get_ciphersuite(const mbedtls_ssl_context *ssl)
+    const char* mbedtls_ssl_get_version(const mbedtls_ssl_context *ssl)
+    # mbedtls_ssl_get_record_expansion
+    size_t mbedtls_ssl_get_max_frag_len(const mbedtls_ssl_context *ssl)
+    const _x509.mbedtls_x509_crt *mbedtls_ssl_get_peer_cert(
+        const mbedtls_ssl_context *ctx)
+    int mbedtls_ssl_get_session(
+        const mbedtls_ssl_context *ssl,
+        mbedtls_ssl_session *session)
+    int mbedtls_ssl_handshake(mbedtls_ssl_context *ctx)
+    int mbedtls_ssl_handshake_step(mbedtls_ssl_context *ssl)
+    int mbedtls_ssl_renegotiate(mbedtls_ssl_context *ssl)
+    int mbedtls_ssl_read(
+        mbedtls_ssl_context *ctx,
+        unsigned char *buf,
+        size_t len)
+    int mbedtls_ssl_write(
+        mbedtls_ssl_context *ctx,
+        const unsigned char *buf,
+        size_t len)
+    # mbedtls_ssl_send_alert_message
+    int mbedtls_ssl_close_notify(mbedtls_ssl_context *ssl)
+    void mbedtls_ssl_free(mbedtls_ssl_context *ctx)
+
+    # mbedtls_ssl_session
+    # -------------------
+    void mbedtls_ssl_session_init(mbedtls_ssl_session *session)
+    void mbedtls_ssl_session_free(mbedtls_ssl_session *session)
+
+
+cdef extern from "mbedtls/ssl_cookie.h" nogil:
+    # This provides callbacks for DTLS.
+
+    ctypedef struct mbedtls_ssl_cookie_ctx:
+        # mbedtls_md_context_t hmac_ctx
+        unsigned long timeout
+        # mbedtls_threading_mutex_t mutex
+
+    void mbedtls_ssl_cookie_init(mbedtls_ssl_cookie_ctx *ctx)
+    int mbedtls_ssl_cookie_setup(
+        mbedtls_ssl_cookie_ctx *ctx,
+        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng,
+    )
+    void mbedtls_ssl_cookie_set_timeout(
+        mbedtls_ssl_cookie_ctx *ctx,
+        unsigned long delay,
+    )
+    void mbedtls_ssl_cookie_free(mbedtls_ssl_cookie_ctx *ctx)
+    mbedtls_ssl_cookie_write_t mbedtls_ssl_cookie_write
+    mbedtls_ssl_cookie_check_t mbedtls_ssl_cookie_check
+
+
+cdef class _DTLSCookie:
+    cdef mbedtls_ssl_cookie_ctx _ctx
+
+
+cdef class _PSKSToreProxy:
+    cdef object _mapping
+
+
+cdef class MbedTLSConfiguration:
+    cdef mbedtls_ssl_config _ctx
+    cdef _chain
+    cdef int *_ciphers
+    cdef const char **_protos
+    cdef _PSKSToreProxy _store
+    cdef _DTLSCookie _cookie
+    cdef object _max_fragmentation_length
+    # cdef'd because we aim at a non-writable structure.
+    cdef _set_validate_certificates(self, validate)
+    cdef _set_certificate_chain(self, chain)
+    cdef _set_ciphers(self, ciphers)
+    cdef _set_inner_protocols(self, protocols)
+    cdef _set_lowest_supported_version(self, version)
+    cdef _set_highest_supported_version(self, version)
+    cdef _set_trust_store(self, object store)
+    cdef _set_max_fragmentation_length(self, object mfl)
+    cdef _set_anti_replay(self, mode)
+    cdef _set_handshake_timeout(self, minimum, maximum)
+    cdef _set_cookie(self, _DTLSCookie cookie)
+    cdef _set_sni_callback(self, callback)
+    cdef _set_pre_shared_key(self, psk)
+    cdef _set_pre_shared_key_store(self, psk_store)
+
+
+cdef class TLSSession:
+    cdef mbedtls_ssl_session _ctx
+
+
+cdef struct _C_Buffers:
+    _rb.ring_buffer_ctx *out_ctx
+    _rb.ring_buffer_ctx *in_ctx
+
+
+cdef class _BaseContext:
+    cdef MbedTLSConfiguration _conf
+
+
+cdef class MbedTLSBuffer:
+    cdef _BaseContext _context
+    cdef mbedtls_ssl_context _ctx
+    cdef _rb.RingBuffer _c_output_buffer
+    cdef _rb.RingBuffer _c_input_buffer
+    cdef _C_Buffers _c_buffers
+    # DTLS only:
+    cdef _timing.mbedtls_timing_delay_context _timer
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/_tls.pyi` & `python-mbedtls-2.7.1/src/mbedtls/_tls.pyi`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2022, Mathias Laurin
-
-from __future__ import annotations
-
-import enum
-import os
-import sys
-from collections import abc
-from typing import Optional, Sequence, Tuple, Union, overload
-
-from mbedtls._tlsi import (
-    Certificate,
-    DTLSConfiguration,
-    DTLSVersion,
-    TLSConfiguration,
-    TLSVersion,
-)
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Literal
-else:
-    from typing import Literal
-
-_VERSION = Tuple[int, int]
-
-def ciphers_available() -> Sequence[str]: ...
-def _tls_to_version(maj_min_version: _VERSION) -> TLSVersion: ...
-def _dtls_to_version(maj_min_version: _VERSION) -> DTLSVersion: ...
-def _tls_from_version(version: TLSVersion) -> Tuple[int, int]: ...
-def _dtls_from_version(version: DTLSVersion) -> Tuple[int, int]: ...
-
-_SUPPORTED_TLS_VERSION: Sequence[TLSVersion]
-_SUPPORTED_DTLS_VERSION: Sequence[DTLSVersion]
-
-class HandshakeStep(enum.Enum):
-    HELLO_REQUEST: int
-    CLIENT_HELLO: int
-    SERVER_HELLO: int
-    SERVER_CERTIFICATE: int
-    SERVER_KEY_EXCHANGE: int
-    CERTIFICATE_REQUEST: int
-    SERVER_HELLO_DONE: int
-    CLIENT_CERTIFICATE: int
-    CLIENT_KEY_EXCHANGE: int
-    CERTIFICATE_VERIFY: int
-    CLIENT_CHANGE_CIPHER_SPEC: int
-    CLIENT_FINISHED: int
-    SERVER_CHANGE_CIPHER_SPEC: int
-    SERVER_FINISHED: int
-    FLUSH_BUFFERS: int
-    HANDSHAKE_WRAPUP: int
-    HANDSHAKE_OVER: int
-    SERVER_NEW_SESSION_TICKET: int
-    SERVER_HELLO_VERIFY_REQUEST_SENT: int
-
-
-class TLSError(Exception): ...
-class WantWriteError(TLSError): ...
-class WantReadError(TLSError): ...
-class RaggedEOF(TLSError): ...
-class HelloVerifyRequest(TLSError): ...
-
-class TrustStore(abc.Sequence[Certificate]):
-    def __init__(
-        self, db: Optional[Union[Sequence[Certificate], TrustStore]] = ...
-    ) -> None: ...
-    @classmethod
-    def system(cls) -> TrustStore: ...
-    @classmethod
-    def from_pem_file(
-        cls, path: Union[str, os.PathLike[str]]
-    ) -> TrustStore: ...
-    def __eq__(self, other: object) -> bool: ...
-    def __bool__(self) -> bool: ...
-    def __len__(self) -> int: ...
-    @overload
-    def __getitem__(self, index: int) -> Certificate: ...
-    @overload
-    def __getitem__(self, s: slice) -> TrustStore: ...
-    def add(self, crt: Certificate) -> None: ...
-
-class Purpose(enum.IntEnum):
-    SERVER_AUTH: int
-    CLIENT_AUTH: int
-
-class _BaseContext:
-    def __init__(
-        self, configuration: Union[TLSConfiguration, DTLSConfiguration]
-    ) -> None: ...
-    def __eq__(self, other: object) -> bool: ...
-    @property
-    def configuration(self) -> Union[TLSConfiguration, DTLSConfiguration]: ...
-    # Don't use `_conf`, for testing purpose only.
-    @property
-    def _conf(self) -> Union[TLSConfiguration, DTLSConfiguration]: ...
-    @property
-    def _purpose(self) -> Purpose: ...
-
-class MbedTLSBuffer:
-    def __init__(
-        self, context: _BaseContext, server_hostname: Optional[str] = None
-    ) -> None: ...
-    @property
-    def _input_buffer(self) -> bytes: ...
-    @property
-    def _output_buffer(self) -> bytes: ...
-    @property
-    def context(self) -> _BaseContext: ...
-    @property
-    def _server_hostname(self) -> str: ...
-    def shutdown(self) -> None: ...
-    def setcookieparam(self, info: bytes) -> None: ...
-    def setmtu(self, mtu: int) -> None: ...
-    def read(self, amt: int) -> bytes: ...
-    def readinto(self, buffer: bytes, amt: int) -> int: ...
-    def write(self, buffer: bytes) -> int: ...
-    def receive_from_network(self, data: bytes) -> None: ...
-    def peek_outgoing(self, amt: int) -> bytes: ...
-    def consume_outgoing(self, amt: int) -> None: ...
-    @overload
-    def getpeercert(self, binary_form: Literal[False]) -> str: ...
-    @overload
-    def getpeercert(self, binary_form: Literal[True]) -> bytes: ...
-    def selected_npn_protocol(self) -> None: ...
-    def negotiated_protocol(self) -> str: ...
-    def cipher(self) -> bytes: ...
-    @property
-    def _handshake_state(self) -> HandshakeStep: ...
-    def do_handshake(self) -> None: ...
-    def negotiated_tls_version(self) -> Union[TLSVersion, DTLSVersion]: ...
-
-class TLSSession: ...
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2022, Mathias Laurin
+
+from __future__ import annotations
+
+import enum
+import os
+import sys
+from collections import abc
+from typing import Optional, Sequence, Tuple, Union, overload
+
+from mbedtls._tlsi import (
+    Certificate,
+    DTLSConfiguration,
+    DTLSVersion,
+    TLSConfiguration,
+    TLSVersion,
+)
+
+if sys.version_info < (3, 8):
+    from typing_extensions import Literal
+else:
+    from typing import Literal
+
+_VERSION = Tuple[int, int]
+
+def ciphers_available() -> Sequence[str]: ...
+def _tls_to_version(maj_min_version: _VERSION) -> TLSVersion: ...
+def _dtls_to_version(maj_min_version: _VERSION) -> DTLSVersion: ...
+def _tls_from_version(version: TLSVersion) -> Tuple[int, int]: ...
+def _dtls_from_version(version: DTLSVersion) -> Tuple[int, int]: ...
+
+_SUPPORTED_TLS_VERSION: Sequence[TLSVersion]
+_SUPPORTED_DTLS_VERSION: Sequence[DTLSVersion]
+
+class HandshakeStep(enum.Enum):
+    HELLO_REQUEST: int
+    CLIENT_HELLO: int
+    SERVER_HELLO: int
+    SERVER_CERTIFICATE: int
+    SERVER_KEY_EXCHANGE: int
+    CERTIFICATE_REQUEST: int
+    SERVER_HELLO_DONE: int
+    CLIENT_CERTIFICATE: int
+    CLIENT_KEY_EXCHANGE: int
+    CERTIFICATE_VERIFY: int
+    CLIENT_CHANGE_CIPHER_SPEC: int
+    CLIENT_FINISHED: int
+    SERVER_CHANGE_CIPHER_SPEC: int
+    SERVER_FINISHED: int
+    FLUSH_BUFFERS: int
+    HANDSHAKE_WRAPUP: int
+    HANDSHAKE_OVER: int
+    SERVER_NEW_SESSION_TICKET: int
+    SERVER_HELLO_VERIFY_REQUEST_SENT: int
+
+
+class TLSError(Exception): ...
+class WantWriteError(TLSError): ...
+class WantReadError(TLSError): ...
+class RaggedEOF(TLSError): ...
+class HelloVerifyRequest(TLSError): ...
+
+class TrustStore(abc.Sequence[Certificate]):
+    def __init__(
+        self, db: Optional[Union[Sequence[Certificate], TrustStore]] = ...
+    ) -> None: ...
+    @classmethod
+    def system(cls) -> TrustStore: ...
+    @classmethod
+    def from_pem_file(
+        cls, path: Union[str, os.PathLike[str]]
+    ) -> TrustStore: ...
+    def __eq__(self, other: object) -> bool: ...
+    def __bool__(self) -> bool: ...
+    def __len__(self) -> int: ...
+    @overload
+    def __getitem__(self, index: int) -> Certificate: ...
+    @overload
+    def __getitem__(self, s: slice) -> TrustStore: ...
+    def add(self, crt: Certificate) -> None: ...
+
+class Purpose(enum.IntEnum):
+    SERVER_AUTH: int
+    CLIENT_AUTH: int
+
+class _BaseContext:
+    def __init__(
+        self, configuration: Union[TLSConfiguration, DTLSConfiguration]
+    ) -> None: ...
+    def __eq__(self, other: object) -> bool: ...
+    @property
+    def configuration(self) -> Union[TLSConfiguration, DTLSConfiguration]: ...
+    # Don't use `_conf`, for testing purpose only.
+    @property
+    def _conf(self) -> Union[TLSConfiguration, DTLSConfiguration]: ...
+    @property
+    def _purpose(self) -> Purpose: ...
+
+class MbedTLSBuffer:
+    def __init__(
+        self, context: _BaseContext, server_hostname: Optional[str] = None
+    ) -> None: ...
+    @property
+    def _input_buffer(self) -> bytes: ...
+    @property
+    def _output_buffer(self) -> bytes: ...
+    @property
+    def context(self) -> _BaseContext: ...
+    @property
+    def _server_hostname(self) -> str: ...
+    def shutdown(self) -> None: ...
+    def setcookieparam(self, info: bytes) -> None: ...
+    def setmtu(self, mtu: int) -> None: ...
+    def read(self, amt: int) -> bytes: ...
+    def readinto(self, buffer: bytes, amt: int) -> int: ...
+    def write(self, buffer: bytes) -> int: ...
+    def receive_from_network(self, data: bytes) -> None: ...
+    def peek_outgoing(self, amt: int) -> bytes: ...
+    def consume_outgoing(self, amt: int) -> None: ...
+    @overload
+    def getpeercert(self, binary_form: Literal[False]) -> str: ...
+    @overload
+    def getpeercert(self, binary_form: Literal[True]) -> bytes: ...
+    def selected_npn_protocol(self) -> None: ...
+    def negotiated_protocol(self) -> str: ...
+    def cipher(self) -> bytes: ...
+    @property
+    def _handshake_state(self) -> HandshakeStep: ...
+    def do_handshake(self) -> None: ...
+    def negotiated_tls_version(self) -> Union[TLSVersion, DTLSVersion]: ...
+
+class TLSSession: ...
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/_tls.pyx` & `python-mbedtls-2.7.1/src/mbedtls/_tls.pyx`

 * *Files 14% similar despite different names*

```diff
@@ -1,1310 +1,1311 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2018, Mathias Laurin
-
-cimport libc.stdio as c_stdio
-from libc.stdlib cimport free, malloc
-
-cimport mbedtls._debug as _debug
-cimport mbedtls._random as _rnd
-cimport mbedtls._timing as _timing
-cimport mbedtls._tls as _tls
-cimport mbedtls.pk as _pk
-cimport mbedtls.x509 as _x509
-
-import enum
-from collections import abc
-from functools import partial
-from itertools import tee
-from pathlib import Path
-
-import certifi
-import cython
-
-import mbedtls._random as _rnd
-import mbedtls._ringbuf as _rb
-import mbedtls.exceptions as _exc
-import mbedtls.pk as _pk
-from mbedtls._tlsi import (
-    DTLSConfiguration,
-    DTLSVersion,
-    MaxFragmentLength,
-    NextProtocol,
-    TLSConfiguration,
-    TLSVersion,
-)
-
-
-cdef _rnd.Random __rng = _rnd.default_rng()
-
-
-class Transport(enum.Enum):
-    STREAM = _tls.MBEDTLS_SSL_TRANSPORT_STREAM
-    DATAGRAM = _tls.MBEDTLS_SSL_TRANSPORT_DATAGRAM
-
-
-cdef class _PSKSToreProxy:
-    def __init__(self, psk_store):
-        if not isinstance(psk_store, abc.Mapping):
-            raise TypeError("Mapping expected but got %r instead" % psk_store)
-        self._mapping = psk_store
-
-    def unwrap(self):
-        return self._mapping
-
-    def __repr__(self):
-        return "%s(%r)" % (type(self).__name__, self._mapping)
-
-    def __str__(self):
-        return self._mapping.__str__()
-
-    def __getitem__(self, key):
-        return self._mapping.__getitem__(key)
-
-    def __iter__(self):
-        return self._mapping.__iter__()
-
-    def __len__(self):
-        return self._mapping.__len__()
-
-
-# Python 2.7: `register()` can be used as a decorator from 3.3.
-abc.Mapping.register(_PSKSToreProxy)
-
-
-@cython.boundscheck(False)
-cdef void _my_debug(void *ctx, int level,
-                    const char *file, int line, const char *str) noexcept nogil:
-    c_stdio.fprintf(<c_stdio.FILE *> ctx, "%s:%04d: %s", file, line, str)
-    c_stdio.fflush(<c_stdio.FILE *> ctx)
-
-
-def _enable_debug_output(_BaseContext context):
-    _tls.mbedtls_ssl_conf_dbg(&context._conf._ctx, _my_debug, c_stdio.stdout)
-
-
-@cython.boundscheck(False)
-cdef int buffer_write(void *ctx, const unsigned char *buf, size_t len) noexcept nogil:
-    """"Write buffer to output buffer."""
-    c_buf = <_tls._C_Buffers *> ctx
-    if len == 0:
-        return _tls.MBEDTLS_ERR_SSL_BAD_INPUT_DATA
-    if _rb.c_len(c_buf.out_ctx) == _rb.c_capacity(c_buf.out_ctx):
-        return _tls.MBEDTLS_ERR_SSL_WANT_READ
-    cdef size_t writelen = min(
-        len, _rb.c_capacity(c_buf.out_ctx) - _rb.c_len(c_buf.out_ctx)
-    )
-    return _rb.c_write(c_buf.out_ctx, buf, writelen)
-
-
-@cython.boundscheck(False)
-cdef int buffer_read(void *ctx, unsigned char *buf, const size_t len) noexcept nogil:
-    """Read from input buffer."""
-    c_buf = <_tls._C_Buffers *> ctx
-    if _rb.c_len(c_buf.in_ctx) == 0:
-        return _tls.MBEDTLS_ERR_SSL_WANT_READ
-    return _rb.c_readinto(c_buf.in_ctx, buf, len)
-
-
-@cython.boundscheck(False)
-cdef int _psk_cb(
-    void *parameter,
-    _tls.mbedtls_ssl_context *ctx,
-    const unsigned char *c_identity,
-    size_t c_identity_len
-) noexcept nogil:
-    """Wrapper for the PSK callback."""
-    # If a valid PSK identity is found, call `mbedtls_ssl_set_hs_psk()` and
-    # return 0. Otherwise, return 1.
-    with gil:
-        store = <_tls._PSKSToreProxy> parameter
-        identity = c_identity[:c_identity_len]
-        try:
-            psk = store[identity.decode("utf8")]
-            _tls.mbedtls_ssl_set_hs_psk(ctx, psk, len(psk))
-            return 0
-        except Exception:
-            return 1
-
-
-def _set_debug_level(int level):
-    """Set debug level for logging."""
-    _debug.mbedtls_debug_set_threshold(level)
-
-
-def __get_ciphersuite_name(ciphersuite_id):
-    """Return a string containing the ciphersuite name.
-
-    Args:
-        ciphersuite_id: The ID of the ciphersuite.
-
-    """
-    return _tls.mbedtls_ssl_get_ciphersuite_name(
-        ciphersuite_id).decode("ascii")
-
-
-def __get_ciphersuite_id(name):
-    """Return the ciphersuite name from ID.
-
-    Args:
-        name (str): The name of the ciphersuite.
-
-    """
-    cdef char[:] c_name = bytearray(name.encode("ascii"))
-    return _tls.mbedtls_ssl_get_ciphersuite_id(&c_name[0])
-
-
-def pairwise(iterable):
-    "s -> (s0,s1), (s1,s2), (s2, s3), ..."
-    a, b = tee(iterable)
-    next(b, None)
-    return zip(a, b)
-
-
-def ciphers_available():
-    """Return the list of ciphersuites supported by the SSL/TLS module.
-
-    See Also:
-        - hashlib.algorithms_available
-        - hmac.algorithms_available
-
-    """
-    cdef const int* ids = _tls.mbedtls_ssl_list_ciphersuites()
-    cdef size_t n = 0
-    ciphersuites = []
-    while ids[n]:
-        ciphersuites.append(__get_ciphersuite_name(ids[n]))
-        n += 1
-    return tuple(ciphersuites)
-
-
-__TLSVersion = {
-    (0x02, 0x00): TLSVersion.SSLv2,
-    (0x03, 0x00): TLSVersion.SSLv3,
-    (0x03, 0x01): TLSVersion.TLSv1,
-    (0x03, 0x02): TLSVersion.TLSv1_1,
-    (0x03, 0x03): TLSVersion.TLSv1_2,
-    (0x03, 0x04): TLSVersion.TLSv1_3,
-}
-
-__DTLSVersion = {
-    (0x03, 0x02): DTLSVersion.DTLSv1_0,
-    (0x03, 0x03): DTLSVersion.DTLSv1_2,
-}
-
-
-def __to_version(maj_min_version, mapping):
-    try:
-        return mapping[maj_min_version]
-    except KeyError as exc:
-        raise ValueError(f"0x{maj_min_version[0]:02x}{maj_min_version[1]:02x}")
-
-
-def __from_version(version, mapping):
-    if not isinstance(version, (TLSVersion, DTLSVersion)):
-        raise TypeError(version)
-    try:
-        return {v: k for k, v in mapping.items()}[version]
-    except KeyError as exc:
-        raise ValueError(str(version)) from exc
-
-
-_tls_to_version = partial(__to_version, mapping=__TLSVersion)
-_dtls_to_version = partial(__to_version, mapping=__DTLSVersion)
-_tls_from_version = partial(__from_version, mapping=__TLSVersion)
-_dtls_from_version = partial(__from_version, mapping=__DTLSVersion)
-
-
-_SUPPORTED_TLS_VERSION = [
-    TLSVersion.TLSv1,
-    TLSVersion.TLSv1_1,
-    TLSVersion.TLSv1_2,
-    # TLSVersion.TLSv1_3,  # experimental in 2.28.0
-]
-
-
-_SUPPORTED_DTLS_VERSION = [
-    DTLSVersion.DTLSv1_0,
-    DTLSVersion.DTLSv1_2,
-]
-
-
-def _check_tls_version(version):
-    if not isinstance(version, TLSVersion):
-        raise TypeError(version)
-    if version is TLSVersion.MINIMUM_SUPPORTED:
-        version = _SUPPORTED_TLS_VERSION[0]
-    if version is TLSVersion.MAXIMUM_SUPPORTED:
-        version = _SUPPORTED_TLS_VERSION[-1]
-    if version not in _SUPPORTED_TLS_VERSION:
-        raise ValueError(version)
-    return version
-
-
-def _check_dtls_version(version):
-    if not isinstance(version, DTLSVersion):
-        raise TypeError(version)
-    if version is DTLSVersion.MINIMUM_SUPPORTED:
-        version = _SUPPORTED_DTLS_VERSION[0]
-    if version is DTLSVersion.MAXIMUM_SUPPORTED:
-        version = _SUPPORTED_DTLS_VERSION[-1]
-    if version not in _SUPPORTED_DTLS_VERSION:
-        raise ValueError(version)
-    return version
-
-
-class HandshakeStep(enum.Enum):
-    HELLO_REQUEST = _tls.MBEDTLS_SSL_HELLO_REQUEST
-    CLIENT_HELLO = _tls.MBEDTLS_SSL_CLIENT_HELLO
-    SERVER_HELLO = _tls.MBEDTLS_SSL_SERVER_HELLO
-    SERVER_CERTIFICATE = _tls.MBEDTLS_SSL_SERVER_CERTIFICATE
-    SERVER_KEY_EXCHANGE = _tls.MBEDTLS_SSL_SERVER_KEY_EXCHANGE
-    CERTIFICATE_REQUEST = _tls.MBEDTLS_SSL_CERTIFICATE_REQUEST
-    SERVER_HELLO_DONE = _tls.MBEDTLS_SSL_SERVER_HELLO_DONE
-    CLIENT_CERTIFICATE = _tls.MBEDTLS_SSL_CLIENT_CERTIFICATE
-    CLIENT_KEY_EXCHANGE = _tls.MBEDTLS_SSL_CLIENT_KEY_EXCHANGE
-    CERTIFICATE_VERIFY = _tls.MBEDTLS_SSL_CERTIFICATE_VERIFY
-    CLIENT_CHANGE_CIPHER_SPEC = _tls.MBEDTLS_SSL_CLIENT_CHANGE_CIPHER_SPEC
-    CLIENT_FINISHED = _tls.MBEDTLS_SSL_CLIENT_FINISHED
-    SERVER_CHANGE_CIPHER_SPEC = _tls.MBEDTLS_SSL_SERVER_CHANGE_CIPHER_SPEC
-    SERVER_FINISHED = _tls.MBEDTLS_SSL_SERVER_FINISHED
-    FLUSH_BUFFERS = _tls.MBEDTLS_SSL_FLUSH_BUFFERS
-    HANDSHAKE_WRAPUP = _tls.MBEDTLS_SSL_HANDSHAKE_WRAPUP
-    HANDSHAKE_OVER = _tls.MBEDTLS_SSL_HANDSHAKE_OVER
-    SERVER_NEW_SESSION_TICKET = _tls.MBEDTLS_SSL_SERVER_NEW_SESSION_TICKET
-    SERVER_HELLO_VERIFY_REQUEST_SENT = (
-        _tls.MBEDTLS_SSL_SERVER_HELLO_VERIFY_REQUEST_SENT
-    )
-
-
-PEM_HEADER = "-----BEGIN CERTIFICATE-----"
-PEM_FOOTER = "-----END CERTIFICATE-----"
-
-
-class WantWriteError(_exc.TLSError):
-    pass
-
-
-class WantReadError(_exc.TLSError):
-    pass
-
-
-class RaggedEOF(_exc.TLSError):
-    pass
-
-
-class HelloVerifyRequest(_exc.TLSError):
-    pass
-
-
-class TrustStore(abc.Sequence):
-    def __init__(self, db=None):
-        if db is None:
-            db = []
-        self._db = list(db)
-
-    def __repr__(self):
-        return "%s(%r)" % (type(self).__name__, self._db)
-
-    @classmethod
-    def system(cls):
-        return cls.from_pem_file(certifi.where())
-
-    @classmethod
-    def from_pem_file(cls, path):
-        self = cls()
-        with Path(path).open() as cacert:
-            pem = None
-            for line in cacert.readlines():
-                if line.startswith(PEM_HEADER):
-                    pem = []
-                elif line.strip().endswith(PEM_FOOTER):
-                    self.add(_x509.CRT.from_PEM("".join(pem)))
-                    pem = None
-                elif pem is not None:
-                    pem.append(line)
-        return self
-
-    def __eq__(self, other):
-        if type(other) is not type(self):
-            return NotImplemented
-        return self._db == other._db
-
-    def __bool__(self):
-        return bool(self._db)
-
-    def __len__(self):
-        return len(self._db)
-
-    def __getitem__(self, item):
-        if isinstance(item, slice):
-            return TrustStore(self._db[slice])
-        return self._db[item]
-
-    def add(self, _x509.CRT crt):
-        if crt in self:
-            return
-        cdef _x509.CRT c_crt
-        if self._db:
-            c_crt = self._db[-1]
-            c_crt.set_next(crt)
-        self._db.append(crt)
-
-
-class Purpose(enum.IntEnum):
-    SERVER_AUTH = _tls.MBEDTLS_SSL_IS_SERVER
-    CLIENT_AUTH = _tls.MBEDTLS_SSL_IS_CLIENT
-
-
-_DEFAULT_VALUE = object()
-
-
-cdef class _DTLSCookie:
-    """DTLS cookie."""
-
-    def __cinit__(self):
-        _tls.mbedtls_ssl_cookie_init(&self._ctx)
-
-    def __dealloc__(self):
-        _tls.mbedtls_ssl_cookie_free(&self._ctx)
-
-    @property
-    def timeout(self):
-        return self._ctx.timeout
-
-    @timeout.setter
-    def timeout(self, unsigned long timeout):
-        _tls.mbedtls_ssl_cookie_set_timeout(&self._ctx, timeout)
-
-    def generate(self):
-        """Generate keys."""
-        _tls.mbedtls_ssl_cookie_setup(
-            &self._ctx, _rnd.mbedtls_ctr_drbg_random, &__rng._ctx)
-
-
-cdef class MbedTLSConfiguration:
-
-    """(D)TLS configuration."""
-
-    def __init__(
-        self,
-        validate_certificates,
-        certificate_chain,
-        ciphers,
-        inner_protocols,
-        lowest_supported_version,
-        highest_supported_version,
-        trust_store,
-        max_fragmentation_length,
-        anti_replay,
-        # badmac_limit
-        handshake_timeout_min,
-        handshake_timeout_max,
-        sni_callback,
-        pre_shared_key,
-        pre_shared_key_store,
-        _transport,
-    ):
-        assert isinstance(_transport, Transport)
-        self._max_fragmentation_length = max_fragmentation_length
-        _exc.check_error(_tls.mbedtls_ssl_config_defaults(
-            &self._ctx,
-            endpoint=0,  # server / client is not known here...
-            transport=_transport.value,
-            preset=_tls.MBEDTLS_SSL_PRESET_DEFAULT))
-        self._set_validate_certificates(validate_certificates)
-        self._set_certificate_chain(certificate_chain)
-        self._set_ciphers(ciphers)
-        self._set_inner_protocols(inner_protocols)
-        self._set_lowest_supported_version(lowest_supported_version)
-        self._set_highest_supported_version(highest_supported_version)
-        self._set_trust_store(trust_store)
-        self._set_max_fragmentation_length(max_fragmentation_length)
-        self._set_anti_replay(anti_replay)
-        self._set_handshake_timeout(
-            handshake_timeout_min, handshake_timeout_max
-        )
-        self._set_sni_callback(sni_callback)
-        self._set_pre_shared_key(pre_shared_key)
-        self._set_pre_shared_key_store(pre_shared_key_store)
-
-        # Set random engine.
-        _tls.mbedtls_ssl_conf_rng(
-            &self._ctx, &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx)
-
-        # Disable renegotiation.
-        _tls.mbedtls_ssl_conf_renegotiation(&self._ctx, 0)
-
-        # For security reasons, we do not make cookie optional here.
-        cdef _tls._DTLSCookie cookie = _tls._DTLSCookie()
-        cookie.generate()
-        self._set_cookie(cookie)
-
-    def __cinit__(self):
-        _tls.mbedtls_ssl_config_init(&self._ctx)
-
-        cdef Py_ssize_t ciphers_sz = len(ciphers_available()) + 1
-        self._ciphers = <int *>malloc(ciphers_sz * sizeof(int))
-        if not self._ciphers:
-            raise MemoryError()
-
-        cdef Py_ssize_t idx = 0
-        for idx in range(ciphers_sz):
-            self._ciphers[idx] = 0
-
-        cdef Py_ssize_t protos_sz = len(NextProtocol) + 1
-        self._protos = <const char **>malloc(protos_sz * sizeof(char *))
-        if not self._protos:
-            raise MemoryError()
-
-        for idx in range(protos_sz):
-            self._protos[idx] = NULL
-
-    def __dealloc__(self):
-        _tls.mbedtls_ssl_config_free(&self._ctx)
-        free(self._ciphers)
-        free(self._protos)
-
-    def __reduce__(self):
-        return (
-            type(self),
-            (
-                self.validate_certificates,
-                self.certificate_chain,
-                self.ciphers,
-                self.inner_protocols,
-                self.lowest_supported_version,
-                self.highest_supported_version,
-                self.trust_store,
-                self.max_fragmentation_length,
-                self.anti_replay,
-                self.handshake_timeout_min,
-                self.handshake_timeout_max,
-                self.sni_callback,
-                self.pre_shared_key,
-                self.pre_shared_key_store,
-                self._transport,
-            ),
-        )
-
-    @property
-    def _transport(self):
-        return Transport(self._ctx.transport)
-
-    cdef _set_validate_certificates(self, validate):
-        """Set the certificate verification mode.
-
-        """  # PEP 543
-        if validate is None:
-            return
-        _tls.mbedtls_ssl_conf_authmode(
-            &self._ctx,
-            _tls.MBEDTLS_SSL_VERIFY_OPTIONAL if validate is False else
-            _tls.MBEDTLS_SSL_VERIFY_REQUIRED)
-
-    @property
-    def validate_certificates(self):
-        return self._ctx.authmode == _tls.MBEDTLS_SSL_VERIFY_REQUIRED
-
-    cdef _set_certificate_chain(self, chain):
-        """The certificate, intermediate certificate, and
-        the corresponding private key for the leaf certificate.
-
-        Args:
-            chain (Tuple[Tuple[Certificate], PrivateKey]):
-                The certificate chain.
-
-        """
-        # PEP 543
-        if not chain:
-            return
-        self._chain = chain
-        certs, pk_key = chain
-        if not certs or not pk_key:
-            return
-        cdef _x509.CRT c_crt, c_crt_next
-        for c_crt, c_crt_next in pairwise(certs):
-            c_crt.set_next(c_crt_next)
-        c_crt = certs[0]
-        c_pk_key = <_pk.CipherBase?> pk_key
-        _exc.check_error(_tls.mbedtls_ssl_conf_own_cert(
-            &self._ctx, &c_crt._ctx, &c_pk_key._ctx))
-
-    @property
-    def certificate_chain(self):
-        key_cert = self._ctx.key_cert
-        if key_cert is NULL:
-            return None
-        chain = []
-        cdef _x509.mbedtls_x509_crt *c_ctx = key_cert.cert
-        while c_ctx is not NULL:
-            chain.append(_x509.CRT.from_DER(c_ctx.raw.p[0:c_ctx.raw.len]))
-            c_ctx = c_ctx.next
-        cdef unsigned char[:] buf = bytearray(_pk.PRV_DER_MAX_BYTES)
-        olen = _exc.check_error(
-            _pk.mbedtls_pk_write_key_der(key_cert.key, &buf[0], buf.size))
-        der = buf[buf.size - olen:buf.size]
-        if _pk.mbedtls_pk_can_do(key_cert.key, _pk.MBEDTLS_PK_RSA) == 0:
-            return tuple(chain), _pk.ECC.from_DER(der)
-        return tuple(chain), _pk.RSA.from_DER(der)
-
-    cdef _set_ciphers(self, ciphers):
-        """The available ciphers for the TLS connections.
-
-        Args:
-            ciphers (Tuple[Union[CipherSuite, int]]): The ciphers.
-
-        """
-        # PEP 543
-        if ciphers is None:
-            return
-        if not frozenset(ciphers).issubset(ciphers_available()):
-            raise NotImplementedError("unsupported ciphers")
-        cdef Py_ssize_t idx = 0
-        self._ciphers[idx] = 0
-        for idx, cipher in enumerate(ciphers):
-            if not isinstance(cipher, int):
-                cipher = __get_ciphersuite_id(cipher)
-            self._ciphers[idx] = cipher
-        self._ciphers[idx + 1] = 0
-        _tls.mbedtls_ssl_conf_ciphersuites(&self._ctx, self._ciphers)
-
-    @property
-    def ciphers(self):
-        ciphers = []
-        cdef int cipher_id
-        cdef Py_ssize_t idx
-        for idx in range(len(ciphers_available())):
-            cipher_id = self._ciphers[idx]
-            if cipher_id == 0:
-                break
-            ciphers.append(__get_ciphersuite_name(cipher_id))
-        return tuple(ciphers)
-
-    cdef _set_inner_protocols(self, protocols):
-        """
-
-        Args:
-            protocols ([Tuple[Union[NextProtocol, bytes]]]): Protocols
-                that connections created with this configuration should
-                advertise as supported during the TLS handshake. These may
-                be advertised using either or both of ALPN or NPN. This
-                list of protocols should be ordered by preference.
-
-        """
-        # PEP 543
-        if protocols is None:
-            return
-        if len(protocols) > len(NextProtocol):
-            raise ValueError("invalid protocols")
-
-        cdef Py_ssize_t idx = 0
-        for idx, proto in enumerate(protocols):
-            if not isinstance(proto, bytes):
-                proto = proto.value
-            self._protos[idx] = proto
-        self._protos[idx + 1] = NULL
-
-        _exc.check_error(_tls.mbedtls_ssl_conf_alpn_protocols(
-            &self._ctx, self._protos))
-
-    @property
-    def inner_protocols(self):
-        protos = []
-        cdef const char* proto
-        for idx in range(len(NextProtocol)):
-            proto = self._protos[idx]
-            if proto is NULL:
-                break
-            protos.append(NextProtocol(proto))
-        return tuple(protos)
-
-    cdef _set_lowest_supported_version(self, version):
-        """The minimum version of TLS that should be allowed.
-
-        Args:
-            version (TLSVersion, or DTLSVersion): The minimum version.
-
-        """  # PEP 543
-        if self._transport is Transport.STREAM:
-            version = _check_tls_version(
-                version
-                if version is not None
-                else TLSVersion.MINIMUM_SUPPORTED
-            )
-        if self._transport is Transport.DATAGRAM:
-            version = _check_dtls_version(
-                version
-                if version is not None
-                else DTLSVersion.MINIMUM_SUPPORTED
-            )
-        try:
-            major, minor = {
-                TLSVersion: _tls_from_version,
-                DTLSVersion: _dtls_from_version,
-            }[type(version)](version)
-        except KeyError as exc:
-            raise TypeError(version) from exc
-
-        _tls.mbedtls_ssl_conf_min_version(&self._ctx, major, minor)
-
-    @property
-    def lowest_supported_version(self):
-        maj_min_version = self._ctx.min_major_ver, self._ctx.min_minor_ver
-        if self._transport is Transport.STREAM:
-            return _tls_to_version(maj_min_version)
-        if self._transport is Transport.DATAGRAM:
-            return _dtls_to_version(maj_min_version)
-        assert 0, "unreachable"
-
-    cdef _set_highest_supported_version(self, version):
-        """The maximum version of TLS that should be allowed.
-
-        Args:
-            version (TLSVersion, or DTLSVersion): The maximum version.
-
-        """  # PEP 543
-        if self._transport is Transport.STREAM:
-            version = _check_tls_version(
-                version
-                if version is not None
-                else TLSVersion.MAXIMUM_SUPPORTED
-            )
-        if self._transport is Transport.DATAGRAM:
-            version = _check_dtls_version(
-                version
-                if version is not None
-                else DTLSVersion.MAXIMUM_SUPPORTED
-            )
-        try:
-            major, minor = {
-                TLSVersion: _tls_from_version,
-                DTLSVersion: _dtls_from_version,
-            }[type(version)](version)
-        except KeyError as exc:
-            raise TypeError(version) from exc
-
-        _tls.mbedtls_ssl_conf_max_version(&self._ctx, major, minor)
-
-    @property
-    def highest_supported_version(self):
-        maj_min_version = self._ctx.max_major_ver, self._ctx.max_minor_ver
-        if self._transport is Transport.STREAM:
-            return _tls_to_version(maj_min_version)
-        if self._transport is Transport.DATAGRAM:
-            return _dtls_to_version(maj_min_version)
-        assert 0, "unreachable"
-
-    cdef _set_trust_store(self, store):
-        """The trust store that connections will use.
-
-        Args:
-            store (TrustStore): The trust store.
-
-        """
-        # PEP 543
-        if not store:
-            return
-        cdef _x509.CRT crt = TrustStore(store)[0]
-        mbedtls_ssl_conf_ca_chain(&self._ctx, &crt._ctx, NULL)
-
-    @property
-    def trust_store(self):
-        store = TrustStore()
-        if self._ctx.ca_chain is NULL:
-            return store
-
-        cdef _x509.mbedtls_x509_crt *c_ctx = self._ctx.ca_chain
-        while c_ctx is not NULL:
-            store.add(_x509.CRT.from_DER(c_ctx.raw.p[0:c_ctx.raw.len]))
-            c_ctx = c_ctx.next
-        return store
-
-    cdef _set_max_fragmentation_length(self, mfl):
-        if mfl is None:
-            return
-
-        if not isinstance(mfl, MaxFragmentLength):
-            raise TypeError(mfl)
-
-        try:
-            _exc.check_error(
-                _tls.mbedtls_ssl_conf_max_frag_len(&self._ctx, mfl.value)
-            )
-        except _exc.TLSError as exc:
-            raise ValueError(mfl) from exc
-
-    @property
-    def max_fragmentation_length(self):
-        # No accessor in backend.
-        return self._max_fragmentation_length
-
-    cdef _set_anti_replay(self, anti_replay):
-        """Set anti replay."""
-        if anti_replay is None:
-            return
-        if self._transport is Transport.STREAM:
-            # not available with TLS
-            raise ValueError(anti_replay)
-        _tls.mbedtls_ssl_conf_dtls_anti_replay(
-            &self._ctx,
-            _tls.MBEDTLS_SSL_ANTI_REPLAY_ENABLED
-            if anti_replay else
-            _tls.MBEDTLS_SSL_ANTI_REPLAY_DISABLED)
-
-    @property
-    def anti_replay(self):
-        if self._transport is Transport.STREAM:
-            return None
-
-        cdef unsigned int enabled = _tls.MBEDTLS_SSL_ANTI_REPLAY_ENABLED
-        return True if self._ctx.anti_replay == enabled else False
-
-    cdef _set_handshake_timeout(self, minimum, maximum):
-        """Set DTLS handshake timeout.
-
-        Args:
-            minimum (float, optional): minimum timeout in seconds.
-            maximum (float, optional): maximum timeout in seconds.
-
-        """
-        if minimum is None and maximum is None:
-            return
-        if self._transport is Transport.STREAM:
-            # not available with TLS
-            raise ValueError((minimum, maximum))
-
-        def validate(extremum, *, default: float) -> float:
-            if extremum is None:
-                return default
-            if extremum < 0.0:
-                raise ValueError(extremum)
-            return extremum
-
-        _tls.mbedtls_ssl_conf_handshake_timeout(
-            &self._ctx,
-            int(1000.0 * validate(minimum, default=1.0)),
-            int(1000.0 * validate(maximum, default=60.0)),
-        )
-
-    @property
-    def handshake_timeout_min(self):
-        """Min handshake timeout in seconds (default 1.0)."""
-        if self._transport is Transport.STREAM:
-            return None
-
-        return float(self._ctx.hs_timeout_min) / 1000.0
-
-    @property
-    def handshake_timeout_max(self):
-        """Max handshake timeout in seconds (default 60.0)."""
-        if self._transport is Transport.STREAM:
-            return None
-
-        return float(self._ctx.hs_timeout_max) / 1000.0
-
-    cdef _set_sni_callback(self, callback):
-        # PEP 543, optional, server-side only
-        if callback is None:
-            return
-        # mbedtls_ssl_conf_sni
-        raise NotImplementedError
-
-    @property
-    def sni_callback(self):
-        return None
-
-    cdef _set_pre_shared_key(self, psk):
-        """Set a pre shared key (PSK) for the client.
-
-        Args:
-            psk ([Tuple[unicode, bytes]]): A tuple with the key and the exected
-                identity name.
-
-        """
-        if psk is None:
-            return
-        try:
-            identity, key = psk
-        except ValueError:
-            raise TypeError("expected a tuple (name, key)")
-        c_identity = identity.encode("utf8")
-        _exc.check_error(_tls.mbedtls_ssl_conf_psk(
-            &self._ctx,
-            key, len(key),
-            c_identity, len(c_identity)))
-
-    @property
-    def pre_shared_key(self):
-        if self._ctx.psk == NULL or self._ctx.psk_identity == NULL:
-            return None
-        key = self._ctx.psk[:self._ctx.psk_len]
-        c_identity = self._ctx.psk_identity[:self._ctx.psk_identity_len]
-        identity = c_identity.decode("utf8")
-        return (identity, key)
-
-    cdef _set_pre_shared_key_store(self, psk_store):
-        # server-side
-        if psk_store is None:
-            return
-        self._store = _PSKSToreProxy(psk_store)  # ownership
-        _tls.mbedtls_ssl_conf_psk_cb(&self._ctx, _psk_cb, <void *> self._store)
-
-    @property
-    def pre_shared_key_store(self):
-        if self._ctx.p_psk == NULL:
-            return None
-        psk_store = <_tls._PSKSToreProxy> self._ctx.p_psk
-        return psk_store.unwrap()
-
-    cdef _set_cookie(self, _tls._DTLSCookie cookie):
-        """Register callbacks for DTLS cookies (server only)."""
-        self._cookie = cookie
-        if cookie is None:
-            _tls.mbedtls_ssl_conf_dtls_cookies(
-                &self._ctx,
-                NULL,
-                NULL,
-                NULL,
-            )
-        else:
-            _tls.mbedtls_ssl_conf_dtls_cookies(
-                &self._ctx,
-                _tls.mbedtls_ssl_cookie_write,
-                _tls.mbedtls_ssl_cookie_check,
-                &self._cookie._ctx,
-            )
-
-
-DEFAULT_CIPHER_LIST = None
-
-
-cdef class TLSSession:
-    def __cinit__(self):
-        """Initialize SSL session structure."""
-        _tls.mbedtls_ssl_session_init(&self._ctx)
-
-    def __dealloc__(self):
-        """Free referenced items in an SSL session."""
-        _tls.mbedtls_ssl_session_free(&self._ctx)
-
-    def __getstate__(self):
-        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
-
-    def __repr__(self):
-        return "%s()" % type(self).__name__
-
-
-cdef class _BaseContext:
-    # _pep543._BaseContext
-    """Context base class."""
-
-    def __init__(self, configuration not None):
-        if isinstance(configuration, TLSConfiguration):
-            self._conf = MbedTLSConfiguration(
-                validate_certificates=configuration.validate_certificates,
-                certificate_chain=configuration.certificate_chain,
-                ciphers=configuration.ciphers,
-                inner_protocols=configuration.inner_protocols,
-                lowest_supported_version=(
-                    configuration.lowest_supported_version
-                ),
-                highest_supported_version=(
-                    configuration.highest_supported_version
-                ),
-                trust_store=configuration.trust_store,
-                max_fragmentation_length=configuration.max_fragmentation_length,
-                anti_replay=None,
-                handshake_timeout_min=None,
-                handshake_timeout_max=None,
-                sni_callback=configuration.sni_callback,
-                pre_shared_key=configuration.pre_shared_key,
-                pre_shared_key_store=configuration.pre_shared_key_store,
-                _transport=Transport.STREAM,
-            )
-        elif isinstance(configuration, DTLSConfiguration):
-            self._conf = MbedTLSConfiguration(
-                validate_certificates=configuration.validate_certificates,
-                certificate_chain=configuration.certificate_chain,
-                ciphers=configuration.ciphers,
-                inner_protocols=configuration.inner_protocols,
-                lowest_supported_version=(
-                    configuration.lowest_supported_version
-                ),
-                highest_supported_version=(
-                    configuration.highest_supported_version
-                ),
-                trust_store=configuration.trust_store,
-                max_fragmentation_length=configuration.max_fragmentation_length,
-                anti_replay=configuration.anti_replay,
-                handshake_timeout_min=configuration.handshake_timeout_min,
-                handshake_timeout_max=configuration.handshake_timeout_max,
-                sni_callback=configuration.sni_callback,
-                pre_shared_key=configuration.pre_shared_key,
-                pre_shared_key_store=configuration.pre_shared_key_store,
-                _transport=Transport.DATAGRAM,
-            )
-        else:
-            # Setting `_conf` is required for delocate on macOS.
-            self._conf = None
-            raise TypeError(configuration)
-
-        _tls.mbedtls_ssl_conf_endpoint(
-            &self._conf._ctx,
-            {
-                Purpose.CLIENT_AUTH: _tls.MBEDTLS_SSL_IS_CLIENT,
-                Purpose.SERVER_AUTH: _tls.MBEDTLS_SSL_IS_SERVER,
-            }[self._purpose])
-
-    def __eq__(self, other):
-        if not isinstance(other, type(self)):
-            return False
-        if not type(self) is type(other):
-            return False
-        return self.configuration == other.configuration
-
-    @property
-    def configuration(self):
-        if self._conf._transport is Transport.STREAM:
-            return TLSConfiguration(
-                validate_certificates=self._conf.validate_certificates,
-                certificate_chain=self._conf.certificate_chain,
-                ciphers=self._conf.ciphers,
-                inner_protocols=self._conf.inner_protocols,
-                lowest_supported_version=self._conf.lowest_supported_version,
-                highest_supported_version=self._conf.highest_supported_version,
-                trust_store=self._conf.trust_store,
-                max_fragmentation_length=self._conf.max_fragmentation_length,
-                sni_callback=self._conf.sni_callback,
-                pre_shared_key=self._conf.pre_shared_key,
-                pre_shared_key_store=self._conf.pre_shared_key_store,
-            )
-        assert self._conf._transport is Transport.DATAGRAM
-        return DTLSConfiguration(
-            validate_certificates=self._conf.validate_certificates,
-            certificate_chain=self._conf.certificate_chain,
-            ciphers=self._conf.ciphers,
-            inner_protocols=self._conf.inner_protocols,
-            lowest_supported_version=self._conf.lowest_supported_version,
-            highest_supported_version=self._conf.highest_supported_version,
-            trust_store=self._conf.trust_store,
-            max_fragmentation_length=self._conf.max_fragmentation_length,
-            anti_replay=self._conf.anti_replay,
-            handshake_timeout_min=self._conf.handshake_timeout_min,
-            handshake_timeout_max=self._conf.handshake_timeout_max,
-            sni_callback=self._conf.sni_callback,
-            pre_shared_key=self._conf.pre_shared_key,
-            pre_shared_key_store=self._conf.pre_shared_key_store,
-        )
-
-    @property
-    def _purpose(self) -> Purpose:
-        raise NotImplementedError
-
-
-TLS_BUFFER_CAPACITY = 2 << 14
-# 32K (MBEDTLS_SSL_DTLS_MAX_BUFFERING)
-
-
-cdef class MbedTLSBuffer:
-    def __init__(self, _BaseContext context, server_hostname=None):
-        self._context = context
-        _exc.check_error(
-            _tls.mbedtls_ssl_setup(&self._ctx, &self._context._conf._ctx)
-        )
-        self._c_output_buffer = _rb.RingBuffer(TLS_BUFFER_CAPACITY)
-        self._c_input_buffer = _rb.RingBuffer(TLS_BUFFER_CAPACITY)
-        self._c_buffers = _tls._C_Buffers(
-            &self._c_output_buffer._ctx,
-            &self._c_input_buffer._ctx
-        )
-        self._reset()
-        _tls.mbedtls_ssl_set_bio(
-            &self._ctx,
-            &self._c_buffers,
-            buffer_write,
-            buffer_read,
-            NULL
-        )
-        self._set_hostname(server_hostname)
-
-    def __cinit__(self):
-        """Initialize an `ssl_context`."""
-        _tls.mbedtls_ssl_init(&self._ctx)
-        _tls.mbedtls_ssl_set_timer_cb(
-            &self._ctx,
-            &self._timer,
-            _timing.mbedtls_timing_set_delay,
-            _timing.mbedtls_timing_get_delay)
-
-    def __dealloc__(self):
-        """Free and clear the internal structures of ctx."""
-        _tls.mbedtls_ssl_free(&self._ctx)
-
-    def __getstate__(self):
-        cdef size_t olen = 0
-        ret = mbedtls_ssl_context_save(&self._ctx, NULL, 0, &olen)
-        if ret != -0x6A00 or olen == 0:
-            # 0x6A00: MBEDTLS_ERR_SSL_BUFFER_TOO_SMALL
-            raise TypeError(
-                f"cannot pickle {self.__class__.__name__!r} object {hex(ret)}"
-            )
-        cdef unsigned char *c_buf = <unsigned char *> malloc(olen)
-        if not c_buf:
-            raise MemoryError()
-        try:
-            if mbedtls_ssl_context_save(&self._ctx, c_buf, olen, &olen) != 0:
-                raise TypeError(
-                    f"cannot pickle {self.__class__.__name__!r} object"
-                )
-            return {
-                "connection": c_buf[:olen],
-                "context": self.context,
-                "server_hostname": self._server_hostname,
-            }
-        finally:
-            free(c_buf)
-
-    def __setstate__(self, state):
-        self.__init__(state["context"], state["server_hostname"])
-        cdef const unsigned char[:] buf = state["connection"]
-        ret = mbedtls_ssl_context_load(&self._ctx, &buf[0], buf.size)
-        if ret != 0:
-            self._reset()
-            raise TypeError(
-                f"cannot unpickle {self.__class__.__name__!r} object"
-            )
-
-    def __repr__(self):
-        return "%s(%r)" % (type(self).__name__, self.context)
-
-    @property
-    def _input_buffer(self):
-        return self._c_input_buffer
-
-    @property
-    def _output_buffer(self):
-        return self._c_output_buffer
-
-    @property
-    def context(self):
-        return self._context
-
-    @property
-    def _verified(self):
-        return _tls.mbedtls_ssl_get_verify_result(&self._ctx) == 0
-
-    @property
-    def _server_hostname(self):
-        # Client side
-        if self._ctx.hostname is NULL:
-            return None
-        return (<bytes> self._ctx.hostname).decode("utf8")
-
-    def _set_hostname(self, hostname):
-        """Set the hostname to check against the received server."""
-        if hostname is None:
-            return
-        # Note: `ssl_set_hostname()` makes a copy so it is safe
-        #       to call with the temporary `hostname_`.
-        hostname_ = hostname.encode("utf8")
-        cdef const char* c_hostname = hostname_
-        _exc.check_error(_tls.mbedtls_ssl_set_hostname(&self._ctx, c_hostname))
-
-    @property
-    def _cookieparam(self):
-        """Client ID for the HelloVerifyRequest.
-
-        Note:
-            Server-side, DTLS only.
-
-        """
-        client_id = bytes(self._ctx.cli_id[0:self._ctx.cli_id_len])
-        return client_id if client_id else None
-
-    def setcookieparam(self, const unsigned char[:] info not None):
-        if info.size == 0:
-            info = b"\0"
-        _tls.mbedtls_ssl_set_client_transport_id(
-            &self._ctx,
-            &info[0],
-            info.size,
-        )
-
-    def setmtu(self, mtu):
-        """Set Maxiumum Transport Unit (MTU) for DTLS.
-
-        Set to zero to unset.
-
-        Raises:
-            OverflowError: If value cannot be converted to UInt16.
-
-        """
-        # DTLS
-        if not isinstance(mtu, int):
-            raise TypeError(mtu)
-        _tls.mbedtls_ssl_set_mtu(&self._ctx, mtu)
-
-    def _reset(self):
-        _exc.check_error(_tls.mbedtls_ssl_session_reset(&self._ctx))
-
-    def shutdown(self):
-        # No error handling:  The connection may be closed already.
-        _tls.mbedtls_ssl_close_notify(&self._ctx)
-        self._reset()
-
-    def _close(self):
-        self.shutdown()
-
-    def read(self, amt):
-        # PEP 543
-        if amt <= 0:
-            return b""
-        buffer = bytearray(amt)
-        view = memoryview(buffer)
-        nread = 0
-        while nread != amt and not self._input_buffer.empty():
-            nread += self.readinto(view[nread:], amt - nread)
-        return bytes(buffer[:nread])
-
-    def readinto(self, unsigned char[:] buffer not None, size_t amt):
-        if buffer.size == 0:
-            return 0
-        if amt <= 0:
-            return 0
-        read = _tls.mbedtls_ssl_read(&self._ctx, &buffer[0], amt)
-        if read > 0:
-            return read
-        if read == 0:
-            raise RaggedEOF()
-        if read == _tls.MBEDTLS_ERR_SSL_WANT_READ:
-            raise WantReadError()
-        if read == _tls.MBEDTLS_ERR_SSL_WANT_WRITE:
-            raise WantWriteError()
-        if read == _tls.MBEDTLS_ERR_SSL_CLIENT_RECONNECT:
-            _exc.check_error(read)  # raises
-            assert 0, "unreachable"
-        self._reset()
-        _exc.check_error(read)  # raises
-        assert 0, "unreachable"
-
-    def write(self, const unsigned char[:] buffer not None):
-        if buffer.size == 0:
-            return 0
-        cdef size_t written = 0
-        while written != buffer.size:
-            ret = _tls.mbedtls_ssl_write(
-                &self._ctx, &buffer[written], buffer.size - written)
-            if ret >= 0:
-                written += ret
-            elif ret == _tls.MBEDTLS_ERR_SSL_WANT_READ:
-                raise WantReadError()
-            elif ret == _tls.MBEDTLS_ERR_SSL_WANT_WRITE:
-                raise WantWriteError()
-            else:
-                self._reset()
-                _exc.check_error(ret)
-        assert written == len(buffer)
-        return len(self._output_buffer)
-
-    def receive_from_network(self, data):
-        # PEP 543
-        # Append data to input buffer.
-        self._input_buffer.write(data, len(data))
-
-    def peek_outgoing(self, amt):
-        # PEP 543
-        # Read from output buffer.
-        if amt == 0:
-            return b""
-        return self._output_buffer.peek(amt)
-
-    def consume_outgoing(self, amt):
-        """Consume `amt` bytes from the output buffer."""
-        # PEP 543
-        self._output_buffer.consume(amt)
-
-    def getpeercert(self, binary_form=False):
-        """Return the peer certificate, or None."""
-        c_crt = _tls.mbedtls_ssl_get_peer_cert(&self._ctx)
-        if c_crt is NULL:
-            return None
-
-        # See `CRT.to_DER()`.
-        der = bytes(c_crt.raw.p[0:c_crt.raw.len])
-        if binary_form:
-            return der
-        return _x509.CRT.from_DER(der)
-
-    def selected_npn_protocol(self):
-        return None
-
-    def negotiated_protocol(self):
-        cdef const char* protocol = _tls.mbedtls_ssl_get_alpn_protocol(
-            &self._ctx)
-        if protocol is NULL:
-            return None
-        return protocol.decode("ascii")
-
-    def _cipher_suite(self):
-        cdef const char* name = _tls.mbedtls_ssl_get_ciphersuite(&self._ctx)
-        if name is NULL:
-            return None
-        ssl_version = self.negotiated_tls_version()
-        secret_bits = None
-        return name.decode("ascii"), ssl_version, secret_bits
-
-    def cipher(self):
-        cipher = self._cipher_suite()
-        if cipher is None:
-            return
-        return cipher[0]
-
-    @property
-    def _handshake_state(self):
-        return HandshakeStep(self._ctx.state)
-
-    def do_handshake(self):
-        self._handle_handshake_response(
-            _tls.mbedtls_ssl_handshake_step(&self._ctx)
-        )
-
-    def _renegotiate(self):
-        """Initialize an SSL renegotiation on the running connection."""
-        self._handle_handshake_response(
-            _tls.mbedtls_ssl_renegotiate(&self._ctx)
-        )
-
-    def _handle_handshake_response(self, ret):
-        if ret == _tls.MBEDTLS_ERR_SSL_WANT_READ:
-            raise WantReadError()
-        if ret == _tls.MBEDTLS_ERR_SSL_WANT_WRITE:
-            raise WantWriteError()
-        if ret == _tls.MBEDTLS_ERR_SSL_HELLO_VERIFY_REQUIRED:
-            self._reset()
-            raise HelloVerifyRequest()
-        if (
-            ret == -0x7100
-            and self._handshake_state is HandshakeStep.HANDSHAKE_OVER
-        ):
-            raise ValueError("handshake already over")
-        if ret < 0:
-            self._reset()
-            _exc.check_error(ret)
-        if ret == 0 and self._output_buffer:
-            raise WantWriteError
-        assert ret == 0
-
-    def _get_channel_binding(self, cb_type="tls-unique"):
-        return None
-
-    def negotiated_tls_version(self):
-        # Strings from `ssl_tls.c`.
-        return {
-            "DTLSv1.0": DTLSVersion.DTLSv1_0,
-            "DTLSv1.2": DTLSVersion.DTLSv1_2,
-            # "SSLv3.0": TLSVersion.SSLv3,
-            "TLSv1.0": TLSVersion.TLSv1,
-            "TLSv1.1": TLSVersion.TLSv1_1,
-            "TLSv1.2": TLSVersion.TLSv1_2,
-            "TLSV1.3": TLSVersion.TLSv1_3,
-        }.get(_tls.mbedtls_ssl_get_version(&self._ctx).decode("ascii"))
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2018, Mathias Laurin
+
+cimport libc.stdio as c_stdio
+from libc.stdlib cimport free, malloc
+
+cimport mbedtls._debug as _debug
+cimport mbedtls._random as _rnd
+cimport mbedtls._timing as _timing
+cimport mbedtls._tls as _tls
+cimport mbedtls.pk as _pk
+cimport mbedtls.x509 as _x509
+
+import enum
+from collections import abc
+from functools import partial
+from itertools import tee
+from pathlib import Path
+
+import certifi
+import cython
+
+import mbedtls._random as _rnd
+import mbedtls._ringbuf as _rb
+import mbedtls.exceptions as _exc
+import mbedtls.pk as _pk
+from mbedtls._tlsi import (
+    DTLSConfiguration,
+    DTLSVersion,
+    MaxFragmentLength,
+    NextProtocol,
+    TLSConfiguration,
+    TLSVersion,
+)
+
+
+cdef _rnd.Random __rng = _rnd.default_rng()
+
+
+class Transport(enum.Enum):
+    STREAM = _tls.MBEDTLS_SSL_TRANSPORT_STREAM
+    DATAGRAM = _tls.MBEDTLS_SSL_TRANSPORT_DATAGRAM
+
+
+cdef class _PSKSToreProxy:
+    def __init__(self, psk_store):
+        if not isinstance(psk_store, abc.Mapping):
+            raise TypeError("Mapping expected but got %r instead" % psk_store)
+        self._mapping = psk_store
+
+    def unwrap(self):
+        return self._mapping
+
+    def __repr__(self):
+        return "%s(%r)" % (type(self).__name__, self._mapping)
+
+    def __str__(self):
+        return self._mapping.__str__()
+
+    def __getitem__(self, key):
+        return self._mapping.__getitem__(key)
+
+    def __iter__(self):
+        return self._mapping.__iter__()
+
+    def __len__(self):
+        return self._mapping.__len__()
+
+
+# Python 2.7: `register()` can be used as a decorator from 3.3.
+abc.Mapping.register(_PSKSToreProxy)
+
+
+@cython.boundscheck(False)
+cdef void _my_debug(void *ctx, int level,
+                    const char *file, int line, const char *str) noexcept nogil:
+    c_stdio.fprintf(<c_stdio.FILE *> ctx, "%s:%04d: %s", file, line, str)
+    c_stdio.fflush(<c_stdio.FILE *> ctx)
+
+
+def _enable_debug_output(_BaseContext context):
+    _tls.mbedtls_ssl_conf_dbg(&context._conf._ctx, _my_debug, c_stdio.stdout)
+
+
+@cython.boundscheck(False)
+cdef int buffer_write(void *ctx, const unsigned char *buf, size_t len) noexcept nogil:
+    """"Write buffer to output buffer."""
+    c_buf = <_tls._C_Buffers *> ctx
+    if len == 0:
+        return _tls.MBEDTLS_ERR_SSL_BAD_INPUT_DATA
+    if _rb.c_len(c_buf.out_ctx) == _rb.c_capacity(c_buf.out_ctx):
+        return _tls.MBEDTLS_ERR_SSL_WANT_READ
+    cdef size_t writelen = min(
+        len, _rb.c_capacity(c_buf.out_ctx) - _rb.c_len(c_buf.out_ctx)
+    )
+    return _rb.c_write(c_buf.out_ctx, buf, writelen)
+
+
+@cython.boundscheck(False)
+cdef int buffer_read(void *ctx, unsigned char *buf, const size_t len) noexcept nogil:
+    """Read from input buffer."""
+    c_buf = <_tls._C_Buffers *> ctx
+    if _rb.c_len(c_buf.in_ctx) == 0:
+        return _tls.MBEDTLS_ERR_SSL_WANT_READ
+    return _rb.c_readinto(c_buf.in_ctx, buf, len)
+
+
+@cython.boundscheck(False)
+cdef int _psk_cb(
+    void *parameter,
+    _tls.mbedtls_ssl_context *ctx,
+    const unsigned char *c_identity,
+    size_t c_identity_len
+) noexcept nogil:
+    """Wrapper for the PSK callback."""
+    # If a valid PSK identity is found, call `mbedtls_ssl_set_hs_psk()` and
+    # return 0. Otherwise, return 1.
+    with gil:
+        store = <_tls._PSKSToreProxy> parameter
+        identity = c_identity[:c_identity_len]
+        try:
+            psk = store[identity.decode("utf8")]
+            _tls.mbedtls_ssl_set_hs_psk(ctx, psk, len(psk))
+            return 0
+        except Exception:
+            return 1
+
+
+def _set_debug_level(int level):
+    """Set debug level for logging."""
+    _debug.mbedtls_debug_set_threshold(level)
+
+
+def __get_ciphersuite_name(ciphersuite_id):
+    """Return a string containing the ciphersuite name.
+
+    Args:
+        ciphersuite_id: The ID of the ciphersuite.
+
+    """
+    return _tls.mbedtls_ssl_get_ciphersuite_name(
+        ciphersuite_id).decode("ascii")
+
+
+def __get_ciphersuite_id(name):
+    """Return the ciphersuite name from ID.
+
+    Args:
+        name (str): The name of the ciphersuite.
+
+    """
+    cdef char[:] c_name = bytearray(name.encode("ascii"))
+    return _tls.mbedtls_ssl_get_ciphersuite_id(&c_name[0])
+
+
+def pairwise(iterable):
+    "s -> (s0,s1), (s1,s2), (s2, s3), ..."
+    a, b = tee(iterable)
+    next(b, None)
+    return zip(a, b)
+
+
+def ciphers_available():
+    """Return the list of ciphersuites supported by the SSL/TLS module.
+
+    See Also:
+        - hashlib.algorithms_available
+        - hmac.algorithms_available
+
+    """
+    cdef const int* ids = _tls.mbedtls_ssl_list_ciphersuites()
+    cdef size_t n = 0
+    ciphersuites = []
+    while ids[n]:
+        ciphersuites.append(__get_ciphersuite_name(ids[n]))
+        n += 1
+    return tuple(ciphersuites)
+
+
+__TLSVersion = {
+    (0x02, 0x00): TLSVersion.SSLv2,
+    (0x03, 0x00): TLSVersion.SSLv3,
+    (0x03, 0x01): TLSVersion.TLSv1,
+    (0x03, 0x02): TLSVersion.TLSv1_1,
+    (0x03, 0x03): TLSVersion.TLSv1_2,
+    (0x03, 0x04): TLSVersion.TLSv1_3,
+}
+
+__DTLSVersion = {
+    (0x03, 0x02): DTLSVersion.DTLSv1_0,
+    (0x03, 0x03): DTLSVersion.DTLSv1_2,
+}
+
+
+def __to_version(maj_min_version, mapping):
+    try:
+        return mapping[maj_min_version]
+    except KeyError as exc:
+        raise ValueError(f"0x{maj_min_version[0]:02x}{maj_min_version[1]:02x}")
+
+
+def __from_version(version, mapping):
+    if not isinstance(version, (TLSVersion, DTLSVersion)):
+        raise TypeError(version)
+    try:
+        return {v: k for k, v in mapping.items()}[version]
+    except KeyError as exc:
+        raise ValueError(str(version)) from exc
+
+
+_tls_to_version = partial(__to_version, mapping=__TLSVersion)
+_dtls_to_version = partial(__to_version, mapping=__DTLSVersion)
+_tls_from_version = partial(__from_version, mapping=__TLSVersion)
+_dtls_from_version = partial(__from_version, mapping=__DTLSVersion)
+
+
+_SUPPORTED_TLS_VERSION = [
+    TLSVersion.TLSv1,
+    TLSVersion.TLSv1_1,
+    TLSVersion.TLSv1_2,
+    # TLSVersion.TLSv1_3,  # experimental in 2.28.0
+]
+
+
+_SUPPORTED_DTLS_VERSION = [
+    DTLSVersion.DTLSv1_0,
+    DTLSVersion.DTLSv1_2,
+]
+
+
+def _check_tls_version(version):
+    if not isinstance(version, TLSVersion):
+        raise TypeError(version)
+    if version is TLSVersion.MINIMUM_SUPPORTED:
+        version = _SUPPORTED_TLS_VERSION[0]
+    if version is TLSVersion.MAXIMUM_SUPPORTED:
+        version = _SUPPORTED_TLS_VERSION[-1]
+    if version not in _SUPPORTED_TLS_VERSION:
+        raise ValueError(version)
+    return version
+
+
+def _check_dtls_version(version):
+    if not isinstance(version, DTLSVersion):
+        raise TypeError(version)
+    if version is DTLSVersion.MINIMUM_SUPPORTED:
+        version = _SUPPORTED_DTLS_VERSION[0]
+    if version is DTLSVersion.MAXIMUM_SUPPORTED:
+        version = _SUPPORTED_DTLS_VERSION[-1]
+    if version not in _SUPPORTED_DTLS_VERSION:
+        raise ValueError(version)
+    return version
+
+
+class HandshakeStep(enum.Enum):
+    HELLO_REQUEST = _tls.MBEDTLS_SSL_HELLO_REQUEST
+    CLIENT_HELLO = _tls.MBEDTLS_SSL_CLIENT_HELLO
+    SERVER_HELLO = _tls.MBEDTLS_SSL_SERVER_HELLO
+    SERVER_CERTIFICATE = _tls.MBEDTLS_SSL_SERVER_CERTIFICATE
+    SERVER_KEY_EXCHANGE = _tls.MBEDTLS_SSL_SERVER_KEY_EXCHANGE
+    CERTIFICATE_REQUEST = _tls.MBEDTLS_SSL_CERTIFICATE_REQUEST
+    SERVER_HELLO_DONE = _tls.MBEDTLS_SSL_SERVER_HELLO_DONE
+    CLIENT_CERTIFICATE = _tls.MBEDTLS_SSL_CLIENT_CERTIFICATE
+    CLIENT_KEY_EXCHANGE = _tls.MBEDTLS_SSL_CLIENT_KEY_EXCHANGE
+    CERTIFICATE_VERIFY = _tls.MBEDTLS_SSL_CERTIFICATE_VERIFY
+    CLIENT_CHANGE_CIPHER_SPEC = _tls.MBEDTLS_SSL_CLIENT_CHANGE_CIPHER_SPEC
+    CLIENT_FINISHED = _tls.MBEDTLS_SSL_CLIENT_FINISHED
+    SERVER_CHANGE_CIPHER_SPEC = _tls.MBEDTLS_SSL_SERVER_CHANGE_CIPHER_SPEC
+    SERVER_FINISHED = _tls.MBEDTLS_SSL_SERVER_FINISHED
+    FLUSH_BUFFERS = _tls.MBEDTLS_SSL_FLUSH_BUFFERS
+    HANDSHAKE_WRAPUP = _tls.MBEDTLS_SSL_HANDSHAKE_WRAPUP
+    HANDSHAKE_OVER = _tls.MBEDTLS_SSL_HANDSHAKE_OVER
+    SERVER_NEW_SESSION_TICKET = _tls.MBEDTLS_SSL_SERVER_NEW_SESSION_TICKET
+    SERVER_HELLO_VERIFY_REQUEST_SENT = (
+        _tls.MBEDTLS_SSL_SERVER_HELLO_VERIFY_REQUEST_SENT
+    )
+
+
+PEM_HEADER = "-----BEGIN CERTIFICATE-----"
+PEM_FOOTER = "-----END CERTIFICATE-----"
+
+
+class WantWriteError(_exc.TLSError):
+    pass
+
+
+class WantReadError(_exc.TLSError):
+    pass
+
+
+class RaggedEOF(_exc.TLSError):
+    pass
+
+
+class HelloVerifyRequest(_exc.TLSError):
+    pass
+
+
+class TrustStore(abc.Sequence):
+    def __init__(self, db=None):
+        if db is None:
+            db = []
+        self._db = list(db)
+
+    def __repr__(self):
+        return "%s(%r)" % (type(self).__name__, self._db)
+
+    @classmethod
+    def system(cls):
+        return cls.from_pem_file(certifi.where())
+
+    @classmethod
+    def from_pem_file(cls, path):
+        self = cls()
+        with Path(path).open() as cacert:
+            pem = None
+            for line in cacert.readlines():
+                if line.startswith(PEM_HEADER):
+                    pem = []
+                elif line.strip().endswith(PEM_FOOTER):
+                    self.add(_x509.CRT.from_PEM("".join(pem)))
+                    pem = None
+                elif pem is not None:
+                    pem.append(line)
+        return self
+
+    def __eq__(self, other):
+        if type(other) is not type(self):
+            return NotImplemented
+        return self._db == other._db
+
+    def __bool__(self):
+        return bool(self._db)
+
+    def __len__(self):
+        return len(self._db)
+
+    def __getitem__(self, item):
+        if isinstance(item, slice):
+            return TrustStore(self._db[slice])
+        return self._db[item]
+
+    def add(self, _x509.CRT crt):
+        if crt in self:
+            return
+        cdef _x509.CRT c_crt
+        if self._db:
+            c_crt = self._db[-1]
+            c_crt.set_next(crt)
+        self._db.append(crt)
+
+
+class Purpose(enum.IntEnum):
+    SERVER_AUTH = _tls.MBEDTLS_SSL_IS_SERVER
+    CLIENT_AUTH = _tls.MBEDTLS_SSL_IS_CLIENT
+
+
+_DEFAULT_VALUE = object()
+
+
+cdef class _DTLSCookie:
+    """DTLS cookie."""
+
+    def __cinit__(self):
+        _tls.mbedtls_ssl_cookie_init(&self._ctx)
+
+    def __dealloc__(self):
+        _tls.mbedtls_ssl_cookie_free(&self._ctx)
+
+    @property
+    def timeout(self):
+        return self._ctx.timeout
+
+    @timeout.setter
+    def timeout(self, unsigned long timeout):
+        _tls.mbedtls_ssl_cookie_set_timeout(&self._ctx, timeout)
+
+    def generate(self):
+        """Generate keys."""
+        _tls.mbedtls_ssl_cookie_setup(
+            &self._ctx, _rnd.mbedtls_ctr_drbg_random, &__rng._ctx)
+
+
+cdef class MbedTLSConfiguration:
+
+    """(D)TLS configuration."""
+
+    def __init__(
+        self,
+        validate_certificates,
+        certificate_chain,
+        ciphers,
+        inner_protocols,
+        lowest_supported_version,
+        highest_supported_version,
+        trust_store,
+        max_fragmentation_length,
+        anti_replay,
+        # badmac_limit
+        handshake_timeout_min,
+        handshake_timeout_max,
+        sni_callback,
+        pre_shared_key,
+        pre_shared_key_store,
+        _transport,
+    ):
+        assert isinstance(_transport, Transport)
+        self._max_fragmentation_length = max_fragmentation_length
+        _exc.check_error(_tls.mbedtls_ssl_config_defaults(
+            &self._ctx,
+            endpoint=0,  # server / client is not known here...
+            transport=_transport.value,
+            preset=_tls.MBEDTLS_SSL_PRESET_DEFAULT))
+        self._set_validate_certificates(validate_certificates)
+        self._set_certificate_chain(certificate_chain)
+        self._set_ciphers(ciphers)
+        self._set_inner_protocols(inner_protocols)
+        self._set_lowest_supported_version(lowest_supported_version)
+        self._set_highest_supported_version(highest_supported_version)
+        self._set_trust_store(trust_store)
+        self._set_max_fragmentation_length(max_fragmentation_length)
+        self._set_anti_replay(anti_replay)
+        self._set_handshake_timeout(
+            handshake_timeout_min, handshake_timeout_max
+        )
+        self._set_sni_callback(sni_callback)
+        self._set_pre_shared_key(pre_shared_key)
+        self._set_pre_shared_key_store(pre_shared_key_store)
+
+        # Set random engine.
+        _tls.mbedtls_ssl_conf_rng(
+            &self._ctx, &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx)
+
+        # Disable renegotiation.
+        _tls.mbedtls_ssl_conf_renegotiation(&self._ctx, 0)
+
+        # For security reasons, we do not make cookie optional here.
+        cdef _tls._DTLSCookie cookie = _tls._DTLSCookie()
+        cookie.generate()
+        self._set_cookie(cookie)
+
+    def __cinit__(self):
+        _tls.mbedtls_ssl_config_init(&self._ctx)
+
+        cdef Py_ssize_t ciphers_sz = len(ciphers_available()) + 1
+        self._ciphers = <int *>malloc(ciphers_sz * sizeof(int))
+        if not self._ciphers:
+            raise MemoryError()
+
+        cdef Py_ssize_t idx = 0
+        for idx in range(ciphers_sz):
+            self._ciphers[idx] = 0
+
+        cdef Py_ssize_t protos_sz = len(NextProtocol) + 1
+        self._protos = <const char **>malloc(protos_sz * sizeof(char *))
+        if not self._protos:
+            raise MemoryError()
+
+        for idx in range(protos_sz):
+            self._protos[idx] = NULL
+
+    def __dealloc__(self):
+        _tls.mbedtls_ssl_config_free(&self._ctx)
+        free(self._ciphers)
+        free(self._protos)
+
+    def __reduce__(self):
+        return (
+            type(self),
+            (
+                self.validate_certificates,
+                self.certificate_chain,
+                self.ciphers,
+                self.inner_protocols,
+                self.lowest_supported_version,
+                self.highest_supported_version,
+                self.trust_store,
+                self.max_fragmentation_length,
+                self.anti_replay,
+                self.handshake_timeout_min,
+                self.handshake_timeout_max,
+                self.sni_callback,
+                self.pre_shared_key,
+                self.pre_shared_key_store,
+                self._transport,
+            ),
+        )
+
+    @property
+    def _transport(self):
+        return Transport(self._ctx.transport)
+
+    cdef _set_validate_certificates(self, validate):
+        """Set the certificate verification mode.
+
+        """  # PEP 543
+        if validate is None:
+            return
+        _tls.mbedtls_ssl_conf_authmode(
+            &self._ctx,
+            _tls.MBEDTLS_SSL_VERIFY_OPTIONAL if validate is False else
+            _tls.MBEDTLS_SSL_VERIFY_REQUIRED)
+
+    @property
+    def validate_certificates(self):
+        return self._ctx.authmode == _tls.MBEDTLS_SSL_VERIFY_REQUIRED
+
+    cdef _set_certificate_chain(self, chain):
+        """The certificate, intermediate certificate, and
+        the corresponding private key for the leaf certificate.
+
+        Args:
+            chain (Tuple[Tuple[Certificate], PrivateKey]):
+                The certificate chain.
+
+        """
+        # PEP 543
+        if not chain:
+            return
+        self._chain = chain
+        certs, pk_key = chain
+        if not certs or not pk_key:
+            return
+        cdef _x509.CRT c_crt, c_crt_next
+        for c_crt, c_crt_next in pairwise(certs):
+            c_crt.set_next(c_crt_next)
+        c_crt = certs[0]
+        c_pk_key = <_pk.CipherBase?> pk_key
+        _exc.check_error(_tls.mbedtls_ssl_conf_own_cert(
+            &self._ctx, &c_crt._ctx, &c_pk_key._ctx))
+
+    @property
+    def certificate_chain(self):
+        key_cert = self._ctx.key_cert
+        if key_cert is NULL:
+            return None
+        chain = []
+        cdef _x509.mbedtls_x509_crt *c_ctx = key_cert.cert
+        while c_ctx is not NULL:
+            chain.append(_x509.CRT.from_DER(c_ctx.raw.p[0:c_ctx.raw.len]))
+            c_ctx = c_ctx.next
+        cdef unsigned char[:] buf = bytearray(_pk.PRV_DER_MAX_BYTES)
+        olen = _exc.check_error(
+            _pk.mbedtls_pk_write_key_der(key_cert.key, &buf[0], buf.size))
+        der = buf[buf.size - olen:buf.size]
+        if _pk.mbedtls_pk_can_do(key_cert.key, _pk.MBEDTLS_PK_RSA) == 0:
+            return tuple(chain), _pk.ECC.from_DER(der)
+        return tuple(chain), _pk.RSA.from_DER(der)
+
+    cdef _set_ciphers(self, ciphers):
+        """The available ciphers for the TLS connections.
+
+        Args:
+            ciphers (Tuple[Union[CipherSuite, int]]): The ciphers.
+
+        """
+        # PEP 543
+        if ciphers is None:
+            return
+        if not frozenset(ciphers).issubset(ciphers_available()):
+            raise NotImplementedError("unsupported ciphers")
+        cdef Py_ssize_t idx = 0
+        self._ciphers[idx] = 0
+        for idx, cipher in enumerate(ciphers):
+            if not isinstance(cipher, int):
+                cipher = __get_ciphersuite_id(cipher)
+            self._ciphers[idx] = cipher
+        self._ciphers[idx + 1] = 0
+        _tls.mbedtls_ssl_conf_ciphersuites(&self._ctx, self._ciphers)
+
+    @property
+    def ciphers(self):
+        ciphers = []
+        cdef int cipher_id
+        cdef Py_ssize_t idx
+        for idx in range(len(ciphers_available())):
+            cipher_id = self._ciphers[idx]
+            if cipher_id == 0:
+                break
+            ciphers.append(__get_ciphersuite_name(cipher_id))
+        return tuple(ciphers)
+
+    cdef _set_inner_protocols(self, protocols):
+        """
+
+        Args:
+            protocols ([Tuple[Union[NextProtocol, bytes]]]): Protocols
+                that connections created with this configuration should
+                advertise as supported during the TLS handshake. These may
+                be advertised using either or both of ALPN or NPN. This
+                list of protocols should be ordered by preference.
+
+        """
+        # PEP 543
+        if protocols is None:
+            return
+        if len(protocols) > len(NextProtocol):
+            raise ValueError("invalid protocols")
+
+        cdef Py_ssize_t idx = 0
+        for idx, proto in enumerate(protocols):
+            if not isinstance(proto, bytes):
+                proto = proto.value
+            self._protos[idx] = proto
+        self._protos[idx + 1] = NULL
+
+        _exc.check_error(_tls.mbedtls_ssl_conf_alpn_protocols(
+            &self._ctx, self._protos))
+
+    @property
+    def inner_protocols(self):
+        protos = []
+        cdef const char* proto
+        for idx in range(len(NextProtocol)):
+            proto = self._protos[idx]
+            if proto is NULL:
+                break
+            protos.append(NextProtocol(proto))
+        return tuple(protos)
+
+    cdef _set_lowest_supported_version(self, version):
+        """The minimum version of TLS that should be allowed.
+
+        Args:
+            version (TLSVersion, or DTLSVersion): The minimum version.
+
+        """  # PEP 543
+        if self._transport is Transport.STREAM:
+            version = _check_tls_version(
+                version
+                if version is not None
+                else TLSVersion.MINIMUM_SUPPORTED
+            )
+        if self._transport is Transport.DATAGRAM:
+            version = _check_dtls_version(
+                version
+                if version is not None
+                else DTLSVersion.MINIMUM_SUPPORTED
+            )
+        try:
+            major, minor = {
+                TLSVersion: _tls_from_version,
+                DTLSVersion: _dtls_from_version,
+            }[type(version)](version)
+        except KeyError as exc:
+            raise TypeError(version) from exc
+
+        _tls.mbedtls_ssl_conf_min_version(&self._ctx, major, minor)
+
+    @property
+    def lowest_supported_version(self):
+        maj_min_version = self._ctx.min_major_ver, self._ctx.min_minor_ver
+        if self._transport is Transport.STREAM:
+            return _tls_to_version(maj_min_version)
+        if self._transport is Transport.DATAGRAM:
+            return _dtls_to_version(maj_min_version)
+        assert 0, "unreachable"
+
+    cdef _set_highest_supported_version(self, version):
+        """The maximum version of TLS that should be allowed.
+
+        Args:
+            version (TLSVersion, or DTLSVersion): The maximum version.
+
+        """  # PEP 543
+        if self._transport is Transport.STREAM:
+            version = _check_tls_version(
+                version
+                if version is not None
+                else TLSVersion.MAXIMUM_SUPPORTED
+            )
+        if self._transport is Transport.DATAGRAM:
+            version = _check_dtls_version(
+                version
+                if version is not None
+                else DTLSVersion.MAXIMUM_SUPPORTED
+            )
+        try:
+            major, minor = {
+                TLSVersion: _tls_from_version,
+                DTLSVersion: _dtls_from_version,
+            }[type(version)](version)
+        except KeyError as exc:
+            raise TypeError(version) from exc
+
+        _tls.mbedtls_ssl_conf_max_version(&self._ctx, major, minor)
+
+    @property
+    def highest_supported_version(self):
+        maj_min_version = self._ctx.max_major_ver, self._ctx.max_minor_ver
+        if self._transport is Transport.STREAM:
+            return _tls_to_version(maj_min_version)
+        if self._transport is Transport.DATAGRAM:
+            return _dtls_to_version(maj_min_version)
+        assert 0, "unreachable"
+
+    cdef _set_trust_store(self, store):
+        """The trust store that connections will use.
+
+        Args:
+            store (TrustStore): The trust store.
+
+        """
+        # PEP 543
+        if not store:
+            return
+        cdef _x509.CRT crt = TrustStore(store)[0]
+        mbedtls_ssl_conf_ca_chain(&self._ctx, &crt._ctx, NULL)
+
+    @property
+    def trust_store(self):
+        store = TrustStore()
+        if self._ctx.ca_chain is NULL:
+            return store
+
+        cdef _x509.mbedtls_x509_crt *c_ctx = self._ctx.ca_chain
+        while c_ctx is not NULL:
+            store.add(_x509.CRT.from_DER(c_ctx.raw.p[0:c_ctx.raw.len]))
+            c_ctx = c_ctx.next
+        return store
+
+    cdef _set_max_fragmentation_length(self, mfl):
+        if mfl is None:
+            return
+
+        if not isinstance(mfl, MaxFragmentLength):
+            raise TypeError(mfl)
+
+        try:
+            _exc.check_error(
+                _tls.mbedtls_ssl_conf_max_frag_len(&self._ctx, mfl.value)
+            )
+        except _exc.TLSError as exc:
+            raise ValueError(mfl) from exc
+
+    @property
+    def max_fragmentation_length(self):
+        # No accessor in backend.
+        return self._max_fragmentation_length
+
+    cdef _set_anti_replay(self, anti_replay):
+        """Set anti replay."""
+        if anti_replay is None:
+            return
+        if self._transport is Transport.STREAM:
+            # not available with TLS
+            raise ValueError(anti_replay)
+        _tls.mbedtls_ssl_conf_dtls_anti_replay(
+            &self._ctx,
+            _tls.MBEDTLS_SSL_ANTI_REPLAY_ENABLED
+            if anti_replay else
+            _tls.MBEDTLS_SSL_ANTI_REPLAY_DISABLED)
+
+    @property
+    def anti_replay(self):
+        if self._transport is Transport.STREAM:
+            return None
+
+        cdef unsigned int enabled = _tls.MBEDTLS_SSL_ANTI_REPLAY_ENABLED
+        return True if self._ctx.anti_replay == enabled else False
+
+    cdef _set_handshake_timeout(self, minimum, maximum):
+        """Set DTLS handshake timeout.
+
+        Args:
+            minimum (float, optional): minimum timeout in seconds.
+            maximum (float, optional): maximum timeout in seconds.
+
+        """
+        if minimum is None and maximum is None:
+            return
+        if self._transport is Transport.STREAM:
+            # not available with TLS
+            raise ValueError((minimum, maximum))
+
+        def validate(extremum, *, default: float) -> float:
+            if extremum is None:
+                return default
+            if extremum < 0.0:
+                raise ValueError(extremum)
+            return extremum
+
+        _tls.mbedtls_ssl_conf_handshake_timeout(
+            &self._ctx,
+            int(1000.0 * validate(minimum, default=1.0)),
+            int(1000.0 * validate(maximum, default=60.0)),
+        )
+
+    @property
+    def handshake_timeout_min(self):
+        """Min handshake timeout in seconds (default 1.0)."""
+        if self._transport is Transport.STREAM:
+            return None
+
+        return float(self._ctx.hs_timeout_min) / 1000.0
+
+    @property
+    def handshake_timeout_max(self):
+        """Max handshake timeout in seconds (default 60.0)."""
+        if self._transport is Transport.STREAM:
+            return None
+
+        return float(self._ctx.hs_timeout_max) / 1000.0
+
+    cdef _set_sni_callback(self, callback):
+        # PEP 543, optional, server-side only
+        if callback is None:
+            return
+        # mbedtls_ssl_conf_sni
+        raise NotImplementedError
+
+    @property
+    def sni_callback(self):
+        return None
+
+    cdef _set_pre_shared_key(self, psk):
+        """Set a pre shared key (PSK) for the client.
+
+        Args:
+            psk ([Tuple[unicode, bytes]]): A tuple with the key and the exected
+                identity name.
+
+        """
+        if psk is None:
+            return
+        try:
+            identity, key = psk
+        except ValueError:
+            raise TypeError("expected a tuple (name, key)")
+        c_identity = identity.encode("utf8")
+        _exc.check_error(_tls.mbedtls_ssl_conf_psk(
+            &self._ctx,
+            key, len(key),
+            c_identity, len(c_identity)))
+
+    @property
+    def pre_shared_key(self):
+        if self._ctx.psk == NULL or self._ctx.psk_identity == NULL:
+            return None
+        key = self._ctx.psk[:self._ctx.psk_len]
+        c_identity = self._ctx.psk_identity[:self._ctx.psk_identity_len]
+        identity = c_identity.decode("utf8")
+        return (identity, key)
+
+    cdef _set_pre_shared_key_store(self, psk_store):
+        # server-side
+        if psk_store is None:
+            return
+        self._store = _PSKSToreProxy(psk_store)  # ownership
+        _tls.mbedtls_ssl_conf_psk_cb(&self._ctx, _psk_cb, <void *> self._store)
+
+    @property
+    def pre_shared_key_store(self):
+        if self._ctx.p_psk == NULL:
+            return None
+        psk_store = <_tls._PSKSToreProxy> self._ctx.p_psk
+        return psk_store.unwrap()
+
+    cdef _set_cookie(self, _tls._DTLSCookie cookie):
+        """Register callbacks for DTLS cookies (server only)."""
+        self._cookie = cookie
+        if cookie is None:
+            _tls.mbedtls_ssl_conf_dtls_cookies(
+                &self._ctx,
+                NULL,
+                NULL,
+                NULL,
+            )
+        else:
+            _tls.mbedtls_ssl_conf_dtls_cookies(
+                &self._ctx,
+                _tls.mbedtls_ssl_cookie_write,
+                _tls.mbedtls_ssl_cookie_check,
+                &self._cookie._ctx,
+            )
+
+
+DEFAULT_CIPHER_LIST = None
+
+
+cdef class TLSSession:
+    def __cinit__(self):
+        """Initialize SSL session structure."""
+        _tls.mbedtls_ssl_session_init(&self._ctx)
+
+    def __dealloc__(self):
+        """Free referenced items in an SSL session."""
+        _tls.mbedtls_ssl_session_free(&self._ctx)
+
+    def __getstate__(self):
+        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
+
+    def __repr__(self):
+        return "%s()" % type(self).__name__
+
+
+cdef class _BaseContext:
+    # _pep543._BaseContext
+    """Context base class."""
+
+    def __init__(self, configuration not None):
+        if isinstance(configuration, TLSConfiguration):
+            self._conf = MbedTLSConfiguration(
+                validate_certificates=configuration.validate_certificates,
+                certificate_chain=configuration.certificate_chain,
+                ciphers=configuration.ciphers,
+                inner_protocols=configuration.inner_protocols,
+                lowest_supported_version=(
+                    configuration.lowest_supported_version
+                ),
+                highest_supported_version=(
+                    configuration.highest_supported_version
+                ),
+                trust_store=configuration.trust_store,
+                max_fragmentation_length=configuration.max_fragmentation_length,
+                anti_replay=None,
+                handshake_timeout_min=None,
+                handshake_timeout_max=None,
+                sni_callback=configuration.sni_callback,
+                pre_shared_key=configuration.pre_shared_key,
+                pre_shared_key_store=configuration.pre_shared_key_store,
+                _transport=Transport.STREAM,
+            )
+        elif isinstance(configuration, DTLSConfiguration):
+            self._conf = MbedTLSConfiguration(
+                validate_certificates=configuration.validate_certificates,
+                certificate_chain=configuration.certificate_chain,
+                ciphers=configuration.ciphers,
+                inner_protocols=configuration.inner_protocols,
+                lowest_supported_version=(
+                    configuration.lowest_supported_version
+                ),
+                highest_supported_version=(
+                    configuration.highest_supported_version
+                ),
+                trust_store=configuration.trust_store,
+                max_fragmentation_length=configuration.max_fragmentation_length,
+                anti_replay=configuration.anti_replay,
+                handshake_timeout_min=configuration.handshake_timeout_min,
+                handshake_timeout_max=configuration.handshake_timeout_max,
+                sni_callback=configuration.sni_callback,
+                pre_shared_key=configuration.pre_shared_key,
+                pre_shared_key_store=configuration.pre_shared_key_store,
+                _transport=Transport.DATAGRAM,
+            )
+        else:
+            # Setting `_conf` is required for delocate on macOS.
+            self._conf = None
+            raise TypeError(configuration)
+
+        _tls.mbedtls_ssl_conf_endpoint(
+            &self._conf._ctx,
+            {
+                Purpose.CLIENT_AUTH: _tls.MBEDTLS_SSL_IS_CLIENT,
+                Purpose.SERVER_AUTH: _tls.MBEDTLS_SSL_IS_SERVER,
+            }[self._purpose])
+
+    def __eq__(self, other):
+        if not isinstance(other, type(self)):
+            return False
+        if not type(self) is type(other):
+            return False
+        return self.configuration == other.configuration
+
+    @property
+    def configuration(self):
+        if self._conf._transport is Transport.STREAM:
+            return TLSConfiguration(
+                validate_certificates=self._conf.validate_certificates,
+                certificate_chain=self._conf.certificate_chain,
+                ciphers=self._conf.ciphers,
+                inner_protocols=self._conf.inner_protocols,
+                lowest_supported_version=self._conf.lowest_supported_version,
+                highest_supported_version=self._conf.highest_supported_version,
+                trust_store=self._conf.trust_store,
+                max_fragmentation_length=self._conf.max_fragmentation_length,
+                sni_callback=self._conf.sni_callback,
+                pre_shared_key=self._conf.pre_shared_key,
+                pre_shared_key_store=self._conf.pre_shared_key_store,
+            )
+        assert self._conf._transport is Transport.DATAGRAM
+        return DTLSConfiguration(
+            validate_certificates=self._conf.validate_certificates,
+            certificate_chain=self._conf.certificate_chain,
+            ciphers=self._conf.ciphers,
+            inner_protocols=self._conf.inner_protocols,
+            lowest_supported_version=self._conf.lowest_supported_version,
+            highest_supported_version=self._conf.highest_supported_version,
+            trust_store=self._conf.trust_store,
+            max_fragmentation_length=self._conf.max_fragmentation_length,
+            anti_replay=self._conf.anti_replay,
+            handshake_timeout_min=self._conf.handshake_timeout_min,
+            handshake_timeout_max=self._conf.handshake_timeout_max,
+            sni_callback=self._conf.sni_callback,
+            pre_shared_key=self._conf.pre_shared_key,
+            pre_shared_key_store=self._conf.pre_shared_key_store,
+        )
+
+    @property
+    def _purpose(self) -> Purpose:
+        raise NotImplementedError
+
+
+TLS_BUFFER_CAPACITY = 2 << 14
+# 32K (MBEDTLS_SSL_DTLS_MAX_BUFFERING)
+
+
+cdef class MbedTLSBuffer:
+    def __init__(self, _BaseContext context, server_hostname=None):
+        self._context = context
+        _exc.check_error(
+            _tls.mbedtls_ssl_setup(&self._ctx, &self._context._conf._ctx)
+        )
+        self._c_output_buffer = _rb.RingBuffer(TLS_BUFFER_CAPACITY)
+        self._c_input_buffer = _rb.RingBuffer(TLS_BUFFER_CAPACITY)
+        self._c_buffers = _tls._C_Buffers(
+            &self._c_output_buffer._ctx,
+            &self._c_input_buffer._ctx
+        )
+        self._reset()
+        _tls.mbedtls_ssl_set_bio(
+            &self._ctx,
+            &self._c_buffers,
+            buffer_write,
+            buffer_read,
+            NULL
+        )
+        self._set_hostname(server_hostname)
+
+    def __cinit__(self):
+        """Initialize an `ssl_context`."""
+        _tls.mbedtls_ssl_init(&self._ctx)
+        _tls.mbedtls_ssl_set_timer_cb(
+            &self._ctx,
+            &self._timer,
+            _timing.mbedtls_timing_set_delay,
+            _timing.mbedtls_timing_get_delay)
+
+    def __dealloc__(self):
+        """Free and clear the internal structures of ctx."""
+        _tls.mbedtls_ssl_free(&self._ctx)
+
+    def __getstate__(self):
+        cdef size_t olen = 0
+        ret = mbedtls_ssl_context_save(&self._ctx, NULL, 0, &olen)
+        if ret != -0x6A00 or olen == 0:
+            # 0x6A00: MBEDTLS_ERR_SSL_BUFFER_TOO_SMALL
+            raise TypeError(
+                f"cannot pickle {self.__class__.__name__!r} object {hex(ret)}"
+            )
+        cdef unsigned char *c_buf = <unsigned char *> malloc(olen)
+        if not c_buf:
+            raise MemoryError()
+        try:
+            if mbedtls_ssl_context_save(&self._ctx, c_buf, olen, &olen) != 0:
+                raise TypeError(
+                    f"cannot pickle {self.__class__.__name__!r} object"
+                )
+            return {
+                "connection": c_buf[:olen],
+                "context": self.context,
+                "server_hostname": self._server_hostname,
+            }
+        finally:
+            free(c_buf)
+
+    def __setstate__(self, state):
+        self.__init__(state["context"], state["server_hostname"])
+        cdef const unsigned char[:] buf = state["connection"]
+        ret = mbedtls_ssl_context_load(&self._ctx, &buf[0], buf.size)
+        if ret != 0:
+            self._reset()
+            raise TypeError(
+                f"cannot unpickle {self.__class__.__name__!r} object"
+            )
+
+    def __repr__(self):
+        return "%s(%r)" % (type(self).__name__, self.context)
+
+    @property
+    def _input_buffer(self):
+        return self._c_input_buffer
+
+    @property
+    def _output_buffer(self):
+        return self._c_output_buffer
+
+    @property
+    def context(self):
+        return self._context
+
+    @property
+    def _verified(self):
+        return _tls.mbedtls_ssl_get_verify_result(&self._ctx) == 0
+
+    @property
+    def _server_hostname(self):
+        # Client side
+        if self._ctx.hostname is NULL:
+            return None
+        return (<bytes> self._ctx.hostname).decode("utf8")
+
+    def _set_hostname(self, hostname):
+        """Set the hostname to check against the received server."""
+        if hostname is None:
+            return
+        # Note: `ssl_set_hostname()` makes a copy so it is safe
+        #       to call with the temporary `hostname_`.
+        hostname_ = hostname.encode("utf8")
+        cdef const char* c_hostname = hostname_
+        _exc.check_error(_tls.mbedtls_ssl_set_hostname(&self._ctx, c_hostname))
+
+    @property
+    def _cookieparam(self):
+        """Client ID for the HelloVerifyRequest.
+
+        Note:
+            Server-side, DTLS only.
+
+        """
+        client_id = bytes(self._ctx.cli_id[0:self._ctx.cli_id_len])
+        return client_id if client_id else None
+
+    def setcookieparam(self, const unsigned char[:] info not None):
+        if info.size == 0:
+            info = b"\0"
+        _tls.mbedtls_ssl_set_client_transport_id(
+            &self._ctx,
+            &info[0],
+            info.size,
+        )
+
+    def setmtu(self, mtu):
+        """Set Maxiumum Transport Unit (MTU) for DTLS.
+
+        Set to zero to unset.
+
+        Raises:
+            OverflowError: If value cannot be converted to UInt16.
+
+        """
+        # DTLS
+        if not isinstance(mtu, int):
+            raise TypeError(mtu)
+        _tls.mbedtls_ssl_set_mtu(&self._ctx, mtu)
+
+    def _reset(self):
+        _exc.check_error(_tls.mbedtls_ssl_session_reset(&self._ctx))
+
+    def shutdown(self):
+        try:
+            _exc.check_error(_tls.mbedtls_ssl_close_notify(&self._ctx))
+        except (WantReadError, WantWriteError):
+            raise
+        except _exc.TLSError:
+            # No error handling:  The connection may be closed already.
+            self._reset()
+
+    def read(self, amt):
+        # PEP 543
+        if amt <= 0:
+            return b""
+        buffer = bytearray(amt)
+        view = memoryview(buffer)
+        nread = 0
+        while nread != amt and not self._input_buffer.empty():
+            nread += self.readinto(view[nread:], amt - nread)
+        return bytes(buffer[:nread])
+
+    def readinto(self, unsigned char[:] buffer not None, size_t amt):
+        if buffer.size == 0:
+            return 0
+        if amt <= 0:
+            return 0
+        read = _tls.mbedtls_ssl_read(&self._ctx, &buffer[0], amt)
+        if read > 0:
+            return read
+        if read == 0:
+            raise RaggedEOF()
+        if read == _tls.MBEDTLS_ERR_SSL_WANT_READ:
+            raise WantReadError()
+        if read == _tls.MBEDTLS_ERR_SSL_WANT_WRITE:
+            raise WantWriteError()
+        if read == _tls.MBEDTLS_ERR_SSL_CLIENT_RECONNECT:
+            _exc.check_error(read)  # raises
+            assert 0, "unreachable"
+        self._reset()
+        _exc.check_error(read)  # raises
+        assert 0, "unreachable"
+
+    def write(self, const unsigned char[:] buffer not None):
+        if buffer.size == 0:
+            return 0
+        cdef size_t written = 0
+        while written != buffer.size:
+            ret = _tls.mbedtls_ssl_write(
+                &self._ctx, &buffer[written], buffer.size - written)
+            if ret >= 0:
+                written += ret
+            elif ret == _tls.MBEDTLS_ERR_SSL_WANT_READ:
+                raise WantReadError()
+            elif ret == _tls.MBEDTLS_ERR_SSL_WANT_WRITE:
+                raise WantWriteError()
+            else:
+                self._reset()
+                _exc.check_error(ret)
+        assert written == len(buffer)
+        return len(self._output_buffer)
+
+    def receive_from_network(self, data):
+        # PEP 543
+        # Append data to input buffer.
+        self._input_buffer.write(data, len(data))
+
+    def peek_outgoing(self, amt):
+        # PEP 543
+        # Read from output buffer.
+        if amt == 0:
+            return b""
+        return self._output_buffer.peek(amt)
+
+    def consume_outgoing(self, amt):
+        """Consume `amt` bytes from the output buffer."""
+        # PEP 543
+        self._output_buffer.consume(amt)
+
+    def getpeercert(self, binary_form=False):
+        """Return the peer certificate, or None."""
+        c_crt = _tls.mbedtls_ssl_get_peer_cert(&self._ctx)
+        if c_crt is NULL:
+            return None
+
+        # See `CRT.to_DER()`.
+        der = bytes(c_crt.raw.p[0:c_crt.raw.len])
+        if binary_form:
+            return der
+        return _x509.CRT.from_DER(der)
+
+    def selected_npn_protocol(self):
+        return None
+
+    def negotiated_protocol(self):
+        cdef const char* protocol = _tls.mbedtls_ssl_get_alpn_protocol(
+            &self._ctx)
+        if protocol is NULL:
+            return None
+        return protocol.decode("ascii")
+
+    def _cipher_suite(self):
+        cdef const char* name = _tls.mbedtls_ssl_get_ciphersuite(&self._ctx)
+        if name is NULL:
+            return None
+        ssl_version = self.negotiated_tls_version()
+        secret_bits = None
+        return name.decode("ascii"), ssl_version, secret_bits
+
+    def cipher(self):
+        cipher = self._cipher_suite()
+        if cipher is None:
+            return
+        return cipher[0]
+
+    @property
+    def _handshake_state(self):
+        return HandshakeStep(self._ctx.state)
+
+    def do_handshake(self):
+        self._handle_handshake_response(
+            _tls.mbedtls_ssl_handshake_step(&self._ctx)
+        )
+
+    def _renegotiate(self):
+        """Initialize an SSL renegotiation on the running connection."""
+        self._handle_handshake_response(
+            _tls.mbedtls_ssl_renegotiate(&self._ctx)
+        )
+
+    def _handle_handshake_response(self, ret):
+        if ret == _tls.MBEDTLS_ERR_SSL_WANT_READ:
+            raise WantReadError()
+        if ret == _tls.MBEDTLS_ERR_SSL_WANT_WRITE:
+            raise WantWriteError()
+        if ret == _tls.MBEDTLS_ERR_SSL_HELLO_VERIFY_REQUIRED:
+            self._reset()
+            raise HelloVerifyRequest()
+        if (
+            ret == -0x7100
+            and self._handshake_state is HandshakeStep.HANDSHAKE_OVER
+        ):
+            raise ValueError("handshake already over")
+        if ret < 0:
+            self._reset()
+            _exc.check_error(ret)
+        if ret == 0 and self._output_buffer:
+            raise WantWriteError
+        assert ret == 0
+
+    def _get_channel_binding(self, cb_type="tls-unique"):
+        return None
+
+    def negotiated_tls_version(self):
+        # Strings from `ssl_tls.c`.
+        return {
+            "DTLSv1.0": DTLSVersion.DTLSv1_0,
+            "DTLSv1.2": DTLSVersion.DTLSv1_2,
+            # "SSLv3.0": TLSVersion.SSLv3,
+            "TLSv1.0": TLSVersion.TLSv1,
+            "TLSv1.1": TLSVersion.TLSv1_1,
+            "TLSv1.2": TLSVersion.TLSv1_2,
+            "TLSV1.3": TLSVersion.TLSv1_3,
+        }.get(_tls.mbedtls_ssl_get_version(&self._ctx).decode("ascii"))
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/_tlsi.py` & `python-mbedtls-2.7.1/src/mbedtls/_tlsi.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,441 +1,445 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2018, Mathias Laurin
-
-"""Interfaces defined in PEP 543 (+ DTLS)."""
-
-from __future__ import annotations
-
-import enum
-import os
-import sys
-from dataclasses import dataclass, field
-from typing import Callable, Mapping, Optional, Tuple, TypeVar, Union
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Literal, Protocol
-else:
-    from typing import Literal, Protocol
-
-if sys.version_info < (3, 9):
-    _PathLike = os.PathLike
-else:
-    _PathLike = os.PathLike[str]
-
-__all__ = ["NextProtocol", "TLSVersion", "DTLSVersion"]
-
-_Path = Union[_PathLike, str]
-
-
-@enum.unique
-class NextProtocol(enum.Enum):
-    H2: bytes = b"h2"
-    H2C: bytes = b"h2c"
-    HTTP1: bytes = b"http/1.1"
-    WEBRTC: bytes = b"webrtc"
-    C_WEBRTC: bytes = b"c-webrtc"
-    FTP: bytes = b"ftp"
-    STUN: bytes = b"stun.nat-discovery"
-    TURN: bytes = b"stun.turn"
-
-
-class MaxFragmentLength(enum.Enum):
-    NONE = 0
-    MFL_512K = 1
-    MFL_1024K = 2
-    MFL_2048K = 3
-    MFL_4096K = 4
-
-
-class TLSVersion(enum.Enum):
-    # PEP 543
-    MINIMUM_SUPPORTED = enum.auto()
-    SSLv2 = enum.auto()
-    SSLv3 = enum.auto()
-    TLSv1 = enum.auto()
-    TLSv1_1 = enum.auto()
-    TLSv1_2 = enum.auto()
-    TLSv1_3 = enum.auto()
-    MAXIMUM_SUPPORTED = enum.auto()
-
-
-class DTLSVersion(enum.Enum):
-    MINIMUM_SUPPORTED = enum.auto()
-    DTLSv1_0 = enum.auto()
-    DTLSv1_2 = enum.auto()
-    MAXIMUM_SUPPORTED = enum.auto()
-
-
-class TrustStore(Protocol):
-    @classmethod
-    def system(cls) -> TrustStore:
-        """Returns a TrustStore object that represents the system
-        trust database.
-
-        """
-
-    @classmethod
-    def from_pem_file(cls, path: _Path) -> TrustStore:
-        """Initializes a trust store from a single file full of PEMs."""
-
-
-class Certificate(Protocol):
-    @classmethod
-    def from_buffer(cls, buffer: bytes) -> Certificate:
-        """Creates a Certificate object from a byte buffer.
-
-        This byte buffer may be either PEM-encoded or DER-encoded. If the
-        buffer is PEM encoded it *must* begin with the standard PEM
-        preamble (a series of dashes followed by the ASCII bytes "BEGIN
-        CERTIFICATE" and another series of dashes). In the absence of that
-        preamble, the implementation may assume that the certificate is
-        DER-encoded instead.
-
-        """
-
-    @classmethod
-    def from_file(cls, path: _Path) -> Certificate:
-        """Creates a Certificate object from a file on disk.
-
-        This method may be a convenience method that wraps ``open`` and
-        ``from_buffer``, but some TLS implementations may be able to
-        provide more-secure or faster methods of loading certificates that
-        do not involve Python code.
-
-        """
-
-
-class PrivateKey(Protocol):
-    @classmethod
-    def from_buffer(
-        cls,
-        buffer: bytes,
-        password: Optional[
-            Union[Callable[[], Union[bytes, bytearray]], bytes, bytearray]
-        ] = None,
-    ) -> PrivateKey:
-        """Creates a PrivateKey object from a byte buffer.
-
-        This byte buffer may be either PEM-encoded or DER-encoded. If the
-        buffer is PEM encoded it *must* begin with the standard PEM
-        preamble (a series of dashes followed by the ASCII bytes "BEGIN",
-        the key type, and another series of dashes). In the absence of
-        that preamble, the implementation may assume that the certificate
-        is DER-encoded instead.
-
-        The key may additionally be encrypted. If it is, the ``password``
-        argument can be used to decrypt the key. The ``password`` argument
-        may be a function to call to get the password for decrypting the
-        private key. It will only be called if the private key is encrypted
-        and a password is necessary. It will be called with no arguments,
-        and it should return either bytes or bytearray containing the
-        password. Alternatively a bytes, or bytearray value may be supplied
-        directly as the password argument. It will be ignored if the
-        private key is not encrypted and no password is needed.
-        """
-
-    @classmethod
-    def from_file(
-        cls,
-        path: _Path,
-        password: Optional[
-            Union[Callable[[], Union[bytes, bytearray]], bytes, bytearray]
-        ] = None,
-    ) -> PrivateKey:
-        """Creates a PrivateKey object from a file on disk.
-
-        This method may be a convenience method that wraps ``open`` and
-        ``from_buffer``, but some TLS implementations may be able to
-        provide more-secure or faster methods of loading certificates that
-        do not involve Python code.
-
-        The ``password`` parameter behaves exactly as the equivalent
-        parameter on ``from_buffer``.
-        """
-
-
-CipherSuite = object
-DEFAULT_CIPHER_LIST = ()
-
-ServerNameCallback = object
-
-
-class __DefaultValue(enum.Enum):
-    DEFAULT_VALUE = enum.auto()
-
-
-_DEFAULT_VALUE = __DefaultValue.DEFAULT_VALUE
-
-T = TypeVar("T")
-_Wrap = Union[T, Literal[__DefaultValue.DEFAULT_VALUE]]
-
-
-def _unwrap(x: _Wrap[T], default: T) -> T:
-    if x is _DEFAULT_VALUE:
-        return default
-    return x
-
-
-_CertificateChain = Tuple[Tuple[Certificate, ...], PrivateKey]
-_Ciphers = Tuple[Union[CipherSuite, int], ...]
-_InnerProtocols = Tuple[Union[NextProtocol, bytes], ...]
-
-
-@dataclass(frozen=True)
-class TLSConfiguration:
-    # pylint: disable=too-many-instance-attributes, too-many-arguments
-    validate_certificates: bool = True
-    certificate_chain: Optional[_CertificateChain] = None
-    ciphers: Optional[_Ciphers] = None
-    inner_protocols: Optional[_InnerProtocols] = None
-    lowest_supported_version: TLSVersion = TLSVersion.TLSv1
-    highest_supported_version: TLSVersion = TLSVersion.MAXIMUM_SUPPORTED
-    trust_store: Optional[TrustStore] = None
-    max_fragmentation_length: Optional[MaxFragmentLength] = None
-    sni_callback: Optional[ServerNameCallback] = None
-    pre_shared_key: Optional[Tuple[str, bytes]] = None
-    pre_shared_key_store: Mapping[str, bytes] = field(default_factory=dict)
-
-    def __eq__(self, other: object) -> bool:
-        if not isinstance(other, TLSConfiguration):
-            return NotImplemented
-        return all(
-            (
-                self.validate_certificates == other.validate_certificates,
-                self.certificate_chain == other.certificate_chain
-                or (
-                    not self.certificate_chain and not other.certificate_chain
-                ),
-                self.ciphers == other.ciphers
-                or (not self.ciphers and not other.ciphers),
-                self.inner_protocols == other.inner_protocols
-                or (not self.inner_protocols and not other.inner_protocols),
-                self.lowest_supported_version == other.lowest_supported_version
-                or (
-                    self.lowest_supported_version
-                    in {
-                        TLSVersion.MINIMUM_SUPPORTED,
-                        TLSVersion.MAXIMUM_SUPPORTED,
-                    }
-                )
-                or (
-                    other.lowest_supported_version
-                    in {
-                        TLSVersion.MINIMUM_SUPPORTED,
-                        TLSVersion.MAXIMUM_SUPPORTED,
-                    }
-                ),
-                self.highest_supported_version
-                == other.highest_supported_version
-                or (
-                    self.highest_supported_version
-                    in {
-                        TLSVersion.MINIMUM_SUPPORTED,
-                        TLSVersion.MAXIMUM_SUPPORTED,
-                    }
-                )
-                or (
-                    other.highest_supported_version
-                    in {
-                        TLSVersion.MINIMUM_SUPPORTED,
-                        TLSVersion.MAXIMUM_SUPPORTED,
-                    }
-                ),
-                self.trust_store == other.trust_store
-                or (not self.trust_store and not other.trust_store),
-                self.max_fragmentation_length
-                == other.max_fragmentation_length,
-                self.sni_callback == other.sni_callback,
-                self.pre_shared_key == other.pre_shared_key,
-                self.pre_shared_key_store == other.pre_shared_key_store,
-            )
-        )
-
-    def update(
-        self,
-        validate_certificates: _Wrap[bool] = _DEFAULT_VALUE,
-        certificate_chain: _Wrap[_CertificateChain] = _DEFAULT_VALUE,
-        ciphers: _Wrap[_Ciphers] = _DEFAULT_VALUE,
-        inner_protocols: _Wrap[_InnerProtocols] = _DEFAULT_VALUE,
-        lowest_supported_version: _Wrap[TLSVersion] = _DEFAULT_VALUE,
-        highest_supported_version: _Wrap[TLSVersion] = _DEFAULT_VALUE,
-        trust_store: _Wrap[TrustStore] = _DEFAULT_VALUE,
-        max_fragmentation_length: _Wrap[MaxFragmentLength] = _DEFAULT_VALUE,
-        sni_callback: _Wrap[Optional[ServerNameCallback]] = _DEFAULT_VALUE,
-        pre_shared_key: _Wrap[Tuple[str, bytes]] = _DEFAULT_VALUE,
-        pre_shared_key_store: _Wrap[Mapping[str, bytes]] = _DEFAULT_VALUE,
-    ) -> TLSConfiguration:
-        """
-        Create a new ``TLSConfiguration``, overriding some of the settings
-        on the original configuration with the new settings.
-        """
-        return self.__class__(
-            validate_certificates=_unwrap(
-                validate_certificates,
-                self.validate_certificates,
-            ),
-            certificate_chain=_unwrap(
-                certificate_chain,
-                self.certificate_chain,
-            ),
-            ciphers=_unwrap(ciphers, self.ciphers),
-            inner_protocols=_unwrap(inner_protocols, self.inner_protocols),
-            lowest_supported_version=_unwrap(
-                lowest_supported_version,
-                self.lowest_supported_version,
-            ),
-            highest_supported_version=_unwrap(
-                highest_supported_version,
-                self.highest_supported_version,
-            ),
-            trust_store=_unwrap(trust_store, self.trust_store),
-            max_fragmentation_length=_unwrap(
-                max_fragmentation_length,
-                self.max_fragmentation_length,
-            ),
-            sni_callback=_unwrap(sni_callback, self.sni_callback),
-            pre_shared_key=_unwrap(pre_shared_key, self.pre_shared_key),
-            pre_shared_key_store=_unwrap(
-                pre_shared_key_store,
-                self.pre_shared_key_store,
-            ),
-        )
-
-
-@dataclass(frozen=True)
-class DTLSConfiguration:
-    # pylint: disable=too-many-instance-attributes, too-many-arguments
-    validate_certificates: bool = True
-    certificate_chain: Optional[_CertificateChain] = None
-    ciphers: Optional[_Ciphers] = None
-    inner_protocols: Optional[_InnerProtocols] = None
-    lowest_supported_version: DTLSVersion = DTLSVersion.DTLSv1_0
-    highest_supported_version: DTLSVersion = DTLSVersion.MAXIMUM_SUPPORTED
-    trust_store: Optional[TrustStore] = None
-    max_fragmentation_length: Optional[MaxFragmentLength] = None
-    anti_replay: bool = True
-    handshake_timeout_min: float = 1.0
-    handshake_timeout_max: float = 60.0
-    sni_callback: Optional[ServerNameCallback] = None
-    pre_shared_key: Optional[Tuple[str, bytes]] = None
-    pre_shared_key_store: Mapping[str, bytes] = field(default_factory=dict)
-
-    def __eq__(self, other: object) -> bool:
-        if not isinstance(other, DTLSConfiguration):
-            return NotImplemented
-        return all(
-            (
-                self.validate_certificates == other.validate_certificates,
-                self.certificate_chain == other.certificate_chain
-                or (
-                    not self.certificate_chain and not other.certificate_chain
-                ),
-                self.ciphers == other.ciphers
-                or (not self.ciphers and not other.ciphers),
-                self.inner_protocols == other.inner_protocols
-                or (not self.inner_protocols and not other.inner_protocols),
-                self.lowest_supported_version == other.lowest_supported_version
-                or (
-                    self.lowest_supported_version
-                    in {
-                        DTLSVersion.MINIMUM_SUPPORTED,
-                        DTLSVersion.MAXIMUM_SUPPORTED,
-                    }
-                )
-                or (
-                    other.lowest_supported_version
-                    in {
-                        DTLSVersion.MINIMUM_SUPPORTED,
-                        DTLSVersion.MAXIMUM_SUPPORTED,
-                    }
-                ),
-                self.highest_supported_version
-                == other.highest_supported_version
-                or (
-                    self.highest_supported_version
-                    in {
-                        DTLSVersion.MINIMUM_SUPPORTED,
-                        DTLSVersion.MAXIMUM_SUPPORTED,
-                    }
-                )
-                or (
-                    other.highest_supported_version
-                    in {
-                        DTLSVersion.MINIMUM_SUPPORTED,
-                        DTLSVersion.MAXIMUM_SUPPORTED,
-                    }
-                ),
-                self.trust_store == other.trust_store
-                or (not self.trust_store and not other.trust_store)
-                or (not self.trust_store and not other.trust_store),
-                self.max_fragmentation_length
-                == other.max_fragmentation_length,
-                self.anti_replay == other.anti_replay,
-                self.handshake_timeout_min == other.handshake_timeout_min,
-                self.handshake_timeout_max == other.handshake_timeout_max,
-                self.sni_callback == other.sni_callback,
-                self.pre_shared_key == other.pre_shared_key,
-                self.pre_shared_key_store == other.pre_shared_key_store,
-            )
-        )
-
-    def update(
-        self,
-        validate_certificates: _Wrap[bool] = _DEFAULT_VALUE,
-        certificate_chain: _Wrap[_CertificateChain] = _DEFAULT_VALUE,
-        ciphers: _Wrap[_Ciphers] = _DEFAULT_VALUE,
-        inner_protocols: _Wrap[_InnerProtocols] = _DEFAULT_VALUE,
-        lowest_supported_version: _Wrap[DTLSVersion] = _DEFAULT_VALUE,
-        highest_supported_version: _Wrap[DTLSVersion] = _DEFAULT_VALUE,
-        trust_store: _Wrap[TrustStore] = _DEFAULT_VALUE,
-        max_fragmentation_length: _Wrap[MaxFragmentLength] = _DEFAULT_VALUE,
-        anti_replay: _Wrap[bool] = _DEFAULT_VALUE,
-        handshake_timeout_min: _Wrap[float] = _DEFAULT_VALUE,
-        handshake_timeout_max: _Wrap[float] = _DEFAULT_VALUE,
-        sni_callback: _Wrap[ServerNameCallback] = _DEFAULT_VALUE,
-        pre_shared_key: _Wrap[Tuple[str, bytes]] = _DEFAULT_VALUE,
-        pre_shared_key_store: _Wrap[Mapping[str, bytes]] = _DEFAULT_VALUE,
-    ) -> DTLSConfiguration:
-        """
-        Create a new ``TLSConfiguration``, overriding some of the settings
-        on the original configuration with the new settings.
-        """
-        return self.__class__(
-            validate_certificates=_unwrap(
-                validate_certificates,
-                self.validate_certificates,
-            ),
-            certificate_chain=_unwrap(
-                certificate_chain,
-                self.certificate_chain,
-            ),
-            ciphers=_unwrap(ciphers, self.ciphers),
-            inner_protocols=_unwrap(inner_protocols, self.inner_protocols),
-            lowest_supported_version=_unwrap(
-                lowest_supported_version,
-                self.lowest_supported_version,
-            ),
-            highest_supported_version=_unwrap(
-                highest_supported_version,
-                self.highest_supported_version,
-            ),
-            trust_store=_unwrap(trust_store, self.trust_store),
-            max_fragmentation_length=_unwrap(
-                max_fragmentation_length,
-                self.max_fragmentation_length,
-            ),
-            anti_replay=_unwrap(anti_replay, self.anti_replay),
-            handshake_timeout_min=_unwrap(
-                handshake_timeout_min,
-                self.handshake_timeout_min,
-            ),
-            handshake_timeout_max=_unwrap(
-                handshake_timeout_max,
-                self.handshake_timeout_max,
-            ),
-            sni_callback=_unwrap(sni_callback, self.sni_callback),
-            pre_shared_key=_unwrap(pre_shared_key, self.pre_shared_key),
-            pre_shared_key_store=_unwrap(
-                pre_shared_key_store,
-                self.pre_shared_key_store,
-            ),
-        )
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2018, Mathias Laurin
+
+"""Interfaces defined in PEP 543 (+ DTLS)."""
+
+from __future__ import annotations
+
+import enum
+import os
+import sys
+from dataclasses import dataclass, field
+from typing import (
+    Callable,
+    Literal,
+    Mapping,
+    Optional,
+    Protocol,
+    Tuple,
+    TypeVar,
+    Union,
+)
+
+if sys.version_info < (3, 9):
+    _PathLike = os.PathLike
+else:
+    _PathLike = os.PathLike[str]
+
+__all__ = ["NextProtocol", "TLSVersion", "DTLSVersion"]
+
+_Path = Union[_PathLike, str]
+
+
+@enum.unique
+class NextProtocol(enum.Enum):
+    H2: bytes = b"h2"
+    H2C: bytes = b"h2c"
+    HTTP1: bytes = b"http/1.1"
+    WEBRTC: bytes = b"webrtc"
+    C_WEBRTC: bytes = b"c-webrtc"
+    FTP: bytes = b"ftp"
+    STUN: bytes = b"stun.nat-discovery"
+    TURN: bytes = b"stun.turn"
+
+
+class MaxFragmentLength(enum.Enum):
+    NONE = 0
+    MFL_512K = 1
+    MFL_1024K = 2
+    MFL_2048K = 3
+    MFL_4096K = 4
+
+
+class TLSVersion(enum.Enum):
+    # PEP 543
+    MINIMUM_SUPPORTED = enum.auto()
+    SSLv2 = enum.auto()
+    SSLv3 = enum.auto()
+    TLSv1 = enum.auto()
+    TLSv1_1 = enum.auto()
+    TLSv1_2 = enum.auto()
+    TLSv1_3 = enum.auto()
+    MAXIMUM_SUPPORTED = enum.auto()
+
+
+class DTLSVersion(enum.Enum):
+    MINIMUM_SUPPORTED = enum.auto()
+    DTLSv1_0 = enum.auto()
+    DTLSv1_2 = enum.auto()
+    MAXIMUM_SUPPORTED = enum.auto()
+
+
+class TrustStore(Protocol):
+    @classmethod
+    def system(cls) -> TrustStore:
+        """Returns a TrustStore object that represents the system
+        trust database.
+
+        """
+
+    @classmethod
+    def from_pem_file(cls, path: _Path) -> TrustStore:
+        """Initializes a trust store from a single file full of PEMs."""
+
+
+class Certificate(Protocol):
+    @classmethod
+    def from_buffer(cls, buffer: bytes) -> Certificate:
+        """Creates a Certificate object from a byte buffer.
+
+        This byte buffer may be either PEM-encoded or DER-encoded. If the
+        buffer is PEM encoded it *must* begin with the standard PEM
+        preamble (a series of dashes followed by the ASCII bytes "BEGIN
+        CERTIFICATE" and another series of dashes). In the absence of that
+        preamble, the implementation may assume that the certificate is
+        DER-encoded instead.
+
+        """
+
+    @classmethod
+    def from_file(cls, path: _Path) -> Certificate:
+        """Creates a Certificate object from a file on disk.
+
+        This method may be a convenience method that wraps ``open`` and
+        ``from_buffer``, but some TLS implementations may be able to
+        provide more-secure or faster methods of loading certificates that
+        do not involve Python code.
+
+        """
+
+
+class PrivateKey(Protocol):
+    @classmethod
+    def from_buffer(
+        cls,
+        buffer: bytes,
+        password: Optional[
+            Union[Callable[[], Union[bytes, bytearray]], bytes, bytearray]
+        ] = None,
+    ) -> PrivateKey:
+        """Creates a PrivateKey object from a byte buffer.
+
+        This byte buffer may be either PEM-encoded or DER-encoded. If the
+        buffer is PEM encoded it *must* begin with the standard PEM
+        preamble (a series of dashes followed by the ASCII bytes "BEGIN",
+        the key type, and another series of dashes). In the absence of
+        that preamble, the implementation may assume that the certificate
+        is DER-encoded instead.
+
+        The key may additionally be encrypted. If it is, the ``password``
+        argument can be used to decrypt the key. The ``password`` argument
+        may be a function to call to get the password for decrypting the
+        private key. It will only be called if the private key is encrypted
+        and a password is necessary. It will be called with no arguments,
+        and it should return either bytes or bytearray containing the
+        password. Alternatively a bytes, or bytearray value may be supplied
+        directly as the password argument. It will be ignored if the
+        private key is not encrypted and no password is needed.
+        """
+
+    @classmethod
+    def from_file(
+        cls,
+        path: _Path,
+        password: Optional[
+            Union[Callable[[], Union[bytes, bytearray]], bytes, bytearray]
+        ] = None,
+    ) -> PrivateKey:
+        """Creates a PrivateKey object from a file on disk.
+
+        This method may be a convenience method that wraps ``open`` and
+        ``from_buffer``, but some TLS implementations may be able to
+        provide more-secure or faster methods of loading certificates that
+        do not involve Python code.
+
+        The ``password`` parameter behaves exactly as the equivalent
+        parameter on ``from_buffer``.
+        """
+
+
+CipherSuite = object
+DEFAULT_CIPHER_LIST = ()
+
+ServerNameCallback = object
+
+
+class __DefaultValue(enum.Enum):
+    DEFAULT_VALUE = enum.auto()
+
+
+_DEFAULT_VALUE = __DefaultValue.DEFAULT_VALUE
+
+T = TypeVar("T")
+_Wrap = Union[T, Literal[__DefaultValue.DEFAULT_VALUE]]
+
+
+def _unwrap(x: _Wrap[T], default: T) -> T:
+    if x is _DEFAULT_VALUE:
+        return default
+    return x
+
+
+_CertificateChain = Tuple[Tuple[Certificate, ...], PrivateKey]
+_Ciphers = Tuple[Union[CipherSuite, int], ...]
+_InnerProtocols = Tuple[Union[NextProtocol, bytes], ...]
+
+
+@dataclass(frozen=True)
+class TLSConfiguration:
+    # pylint: disable=too-many-instance-attributes, too-many-arguments
+    validate_certificates: bool = True
+    certificate_chain: Optional[_CertificateChain] = None
+    ciphers: Optional[_Ciphers] = None
+    inner_protocols: Optional[_InnerProtocols] = None
+    lowest_supported_version: TLSVersion = TLSVersion.TLSv1
+    highest_supported_version: TLSVersion = TLSVersion.MAXIMUM_SUPPORTED
+    trust_store: Optional[TrustStore] = None
+    max_fragmentation_length: Optional[MaxFragmentLength] = None
+    sni_callback: Optional[ServerNameCallback] = None
+    pre_shared_key: Optional[Tuple[str, bytes]] = None
+    pre_shared_key_store: Mapping[str, bytes] = field(default_factory=dict)
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, TLSConfiguration):
+            return NotImplemented
+        return all(
+            (
+                self.validate_certificates == other.validate_certificates,
+                self.certificate_chain == other.certificate_chain
+                or (
+                    not self.certificate_chain and not other.certificate_chain
+                ),
+                self.ciphers == other.ciphers
+                or (not self.ciphers and not other.ciphers),
+                self.inner_protocols == other.inner_protocols
+                or (not self.inner_protocols and not other.inner_protocols),
+                self.lowest_supported_version == other.lowest_supported_version
+                or (
+                    self.lowest_supported_version
+                    in {
+                        TLSVersion.MINIMUM_SUPPORTED,
+                        TLSVersion.MAXIMUM_SUPPORTED,
+                    }
+                )
+                or (
+                    other.lowest_supported_version
+                    in {
+                        TLSVersion.MINIMUM_SUPPORTED,
+                        TLSVersion.MAXIMUM_SUPPORTED,
+                    }
+                ),
+                self.highest_supported_version
+                == other.highest_supported_version
+                or (
+                    self.highest_supported_version
+                    in {
+                        TLSVersion.MINIMUM_SUPPORTED,
+                        TLSVersion.MAXIMUM_SUPPORTED,
+                    }
+                )
+                or (
+                    other.highest_supported_version
+                    in {
+                        TLSVersion.MINIMUM_SUPPORTED,
+                        TLSVersion.MAXIMUM_SUPPORTED,
+                    }
+                ),
+                self.trust_store == other.trust_store
+                or (not self.trust_store and not other.trust_store),
+                self.max_fragmentation_length
+                == other.max_fragmentation_length,
+                self.sni_callback == other.sni_callback,
+                self.pre_shared_key == other.pre_shared_key,
+                self.pre_shared_key_store == other.pre_shared_key_store,
+            )
+        )
+
+    def update(
+        self,
+        validate_certificates: _Wrap[bool] = _DEFAULT_VALUE,
+        certificate_chain: _Wrap[_CertificateChain] = _DEFAULT_VALUE,
+        ciphers: _Wrap[_Ciphers] = _DEFAULT_VALUE,
+        inner_protocols: _Wrap[_InnerProtocols] = _DEFAULT_VALUE,
+        lowest_supported_version: _Wrap[TLSVersion] = _DEFAULT_VALUE,
+        highest_supported_version: _Wrap[TLSVersion] = _DEFAULT_VALUE,
+        trust_store: _Wrap[TrustStore] = _DEFAULT_VALUE,
+        max_fragmentation_length: _Wrap[MaxFragmentLength] = _DEFAULT_VALUE,
+        sni_callback: _Wrap[Optional[ServerNameCallback]] = _DEFAULT_VALUE,
+        pre_shared_key: _Wrap[Tuple[str, bytes]] = _DEFAULT_VALUE,
+        pre_shared_key_store: _Wrap[Mapping[str, bytes]] = _DEFAULT_VALUE,
+    ) -> TLSConfiguration:
+        """
+        Create a new ``TLSConfiguration``, overriding some of the settings
+        on the original configuration with the new settings.
+        """
+        return self.__class__(
+            validate_certificates=_unwrap(
+                validate_certificates,
+                self.validate_certificates,
+            ),
+            certificate_chain=_unwrap(
+                certificate_chain,
+                self.certificate_chain,
+            ),
+            ciphers=_unwrap(ciphers, self.ciphers),
+            inner_protocols=_unwrap(inner_protocols, self.inner_protocols),
+            lowest_supported_version=_unwrap(
+                lowest_supported_version,
+                self.lowest_supported_version,
+            ),
+            highest_supported_version=_unwrap(
+                highest_supported_version,
+                self.highest_supported_version,
+            ),
+            trust_store=_unwrap(trust_store, self.trust_store),
+            max_fragmentation_length=_unwrap(
+                max_fragmentation_length,
+                self.max_fragmentation_length,
+            ),
+            sni_callback=_unwrap(sni_callback, self.sni_callback),
+            pre_shared_key=_unwrap(pre_shared_key, self.pre_shared_key),
+            pre_shared_key_store=_unwrap(
+                pre_shared_key_store,
+                self.pre_shared_key_store,
+            ),
+        )
+
+
+@dataclass(frozen=True)
+class DTLSConfiguration:
+    # pylint: disable=too-many-instance-attributes, too-many-arguments
+    validate_certificates: bool = True
+    certificate_chain: Optional[_CertificateChain] = None
+    ciphers: Optional[_Ciphers] = None
+    inner_protocols: Optional[_InnerProtocols] = None
+    lowest_supported_version: DTLSVersion = DTLSVersion.DTLSv1_0
+    highest_supported_version: DTLSVersion = DTLSVersion.MAXIMUM_SUPPORTED
+    trust_store: Optional[TrustStore] = None
+    max_fragmentation_length: Optional[MaxFragmentLength] = None
+    anti_replay: bool = True
+    handshake_timeout_min: float = 1.0
+    handshake_timeout_max: float = 60.0
+    sni_callback: Optional[ServerNameCallback] = None
+    pre_shared_key: Optional[Tuple[str, bytes]] = None
+    pre_shared_key_store: Mapping[str, bytes] = field(default_factory=dict)
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, DTLSConfiguration):
+            return NotImplemented
+        return all(
+            (
+                self.validate_certificates == other.validate_certificates,
+                self.certificate_chain == other.certificate_chain
+                or (
+                    not self.certificate_chain and not other.certificate_chain
+                ),
+                self.ciphers == other.ciphers
+                or (not self.ciphers and not other.ciphers),
+                self.inner_protocols == other.inner_protocols
+                or (not self.inner_protocols and not other.inner_protocols),
+                self.lowest_supported_version == other.lowest_supported_version
+                or (
+                    self.lowest_supported_version
+                    in {
+                        DTLSVersion.MINIMUM_SUPPORTED,
+                        DTLSVersion.MAXIMUM_SUPPORTED,
+                    }
+                )
+                or (
+                    other.lowest_supported_version
+                    in {
+                        DTLSVersion.MINIMUM_SUPPORTED,
+                        DTLSVersion.MAXIMUM_SUPPORTED,
+                    }
+                ),
+                self.highest_supported_version
+                == other.highest_supported_version
+                or (
+                    self.highest_supported_version
+                    in {
+                        DTLSVersion.MINIMUM_SUPPORTED,
+                        DTLSVersion.MAXIMUM_SUPPORTED,
+                    }
+                )
+                or (
+                    other.highest_supported_version
+                    in {
+                        DTLSVersion.MINIMUM_SUPPORTED,
+                        DTLSVersion.MAXIMUM_SUPPORTED,
+                    }
+                ),
+                self.trust_store == other.trust_store
+                or (not self.trust_store and not other.trust_store)
+                or (not self.trust_store and not other.trust_store),
+                self.max_fragmentation_length
+                == other.max_fragmentation_length,
+                self.anti_replay == other.anti_replay,
+                self.handshake_timeout_min == other.handshake_timeout_min,
+                self.handshake_timeout_max == other.handshake_timeout_max,
+                self.sni_callback == other.sni_callback,
+                self.pre_shared_key == other.pre_shared_key,
+                self.pre_shared_key_store == other.pre_shared_key_store,
+            )
+        )
+
+    def update(
+        self,
+        validate_certificates: _Wrap[bool] = _DEFAULT_VALUE,
+        certificate_chain: _Wrap[_CertificateChain] = _DEFAULT_VALUE,
+        ciphers: _Wrap[_Ciphers] = _DEFAULT_VALUE,
+        inner_protocols: _Wrap[_InnerProtocols] = _DEFAULT_VALUE,
+        lowest_supported_version: _Wrap[DTLSVersion] = _DEFAULT_VALUE,
+        highest_supported_version: _Wrap[DTLSVersion] = _DEFAULT_VALUE,
+        trust_store: _Wrap[TrustStore] = _DEFAULT_VALUE,
+        max_fragmentation_length: _Wrap[MaxFragmentLength] = _DEFAULT_VALUE,
+        anti_replay: _Wrap[bool] = _DEFAULT_VALUE,
+        handshake_timeout_min: _Wrap[float] = _DEFAULT_VALUE,
+        handshake_timeout_max: _Wrap[float] = _DEFAULT_VALUE,
+        sni_callback: _Wrap[ServerNameCallback] = _DEFAULT_VALUE,
+        pre_shared_key: _Wrap[Tuple[str, bytes]] = _DEFAULT_VALUE,
+        pre_shared_key_store: _Wrap[Mapping[str, bytes]] = _DEFAULT_VALUE,
+    ) -> DTLSConfiguration:
+        """
+        Create a new ``TLSConfiguration``, overriding some of the settings
+        on the original configuration with the new settings.
+        """
+        return self.__class__(
+            validate_certificates=_unwrap(
+                validate_certificates,
+                self.validate_certificates,
+            ),
+            certificate_chain=_unwrap(
+                certificate_chain,
+                self.certificate_chain,
+            ),
+            ciphers=_unwrap(ciphers, self.ciphers),
+            inner_protocols=_unwrap(inner_protocols, self.inner_protocols),
+            lowest_supported_version=_unwrap(
+                lowest_supported_version,
+                self.lowest_supported_version,
+            ),
+            highest_supported_version=_unwrap(
+                highest_supported_version,
+                self.highest_supported_version,
+            ),
+            trust_store=_unwrap(trust_store, self.trust_store),
+            max_fragmentation_length=_unwrap(
+                max_fragmentation_length,
+                self.max_fragmentation_length,
+            ),
+            anti_replay=_unwrap(anti_replay, self.anti_replay),
+            handshake_timeout_min=_unwrap(
+                handshake_timeout_min,
+                self.handshake_timeout_min,
+            ),
+            handshake_timeout_max=_unwrap(
+                handshake_timeout_max,
+                self.handshake_timeout_max,
+            ),
+            sni_callback=_unwrap(sni_callback, self.sni_callback),
+            pre_shared_key=_unwrap(pre_shared_key, self.pre_shared_key),
+            pre_shared_key_store=_unwrap(
+                pre_shared_key_store,
+                self.pre_shared_key_store,
+            ),
+        )
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/cipher/AES.py` & `python-mbedtls-2.7.1/src/mbedtls/cipher/AES.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,100 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2016, Elaborated Networks GmbH
-# Copyright (c) 2019, Mathias Laurin
-
-"""Advanced Encryption Standard (AES) cipher established by the U.S.
-NIST in 2001.
-
-"""
-
-from __future__ import annotations
-
-import sys
-from typing import Optional, Union, overload
-
-from mbedtls.exceptions import TLSError
-
-from ._cipher import AEADCipher, Cipher, Mode
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Final, Literal
-else:
-    from typing import Final, Literal
-
-__all__ = ["block_size", "key_size", "new"]
-
-
-block_size: Final = 16
-key_size: Final = None
-
-
-@overload
-def new(
-    key: bytes,
-    mode: Literal[Mode.CCM, Mode.GCM],
-    iv: Optional[bytes] = ...,
-    ad: Optional[bytes] = ...,
-) -> AEADCipher:
-    ...
-
-
-@overload
-def new(
-    key: bytes,
-    mode: Literal[Mode.CBC, Mode.CFB, Mode.CTR, Mode.ECB, Mode.OFB, Mode.XTS],
-    iv: Optional[bytes] = ...,
-) -> Cipher:
-    ...
-
-
-def new(
-    key: bytes,
-    mode: Union[Mode, int],
-    iv: Optional[bytes] = None,
-    ad: Optional[bytes] = None,
-) -> Union[AEADCipher, Cipher]:
-    """Return a `Cipher` object that can perform AES encryption and
-    decryption.
-
-    Advanced Encryption Standard (AES) cipher established by the U.S.
-    NIST in 2001.
-
-    Parameters:
-        key: The key to encrypt decrypt.  If None,
-            encryption and decryption are unavailable.
-        mode: The mode of operation of the cipher.
-        iv: The initialization vector (IV).  The IV is
-            required for every mode but ECB and CTR where it is ignored.
-            If not set, the IV is initialized to all 0, which should not
-            be used for encryption.
-
-    """
-    mode_ = Mode(mode)
-    if mode_ in {
-        Mode.CBC,
-        Mode.CCM,
-        Mode.CFB,
-        Mode.CTR,
-        Mode.ECB,
-        Mode.GCM,
-        Mode.OFB,
-    }:
-        if len(key) not in {16, 24, 32}:
-            raise TLSError(
-                msg="key size must 16, 24, or 32 bytes, got %i" % len(key)
-            )
-    elif mode_ is Mode.XTS:
-        if len(key) not in {32, 64}:
-            raise TLSError(
-                msg="key size must 32, or 64 bytes, got %i" % len(key)
-            )
-    else:
-        raise TLSError(msg="unsupported mode %r" % mode_)
-    if mode_ is Mode.XTS:
-        name = ("AES-%i-%s" % (len(key) * 4, mode_.name)).encode("ascii")
-    else:
-        name = (
-            "AES-%i-%s%s"
-            % (
-                len(key) * 8,
-                mode_.name,
-                "128" if mode_ is Mode.CFB else "",
-            )
-        ).encode("ascii")
-    if mode_ in {Mode.GCM, Mode.CCM}:
-        return AEADCipher(name, key, mode_, iv, ad)
-    return Cipher(name, key, mode_, iv)
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2016, Elaborated Networks GmbH
+# Copyright (c) 2019, Mathias Laurin
+
+"""Advanced Encryption Standard (AES) cipher established by the U.S.
+NIST in 2001.
+
+"""
+
+from __future__ import annotations
+
+from typing import Final, Literal, Optional, Union, overload
+
+from mbedtls.exceptions import TLSError
+
+from ._cipher import AEADCipher, Cipher, Mode
+
+__all__ = ["block_size", "key_size", "new"]
+
+
+block_size: Final = 16
+key_size: Final = None
+
+
+@overload
+def new(
+    key: bytes,
+    mode: Literal[Mode.CCM, Mode.GCM],
+    iv: Optional[bytes] = ...,
+    ad: Optional[bytes] = ...,
+) -> AEADCipher:
+    ...
+
+
+@overload
+def new(
+    key: bytes,
+    mode: Literal[Mode.CBC, Mode.CFB, Mode.CTR, Mode.ECB, Mode.OFB, Mode.XTS],
+    iv: Optional[bytes] = ...,
+) -> Cipher:
+    ...
+
+
+def new(
+    key: bytes,
+    mode: Union[Mode, int],
+    iv: Optional[bytes] = None,
+    ad: Optional[bytes] = None,
+) -> Union[AEADCipher, Cipher]:
+    """Return a `Cipher` object that can perform AES encryption and
+    decryption.
+
+    Advanced Encryption Standard (AES) cipher established by the U.S.
+    NIST in 2001.
+
+    Parameters:
+        key: The key to encrypt decrypt.  If None,
+            encryption and decryption are unavailable.
+        mode: The mode of operation of the cipher.
+        iv: The initialization vector (IV).  The IV is
+            required for every mode but ECB and CTR where it is ignored.
+            If not set, the IV is initialized to all 0, which should not
+            be used for encryption.
+
+    """
+    mode_ = Mode(mode)
+    if mode_ in {
+        Mode.CBC,
+        Mode.CCM,
+        Mode.CFB,
+        Mode.CTR,
+        Mode.ECB,
+        Mode.GCM,
+        Mode.OFB,
+    }:
+        if len(key) not in {16, 24, 32}:
+            raise TLSError(
+                msg="key size must 16, 24, or 32 bytes, got %i" % len(key)
+            )
+    elif mode_ is Mode.XTS:
+        if len(key) not in {32, 64}:
+            raise TLSError(
+                msg="key size must 32, or 64 bytes, got %i" % len(key)
+            )
+    else:
+        raise TLSError(msg="unsupported mode %r" % mode_)
+    if mode_ is Mode.XTS:
+        name = ("AES-%i-%s" % (len(key) * 4, mode_.name)).encode("ascii")
+    else:
+        name = (
+            "AES-%i-%s%s"
+            % (
+                len(key) * 8,
+                mode_.name,
+                "128" if mode_ is Mode.CFB else "",
+            )
+        ).encode("ascii")
+    if mode_ in {Mode.GCM, Mode.CCM}:
+        return AEADCipher(name, key, mode_, iv, ad)
+    return Cipher(name, key, mode_, iv)
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/cipher/ARC4.py` & `python-mbedtls-2.7.1/src/mbedtls/cipher/ARC4.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,47 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2016, Elaborated Networks GmbH
-# Copyright (c) 2019, Mathias Laurin
-
-"""Alleged River Cipher 4 cipher (ARC4 or ARCFOUR) designed in 1987
-at RSA Security."""
-
-from __future__ import annotations
-
-import sys
-from typing import Optional, Union
-
-from mbedtls.exceptions import TLSError
-
-from ._cipher import Cipher, Mode
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Final, Literal
-else:
-    from typing import Final, Literal
-
-__all__ = ["block_size", "key_size", "new"]
-
-block_size: Final = 1
-key_size: Final = 16
-
-
-def new(
-    key: bytes,
-    mode: Optional[Union[int, Literal[Mode.STREAM]]] = None,
-    iv: Optional[bytes] = None,
-) -> Cipher:
-    """Return a `Cipher` object that can perform ARC4 encryption and
-    decryption.
-
-    Alleged River Cipher 4 cipher (ARC4 or ARCFOUR) designed in 1987
-    at RSA Security.
-
-    Parameters:
-        key: The key to encrypt decrypt.  If None,
-            encryption and decryption are unavailable.
-        mode: The feedback mode is ignored for ARC4.
-        iv: ARC4 does not use IV.
-
-    """
-    if len(key) != key_size:
-        raise TLSError(
-            msg="key size must be %i bytes, got %i" % (key_size, len(key))
-        )
-    if mode not in {None, Mode.STREAM}:
-        raise TLSError(msg="unsupported mode %r" % mode)
-    name = ("ARC4-%i" % (len(key) * 8)).encode("ascii")
-    return Cipher(name, key, Mode.STREAM, iv)
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2016, Elaborated Networks GmbH
+# Copyright (c) 2019, Mathias Laurin
+
+"""Alleged River Cipher 4 cipher (ARC4 or ARCFOUR) designed in 1987
+at RSA Security."""
+
+from __future__ import annotations
+
+from typing import Final, Literal, Optional, Union
+
+from mbedtls.exceptions import TLSError
+
+from ._cipher import Cipher, Mode
+
+__all__ = ["block_size", "key_size", "new"]
+
+block_size: Final = 1
+key_size: Final = 16
+
+
+def new(
+    key: bytes,
+    mode: Optional[Union[int, Literal[Mode.STREAM]]] = None,
+    iv: Optional[bytes] = None,
+) -> Cipher:
+    """Return a `Cipher` object that can perform ARC4 encryption and
+    decryption.
+
+    Alleged River Cipher 4 cipher (ARC4 or ARCFOUR) designed in 1987
+    at RSA Security.
+
+    Parameters:
+        key: The key to encrypt decrypt.  If None,
+            encryption and decryption are unavailable.
+        mode: The feedback mode is ignored for ARC4.
+        iv: ARC4 does not use IV.
+
+    """
+    if len(key) != key_size:
+        raise TLSError(
+            msg="key size must be %i bytes, got %i" % (key_size, len(key))
+        )
+    if mode not in {None, Mode.STREAM}:
+        raise TLSError(msg="unsupported mode %r" % mode)
+    name = ("ARC4-%i" % (len(key) * 8)).encode("ascii")
+    return Cipher(name, key, Mode.STREAM, iv)
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/cipher/ARIA.py` & `python-mbedtls-2.7.1/src/mbedtls/cipher/ARIA.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,63 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2019, Mathias Laurin
-
-"""The ARIA algorithm is a symmetric block cipher that can encrypt and
-decrypt information. It is defined by the Korean Agency for Technology
-and Standards (KATS) in *KS X 1213:2004* (in Korean, but see
-http://210.104.33.10/ARIA/index-e.html in English) and also described by
-the IETF in *RFC 5794*.
-
-"""
-
-from __future__ import annotations
-
-import sys
-from typing import Optional, Union
-
-from mbedtls.exceptions import TLSError
-
-from ._cipher import Cipher, Mode
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Final, Literal
-else:
-    from typing import Final, Literal
-
-__all__ = ["block_size", "key_size", "new"]
-
-
-block_size: Final = 16
-key_size: Final = None
-
-
-def new(
-    key: bytes,
-    mode: Union[int, Literal[Mode.CBC, Mode.CTR, Mode.ECB, Mode.GCM]],
-    iv: Optional[bytes] = None,
-) -> Cipher:
-    """Return a `Cipher` object that can perform ARIA encryption and
-    decryption.
-
-    ARIA is a block cipher designed in 2003 by a large group of South
-    Korean researchers. In 2004, the Korean Agency for Technology and
-    Standards selected it as a standard cryptographic technique.
-
-    Parameters:
-        key: The key to encrypt decrypt.
-        mode: The mode of operation of the cipher.
-        iv: The initialization vector (IV).  The IV is
-            required for every mode but ECB and CTR where it is ignored.
-            If not set, the IV is initialized to all 0, which should not
-            be used for encryption.
-
-    """
-    mode_ = Mode(mode)
-    if mode_ in {
-        Mode.CBC,
-        # Mode.CFB128,
-        Mode.CTR,
-        Mode.ECB,
-        Mode.GCM,
-    }:
-        if len(key) * 8 not in {128, 192, 256}:
-            raise TLSError(
-                msg="key size must 16, 24, or 32 bytes, got %i" % len(key)
-            )
-    else:
-        raise TLSError(msg="unsupported mode %r" % mode_)
-    name = ("ARIA-%i-%s" % (len(key) * 8, mode_.name)).encode("ascii")
-    return Cipher(name, key, mode_, iv)
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2019, Mathias Laurin
+
+"""The ARIA algorithm is a symmetric block cipher that can encrypt and
+decrypt information. It is defined by the Korean Agency for Technology
+and Standards (KATS) in *KS X 1213:2004* (in Korean, but see
+http://210.104.33.10/ARIA/index-e.html in English) and also described by
+the IETF in *RFC 5794*.
+
+"""
+
+from __future__ import annotations
+
+from typing import Final, Literal, Optional, Union
+
+from mbedtls.exceptions import TLSError
+
+from ._cipher import Cipher, Mode
+
+__all__ = ["block_size", "key_size", "new"]
+
+
+block_size: Final = 16
+key_size: Final = None
+
+
+def new(
+    key: bytes,
+    mode: Union[int, Literal[Mode.CBC, Mode.CTR, Mode.ECB, Mode.GCM]],
+    iv: Optional[bytes] = None,
+) -> Cipher:
+    """Return a `Cipher` object that can perform ARIA encryption and
+    decryption.
+
+    ARIA is a block cipher designed in 2003 by a large group of South
+    Korean researchers. In 2004, the Korean Agency for Technology and
+    Standards selected it as a standard cryptographic technique.
+
+    Parameters:
+        key: The key to encrypt decrypt.
+        mode: The mode of operation of the cipher.
+        iv: The initialization vector (IV).  The IV is
+            required for every mode but ECB and CTR where it is ignored.
+            If not set, the IV is initialized to all 0, which should not
+            be used for encryption.
+
+    """
+    mode_ = Mode(mode)
+    if mode_ in {
+        Mode.CBC,
+        # Mode.CFB128,
+        Mode.CTR,
+        Mode.ECB,
+        Mode.GCM,
+    }:
+        if len(key) * 8 not in {128, 192, 256}:
+            raise TLSError(
+                msg="key size must 16, 24, or 32 bytes, got %i" % len(key)
+            )
+    else:
+        raise TLSError(msg="unsupported mode %r" % mode_)
+    name = ("ARIA-%i-%s" % (len(key) * 8, mode_.name)).encode("ascii")
+    return Cipher(name, key, mode_, iv)
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/cipher/CHACHA20.py` & `python-mbedtls-2.7.1/src/mbedtls/cipher/CHACHA20.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,77 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2019, Stephen Y.
-
-"""Salsa20 and the closely related ChaCha are stream ciphers
-developed by Daniel J. Bernstein.
-
-"""
-
-from __future__ import annotations
-
-import sys
-from typing import Optional, Union, overload
-
-from mbedtls.exceptions import TLSError
-
-from ._cipher import AEADCipher, Cipher, Mode
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Final, Literal
-else:
-    from typing import Final, Literal
-
-__all__ = ["block_size", "key_size", "new"]
-
-
-block_size: Final = 1
-key_size: Final = 32
-
-
-@overload
-def new(
-    key: bytes,
-    mode: Literal[Mode.STREAM],
-    iv: Optional[bytes] = ...,
-) -> Cipher:
-    ...
-
-
-@overload
-def new(
-    key: bytes,
-    mode: Literal[Mode.CHACHAPOLY],
-    iv: Optional[bytes] = ...,
-    ad: Optional[bytes] = ...,
-) -> AEADCipher:
-    ...
-
-
-def new(
-    key: bytes,
-    mode: Union[Literal[Mode.STREAM], Literal[Mode.CHACHAPOLY], int],
-    iv: Optional[bytes] = None,
-    ad: Optional[bytes] = None,
-) -> Union[Cipher, AEADCipher]:
-    """Return a `Cipher` object that can perform ChaCha20 encryption and
-    decryption.
-
-    ChaCha was created by Daniel Bernstein as a variant of
-    its Salsa cipher https://cr.yp.to/chacha/chacha-20080128.pdf
-    ChaCha20 is the variant with 20 rounds, that was also standardized
-    in RFC 7539.
-
-    Parameters:
-        key: The key to encrypt decrypt.  If None,
-            encryption and decryption are unavailable.
-        mode: The mode of operation of the cipher.
-        iv: The initialization vector (IV).  The IV is
-            required for every mode but ECB and CTR where it is ignored.
-            If not set, the IV is initialized to all 0, which should not
-            be used for encryption.
-        ad: The associated data for ChaCha/Poly mode.
-
-    """
-    mode_ = Mode(mode)
-    if len(key) != key_size:
-        raise TLSError(msg="key size must 32 bytes, got %r" % len(key))
-    if mode_ == Mode.STREAM:
-        assert ad is None
-        return Cipher(b"CHACHA20", key, mode_, iv)
-    if mode_ == Mode.CHACHAPOLY:
-        ad = b"" if ad is None else ad
-        return AEADCipher(b"CHACHA20-POLY1305", key, mode_, iv, ad)
-    raise TLSError(msg="unsupported mode %r" % mode_)
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2019, Stephen Y.
+
+"""Salsa20 and the closely related ChaCha are stream ciphers
+developed by Daniel J. Bernstein.
+
+"""
+
+from __future__ import annotations
+
+from typing import Final, Literal, Optional, Union, overload
+
+from mbedtls.exceptions import TLSError
+
+from ._cipher import AEADCipher, Cipher, Mode
+
+__all__ = ["block_size", "key_size", "new"]
+
+
+block_size: Final = 1
+key_size: Final = 32
+
+
+@overload
+def new(
+    key: bytes,
+    mode: Literal[Mode.STREAM],
+    iv: Optional[bytes] = ...,
+) -> Cipher:
+    ...
+
+
+@overload
+def new(
+    key: bytes,
+    mode: Literal[Mode.CHACHAPOLY],
+    iv: Optional[bytes] = ...,
+    ad: Optional[bytes] = ...,
+) -> AEADCipher:
+    ...
+
+
+def new(
+    key: bytes,
+    mode: Union[Literal[Mode.STREAM], Literal[Mode.CHACHAPOLY], int],
+    iv: Optional[bytes] = None,
+    ad: Optional[bytes] = None,
+) -> Union[Cipher, AEADCipher]:
+    """Return a `Cipher` object that can perform ChaCha20 encryption and
+    decryption.
+
+    ChaCha was created by Daniel Bernstein as a variant of
+    its Salsa cipher https://cr.yp.to/chacha/chacha-20080128.pdf
+    ChaCha20 is the variant with 20 rounds, that was also standardized
+    in RFC 7539.
+
+    Parameters:
+        key: The key to encrypt decrypt.  If None,
+            encryption and decryption are unavailable.
+        mode: The mode of operation of the cipher.
+        iv: The initialization vector (IV).  The IV is
+            required for every mode but ECB and CTR where it is ignored.
+            If not set, the IV is initialized to all 0, which should not
+            be used for encryption.
+        ad: The associated data for ChaCha/Poly mode.
+
+    """
+    mode_ = Mode(mode)
+    if len(key) != key_size:
+        raise TLSError(msg="key size must 32 bytes, got %r" % len(key))
+    if mode_ == Mode.STREAM:
+        assert ad is None
+        return Cipher(b"CHACHA20", key, mode_, iv)
+    if mode_ == Mode.CHACHAPOLY:
+        ad = b"" if ad is None else ad
+        return AEADCipher(b"CHACHA20-POLY1305", key, mode_, iv, ad)
+    raise TLSError(msg="unsupported mode %r" % mode_)
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/cipher/Camellia.py` & `python-mbedtls-2.7.1/src/mbedtls/cipher/Camellia.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,55 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2016, Elaborated Networks GmbH
-# Copyright (c) 2019, Mathias Laurin
-
-"""Camellia cipher developed by Japan's Mitsubishi an NTT in 2000."""
-
-
-from __future__ import annotations
-
-import sys
-from typing import Optional, Union
-
-from mbedtls.exceptions import TLSError
-
-from ._cipher import Cipher, Mode
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Final, Literal
-else:
-    from typing import Final, Literal
-
-__all__ = ["block_size", "key_size", "new"]
-
-block_size: Final = 16
-key_size: Final = None
-
-
-def new(
-    key: bytes,
-    mode: Union[
-        int, Literal[Mode.CBC, Mode.CFB, Mode.CTR, Mode.ECB, Mode.GCM]
-    ],
-    iv: Optional[bytes] = None,
-) -> Cipher:
-    """Return a `Cipher` object that can perform Camellia encryption and
-    decryption.
-
-    Camellia cipher developed by Japan's Mitsubishi an NTT in 2000.
-
-    Parameters:
-        key: The key to encrypt decrypt.  If None,
-            encryption and decryption are unavailable.
-        mode: The mode of operation of the cipher.
-        iv: The initialization vector (IV).  The IV is
-            required for every mode but ECB and CTR where it is ignored.
-            If not set, the IV is initialized to all 0, which should not
-            be used for encryption.
-
-    """
-    mode_ = Mode(mode)
-    if len(key) not in {16, 24, 32}:
-        raise TLSError(
-            msg="key size must 16, 24, or 32 bytes, got %r" % len(key)
-        )
-    if mode_ not in {Mode.CBC, Mode.CFB, Mode.CTR, Mode.ECB, Mode.GCM}:
-        raise TLSError(msg="unsupported mode %r" % mode_)
-    name = (
-        "CAMELLIA-%i-%s%s"
-        % (len(key) * 8, mode_.name, "128" if mode_ is Mode.CFB else "")
-    ).encode("ascii")
-    return Cipher(name, key, mode_, iv)
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2016, Elaborated Networks GmbH
+# Copyright (c) 2019, Mathias Laurin
+
+"""Camellia cipher developed by Japan's Mitsubishi an NTT in 2000."""
+
+
+from __future__ import annotations
+
+from typing import Final, Literal, Optional, Union
+
+from mbedtls.exceptions import TLSError
+
+from ._cipher import Cipher, Mode
+
+__all__ = ["block_size", "key_size", "new"]
+
+block_size: Final = 16
+key_size: Final = None
+
+
+def new(
+    key: bytes,
+    mode: Union[
+        int, Literal[Mode.CBC, Mode.CFB, Mode.CTR, Mode.ECB, Mode.GCM]
+    ],
+    iv: Optional[bytes] = None,
+) -> Cipher:
+    """Return a `Cipher` object that can perform Camellia encryption and
+    decryption.
+
+    Camellia cipher developed by Japan's Mitsubishi an NTT in 2000.
+
+    Parameters:
+        key: The key to encrypt decrypt.  If None,
+            encryption and decryption are unavailable.
+        mode: The mode of operation of the cipher.
+        iv: The initialization vector (IV).  The IV is
+            required for every mode but ECB and CTR where it is ignored.
+            If not set, the IV is initialized to all 0, which should not
+            be used for encryption.
+
+    """
+    mode_ = Mode(mode)
+    if len(key) not in {16, 24, 32}:
+        raise TLSError(
+            msg="key size must 16, 24, or 32 bytes, got %r" % len(key)
+        )
+    if mode_ not in {Mode.CBC, Mode.CFB, Mode.CTR, Mode.ECB, Mode.GCM}:
+        raise TLSError(msg="unsupported mode %r" % mode_)
+    name = (
+        "CAMELLIA-%i-%s%s"
+        % (len(key) * 8, mode_.name, "128" if mode_ is Mode.CFB else "")
+    ).encode("ascii")
+    return Cipher(name, key, mode_, iv)
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/cipher/DES.py` & `python-mbedtls-2.7.1/src/mbedtls/cipher/DES.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,49 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2016, Elaborated Networks GmbH
-# Copyright (c) 2019, Mathias Laurin
-
-"""Data Encryption Standard (DES) cipher developed by IBM
-in the 70's."""
-
-from __future__ import annotations
-
-import sys
-from typing import Optional, Union
-
-from mbedtls.exceptions import TLSError
-
-from ._cipher import Cipher, Mode
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Final, Literal
-else:
-    from typing import Final, Literal
-
-__all__ = ["block_size", "key_size", "new"]
-
-
-block_size: Final = 8
-key_size: Final = 8
-
-
-def new(
-    key: bytes,
-    mode: Union[int, Literal[Mode.CBC, Mode.ECB]],
-    iv: Optional[bytes] = None,
-) -> Cipher:
-    """Return a `Cipher` object that can perform DES encryption and
-    decryption.
-
-    Data Encryption Standard (DES) cipher developed by IBM in the 70's.
-
-    Parameters:
-        key: The key to encrypt decrypt.  If None,
-            encryption and decryption are unavailable.
-        mode: The mode of operation of the cipher.
-        iv: The initialization vector (IV).  The IV is
-            required for every mode but ECB and CTR where it is ignored.
-            If not set, the IV is initialized to all 0, which should not
-            be used for encryption.
-
-    """
-    mode_ = Mode(mode)
-    if len(key) != key_size:
-        raise TLSError(msg="key size must be 16 bytes, got %r" % len(key))
-    if mode_ not in {Mode.CBC, Mode.ECB}:
-        raise TLSError(msg="unsupported mode %r" % mode_)
-    name = ("DES-%s" % mode_.name).encode("ascii")
-    return Cipher(name, key, mode_, iv)
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2016, Elaborated Networks GmbH
+# Copyright (c) 2019, Mathias Laurin
+
+"""Data Encryption Standard (DES) cipher developed by IBM
+in the 70's."""
+
+from __future__ import annotations
+
+from typing import Final, Literal, Optional, Union
+
+from mbedtls.exceptions import TLSError
+
+from ._cipher import Cipher, Mode
+
+__all__ = ["block_size", "key_size", "new"]
+
+
+block_size: Final = 8
+key_size: Final = 8
+
+
+def new(
+    key: bytes,
+    mode: Union[int, Literal[Mode.CBC, Mode.ECB]],
+    iv: Optional[bytes] = None,
+) -> Cipher:
+    """Return a `Cipher` object that can perform DES encryption and
+    decryption.
+
+    Data Encryption Standard (DES) cipher developed by IBM in the 70's.
+
+    Parameters:
+        key: The key to encrypt decrypt.  If None,
+            encryption and decryption are unavailable.
+        mode: The mode of operation of the cipher.
+        iv: The initialization vector (IV).  The IV is
+            required for every mode but ECB and CTR where it is ignored.
+            If not set, the IV is initialized to all 0, which should not
+            be used for encryption.
+
+    """
+    mode_ = Mode(mode)
+    if len(key) != key_size:
+        raise TLSError(msg="key size must be 16 bytes, got %r" % len(key))
+    if mode_ not in {Mode.CBC, Mode.ECB}:
+        raise TLSError(msg="unsupported mode %r" % mode_)
+    name = ("DES-%s" % mode_.name).encode("ascii")
+    return Cipher(name, key, mode_, iv)
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/cipher/DES3.py` & `python-mbedtls-2.7.1/src/mbedtls/cipher/DES3.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,52 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2016, Elaborated Networks GmbH
-# Copyright (c) 2019, Mathias Laurin
-
-"""Three-key triple DES cipher (also known as DES3, 3DES,
-Triple DES, or DES-EDE3)."""
-
-from __future__ import annotations
-
-import sys
-from typing import Optional, Union
-
-from mbedtls.exceptions import TLSError
-
-from ._cipher import Cipher, Mode
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Final, Literal
-else:
-    from typing import Final, Literal
-
-__all__ = ["block_size", "key_size", "new"]
-
-
-block_size: Final = 8
-key_size: Final = 24
-
-
-def new(
-    key: bytes,
-    mode: Union[int, Literal[Mode.CBC, Mode.ECB]],
-    iv: Optional[bytes] = None,
-) -> Cipher:
-    """Return a `Cipher` object that can perform three-key triple DES
-    encryption and decryption.
-
-    Three-key triple DES cipher (also known as DES3, 3DES,
-    Triple DES, or DES-EDE3).
-
-    Parameters:
-        key: The key to encrypt decrypt.  If None,
-            encryption and decryption are unavailable.
-        mode: The mode of operation of the cipher.
-        iv: The initialization vector (IV).  The IV is
-            required for every mode but ECB and CTR where it is ignored.
-            If not set, the IV is initialized to all 0, which should not
-            be used for encryption.
-
-    """
-    mode_ = Mode(mode)
-    if len(key) != key_size:
-        raise TLSError(
-            msg="key size must be %i bytes, got %i" % (key_size, len(key))
-        )
-    if mode_ not in {Mode.CBC, Mode.ECB}:
-        raise TLSError(msg="unsupported mode %r" % mode_)
-    name = ("DES-EDE3-%s" % mode_.name).encode("ascii")
-    return Cipher(name, key, mode_, iv)
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2016, Elaborated Networks GmbH
+# Copyright (c) 2019, Mathias Laurin
+
+"""Three-key triple DES cipher (also known as DES3, 3DES,
+Triple DES, or DES-EDE3)."""
+
+from __future__ import annotations
+
+from typing import Final, Literal, Optional, Union
+
+from mbedtls.exceptions import TLSError
+
+from ._cipher import Cipher, Mode
+
+__all__ = ["block_size", "key_size", "new"]
+
+
+block_size: Final = 8
+key_size: Final = 24
+
+
+def new(
+    key: bytes,
+    mode: Union[int, Literal[Mode.CBC, Mode.ECB]],
+    iv: Optional[bytes] = None,
+) -> Cipher:
+    """Return a `Cipher` object that can perform three-key triple DES
+    encryption and decryption.
+
+    Three-key triple DES cipher (also known as DES3, 3DES,
+    Triple DES, or DES-EDE3).
+
+    Parameters:
+        key: The key to encrypt decrypt.  If None,
+            encryption and decryption are unavailable.
+        mode: The mode of operation of the cipher.
+        iv: The initialization vector (IV).  The IV is
+            required for every mode but ECB and CTR where it is ignored.
+            If not set, the IV is initialized to all 0, which should not
+            be used for encryption.
+
+    """
+    mode_ = Mode(mode)
+    if len(key) != key_size:
+        raise TLSError(
+            msg="key size must be %i bytes, got %i" % (key_size, len(key))
+        )
+    if mode_ not in {Mode.CBC, Mode.ECB}:
+        raise TLSError(msg="unsupported mode %r" % mode_)
+    name = ("DES-EDE3-%s" % mode_.name).encode("ascii")
+    return Cipher(name, key, mode_, iv)
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/cipher/__init__.py` & `python-mbedtls-2.7.1/src/mbedtls/cipher/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,116 +1,109 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2016, Elaborated Networks GmbH
-# Copyright (c) 2019, Mathias Laurin
-
-"""The cipher package provide symmetric encryption and decryption.
-
-The API follows the recommendations from PEP 272 "API for Block
-Encryption Algorithms"
-
-"""
-
-from __future__ import annotations
-
-import sys
-from typing import Optional
-
-from mbedtls.cipher import (
-    AES,
-    ARC4,
-    ARIA,
-    CHACHA20,
-    DES,
-    DES3,
-    Blowfish,
-    Camellia,
-    DES3dbl,
-)
-from mbedtls.cipher._cipher import AEADCipher as AEADCipher
-from mbedtls.cipher._cipher import Cipher as Cipher
-from mbedtls.cipher._cipher import Mode as Mode
-from mbedtls.cipher._cipher import (
-    get_supported_ciphers as get_supported_ciphers,
-)
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Final, Protocol, runtime_checkable
-else:
-    from typing import Final, Protocol, runtime_checkable
-
-
-# Add module-level aliases to comply with PEP 272.
-MODE_ECB: Final = Mode.ECB.value
-MODE_CBC: Final = Mode.CBC.value
-MODE_CFB: Final = Mode.CFB.value
-MODE_OFB: Final = Mode.OFB.value
-MODE_CTR: Final = Mode.CTR.value
-MODE_GCM: Final = Mode.GCM.value
-MODE_STREAM: Final = Mode.STREAM.value
-MODE_CCM: Final = Mode.CCM.value
-MODE_XTS: Final = Mode.XTS.value
-MODE_CHACHAPOLY: Final = Mode.CHACHAPOLY.value
-
-
-@runtime_checkable
-class CipherType(Protocol):
-    @property
-    def __name__(self) -> str:
-        ...
-
-    @property
-    def block_size(self) -> int:
-        ...
-
-    @property
-    def key_size(self) -> int:
-        ...
-
-    def new(self, key: bytes, mode: Mode, iv: Optional[bytes]) -> Cipher:
-        ...
-
-
-@runtime_checkable
-class AEADCipherType(Protocol):
-    @property
-    def __name__(self) -> str:
-        ...
-
-    @property
-    def block_size(self) -> int:
-        ...
-
-    @property
-    def key_size(self) -> int:
-        ...
-
-    def new(
-        self, key: bytes, mode: Mode, iv: Optional[bytes], ad: Optional[bytes]
-    ) -> AEADCipher:
-        ...
-
-
-__all__ = (
-    "AEADCipherType",
-    "AES",
-    "ARC4",
-    "ARIA",
-    "Blowfish",
-    "Camellia",
-    "DES",
-    "DES3",
-    "DES3dbl",
-    "CHACHA20",
-    "CipherType",
-    "get_supported_ciphers",
-    "Mode",
-    "MODE_ECB",
-    "MODE_CBC",
-    "MODE_CFB",
-    "MODE_OFB",
-    "MODE_CTR",
-    "MODE_GCM",
-    "MODE_STREAM",
-    "MODE_CCM",
-    "MODE_XTS",
-    "MODE_CHACHAPOLY",
-)
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2016, Elaborated Networks GmbH
+# Copyright (c) 2019, Mathias Laurin
+
+"""The cipher package provide symmetric encryption and decryption.
+
+The API follows the recommendations from PEP 272 "API for Block
+Encryption Algorithms"
+
+"""
+
+from __future__ import annotations
+
+from typing import Final, Optional, Protocol, runtime_checkable
+
+from mbedtls.cipher import (
+    AES,
+    ARC4,
+    ARIA,
+    CHACHA20,
+    DES,
+    DES3,
+    Blowfish,
+    Camellia,
+    DES3dbl,
+)
+from mbedtls.cipher._cipher import AEADCipher as AEADCipher
+from mbedtls.cipher._cipher import Cipher as Cipher
+from mbedtls.cipher._cipher import Mode as Mode
+from mbedtls.cipher._cipher import (
+    get_supported_ciphers as get_supported_ciphers,
+)
+
+# Add module-level aliases to comply with PEP 272.
+MODE_ECB: Final = Mode.ECB.value
+MODE_CBC: Final = Mode.CBC.value
+MODE_CFB: Final = Mode.CFB.value
+MODE_OFB: Final = Mode.OFB.value
+MODE_CTR: Final = Mode.CTR.value
+MODE_GCM: Final = Mode.GCM.value
+MODE_STREAM: Final = Mode.STREAM.value
+MODE_CCM: Final = Mode.CCM.value
+MODE_XTS: Final = Mode.XTS.value
+MODE_CHACHAPOLY: Final = Mode.CHACHAPOLY.value
+
+
+@runtime_checkable
+class CipherType(Protocol):
+    @property
+    def __name__(self) -> str:
+        ...
+
+    @property
+    def block_size(self) -> int:
+        ...
+
+    @property
+    def key_size(self) -> int:
+        ...
+
+    def new(self, key: bytes, mode: Mode, iv: Optional[bytes]) -> Cipher:
+        ...
+
+
+@runtime_checkable
+class AEADCipherType(Protocol):
+    @property
+    def __name__(self) -> str:
+        ...
+
+    @property
+    def block_size(self) -> int:
+        ...
+
+    @property
+    def key_size(self) -> int:
+        ...
+
+    def new(
+        self, key: bytes, mode: Mode, iv: Optional[bytes], ad: Optional[bytes]
+    ) -> AEADCipher:
+        ...
+
+
+__all__ = (
+    "AEADCipherType",
+    "AES",
+    "ARC4",
+    "ARIA",
+    "Blowfish",
+    "Camellia",
+    "DES",
+    "DES3",
+    "DES3dbl",
+    "CHACHA20",
+    "CipherType",
+    "get_supported_ciphers",
+    "Mode",
+    "MODE_ECB",
+    "MODE_CBC",
+    "MODE_CFB",
+    "MODE_OFB",
+    "MODE_CTR",
+    "MODE_GCM",
+    "MODE_STREAM",
+    "MODE_CCM",
+    "MODE_XTS",
+    "MODE_CHACHAPOLY",
+)
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/exceptions.pyx` & `python-mbedtls-2.7.1/src/mbedtls/exceptions.pyx`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2018, Mathias Laurin
-
-"""This module defines exceptions and errors."""
-
-
-from libc.stdlib cimport free, malloc
-
-cimport mbedtls.exceptions as _exc
-
-__all__ = ("TLSError",)
-
-
-class TLSError(Exception):
-    """Exception raise by Mbed TLS."""
-
-    def __init__(self, err=None, msg=""):
-        super().__init__()
-        if err is not None:
-            assert err >= 0
-        self.err = err
-        self._msg = msg
-
-    @property
-    def msg(self):
-        if self.err is None:
-            return self._msg
-
-        # Set buflen to 200 as in `strerror.c`.
-        cdef size_t buflen = 200
-        cdef char* buffer = <char*>malloc(buflen * sizeof(char))
-        if not buffer:
-            raise MemoryError()
-        try:
-            _exc.mbedtls_strerror(self.err, &buffer[0], buflen)
-            output = bytes(buffer[:buflen])
-            try:
-                olen = output.index(b"\0")
-            except ValueError:
-                olen = buflen
-            return output[:olen].decode("ascii")
-        finally:
-            free(buffer)
-
-    def __str__(self):
-        if self.err is None:
-            return "%s(%s)" % (type(self).__name__, self.msg)
-        else:
-            return "%s([0x%04X] %r)" % (self.__class__.__name__,
-                                        self.err, self.msg)
-
-
-cpdef check_error(const int err):
-    if err >= 0:
-        return err
-    raise TLSError(-err)
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2018, Mathias Laurin
+
+"""This module defines exceptions and errors."""
+
+
+from libc.stdlib cimport free, malloc
+
+cimport mbedtls.exceptions as _exc
+
+__all__ = ("TLSError",)
+
+
+class TLSError(Exception):
+    """Exception raise by Mbed TLS."""
+
+    def __init__(self, err=None, msg=""):
+        super().__init__()
+        if err is not None:
+            assert err >= 0
+        self.err = err
+        self._msg = msg
+
+    @property
+    def msg(self):
+        if self.err is None:
+            return self._msg
+
+        # Set buflen to 200 as in `strerror.c`.
+        cdef size_t buflen = 200
+        cdef char* buffer = <char*>malloc(buflen * sizeof(char))
+        if not buffer:
+            raise MemoryError()
+        try:
+            _exc.mbedtls_strerror(self.err, &buffer[0], buflen)
+            output = bytes(buffer[:buflen])
+            try:
+                olen = output.index(b"\0")
+            except ValueError:
+                olen = buflen
+            return output[:olen].decode("ascii")
+        finally:
+            free(buffer)
+
+    def __str__(self):
+        if self.err is None:
+            return "%s(%s)" % (type(self).__name__, self.msg)
+        else:
+            return "%s([0x%04X] %r)" % (self.__class__.__name__,
+                                        self.err, self.msg)
+
+
+cpdef check_error(const int err):
+    if err >= 0:
+        return err
+    raise TLSError(-err)
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/hashlib.py` & `python-mbedtls-2.7.1/src/mbedtls/hashlib.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,97 +1,91 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2015, Elaborated Networks GmbH
-# Copyright (c) 2019, Mathias Laurin
-
-"""Generic message digest wrapper (hash algorithm)."""
-
-from __future__ import annotations
-
-import sys
-from typing import Optional
-
-# pylint: disable=no-name-in-module
-from mbedtls._md import Hash as Hash
-from mbedtls._md import algorithms_available as algorithms_available
-from mbedtls._md import algorithms_guaranteed as algorithms_guaranteed
-
-# pylint: enable=no-name-in-module
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Protocol
-else:
-    from typing import Protocol
-
-
-# Work around pyflakes' F401: imported but unused
-assert algorithms_available
-assert algorithms_guaranteed
-
-
-class Algorithm(Protocol):
-    def __call__(self, buffer: Optional[bytes] = ...) -> Hash:
-        ...
-
-
-def new(name: str, buffer: Optional[bytes] = None) -> Hash:
-    """A generic constructor that takes the string name of the desired
-    algorithm as its first parameter.
-
-    """
-    block_size = {
-        "md2": 16,
-        "md4": 64,
-        "md5": 64,
-        "sha1": 64,
-        "sha224": 64,
-        "sha256": 64,
-        "sha384": 128,
-        "sha512": 128,
-        "ripemd160": 64,
-    }.get(name.lower(), 64)
-    return Hash(name, buffer, block_size=block_size)
-
-
-def md2(buffer: Optional[bytes] = None) -> Hash:
-    """MD2 message-digest algorithm."""
-    return new("md2", buffer)  # pragma: no cover
-
-
-def md4(buffer: Optional[bytes] = None) -> Hash:
-    """MD4 message-digest algorithm."""
-    return new("md4", buffer)  # pragma: no cover
-
-
-def md5(buffer: Optional[bytes] = None) -> Hash:
-    """MD5 message-digest algorithm."""
-    return new("md5", buffer)
-
-
-def sha1(buffer: Optional[bytes] = None) -> Hash:
-    """Secure Hash Algorithm 1 (SHA-1)."""
-    return new("sha1", buffer)
-
-
-def sha224(buffer: Optional[bytes] = None) -> Hash:
-    """Secure Hash Algorithm 2 (SHA-2) with 224 bits hash value."""
-    return new("sha224", buffer)
-
-
-def sha256(buffer: Optional[bytes] = None) -> Hash:
-    """Secure Hash Algorithm 2 (SHA-2) with 256 bits hash value."""
-    return new("sha256", buffer)
-
-
-def sha384(buffer: Optional[bytes] = None) -> Hash:
-    """Secure Hash Algorithm 2 (SHA-2) with 384 bits hash value."""
-    return new("sha384", buffer)
-
-
-def sha512(buffer: Optional[bytes] = None) -> Hash:
-    """Secure Hash Algorithm 2 (SHA-2) with 512 bits hash value."""
-    return new("sha512", buffer)
-
-
-def ripemd160(buffer: Optional[bytes] = None) -> Hash:
-    """RACE Integrity Primitives Evaluation Message Digest (RIPEMD) with
-    160 bits hash value."""
-    return new("ripemd160", buffer)
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2015, Elaborated Networks GmbH
+# Copyright (c) 2019, Mathias Laurin
+
+"""Generic message digest wrapper (hash algorithm)."""
+
+from __future__ import annotations
+
+from typing import Optional, Protocol
+
+# pylint: disable=no-name-in-module
+from mbedtls._md import Hash as Hash
+from mbedtls._md import algorithms_available as algorithms_available
+from mbedtls._md import algorithms_guaranteed as algorithms_guaranteed
+
+# pylint: enable=no-name-in-module
+
+
+# Work around pyflakes' F401: imported but unused
+assert algorithms_available
+assert algorithms_guaranteed
+
+
+class Algorithm(Protocol):
+    def __call__(self, buffer: Optional[bytes] = ...) -> Hash:
+        ...
+
+
+def new(name: str, buffer: Optional[bytes] = None) -> Hash:
+    """A generic constructor that takes the string name of the desired
+    algorithm as its first parameter.
+
+    """
+    block_size = {
+        "md2": 16,
+        "md4": 64,
+        "md5": 64,
+        "sha1": 64,
+        "sha224": 64,
+        "sha256": 64,
+        "sha384": 128,
+        "sha512": 128,
+        "ripemd160": 64,
+    }.get(name.lower(), 64)
+    return Hash(name, buffer, block_size=block_size)
+
+
+def md2(buffer: Optional[bytes] = None) -> Hash:
+    """MD2 message-digest algorithm."""
+    return new("md2", buffer)  # pragma: no cover
+
+
+def md4(buffer: Optional[bytes] = None) -> Hash:
+    """MD4 message-digest algorithm."""
+    return new("md4", buffer)  # pragma: no cover
+
+
+def md5(buffer: Optional[bytes] = None) -> Hash:
+    """MD5 message-digest algorithm."""
+    return new("md5", buffer)
+
+
+def sha1(buffer: Optional[bytes] = None) -> Hash:
+    """Secure Hash Algorithm 1 (SHA-1)."""
+    return new("sha1", buffer)
+
+
+def sha224(buffer: Optional[bytes] = None) -> Hash:
+    """Secure Hash Algorithm 2 (SHA-2) with 224 bits hash value."""
+    return new("sha224", buffer)
+
+
+def sha256(buffer: Optional[bytes] = None) -> Hash:
+    """Secure Hash Algorithm 2 (SHA-2) with 256 bits hash value."""
+    return new("sha256", buffer)
+
+
+def sha384(buffer: Optional[bytes] = None) -> Hash:
+    """Secure Hash Algorithm 2 (SHA-2) with 384 bits hash value."""
+    return new("sha384", buffer)
+
+
+def sha512(buffer: Optional[bytes] = None) -> Hash:
+    """Secure Hash Algorithm 2 (SHA-2) with 512 bits hash value."""
+    return new("sha512", buffer)
+
+
+def ripemd160(buffer: Optional[bytes] = None) -> Hash:
+    """RACE Integrity Primitives Evaluation Message Digest (RIPEMD) with
+    160 bits hash value."""
+    return new("ripemd160", buffer)
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/hkdf.pyi` & `python-mbedtls-2.7.1/src/mbedtls/hkdf.pyi`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2022, Mathias Laurin
-
-from __future__ import annotations
-
-from typing import Optional
-
-from .hmac import Algorithm
-
-def hkdf(
-    key: bytes,
-    length: int,
-    info: bytes,
-    salt: Optional[bytes] = None,
-    digestmod: Optional[Algorithm] = None,
-) -> bytes: ...
-def extract(
-    key: bytes,
-    salt: Optional[bytes] = None,
-    digestmod: Optional[Algorithm] = None,
-) -> bytes: ...
-def expand(
-    prk: bytes,
-    length: int,
-    info: bytes,
-    digestmod: Optional[Algorithm] = None,
-) -> bytes: ...
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2022, Mathias Laurin
+
+from __future__ import annotations
+
+from typing import Optional
+
+from .hmac import Algorithm
+
+def hkdf(
+    key: bytes,
+    length: int,
+    info: bytes,
+    salt: Optional[bytes] = None,
+    digestmod: Optional[Algorithm] = None,
+) -> bytes: ...
+def extract(
+    key: bytes,
+    salt: Optional[bytes] = None,
+    digestmod: Optional[Algorithm] = None,
+) -> bytes: ...
+def expand(
+    prk: bytes,
+    length: int,
+    info: bytes,
+    digestmod: Optional[Algorithm] = None,
+) -> bytes: ...
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/hmac.py` & `python-mbedtls-2.7.1/src/mbedtls/hmac.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,101 +1,95 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2015, Elaborated Networks GmbH
-# Copyright (c) 2019, Mathias Laurin
-
-"""Generic message digest wrapper (hash algorithm)."""
-
-from __future__ import annotations
-
-import sys
-from typing import Optional
-
-# pylint: disable=no-name-in-module
-from mbedtls._md import Hmac as Hmac
-from mbedtls._md import algorithms_available as algorithms_available
-from mbedtls._md import algorithms_guaranteed as algorithms_guaranteed
-
-# pylint: enable=no-name-in-module
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Protocol
-else:
-    from typing import Protocol
-
-
-# Work around pyflakes' F401: imported but unused
-assert algorithms_available
-assert algorithms_guaranteed
-
-
-class Algorithm(Protocol):
-    def __call__(self, key: bytes, buffer: Optional[bytes] = ...) -> Hmac:
-        ...
-
-
-def new(
-    key: bytes, buffer: Optional[bytes] = None, digestmod: Optional[str] = None
-) -> Hmac:
-    """A generic constructor that takes the key algorithm as its first
-    parameter.
-
-    """
-    if digestmod is None:
-        digestmod = "md5"
-    block_size = {
-        "md2": 16,
-        "md4": 64,
-        "md5": 64,
-        "sha1": 64,
-        "sha224": 64,
-        "sha256": 64,
-        "sha384": 128,
-        "sha512": 128,
-        "ripemd160": 64,
-    }.get(digestmod.lower(), 64)
-    return Hmac(key, digestmod, buffer, block_size=block_size)
-
-
-def md2(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
-    """MD2 message-digest algorithm."""
-    return new(key, buffer, "md2")  # pragma: no cover
-
-
-def md4(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
-    """MD4 message-digest algorithm."""
-    return new(key, buffer, "md4")  # pragma: no cover
-
-
-def md5(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
-    """MD5 message-digest algorithm."""
-    return new(key, buffer, "md5")
-
-
-def sha1(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
-    """Secure Hmac Algorithm 1 (SHA-1)."""
-    return new(key, buffer, "sha1")
-
-
-def sha224(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
-    """Secure Hmac Algorithm 2 (SHA-2) with 224 bits hash value."""
-    return new(key, buffer, "sha224")
-
-
-def sha256(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
-    """Secure Hmac Algorithm 2 (SHA-2) with 256 bits hash value."""
-    return new(key, buffer, "sha256")
-
-
-def sha384(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
-    """Secure Hmac Algorithm 2 (SHA-2) with 384 bits hash value."""
-    return new(key, buffer, "sha384")
-
-
-def sha512(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
-    """Secure Hmac Algorithm 2 (SHA-2) with 512 bits hash value."""
-    return new(key, buffer, "sha512")
-
-
-def ripemd160(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
-    """RACE Integrity Primitives Evaluation Message Digest (RIPEMD) with
-    160 bits hash value."""
-    return new(key, buffer, "ripemd160")
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2015, Elaborated Networks GmbH
+# Copyright (c) 2019, Mathias Laurin
+
+"""Generic message digest wrapper (hash algorithm)."""
+
+from __future__ import annotations
+
+from typing import Optional, Protocol
+
+# pylint: disable=no-name-in-module
+from mbedtls._md import Hmac as Hmac
+from mbedtls._md import algorithms_available as algorithms_available
+from mbedtls._md import algorithms_guaranteed as algorithms_guaranteed
+
+# pylint: enable=no-name-in-module
+
+
+# Work around pyflakes' F401: imported but unused
+assert algorithms_available
+assert algorithms_guaranteed
+
+
+class Algorithm(Protocol):
+    def __call__(self, key: bytes, buffer: Optional[bytes] = ...) -> Hmac:
+        ...
+
+
+def new(
+    key: bytes, buffer: Optional[bytes] = None, digestmod: Optional[str] = None
+) -> Hmac:
+    """A generic constructor that takes the key algorithm as its first
+    parameter.
+
+    """
+    if digestmod is None:
+        digestmod = "md5"
+    block_size = {
+        "md2": 16,
+        "md4": 64,
+        "md5": 64,
+        "sha1": 64,
+        "sha224": 64,
+        "sha256": 64,
+        "sha384": 128,
+        "sha512": 128,
+        "ripemd160": 64,
+    }.get(digestmod.lower(), 64)
+    return Hmac(key, digestmod, buffer, block_size=block_size)
+
+
+def md2(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
+    """MD2 message-digest algorithm."""
+    return new(key, buffer, "md2")  # pragma: no cover
+
+
+def md4(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
+    """MD4 message-digest algorithm."""
+    return new(key, buffer, "md4")  # pragma: no cover
+
+
+def md5(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
+    """MD5 message-digest algorithm."""
+    return new(key, buffer, "md5")
+
+
+def sha1(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
+    """Secure Hmac Algorithm 1 (SHA-1)."""
+    return new(key, buffer, "sha1")
+
+
+def sha224(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
+    """Secure Hmac Algorithm 2 (SHA-2) with 224 bits hash value."""
+    return new(key, buffer, "sha224")
+
+
+def sha256(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
+    """Secure Hmac Algorithm 2 (SHA-2) with 256 bits hash value."""
+    return new(key, buffer, "sha256")
+
+
+def sha384(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
+    """Secure Hmac Algorithm 2 (SHA-2) with 384 bits hash value."""
+    return new(key, buffer, "sha384")
+
+
+def sha512(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
+    """Secure Hmac Algorithm 2 (SHA-2) with 512 bits hash value."""
+    return new(key, buffer, "sha512")
+
+
+def ripemd160(key: bytes, buffer: Optional[bytes] = None) -> Hmac:
+    """RACE Integrity Primitives Evaluation Message Digest (RIPEMD) with
+    160 bits hash value."""
+    return new(key, buffer, "ripemd160")
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/mpi.pyi` & `python-mbedtls-2.7.1/src/mbedtls/mpi.pyi`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2022, Mathias Laurin
-
-from __future__ import annotations
-
-import numbers
-import sys
-from typing import Any, NoReturn, Optional, Tuple, Union, overload
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Literal
-else:
-    from typing import Literal
-
-_Integral = Union[numbers.Integral, int]
-
-class MPI(numbers.Integral):
-    def __init__(self, __value: _Integral = 0) -> None: ...
-    def __reduce__(self) -> Tuple[Any, ...]: ...
-    def __str__(self) -> str: ...
-    def __repr__(self) -> str: ...
-    def bit_length(self) -> int: ...
-    @classmethod
-    def from_int(cls, __value: int) -> MPI: ...
-    @classmethod
-    def from_bytes(
-        cls, __data: bytes, byteorder: Literal["big", "little"] = "big"
-    ) -> MPI: ...
-    def to_bytes(
-        self, length: int, byteorder: Literal["big", "little"]
-    ) -> bytes: ...
-    @classmethod
-    def prime(cls, size: int) -> MPI: ...
-    def __hash__(self) -> int: ...
-    def __bool__(self) -> bool: ...
-    def __add__(self, __other: object) -> MPI: ...
-    def __radd__(self, __other: object) -> MPI: ...
-    def __neg__(self) -> NoReturn: ...
-    def __pos__(self) -> MPI: ...
-    def __sub__(self, __other: object) -> MPI: ...
-    def __mul__(self, __other: object) -> MPI: ...
-    def __rmul__(self, __other: object) -> MPI: ...
-    def __truediv__(self, __other: object) -> MPI: ...
-    def __rtruediv__(self, __other: object) -> MPI: ...
-    def __pow__(
-        self, __exponent: _Integral, __modulus: Optional[_Integral] = ...
-    ) -> MPI: ...
-    def __rpow__(self, __other: Any) -> Any: ...
-    def __abs__(self) -> MPI: ...
-    def __eq__(self, __other: object) -> bool: ...
-    def __float__(self) -> float: ...
-    # mypy wants int but that should be Integral according to
-    # the documentation to trunc, floor, and ceil.
-    def __trunc__(self) -> int: ...
-    def __floor__(self) -> int: ...
-    def __ceil__(self) -> int: ...
-    @overload
-    def __round__(self, ndigits: None = ...) -> int: ...
-    @overload
-    def __round__(self, ndigits: int) -> _Integral: ...
-    def __divmod__(self, __other: _Integral) -> Tuple[MPI, MPI]: ...
-    def __floordiv__(self, __other: object) -> int: ...
-    def __rfloordiv__(self, __other: object) -> int: ...
-    def __mod__(self, __other: _Integral) -> MPI: ...
-    def __rmod__(self, __other: _Integral) -> MPI: ...
-    def __lt__(self, __other: _Integral) -> bool: ...
-    def __le__(self, __other: _Integral) -> bool: ...
-    def __gt__(self, __other: _Integral) -> bool: ...
-    def __ge__(self, __other: _Integral) -> bool: ...
-    def __complex__(self) -> complex: ...
-    def __real__(self) -> MPI: ...
-    def imag(self) -> Literal[0]: ...
-    def conjugate(self) -> MPI: ...
-    def __int__(self) -> int: ...
-    def __index__(self) -> int: ...
-    def __lshift__(self, __other: _Integral) -> MPI: ...
-    def __rlshift__(self, __other: _Integral) -> MPI: ...
-    def __rshift__(self, __other: _Integral) -> MPI: ...
-    def __rrshift__(self, __other: _Integral) -> MPI: ...
-    def __and__(self, __other: _Integral) -> MPI: ...
-    def __rand__(self, __other: _Integral) -> MPI: ...
-    def __xor__(self, __other: _Integral) -> MPI: ...
-    def __rxor__(self, __other: _Integral) -> MPI: ...
-    def __or__(self, __other: _Integral) -> MPI: ...
-    def __ror__(self, __other: _Integral) -> MPI: ...
-    def __invert__(self) -> NoReturn: ...
-    @property
-    def numerator(self) -> int: ...
-    @property
-    def denominator(self) -> Literal[1]: ...
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2022, Mathias Laurin
+
+from __future__ import annotations
+
+import numbers
+import sys
+from typing import Any, NoReturn, Optional, Tuple, Union, overload
+
+if sys.version_info < (3, 8):
+    from typing_extensions import Literal
+else:
+    from typing import Literal
+
+_Integral = Union[numbers.Integral, int]
+
+class MPI(numbers.Integral):
+    def __init__(self, __value: _Integral = 0) -> None: ...
+    def __reduce__(self) -> Tuple[Any, ...]: ...
+    def __str__(self) -> str: ...
+    def __repr__(self) -> str: ...
+    def bit_length(self) -> int: ...
+    @classmethod
+    def from_int(cls, __value: int) -> MPI: ...
+    @classmethod
+    def from_bytes(
+        cls, __data: bytes, byteorder: Literal["big", "little"] = "big"
+    ) -> MPI: ...
+    def to_bytes(
+        self, length: int, byteorder: Literal["big", "little"]
+    ) -> bytes: ...
+    @classmethod
+    def prime(cls, size: int) -> MPI: ...
+    def __hash__(self) -> int: ...
+    def __bool__(self) -> bool: ...
+    def __add__(self, __other: object) -> MPI: ...
+    def __radd__(self, __other: object) -> MPI: ...
+    def __neg__(self) -> NoReturn: ...
+    def __pos__(self) -> MPI: ...
+    def __sub__(self, __other: object) -> MPI: ...
+    def __mul__(self, __other: object) -> MPI: ...
+    def __rmul__(self, __other: object) -> MPI: ...
+    def __truediv__(self, __other: object) -> MPI: ...
+    def __rtruediv__(self, __other: object) -> MPI: ...
+    def __pow__(
+        self, __exponent: _Integral, __modulus: Optional[_Integral] = ...
+    ) -> MPI: ...
+    def __rpow__(self, __other: Any) -> Any: ...
+    def __abs__(self) -> MPI: ...
+    def __eq__(self, __other: object) -> bool: ...
+    def __float__(self) -> float: ...
+    # mypy wants int but that should be Integral according to
+    # the documentation to trunc, floor, and ceil.
+    def __trunc__(self) -> int: ...
+    def __floor__(self) -> int: ...
+    def __ceil__(self) -> int: ...
+    @overload
+    def __round__(self, ndigits: None = ...) -> int: ...
+    @overload
+    def __round__(self, ndigits: int) -> _Integral: ...
+    def __divmod__(self, __other: _Integral) -> Tuple[MPI, MPI]: ...
+    def __floordiv__(self, __other: object) -> int: ...
+    def __rfloordiv__(self, __other: object) -> int: ...
+    def __mod__(self, __other: _Integral) -> MPI: ...
+    def __rmod__(self, __other: _Integral) -> MPI: ...
+    def __lt__(self, __other: _Integral) -> bool: ...
+    def __le__(self, __other: _Integral) -> bool: ...
+    def __gt__(self, __other: _Integral) -> bool: ...
+    def __ge__(self, __other: _Integral) -> bool: ...
+    def __complex__(self) -> complex: ...
+    def __real__(self) -> MPI: ...
+    def imag(self) -> Literal[0]: ...
+    def conjugate(self) -> MPI: ...
+    def __int__(self) -> int: ...
+    def __index__(self) -> int: ...
+    def __lshift__(self, __other: _Integral) -> MPI: ...
+    def __rlshift__(self, __other: _Integral) -> MPI: ...
+    def __rshift__(self, __other: _Integral) -> MPI: ...
+    def __rrshift__(self, __other: _Integral) -> MPI: ...
+    def __and__(self, __other: _Integral) -> MPI: ...
+    def __rand__(self, __other: _Integral) -> MPI: ...
+    def __xor__(self, __other: _Integral) -> MPI: ...
+    def __rxor__(self, __other: _Integral) -> MPI: ...
+    def __or__(self, __other: _Integral) -> MPI: ...
+    def __ror__(self, __other: _Integral) -> MPI: ...
+    def __invert__(self) -> NoReturn: ...
+    @property
+    def numerator(self) -> int: ...
+    @property
+    def denominator(self) -> Literal[1]: ...
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/mpi.pyx` & `python-mbedtls-2.7.1/src/mbedtls/mpi.pyx`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,372 +1,372 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2018, Mathias Laurin
-
-# cython: c_api_binop_methods=True
-
-"""Multi-precision integer library (MPI)."""
-
-
-from libc.stdlib cimport free, malloc
-
-cimport mbedtls._random as _rnd
-cimport mbedtls.mpi as _mpi
-
-import math
-import numbers
-from binascii import hexlify, unhexlify
-
-import mbedtls._platform as _plt
-import mbedtls._random as _rnd
-import mbedtls.exceptions as _exc
-
-
-cdef _rnd.Random __rng = _rnd.default_rng()
-
-
-cdef to_bytes(value):
-    xx = "{:02x}".format(value)
-    return unhexlify((xx if not len(xx) % 2 else "0" + xx).encode("ascii"))
-
-
-cdef from_bytes(value):
-    return int(hexlify(value), 16)
-
-
-cdef from_mpi_p(_mpi.mbedtls_mpi *mpi_p):
-    cdef _mpi.MPI new_mpi = _mpi.MPI()
-    _mpi.mbedtls_mpi_copy(&new_mpi._ctx, mpi_p)
-    return new_mpi
-
-
-cdef class MPI:
-    """Multi-precision integer.
-
-    This class implements `numbers.Integral`.  The representation
-    of the MPI is overwritten with random bytes when the MPI is
-    garbage collected.
-
-    """
-    def __init__(self, value=0):
-        if isinstance(value, MPI):
-            value_ = <MPI> value
-            _exc.check_error(mbedtls_mpi_copy(&self._ctx, &value_._ctx))
-        else:
-            value = to_bytes(int(value))
-            self._read_bytes(value)
-
-    def __cinit__(self):
-        """Initialize one MPI."""
-        _mpi.mbedtls_mpi_init(&self._ctx)
-
-    def __dealloc__(self):
-        """Unallocate one MPI."""
-        _exc.check_error(mbedtls_mpi_fill_random(
-            &self._ctx, self._len(),
-            &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
-        _mpi.mbedtls_mpi_free(&self._ctx)
-
-    def __reduce__(self):
-        byteorder = "big"
-        return type(self).from_bytes, (
-            self.to_bytes(self._len(), byteorder),
-            byteorder,
-        )
-
-    cdef size_t _len(self):
-        """Return the total size in bytes."""
-        return _mpi.mbedtls_mpi_size(&self._ctx)
-
-    def _read_bytes(self, const unsigned char[:] data not None):
-        if data.size == 0:
-            return MPI(0)
-        _exc.check_error(
-            _mpi.mbedtls_mpi_read_binary(&self._ctx, &data[0], data.shape[0]))
-
-    def __str__(self):
-        return "%i" % int(self)
-
-    def __repr__(self):
-        return "%s(%i)" % (type(self).__name__, self)
-
-    def bit_length(self):
-        """Return the number of bits necessary to represent MPI in binary."""
-        return _mpi.mbedtls_mpi_bitlen(&self._ctx)
-
-    @classmethod
-    def from_int(cls, value):
-        # mbedtls_mpi_lset is 'limited' to 64 bits.
-        return cls.from_bytes(to_bytes(value), byteorder="big")
-
-    @classmethod
-    def from_bytes(cls, const unsigned char[:] data, byteorder):
-        assert byteorder in {"big", "little"}
-        self = cls()
-        self._read_bytes(data[::-1 if byteorder == "little" else 1])
-        return self
-
-    def to_bytes(self, const size_t length, byteorder):
-        assert byteorder in {"big", "little"}
-        cdef unsigned char* output = <unsigned char*>malloc(
-            length * sizeof(unsigned char))
-        if not output:
-            raise MemoryError()
-        try:
-            _exc.check_error(_mpi.mbedtls_mpi_write_binary(
-                &self._ctx, output, length))
-            return output[:length][::-1 if byteorder == "little" else 1]
-        except Exception as exc:
-            raise OverflowError from exc
-        finally:
-            free(output)
-
-    __bytes__ = to_bytes
-
-    @classmethod
-    def prime(cls, size):
-        """Return an MPI that is probably prime."""
-        cdef MPI self_ = cls()
-        _exc.check_error(mbedtls_mpi_gen_prime(
-            &self_._ctx, size, 0,
-            &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
-        return self_
-
-    def __hash__(self):
-        return int(self)
-
-    def __bool__(self):
-        return self != 0
-
-    def __add__(self, other):
-        if not all((isinstance(self, numbers.Integral),
-                    isinstance(other, numbers.Integral))):
-            return NotImplemented
-        cdef MPI self_ = MPI(self)
-        cdef MPI other_ = MPI(other)
-        cdef MPI result = MPI()
-        _exc.check_error(mbedtls_mpi_add_mpi(
-            &result._ctx, &self_._ctx, &other_._ctx))
-        return result
-
-    def __neg__(self):
-        raise TypeError("negative value")
-
-    def __pos__(self):
-        return self
-
-    def __sub__(self, other):
-        if not all((isinstance(self, numbers.Integral),
-                    isinstance(other, numbers.Integral))):
-            return NotImplemented
-        cdef MPI self_ = MPI(self)
-        cdef MPI other_ = MPI(other)
-        cdef MPI result = MPI()
-        _exc.check_error(mbedtls_mpi_sub_mpi(
-            &result._ctx, &self_._ctx, &other_._ctx))
-        return result
-
-    def __mul__(self, other):
-        if not all((isinstance(self, numbers.Integral),
-                    isinstance(other, numbers.Integral))):
-            return NotImplemented
-        cdef MPI self_ = MPI(self)
-        cdef MPI other_ = MPI(other)
-        cdef MPI result = MPI()
-        _exc.check_error(mbedtls_mpi_mul_mpi(
-            &result._ctx, &self_._ctx, &other_._ctx))
-        return result
-
-    def __truediv__(self, other):
-        return NotImplemented
-
-    def __pow__(MPI self, exponent, modulus):
-        if modulus is None:
-            modulus = 0
-        if not isinstance(exponent, numbers.Integral):
-            return TypeError("exponent should be an integer")
-        if not isinstance(modulus, numbers.Integral):
-            return TypeError("modulus should be an integer")
-        if exponent < 0:
-            raise ValueError("exponent must be greater than zero")
-        cdef MPI result = MPI()
-        cdef MPI exponent_ = MPI(exponent)
-        cdef MPI modulus_ = MPI(modulus)
-        _exc.check_error(
-            mbedtls_mpi_exp_mod(
-                &result._ctx, &self._ctx, &exponent_._ctx, &modulus_._ctx, NULL
-            )
-        )
-        return result
-
-    def __abs__(self):
-        # Negative values are not supported.
-        return self
-
-    def __eq__(MPI self, other):
-        if not isinstance(other, numbers.Integral):
-            return NotImplemented
-        if not isinstance(other, MPI):
-            other = MPI(other)
-        cdef MPI other_ = other
-        return mbedtls_mpi_cmp_mpi(&self._ctx, &other_._ctx) == 0
-
-    def __float__(self):
-        return float(int(self))
-
-    def __trunc__(self):
-        return self
-
-    def __floor__(self):
-        return self
-
-    def __ceil__(self):
-        return self
-
-    def __round__(self, ndigits=None):
-        if ndigits is None:
-            return self
-        if not isinstance(ndigits, numbers.Integral):
-            raise TypeError(ndigits)
-        if ndigits <= 0:
-            return self
-        return round(int(self), ndigits)
-
-    def __divmod__(self, other):
-        if not all((isinstance(self, numbers.Integral),
-                    isinstance(other, numbers.Integral))):
-            return NotImplemented
-        cdef MPI self_ = MPI(self)
-        cdef MPI other_ = MPI(other)
-        cdef MPI quotient = MPI()
-        cdef MPI rest = MPI()
-        _exc.check_error(mbedtls_mpi_div_mpi(
-            &quotient._ctx, &rest._ctx, &self_._ctx, &other_._ctx))
-        return quotient, rest
-
-    def __floordiv__(self, other):
-        return divmod(self, other)[0]
-
-    def __mod__(self, other):
-        if not all((isinstance(self, numbers.Integral),
-                    isinstance(other, numbers.Integral))):
-            return NotImplemented
-        cdef MPI self_ = MPI(self)
-        cdef MPI other_ = MPI(other)
-        cdef MPI result = MPI()
-        _exc.check_error(mbedtls_mpi_mod_mpi(
-            &result._ctx, &self_._ctx, &other_._ctx))
-        return result
-
-    def __lt__(MPI self, other):
-        if not isinstance(other, numbers.Integral):
-            return NotImplemented
-        if not isinstance(other, MPI):
-            other = MPI(other)
-        cdef MPI other_ = other
-        return mbedtls_mpi_cmp_mpi(&self._ctx, &other_._ctx) == -1
-
-    def __le__(MPI self, other):
-        return self < other or self == other
-
-    def __gt__(MPI self, other):
-        return not self <= other
-
-    def __ge__(MPI self, other):
-        return self > other or self == other
-
-    def __complex__(self):
-        return complex(float(self))
-
-    def real(self):
-        return self
-
-    def imag(self):
-        return 0
-
-    def conjugate(self):
-        return self
-
-    def __int__(self):
-        n = self._len()
-        if n:
-            return from_bytes(self.to_bytes(n, byteorder="big"))
-        else:
-            return 0
-
-    def __index__(self):
-        return int(self)
-
-    def __lshift__(MPI self, other):
-        _exc.check_error(mbedtls_mpi_shift_l(&self._ctx, int(other)))
-        return self
-
-    def __rshift__(MPI self, other):
-        _exc.check_error(mbedtls_mpi_shift_r(&self._ctx, int(other)))
-        return self
-
-    def __and__(MPI self, other):
-        if not isinstance(other, MPI):
-            other = MPI(other)
-        cdef size_t size = int(
-            math.ceil(max(self.bit_length(), other.bit_length()) / 8)
-        )
-        self_bin = bytearray(self.to_bytes(size, "big"))
-        other_bin = bytearray(other.to_bytes(size, "big"))
-        output = bytearray(size)
-        cdef size_t ii
-        for ii in range(size):
-            output[ii] = self_bin[ii] & other_bin[ii]
-        result = MPI.from_bytes(output, "big")
-        _plt.zeroize(self_bin)
-        _plt.zeroize(other_bin)
-        _plt.zeroize(output)
-        return result
-
-    def __xor__(MPI self, other):
-        if not isinstance(other, MPI):
-            other = MPI(other)
-        cdef size_t size = int(
-            math.ceil(max(self.bit_length(), other.bit_length()) / 8)
-        )
-        self_bin = bytearray(self.to_bytes(size, "big"))
-        other_bin = bytearray(other.to_bytes(size, "big"))
-        output = bytearray(size)
-        cdef size_t ii
-        for ii in range(size):
-            output[ii] = self_bin[ii] ^ other_bin[ii]
-        result = MPI.from_bytes(output, "big")
-        _plt.zeroize(self_bin)
-        _plt.zeroize(other_bin)
-        _plt.zeroize(output)
-        return result
-
-    def __or__(MPI self, other):
-        if not isinstance(other, MPI):
-            other = MPI(other)
-        cdef size_t size = int(
-            math.ceil(max(self.bit_length(), other.bit_length()) / 8)
-        )
-        self_bin = bytearray(self.to_bytes(size, "big"))
-        other_bin = bytearray(other.to_bytes(size, "big"))
-        output = bytearray(size)
-        cdef size_t ii
-        for ii in range(size):
-            output[ii] = self_bin[ii] | other_bin[ii]
-        result = MPI.from_bytes(output, "big")
-        _plt.zeroize(self_bin)
-        _plt.zeroize(other_bin)
-        _plt.zeroize(output)
-        return result
-
-    def __invert__(self):
-        raise TypeError("negative value")
-
-    @property
-    def numerator(self):
-        return self
-
-    @property
-    def denominator(self):
-        return 1
-
-
-numbers.Integral.register(MPI)
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2018, Mathias Laurin
+
+# cython: c_api_binop_methods=True
+
+"""Multi-precision integer library (MPI)."""
+
+
+from libc.stdlib cimport free, malloc
+
+cimport mbedtls._random as _rnd
+cimport mbedtls.mpi as _mpi
+
+import math
+import numbers
+from binascii import hexlify, unhexlify
+
+import mbedtls._platform as _plt
+import mbedtls._random as _rnd
+import mbedtls.exceptions as _exc
+
+
+cdef _rnd.Random __rng = _rnd.default_rng()
+
+
+cdef to_bytes(value):
+    xx = "{:02x}".format(value)
+    return unhexlify((xx if not len(xx) % 2 else "0" + xx).encode("ascii"))
+
+
+cdef from_bytes(value):
+    return int(hexlify(value), 16)
+
+
+cdef from_mpi_p(_mpi.mbedtls_mpi *mpi_p):
+    cdef _mpi.MPI new_mpi = _mpi.MPI()
+    _mpi.mbedtls_mpi_copy(&new_mpi._ctx, mpi_p)
+    return new_mpi
+
+
+cdef class MPI:
+    """Multi-precision integer.
+
+    This class implements `numbers.Integral`.  The representation
+    of the MPI is overwritten with random bytes when the MPI is
+    garbage collected.
+
+    """
+    def __init__(self, value=0):
+        if isinstance(value, MPI):
+            value_ = <MPI> value
+            _exc.check_error(mbedtls_mpi_copy(&self._ctx, &value_._ctx))
+        else:
+            value = to_bytes(int(value))
+            self._read_bytes(value)
+
+    def __cinit__(self):
+        """Initialize one MPI."""
+        _mpi.mbedtls_mpi_init(&self._ctx)
+
+    def __dealloc__(self):
+        """Unallocate one MPI."""
+        _exc.check_error(mbedtls_mpi_fill_random(
+            &self._ctx, self._len(),
+            &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
+        _mpi.mbedtls_mpi_free(&self._ctx)
+
+    def __reduce__(self):
+        byteorder = "big"
+        return type(self).from_bytes, (
+            self.to_bytes(self._len(), byteorder),
+            byteorder,
+        )
+
+    cdef size_t _len(self):
+        """Return the total size in bytes."""
+        return _mpi.mbedtls_mpi_size(&self._ctx)
+
+    def _read_bytes(self, const unsigned char[:] data not None):
+        if data.size == 0:
+            return MPI(0)
+        _exc.check_error(
+            _mpi.mbedtls_mpi_read_binary(&self._ctx, &data[0], data.shape[0]))
+
+    def __str__(self):
+        return "%i" % int(self)
+
+    def __repr__(self):
+        return "%s(%i)" % (type(self).__name__, self)
+
+    def bit_length(self):
+        """Return the number of bits necessary to represent MPI in binary."""
+        return _mpi.mbedtls_mpi_bitlen(&self._ctx)
+
+    @classmethod
+    def from_int(cls, value):
+        # mbedtls_mpi_lset is 'limited' to 64 bits.
+        return cls.from_bytes(to_bytes(value), byteorder="big")
+
+    @classmethod
+    def from_bytes(cls, const unsigned char[:] data, byteorder):
+        assert byteorder in {"big", "little"}
+        self = cls()
+        self._read_bytes(data[::-1 if byteorder == "little" else 1])
+        return self
+
+    def to_bytes(self, const size_t length, byteorder):
+        assert byteorder in {"big", "little"}
+        cdef unsigned char* output = <unsigned char*>malloc(
+            length * sizeof(unsigned char))
+        if not output:
+            raise MemoryError()
+        try:
+            _exc.check_error(_mpi.mbedtls_mpi_write_binary(
+                &self._ctx, output, length))
+            return output[:length][::-1 if byteorder == "little" else 1]
+        except Exception as exc:
+            raise OverflowError from exc
+        finally:
+            free(output)
+
+    __bytes__ = to_bytes
+
+    @classmethod
+    def prime(cls, size):
+        """Return an MPI that is probably prime."""
+        cdef MPI self_ = cls()
+        _exc.check_error(mbedtls_mpi_gen_prime(
+            &self_._ctx, size, 0,
+            &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
+        return self_
+
+    def __hash__(self):
+        return int(self)
+
+    def __bool__(self):
+        return self != 0
+
+    def __add__(self, other):
+        if not all((isinstance(self, numbers.Integral),
+                    isinstance(other, numbers.Integral))):
+            return NotImplemented
+        cdef MPI self_ = MPI(self)
+        cdef MPI other_ = MPI(other)
+        cdef MPI result = MPI()
+        _exc.check_error(mbedtls_mpi_add_mpi(
+            &result._ctx, &self_._ctx, &other_._ctx))
+        return result
+
+    def __neg__(self):
+        raise TypeError("negative value")
+
+    def __pos__(self):
+        return self
+
+    def __sub__(self, other):
+        if not all((isinstance(self, numbers.Integral),
+                    isinstance(other, numbers.Integral))):
+            return NotImplemented
+        cdef MPI self_ = MPI(self)
+        cdef MPI other_ = MPI(other)
+        cdef MPI result = MPI()
+        _exc.check_error(mbedtls_mpi_sub_mpi(
+            &result._ctx, &self_._ctx, &other_._ctx))
+        return result
+
+    def __mul__(self, other):
+        if not all((isinstance(self, numbers.Integral),
+                    isinstance(other, numbers.Integral))):
+            return NotImplemented
+        cdef MPI self_ = MPI(self)
+        cdef MPI other_ = MPI(other)
+        cdef MPI result = MPI()
+        _exc.check_error(mbedtls_mpi_mul_mpi(
+            &result._ctx, &self_._ctx, &other_._ctx))
+        return result
+
+    def __truediv__(self, other):
+        return NotImplemented
+
+    def __pow__(MPI self, exponent, modulus):
+        if modulus is None:
+            modulus = 0
+        if not isinstance(exponent, numbers.Integral):
+            return TypeError("exponent should be an integer")
+        if not isinstance(modulus, numbers.Integral):
+            return TypeError("modulus should be an integer")
+        if exponent < 0:
+            raise ValueError("exponent must be greater than zero")
+        cdef MPI result = MPI()
+        cdef MPI exponent_ = MPI(exponent)
+        cdef MPI modulus_ = MPI(modulus)
+        _exc.check_error(
+            mbedtls_mpi_exp_mod(
+                &result._ctx, &self._ctx, &exponent_._ctx, &modulus_._ctx, NULL
+            )
+        )
+        return result
+
+    def __abs__(self):
+        # Negative values are not supported.
+        return self
+
+    def __eq__(MPI self, other):
+        if not isinstance(other, numbers.Integral):
+            return NotImplemented
+        if not isinstance(other, MPI):
+            other = MPI(other)
+        cdef MPI other_ = other
+        return mbedtls_mpi_cmp_mpi(&self._ctx, &other_._ctx) == 0
+
+    def __float__(self):
+        return float(int(self))
+
+    def __trunc__(self):
+        return self
+
+    def __floor__(self):
+        return self
+
+    def __ceil__(self):
+        return self
+
+    def __round__(self, ndigits=None):
+        if ndigits is None:
+            return self
+        if not isinstance(ndigits, numbers.Integral):
+            raise TypeError(ndigits)
+        if ndigits <= 0:
+            return self
+        return round(int(self), ndigits)
+
+    def __divmod__(self, other):
+        if not all((isinstance(self, numbers.Integral),
+                    isinstance(other, numbers.Integral))):
+            return NotImplemented
+        cdef MPI self_ = MPI(self)
+        cdef MPI other_ = MPI(other)
+        cdef MPI quotient = MPI()
+        cdef MPI rest = MPI()
+        _exc.check_error(mbedtls_mpi_div_mpi(
+            &quotient._ctx, &rest._ctx, &self_._ctx, &other_._ctx))
+        return quotient, rest
+
+    def __floordiv__(self, other):
+        return divmod(self, other)[0]
+
+    def __mod__(self, other):
+        if not all((isinstance(self, numbers.Integral),
+                    isinstance(other, numbers.Integral))):
+            return NotImplemented
+        cdef MPI self_ = MPI(self)
+        cdef MPI other_ = MPI(other)
+        cdef MPI result = MPI()
+        _exc.check_error(mbedtls_mpi_mod_mpi(
+            &result._ctx, &self_._ctx, &other_._ctx))
+        return result
+
+    def __lt__(MPI self, other):
+        if not isinstance(other, numbers.Integral):
+            return NotImplemented
+        if not isinstance(other, MPI):
+            other = MPI(other)
+        cdef MPI other_ = other
+        return mbedtls_mpi_cmp_mpi(&self._ctx, &other_._ctx) == -1
+
+    def __le__(MPI self, other):
+        return self < other or self == other
+
+    def __gt__(MPI self, other):
+        return not self <= other
+
+    def __ge__(MPI self, other):
+        return self > other or self == other
+
+    def __complex__(self):
+        return complex(float(self))
+
+    def real(self):
+        return self
+
+    def imag(self):
+        return 0
+
+    def conjugate(self):
+        return self
+
+    def __int__(self):
+        n = self._len()
+        if n:
+            return from_bytes(self.to_bytes(n, byteorder="big"))
+        else:
+            return 0
+
+    def __index__(self):
+        return int(self)
+
+    def __lshift__(MPI self, other):
+        _exc.check_error(mbedtls_mpi_shift_l(&self._ctx, int(other)))
+        return self
+
+    def __rshift__(MPI self, other):
+        _exc.check_error(mbedtls_mpi_shift_r(&self._ctx, int(other)))
+        return self
+
+    def __and__(MPI self, other):
+        if not isinstance(other, MPI):
+            other = MPI(other)
+        cdef size_t size = int(
+            math.ceil(max(self.bit_length(), other.bit_length()) / 8)
+        )
+        self_bin = bytearray(self.to_bytes(size, "big"))
+        other_bin = bytearray(other.to_bytes(size, "big"))
+        output = bytearray(size)
+        cdef size_t ii
+        for ii in range(size):
+            output[ii] = self_bin[ii] & other_bin[ii]
+        result = MPI.from_bytes(output, "big")
+        _plt.zeroize(self_bin)
+        _plt.zeroize(other_bin)
+        _plt.zeroize(output)
+        return result
+
+    def __xor__(MPI self, other):
+        if not isinstance(other, MPI):
+            other = MPI(other)
+        cdef size_t size = int(
+            math.ceil(max(self.bit_length(), other.bit_length()) / 8)
+        )
+        self_bin = bytearray(self.to_bytes(size, "big"))
+        other_bin = bytearray(other.to_bytes(size, "big"))
+        output = bytearray(size)
+        cdef size_t ii
+        for ii in range(size):
+            output[ii] = self_bin[ii] ^ other_bin[ii]
+        result = MPI.from_bytes(output, "big")
+        _plt.zeroize(self_bin)
+        _plt.zeroize(other_bin)
+        _plt.zeroize(output)
+        return result
+
+    def __or__(MPI self, other):
+        if not isinstance(other, MPI):
+            other = MPI(other)
+        cdef size_t size = int(
+            math.ceil(max(self.bit_length(), other.bit_length()) / 8)
+        )
+        self_bin = bytearray(self.to_bytes(size, "big"))
+        other_bin = bytearray(other.to_bytes(size, "big"))
+        output = bytearray(size)
+        cdef size_t ii
+        for ii in range(size):
+            output[ii] = self_bin[ii] | other_bin[ii]
+        result = MPI.from_bytes(output, "big")
+        _plt.zeroize(self_bin)
+        _plt.zeroize(other_bin)
+        _plt.zeroize(output)
+        return result
+
+    def __invert__(self):
+        raise TypeError("negative value")
+
+    @property
+    def numerator(self):
+        return self
+
+    @property
+    def denominator(self):
+        return 1
+
+
+numbers.Integral.register(MPI)
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/pk.pxd` & `python-mbedtls-2.7.1/src/mbedtls/pk.pxd`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2016, Elaborated Networks GmbH
-# Copyright (c) 2018, Mathias Laurin
-
-cimport mbedtls._dhm as _dhm
-cimport mbedtls._ecdh as _ecdh
-cimport mbedtls._ecp as _ecp
-cimport mbedtls._md as _md
-cimport mbedtls._rsa as _rsa
-cimport mbedtls.mpi as _mpi
-
-
-cdef extern from "mbedtls/pk.h" nogil:
-    ctypedef enum mbedtls_pk_type_t:
-        MBEDTLS_PK_NONE=0
-        MBEDTLS_PK_RSA
-        MBEDTLS_PK_ECKEY
-        MBEDTLS_PK_ECKEY_DH
-        MBEDTLS_PK_ECDSA
-        MBEDTLS_PK_RSA_ALT
-        MBEDTLS_PK_RSASSA_PSS
-
-    ctypedef struct mbedtls_pk_rsassa_pss_options:
-        pass
-
-    ctypedef struct mbedtls_pk_info_t:
-        pass
-
-    ctypedef struct mbedtls_pk_context:
-        pass
-
-    _rsa.mbedtls_rsa_context *mbedtls_pk_rsa(const mbedtls_pk_context pk)
-    _ecp.mbedtls_ecp_keypair *mbedtls_pk_ec(const mbedtls_pk_context pk)
-    # RSA-alt function pointer types
-    const mbedtls_pk_info_t *mbedtls_pk_info_from_type(
-        mbedtls_pk_type_t pk_type)
-    void mbedtls_pk_init(mbedtls_pk_context *ctx)
-    void mbedtls_pk_free(mbedtls_pk_context *ctx)
-    int mbedtls_pk_setup(mbedtls_pk_context *ctx,
-                         const mbedtls_pk_info_t *info)
-
-    size_t mbedtls_pk_get_bitlen(const mbedtls_pk_context *ctx)
-    size_t mbedtls_pk_get_len(const mbedtls_pk_context *ctx)
-    int mbedtls_pk_can_do(const mbedtls_pk_context *ctx,
-                          mbedtls_pk_type_t type)
-
-    int mbedtls_pk_verify(
-        mbedtls_pk_context *ctx, _md.mbedtls_md_type_t md_alg,
-        const unsigned char *hash, size_t hash_len,
-        const unsigned char *sig, size_t sig_len)
-    # int mbedtls_pk_verify_ext(
-    #     mbedtls_pk_type_t type, const void *options,
-    #     mbedtls_pk_context *ctx, _md.mbedtls_md_type_t md_alg,
-    #     const unsigned char *hash, size_t hash_len,
-    #     const unsigned char *sig, size_t sig_len)
-
-    int mbedtls_pk_sign(
-        mbedtls_pk_context *ctx, _md.mbedtls_md_type_t md_alg,
-        const unsigned char *hash, size_t hash_len,
-        unsigned char *sig, size_t *sig_len,
-        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng)
-
-    int mbedtls_pk_decrypt(
-        mbedtls_pk_context *ctx,
-        const unsigned char *input, size_t ilen,
-        unsigned char *output, size_t *olen, size_t osize,
-        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng)
-    int mbedtls_pk_encrypt(
-        mbedtls_pk_context *ctx,
-        const unsigned char *input, size_t ilen,
-        unsigned char *output, size_t *olen, size_t osize,
-        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng)
-
-    int mbedtls_pk_check_pair(const mbedtls_pk_context *pub,
-                              const mbedtls_pk_context *prv)
-    # int mbedtls_pk_debug(const mbedtls_pk_context *ctx,
-    #                      mbedtls_pk_debug_item *items)
-    const char * mbedtls_pk_get_name(const mbedtls_pk_context *ctx)
-    mbedtls_pk_type_t mbedtls_pk_get_type(const mbedtls_pk_context *ctx)
-
-    int mbedtls_pk_parse_key(
-        mbedtls_pk_context *ctx,
-        const unsigned char *key, size_t keylen,
-        const unsigned char *pwd, size_t pwdlen)
-    int mbedtls_pk_parse_public_key(
-        mbedtls_pk_context *ctx,
-        const unsigned char *key, size_t keylen)
-
-    # int mbedtls_pk_parse_keyfile(
-    #     mbedtls_pk_context *ctx,
-    #     const char *path, const char *password)
-    # int mbedtls_pk_parse_public_keyfile(
-    #     mbedtls_pk_context *ctx, const char *path)
-
-    int mbedtls_pk_write_key_der(
-        mbedtls_pk_context *ctx,
-        unsigned char *buf, size_t size)
-    int mbedtls_pk_write_pubkey_der(
-        mbedtls_pk_context *ctx,
-        unsigned char *buf, size_t size)
-    int mbedtls_pk_write_pubkey_pem(
-        mbedtls_pk_context *ctx,
-        unsigned char *buf, size_t size)
-    int mbedtls_pk_write_key_pem(
-        mbedtls_pk_context *ctx,
-        unsigned char *buf, size_t size)
-
-
-cdef class CipherBase:
-    cdef mbedtls_pk_context _ctx
-
-
-cdef class RSA(CipherBase):
-    pass
-
-
-cdef class ECC(CipherBase):
-    cdef _curve
-
-
-cdef class ECPoint:
-    cdef _ecp.mbedtls_ecp_point _ctx
-
-
-cdef class DHBase:
-    cdef _dhm.mbedtls_dhm_context _ctx
-
-
-cdef class ECDHBase:
-    cdef _ecdh.mbedtls_ecdh_context _ctx
-    cdef curve
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2016, Elaborated Networks GmbH
+# Copyright (c) 2018, Mathias Laurin
+
+cimport mbedtls._dhm as _dhm
+cimport mbedtls._ecdh as _ecdh
+cimport mbedtls._ecp as _ecp
+cimport mbedtls._md as _md
+cimport mbedtls._rsa as _rsa
+cimport mbedtls.mpi as _mpi
+
+
+cdef extern from "mbedtls/pk.h" nogil:
+    ctypedef enum mbedtls_pk_type_t:
+        MBEDTLS_PK_NONE=0
+        MBEDTLS_PK_RSA
+        MBEDTLS_PK_ECKEY
+        MBEDTLS_PK_ECKEY_DH
+        MBEDTLS_PK_ECDSA
+        MBEDTLS_PK_RSA_ALT
+        MBEDTLS_PK_RSASSA_PSS
+
+    ctypedef struct mbedtls_pk_rsassa_pss_options:
+        pass
+
+    ctypedef struct mbedtls_pk_info_t:
+        pass
+
+    ctypedef struct mbedtls_pk_context:
+        pass
+
+    _rsa.mbedtls_rsa_context *mbedtls_pk_rsa(const mbedtls_pk_context pk)
+    _ecp.mbedtls_ecp_keypair *mbedtls_pk_ec(const mbedtls_pk_context pk)
+    # RSA-alt function pointer types
+    const mbedtls_pk_info_t *mbedtls_pk_info_from_type(
+        mbedtls_pk_type_t pk_type)
+    void mbedtls_pk_init(mbedtls_pk_context *ctx)
+    void mbedtls_pk_free(mbedtls_pk_context *ctx)
+    int mbedtls_pk_setup(mbedtls_pk_context *ctx,
+                         const mbedtls_pk_info_t *info)
+
+    size_t mbedtls_pk_get_bitlen(const mbedtls_pk_context *ctx)
+    size_t mbedtls_pk_get_len(const mbedtls_pk_context *ctx)
+    int mbedtls_pk_can_do(const mbedtls_pk_context *ctx,
+                          mbedtls_pk_type_t type)
+
+    int mbedtls_pk_verify(
+        mbedtls_pk_context *ctx, _md.mbedtls_md_type_t md_alg,
+        const unsigned char *hash, size_t hash_len,
+        const unsigned char *sig, size_t sig_len)
+    # int mbedtls_pk_verify_ext(
+    #     mbedtls_pk_type_t type, const void *options,
+    #     mbedtls_pk_context *ctx, _md.mbedtls_md_type_t md_alg,
+    #     const unsigned char *hash, size_t hash_len,
+    #     const unsigned char *sig, size_t sig_len)
+
+    int mbedtls_pk_sign(
+        mbedtls_pk_context *ctx, _md.mbedtls_md_type_t md_alg,
+        const unsigned char *hash, size_t hash_len,
+        unsigned char *sig, size_t *sig_len,
+        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng)
+
+    int mbedtls_pk_decrypt(
+        mbedtls_pk_context *ctx,
+        const unsigned char *input, size_t ilen,
+        unsigned char *output, size_t *olen, size_t osize,
+        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng)
+    int mbedtls_pk_encrypt(
+        mbedtls_pk_context *ctx,
+        const unsigned char *input, size_t ilen,
+        unsigned char *output, size_t *olen, size_t osize,
+        int (*f_rng)(void *, unsigned char *, size_t), void *p_rng)
+
+    int mbedtls_pk_check_pair(const mbedtls_pk_context *pub,
+                              const mbedtls_pk_context *prv)
+    # int mbedtls_pk_debug(const mbedtls_pk_context *ctx,
+    #                      mbedtls_pk_debug_item *items)
+    const char * mbedtls_pk_get_name(const mbedtls_pk_context *ctx)
+    mbedtls_pk_type_t mbedtls_pk_get_type(const mbedtls_pk_context *ctx)
+
+    int mbedtls_pk_parse_key(
+        mbedtls_pk_context *ctx,
+        const unsigned char *key, size_t keylen,
+        const unsigned char *pwd, size_t pwdlen)
+    int mbedtls_pk_parse_public_key(
+        mbedtls_pk_context *ctx,
+        const unsigned char *key, size_t keylen)
+
+    # int mbedtls_pk_parse_keyfile(
+    #     mbedtls_pk_context *ctx,
+    #     const char *path, const char *password)
+    # int mbedtls_pk_parse_public_keyfile(
+    #     mbedtls_pk_context *ctx, const char *path)
+
+    int mbedtls_pk_write_key_der(
+        mbedtls_pk_context *ctx,
+        unsigned char *buf, size_t size)
+    int mbedtls_pk_write_pubkey_der(
+        mbedtls_pk_context *ctx,
+        unsigned char *buf, size_t size)
+    int mbedtls_pk_write_pubkey_pem(
+        mbedtls_pk_context *ctx,
+        unsigned char *buf, size_t size)
+    int mbedtls_pk_write_key_pem(
+        mbedtls_pk_context *ctx,
+        unsigned char *buf, size_t size)
+
+
+cdef class CipherBase:
+    cdef mbedtls_pk_context _ctx
+
+
+cdef class RSA(CipherBase):
+    pass
+
+
+cdef class ECC(CipherBase):
+    cdef _curve
+
+
+cdef class ECPoint:
+    cdef _ecp.mbedtls_ecp_point _ctx
+
+
+cdef class DHBase:
+    cdef _dhm.mbedtls_dhm_context _ctx
+
+
+cdef class ECDHBase:
+    cdef _ecdh.mbedtls_ecdh_context _ctx
+    cdef curve
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/pk.pyi` & `python-mbedtls-2.7.1/src/mbedtls/pk.pyi`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,265 +1,265 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2022, Mathias Laurin
-
-from __future__ import annotations
-
-import enum
-import numbers
-import os
-import sys
-from typing import (
-    Callable,
-    NamedTuple,
-    NoReturn,
-    Optional,
-    Sequence,
-    Type,
-    TypeVar,
-    Union,
-    overload,
-)
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Final, Literal
-else:
-    from typing import Final, Literal
-
-if sys.version_info < (3, 9):
-    _PathLike = os.PathLike
-else:
-    _PathLike = os.PathLike[str]
-
-_Path = Union[_PathLike, str]
-CIPHER_NAME: Final[Sequence[bytes]] = ...
-_DER = bytes
-_PEM = str
-_NUM = int
-_MPI = Union[numbers.Integral, int]
-
-class CipherType(enum.Enum):
-    NONE: int
-    RSA: int
-    ECKEY: int
-    ECKEY_DH: int
-    ECDSA: int
-    RSA_ALT: int
-    RSASSA_PSS: int
-
-class KeyPair(NamedTuple):
-    private: Union[_DER, _PEM]
-    public: Union[_DER, _PEM]
-
-class Curve(bytes, enum.Enum):
-    SECP192R1: bytes
-    SECP224R1: bytes
-    SECP256R1: bytes
-    SECP384R1: bytes
-    SECP521R1: bytes
-    BRAINPOOLP256R1: bytes
-    BRAINPOOLP384R1: bytes
-    BRAINPOOLP512R1: bytes
-    SECP192K1: bytes
-    SECP224K1: bytes
-    SECP256K1: bytes
-    CURVE25519: bytes
-    CURVE448: bytes
-
-def check_pair(pub: CipherBase, priv: CipherBase) -> bool: ...
-def get_supported_ciphers() -> Sequence[bytes]: ...
-def get_supported_curves() -> Sequence[Curve]: ...
-
-# `Self` (PEP 673) should work as well but did not with typing_extensions 4.2.0
-_TCipherBase = TypeVar("_TCipherBase", bound=CipherBase)
-
-class CipherBase:
-    def __init__(
-        self,
-        name: bytes,
-        key: Optional[bytes] = ...,
-        password: Optional[bytes] = ...,
-    ) -> None: ...
-    def __hash__(self) -> int: ...
-    def __eq__(self, other: object) -> bool: ...
-    @classmethod
-    def from_buffer(
-        cls: Type[_TCipherBase],
-        buffer: bytes,
-        password: Optional[
-            Union[Callable[[], Union[bytes, bytearray]], bytes, bytearray]
-        ] = None,
-    ) -> _TCipherBase: ...
-    @classmethod
-    def from_file(
-        cls: Type[_TCipherBase],
-        path: _Path,
-        password: Optional[
-            Union[Callable[[], Union[bytes, bytearray]], bytes, bytearray]
-        ] = None,
-    ) -> _TCipherBase: ...
-    @classmethod
-    def from_DER(cls: Type[_TCipherBase], key: bytes) -> _TCipherBase: ...
-    @classmethod
-    def from_PEM(cls: Type[_TCipherBase], key: str) -> _TCipherBase: ...
-    @property
-    def name(self) -> bytes: ...
-    @property
-    def key_size(self) -> int: ...
-    def _has_private(self) -> bool: ...
-    def _has_public(self) -> bool: ...
-    def sign(
-        self, message: bytes, digestmod: Optional[str] = ...
-    ) -> bytes: ...
-    def verify(
-        self, message: bytes, signature: bytes, digestmod: str
-    ) -> bool: ...
-    def encrypt(self, message: bytes) -> bytes: ...
-    def decrypt(self, message: bytes) -> bytes: ...
-    def to_PEM(self) -> KeyPair: ...
-    def __str__(self) -> _PEM: ...
-    def to_DER(self) -> KeyPair: ...
-    def to_bytes(self) -> _DER: ...
-    def __bytes__(self) -> _DER: ...
-
-class RSA(CipherBase):
-    def __init__(
-        self, key: Optional[bytes] = ..., password: Optional[bytes] = ...
-    ) -> None: ...
-    def generate(self, key_size: int = ..., exponent: int = ...) -> _DER: ...
-    @overload
-    def export_key(self, format: Literal["DER"]) -> _DER: ...
-    @overload
-    def export_key(self, format: Literal["PEM"]) -> _PEM: ...
-    @overload
-    def export_key(self) -> Union[_DER, _PEM]: ...
-    @overload
-    def export_public_key(self, format: Literal["DER"]) -> _DER: ...
-    @overload
-    def export_public_key(self, format: Literal["PEM"]) -> _PEM: ...
-    @overload
-    def export_public_key(self) -> Union[_DER, _PEM]: ...
-
-class ECPoint:
-    def __init__(self, x: _MPI, y: _MPI, z: _MPI) -> None: ...
-    @property
-    def x(self) -> _MPI: ...
-    @property
-    def y(self) -> _MPI: ...
-    @property
-    def z(self) -> _MPI: ...
-    def __str__(self) -> str: ...
-    def __repr__(self) -> str: ...
-    def __eq__(self, other: object) -> bool: ...
-    def __hash__(self) -> int: ...
-    def __bool__(self) -> bool: ...
-
-class ECC(CipherBase):
-    def __init__(
-        self,
-        curve: Optional[Curve] = ...,
-        key: Optional[bytes] = ...,
-        password: Optional[bytes] = ...,
-    ) -> None: ...
-    @property
-    def curve(self) -> Curve: ...
-    def generate(self) -> bytes: ...
-    @overload
-    def export_key(self, format: Literal["DER"]) -> _DER: ...
-    @overload
-    def export_key(self, format: Literal["PEM"]) -> _PEM: ...
-    @overload
-    def export_key(self, format: Literal["NUM"]) -> _NUM: ...
-    @overload
-    def export_key(self) -> Union[_DER, _PEM, _NUM]: ...
-    @overload
-    def export_public_key(self, format: Literal["DER"]) -> _DER: ...
-    @overload
-    def export_public_key(self, format: Literal["PEM"]) -> _PEM: ...
-    @overload
-    def export_public_key(self, format: Literal["POINT"]) -> ECPoint: ...
-    @overload
-    def export_public_key(self) -> Union[_DER, _PEM, ECPoint]: ...
-
-class DHServer:
-    def __init__(self, modulus: _MPI, generator: _MPI) -> None: ...
-    def __getstate__(self) -> NoReturn: ...
-    @property
-    def key_size(self) -> int: ...
-    @property
-    def modulus(self) -> _MPI: ...
-    @property
-    def generator(self) -> _MPI: ...
-    @property
-    def _secret(self) -> _MPI: ...
-    @property
-    def shared_secret(self) -> _MPI: ...
-    def generate_secret(self) -> _MPI: ...
-    def generate(self) -> bytes: ...
-    def import_CKE(self, buffer: bytes) -> None: ...
-
-class DHClient:
-    def __init__(self, modulus: _MPI, generator: _MPI) -> None: ...
-    def __getstate__(self) -> NoReturn: ...
-    @property
-    def key_size(self) -> int: ...
-    @property
-    def modulus(self) -> _MPI: ...
-    @property
-    def generator(self) -> _MPI: ...
-    @property
-    def _secret(self) -> _MPI: ...
-    @property
-    def shared_secret(self) -> _MPI: ...
-    def generate_secret(self) -> _MPI: ...
-    def generate(self) -> bytes: ...
-    def import_SKE(self, buffer: bytes) -> None: ...
-
-class ECDHClient:
-    private_key: _MPI
-    public_key: ECPoint
-    peers_public_key: ECPoint
-    def __init__(self, ecc: ECC) -> None: ...
-    def __getstate__(self) -> NoReturn: ...
-    def _has_private(self) -> bool: ...
-    def _has_public(self) -> bool: ...
-    def _has_peers_public(self) -> bool: ...
-    @property
-    def shared_secret(self) -> _MPI: ...
-    def generate_secret(self) -> _MPI: ...
-    def generate_public_key(self) -> None: ...
-    def generate(self) -> bytes: ...
-    def import_SKE(self, buffer: bytes) -> None: ...
-
-class ECDHServer:
-    private_key: _MPI
-    public_key: ECPoint
-    peers_public_key: ECPoint
-    def __init__(self, ecc: ECC) -> None: ...
-    def __getstate__(self) -> NoReturn: ...
-    def _has_private(self) -> bool: ...
-    def _has_public(self) -> bool: ...
-    def _has_peers_public(self) -> bool: ...
-    @property
-    def shared_secret(self) -> _MPI: ...
-    def generate_secret(self) -> _MPI: ...
-    def generate_public_key(self) -> None: ...
-    def generate(self) -> bytes: ...
-    def import_CKE(self, buffer: bytes) -> None: ...
-
-class ECDHNaive:
-    private_key: _MPI
-    public_key: ECPoint
-    peers_public_key: ECPoint
-    def __init__(self, curve: Optional[Curve] = ...) -> None: ...
-    def __getstate__(self) -> NoReturn: ...
-    def _has_private(self) -> bool: ...
-    def _has_public(self) -> bool: ...
-    def _has_peers_public(self) -> bool: ...
-    @property
-    def shared_secret(self) -> _MPI: ...
-    def generate_secret(self) -> _MPI: ...
-    def generate_public_key(self) -> None: ...
-    def generate(self) -> ECPoint: ...
-    def import_SKE(self, buffer: bytes) -> None: ...
-    # extra methods
-    def import_peer_public(self, pubkey: ECPoint) -> None: ...
-    def import_peers_public(self, pubkey: ECPoint) -> None: ...
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2022, Mathias Laurin
+
+from __future__ import annotations
+
+import enum
+import numbers
+import os
+import sys
+from typing import (
+    Callable,
+    NamedTuple,
+    NoReturn,
+    Optional,
+    Sequence,
+    Type,
+    TypeVar,
+    Union,
+    overload,
+)
+
+if sys.version_info < (3, 8):
+    from typing_extensions import Final, Literal
+else:
+    from typing import Final, Literal
+
+if sys.version_info < (3, 9):
+    _PathLike = os.PathLike
+else:
+    _PathLike = os.PathLike[str]
+
+_Path = Union[_PathLike, str]
+CIPHER_NAME: Final[Sequence[bytes]] = ...
+_DER = bytes
+_PEM = str
+_NUM = int
+_MPI = Union[numbers.Integral, int]
+
+class CipherType(enum.Enum):
+    NONE: int
+    RSA: int
+    ECKEY: int
+    ECKEY_DH: int
+    ECDSA: int
+    RSA_ALT: int
+    RSASSA_PSS: int
+
+class KeyPair(NamedTuple):
+    private: Union[_DER, _PEM]
+    public: Union[_DER, _PEM]
+
+class Curve(bytes, enum.Enum):
+    SECP192R1: bytes
+    SECP224R1: bytes
+    SECP256R1: bytes
+    SECP384R1: bytes
+    SECP521R1: bytes
+    BRAINPOOLP256R1: bytes
+    BRAINPOOLP384R1: bytes
+    BRAINPOOLP512R1: bytes
+    SECP192K1: bytes
+    SECP224K1: bytes
+    SECP256K1: bytes
+    CURVE25519: bytes
+    CURVE448: bytes
+
+def check_pair(pub: CipherBase, priv: CipherBase) -> bool: ...
+def get_supported_ciphers() -> Sequence[bytes]: ...
+def get_supported_curves() -> Sequence[Curve]: ...
+
+# `Self` (PEP 673) should work as well but did not with typing_extensions 4.2.0
+_TCipherBase = TypeVar("_TCipherBase", bound=CipherBase)
+
+class CipherBase:
+    def __init__(
+        self,
+        name: bytes,
+        key: Optional[bytes] = ...,
+        password: Optional[bytes] = ...,
+    ) -> None: ...
+    def __hash__(self) -> int: ...
+    def __eq__(self, other: object) -> bool: ...
+    @classmethod
+    def from_buffer(
+        cls: Type[_TCipherBase],
+        buffer: bytes,
+        password: Optional[
+            Union[Callable[[], Union[bytes, bytearray]], bytes, bytearray]
+        ] = None,
+    ) -> _TCipherBase: ...
+    @classmethod
+    def from_file(
+        cls: Type[_TCipherBase],
+        path: _Path,
+        password: Optional[
+            Union[Callable[[], Union[bytes, bytearray]], bytes, bytearray]
+        ] = None,
+    ) -> _TCipherBase: ...
+    @classmethod
+    def from_DER(cls: Type[_TCipherBase], key: bytes) -> _TCipherBase: ...
+    @classmethod
+    def from_PEM(cls: Type[_TCipherBase], key: str) -> _TCipherBase: ...
+    @property
+    def name(self) -> bytes: ...
+    @property
+    def key_size(self) -> int: ...
+    def _has_private(self) -> bool: ...
+    def _has_public(self) -> bool: ...
+    def sign(
+        self, message: bytes, digestmod: Optional[str] = ...
+    ) -> bytes: ...
+    def verify(
+        self, message: bytes, signature: bytes, digestmod: str
+    ) -> bool: ...
+    def encrypt(self, message: bytes) -> bytes: ...
+    def decrypt(self, message: bytes) -> bytes: ...
+    def to_PEM(self) -> KeyPair: ...
+    def __str__(self) -> _PEM: ...
+    def to_DER(self) -> KeyPair: ...
+    def to_bytes(self) -> _DER: ...
+    def __bytes__(self) -> _DER: ...
+
+class RSA(CipherBase):
+    def __init__(
+        self, key: Optional[bytes] = ..., password: Optional[bytes] = ...
+    ) -> None: ...
+    def generate(self, key_size: int = ..., exponent: int = ...) -> _DER: ...
+    @overload
+    def export_key(self, format: Literal["DER"]) -> _DER: ...
+    @overload
+    def export_key(self, format: Literal["PEM"]) -> _PEM: ...
+    @overload
+    def export_key(self) -> Union[_DER, _PEM]: ...
+    @overload
+    def export_public_key(self, format: Literal["DER"]) -> _DER: ...
+    @overload
+    def export_public_key(self, format: Literal["PEM"]) -> _PEM: ...
+    @overload
+    def export_public_key(self) -> Union[_DER, _PEM]: ...
+
+class ECPoint:
+    def __init__(self, x: _MPI, y: _MPI, z: _MPI) -> None: ...
+    @property
+    def x(self) -> _MPI: ...
+    @property
+    def y(self) -> _MPI: ...
+    @property
+    def z(self) -> _MPI: ...
+    def __str__(self) -> str: ...
+    def __repr__(self) -> str: ...
+    def __eq__(self, other: object) -> bool: ...
+    def __hash__(self) -> int: ...
+    def __bool__(self) -> bool: ...
+
+class ECC(CipherBase):
+    def __init__(
+        self,
+        curve: Optional[Curve] = ...,
+        key: Optional[bytes] = ...,
+        password: Optional[bytes] = ...,
+    ) -> None: ...
+    @property
+    def curve(self) -> Curve: ...
+    def generate(self) -> bytes: ...
+    @overload
+    def export_key(self, format: Literal["DER"]) -> _DER: ...
+    @overload
+    def export_key(self, format: Literal["PEM"]) -> _PEM: ...
+    @overload
+    def export_key(self, format: Literal["NUM"]) -> _NUM: ...
+    @overload
+    def export_key(self) -> Union[_DER, _PEM, _NUM]: ...
+    @overload
+    def export_public_key(self, format: Literal["DER"]) -> _DER: ...
+    @overload
+    def export_public_key(self, format: Literal["PEM"]) -> _PEM: ...
+    @overload
+    def export_public_key(self, format: Literal["POINT"]) -> ECPoint: ...
+    @overload
+    def export_public_key(self) -> Union[_DER, _PEM, ECPoint]: ...
+
+class DHServer:
+    def __init__(self, modulus: _MPI, generator: _MPI) -> None: ...
+    def __getstate__(self) -> NoReturn: ...
+    @property
+    def key_size(self) -> int: ...
+    @property
+    def modulus(self) -> _MPI: ...
+    @property
+    def generator(self) -> _MPI: ...
+    @property
+    def _secret(self) -> _MPI: ...
+    @property
+    def shared_secret(self) -> _MPI: ...
+    def generate_secret(self) -> _MPI: ...
+    def generate(self) -> bytes: ...
+    def import_CKE(self, buffer: bytes) -> None: ...
+
+class DHClient:
+    def __init__(self, modulus: _MPI, generator: _MPI) -> None: ...
+    def __getstate__(self) -> NoReturn: ...
+    @property
+    def key_size(self) -> int: ...
+    @property
+    def modulus(self) -> _MPI: ...
+    @property
+    def generator(self) -> _MPI: ...
+    @property
+    def _secret(self) -> _MPI: ...
+    @property
+    def shared_secret(self) -> _MPI: ...
+    def generate_secret(self) -> _MPI: ...
+    def generate(self) -> bytes: ...
+    def import_SKE(self, buffer: bytes) -> None: ...
+
+class ECDHClient:
+    private_key: _MPI
+    public_key: ECPoint
+    peers_public_key: ECPoint
+    def __init__(self, ecc: ECC) -> None: ...
+    def __getstate__(self) -> NoReturn: ...
+    def _has_private(self) -> bool: ...
+    def _has_public(self) -> bool: ...
+    def _has_peers_public(self) -> bool: ...
+    @property
+    def shared_secret(self) -> _MPI: ...
+    def generate_secret(self) -> _MPI: ...
+    def generate_public_key(self) -> None: ...
+    def generate(self) -> bytes: ...
+    def import_SKE(self, buffer: bytes) -> None: ...
+
+class ECDHServer:
+    private_key: _MPI
+    public_key: ECPoint
+    peers_public_key: ECPoint
+    def __init__(self, ecc: ECC) -> None: ...
+    def __getstate__(self) -> NoReturn: ...
+    def _has_private(self) -> bool: ...
+    def _has_public(self) -> bool: ...
+    def _has_peers_public(self) -> bool: ...
+    @property
+    def shared_secret(self) -> _MPI: ...
+    def generate_secret(self) -> _MPI: ...
+    def generate_public_key(self) -> None: ...
+    def generate(self) -> bytes: ...
+    def import_CKE(self, buffer: bytes) -> None: ...
+
+class ECDHNaive:
+    private_key: _MPI
+    public_key: ECPoint
+    peers_public_key: ECPoint
+    def __init__(self, curve: Optional[Curve] = ...) -> None: ...
+    def __getstate__(self) -> NoReturn: ...
+    def _has_private(self) -> bool: ...
+    def _has_public(self) -> bool: ...
+    def _has_peers_public(self) -> bool: ...
+    @property
+    def shared_secret(self) -> _MPI: ...
+    def generate_secret(self) -> _MPI: ...
+    def generate_public_key(self) -> None: ...
+    def generate(self) -> ECPoint: ...
+    def import_SKE(self, buffer: bytes) -> None: ...
+    # extra methods
+    def import_peer_public(self, pubkey: ECPoint) -> None: ...
+    def import_peers_public(self, pubkey: ECPoint) -> None: ...
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/pk.pyx` & `python-mbedtls-2.7.1/src/mbedtls/pk.pyx`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,1148 +1,1148 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2016, Elaborated Networks GmbH
-# Copyright (c) 2018, Mathias Laurin
-
-"""Public key (PK) library.
-
-The library handles RSA certificates and ECC (elliptic curve
-cryptography).
-
-The RSA and ECC classes offer compatible APIs.  They may be used
-interchangeably.
-
-ECDHServer and ECDHClient should be used for ephemeral Elliptic Curve
-Diffie-Hellman exchange.
-
-"""
-
-
-from libc.stdlib cimport free, malloc
-from libc.string cimport memset
-
-cimport mbedtls._dhm as _dhm
-cimport mbedtls._ecdh as _ecdh
-cimport mbedtls._ecp as _ecp
-cimport mbedtls._random as _rnd
-cimport mbedtls._rsa as _rsa
-cimport mbedtls.mpi as _mpi
-cimport mbedtls.pk as _pk
-
-import enum
-import re
-from collections import namedtuple
-from functools import partial
-from pathlib import Path
-
-import mbedtls._random as _rnd
-import mbedtls.exceptions as _exc
-from mbedtls.hashlib import new as _new_hash
-
-__all__ = ("check_pair", "get_supported_ciphers", "get_supported_curves",
-           "Curve", "RSA", "ECC", "DHServer", "DHClient",
-           "ECDHServer", "ECDHClient", "ECDHNaive")
-
-
-CIPHER_NAME = (
-    b"NONE",
-    b"RSA",
-    b"EC",
-    b"EC_DH",
-    b"ECDSA",
-    # b"RSA_ALT",
-    # b"RSASSA_PSS",
-)
-
-
-class CipherType(enum.Enum):
-    NONE = _pk.MBEDTLS_PK_NONE
-    RSA = _pk.MBEDTLS_PK_RSA
-    ECKEY = _pk.MBEDTLS_PK_ECKEY
-    ECKEY_DH = _pk.MBEDTLS_PK_ECKEY_DH
-    ECDSA = _pk.MBEDTLS_PK_ECDSA
-    RSA_ALT = _pk.MBEDTLS_PK_RSA_ALT
-    RSASSA_PSS = _pk.MBEDTLS_PK_RSASSA_PSS
-
-
-KeyPair = namedtuple("KeyPair", ["private", "public"])
-
-
-class Curve(bytes, enum.Enum):
-
-    """Elliptic curves."""
-
-    SECP192R1 = b'secp192r1'
-    SECP224R1 = b'secp224r1'
-    SECP256R1 = b'secp256r1'
-    SECP384R1 = b'secp384r1'
-    SECP521R1 = b'secp521r1'
-    BRAINPOOLP256R1 = b'brainpoolP256r1'
-    BRAINPOOLP384R1 = b'brainpoolP384r1'
-    BRAINPOOLP512R1 = b'brainpoolP512r1'
-    SECP192K1 = b'secp192k1'
-    SECP224K1 = b'secp224k1'
-    SECP256K1 = b'secp256k1'
-    CURVE25519 = b'x25519'
-    CURVE448 = b'x448'
-
-
-# The following calculations come from mbedtls/library/pkwrite.c.
-RSA_PUB_DER_MAX_BYTES = 38 + 2 * _mpi.MBEDTLS_MPI_MAX_SIZE
-MPI_MAX_SIZE_2 = _mpi.MBEDTLS_MPI_MAX_SIZE // 2 + _mpi.MBEDTLS_MPI_MAX_SIZE % 2
-RSA_PRV_DER_MAX_BYTES = 47 + 3 * _mpi.MBEDTLS_MPI_MAX_SIZE + 5 * MPI_MAX_SIZE_2
-
-ECP_PUB_DER_MAX_BYTES = 30 + 2 * _ecp.MBEDTLS_ECP_MAX_BYTES
-ECP_PRV_DER_MAX_BYTES = 29 + 3 * _ecp.MBEDTLS_ECP_MAX_BYTES
-
-PUB_DER_MAX_BYTES = max(RSA_PUB_DER_MAX_BYTES, ECP_PUB_DER_MAX_BYTES)
-PRV_DER_MAX_BYTES = max(RSA_PRV_DER_MAX_BYTES, ECP_PRV_DER_MAX_BYTES)
-
-del RSA_PUB_DER_MAX_BYTES, MPI_MAX_SIZE_2, RSA_PRV_DER_MAX_BYTES
-del ECP_PUB_DER_MAX_BYTES, ECP_PRV_DER_MAX_BYTES
-
-
-cpdef check_pair(CipherBase pub, CipherBase pri):
-    """Check if a public-private pair of keys matches."""
-    return _pk.mbedtls_pk_check_pair(&pub._ctx, &pri._ctx) == 0
-
-
-def _type_from_name(name):
-    return {name: n for n, name in enumerate(CIPHER_NAME)}.get(name, 0)
-
-
-cpdef get_supported_ciphers():
-    return CIPHER_NAME
-
-
-def get_supported_curves():
-    """Return the list of supported curves in order of preference."""
-    cdef const _ecp.mbedtls_ecp_curve_info* info = _ecp.mbedtls_ecp_curve_list()
-    names, idx = [], 0
-    while info[idx].name != NULL:
-        names.append(Curve(bytes(info[idx].name)))
-        idx += 1
-    return names
-
-
-cdef curve_name_to_grp_id(curve):
-    cdef const _ecp.mbedtls_ecp_curve_info* info = _ecp.mbedtls_ecp_curve_list()
-    idx = 0
-    while info[idx].name != NULL:
-        if info[idx].name == curve:
-            return info[idx].grp_id
-        idx += 1
-    raise LookupError(curve.decode("ascii") + " not found")
-
-
-cdef _rnd.Random __rng = _rnd.default_rng()
-
-
-def _get_md_alg(digestmod):
-    """Return the hash object.
-
-    Arguments:
-        digestmod: The digest name or digest constructor for the
-            Cipher object to use.  It supports any name suitable to
-            `mbedtls.hash.new()`.
-
-    """
-    # `digestmod` handling below is adapted from CPython's
-    # `hmac.py`.
-    if callable(digestmod):
-        return digestmod
-    elif isinstance(digestmod, (str, unicode)):
-        return partial(_new_hash, digestmod)
-    else:
-        raise TypeError("a valid digestmod is required, got %r" % digestmod)
-
-
-cdef class CipherBase:
-    """Base class to RSA and ECC ciphers.
-
-    Parameters:
-        name (bytes): The cipher name known to mbed TLS.
-        key (bytes, optional): A key (public or private half).
-        password (bytes, optional): The password for the key.
-
-    """
-    def __init__(self,
-                 name,
-                 const unsigned char[:] key=None,
-                 const unsigned char[:] password=None):
-        _exc.check_error(_pk.mbedtls_pk_setup(
-            &self._ctx,
-            _pk.mbedtls_pk_info_from_type(
-                _type_from_name(name)
-            )
-        ))
-        if key is None or key.size == 0:
-            return
-        mbedtls_pk_free(&self._ctx)  # The context must be reset on entry.
-        try:
-            if password is None or password.size == 0:
-                _exc.check_error(_pk.mbedtls_pk_parse_key(
-                    &self._ctx, &key[0], key.size, NULL, 0
-                ))
-            else:
-                _exc.check_error(_pk.mbedtls_pk_parse_key(
-                    &self._ctx, &key[0], key.size, &password[0], password.size
-                ))
-        except _exc.TLSError:
-            _exc.check_error(_pk.mbedtls_pk_parse_public_key(
-                &self._ctx, &key[0], key.size))
-
-    def __cinit__(self):
-        """Initialize the context."""
-        _pk.mbedtls_pk_init(&self._ctx)
-
-    def __reduce__(self):
-        key = self.export_key()
-        if not key:
-            key = self.export_public_key()
-        return type(self).from_buffer, (key,)
-
-    def __dealloc__(self):
-        """Free and clear the context."""
-        _pk.mbedtls_pk_free(&self._ctx)
-
-    def __hash__(self):
-        if self._has_private():
-            return hash(self.export_key(format="DER"))
-        else:
-            return hash(self.export_public_key(format="DER"))
-
-    def __eq__(self, other):
-        if isinstance(other, str):
-            other = other.encode("ascii")
-        if isinstance(other, bytes):
-            try:
-                other = type(self).from_buffer(other)
-            except (_exc.TLSError, ValueError, TypeError):
-                return False
-        if type(other) is not type(self):
-            return False
-        if self._has_private() or other._has_private():
-            return other.export_key() == self.export_key()
-        elif not (self._has_private() and other._has_private()):
-            return other.export_public_key() == self.export_public_key()
-
-    @classmethod
-    def from_buffer(
-        cls,
-        const unsigned char[:] key not None,
-        password=None,
-    ):
-        """Import a key (public or private half).
-
-        The public half is generated upon importing a private key.
-
-        Arguments:
-            key (bytes): The key in PEM or DER format.
-            password (bytes, optional): The password for
-                password-protected private keys.
-
-        """
-        bkey = bytes(key)
-        if re.search(b"^-----BEGIN.+END.+-----\\s+$", bkey, re.DOTALL):
-            # PEM must be null-terminated.
-            bkey = bkey + b"\0"
-        if callable(password):
-            return cls(key=bkey, password=password())
-        return cls(key=bkey, password=password)
-
-    @classmethod
-    def from_file(cls, path, password=None):
-        return cls.from_buffer(Path(path).read_bytes(), password)
-
-    @classmethod
-    def from_DER(cls, const unsigned char[:] key not None):
-        return cls.from_buffer(key)
-
-    @classmethod
-    def from_PEM(cls, key):
-        """Import a key (public or private half)."""
-        return cls.from_buffer(key.encode("ascii"))
-
-    @property
-    def _type(self):
-        """Return the type of the cipher."""
-        return _pk.mbedtls_pk_get_type(&self._ctx)
-
-    @property
-    def name(self):
-        """Return the name of the cipher."""
-        return _pk.mbedtls_pk_get_name(&self._ctx)
-
-    @property
-    def _bitlen(self):
-        """Return the size of the key, in bits."""
-        return _pk.mbedtls_pk_get_bitlen(&self._ctx)
-
-    @property
-    def key_size(self):
-        """Return the size of the key, in bytes."""
-        return _pk.mbedtls_pk_get_len(&self._ctx)
-
-    def _has_private(self):
-        """Return `True` if the key contains a valid private half."""
-        raise NotImplementedError
-
-    def _has_public(self):
-        """Return `True` if the key contains a valid public half."""
-        raise NotImplementedError
-
-    def sign(self,
-             const unsigned char[:] message not None,
-             digestmod=None):
-        """Make signature, including padding if relevant.
-
-        Arguments:
-            message (bytes): The message to sign.
-            digestmod (optional): The digest name or digest constructor.
-
-        Return:
-            bytes or None: The signature or None if the cipher does not
-                contain a private key.
-
-        """
-        if digestmod is None:
-            digestmod = 'sha256'
-        if not self._has_private():
-            return None
-        md_alg = _get_md_alg(digestmod)(message)
-        cdef const unsigned char[:] hash_ = md_alg.digest()
-        cdef size_t sig_len = 0
-        cdef unsigned char* output = <unsigned char*>malloc(
-            _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
-        if not output:
-            raise MemoryError()
-        try:
-            _exc.check_error(_pk.mbedtls_pk_sign(
-                &self._ctx, md_alg._type,
-                &hash_[0], hash_.size,
-                &output[0], &sig_len,
-                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
-            assert sig_len != 0
-            return output[:sig_len]
-        finally:
-            free(output)
-
-    def verify(self,
-               const unsigned char[:] message not None,
-               const unsigned char[:] signature not None,
-               digestmod=None):
-        """Verify signature, including padding if relevant.
-
-        Arguments:
-            message (bytes): The message to sign.
-            signature (bytes): The signature to verify.
-            digestmod (optional): The digest name or digest constructor.
-
-        Return:
-            bool: True if the verification passed, False otherwise.
-
-        """
-        if signature.size == 0:
-            return False
-        if digestmod is None:
-            digestmod = 'sha256'
-        md_alg = _get_md_alg(digestmod)(message)
-        cdef const unsigned char[:] hash_ = md_alg.digest()
-        return _pk.mbedtls_pk_verify(
-            &self._ctx, md_alg._type,
-            &hash_[0], hash_.size,
-            &signature[0], signature.size) == 0
-
-    def encrypt(self, const unsigned char[:] message not None):
-        """Encrypt message (including padding if relevant).
-
-        Arguments:
-            message (bytes): Message to encrypt.
-
-        """
-        if message.size == 0:
-            message = b"\0"
-        cdef size_t olen = 0
-        cdef unsigned char* output = <unsigned char*>malloc(
-            _mpi.MBEDTLS_MPI_MAX_SIZE // 2 * sizeof(unsigned char))
-        if not output:
-            raise MemoryError()
-        try:
-            _exc.check_error(_pk.mbedtls_pk_encrypt(
-                &self._ctx, &message[0], message.size,
-                output, &olen, self.key_size,
-                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
-            return output[:olen]
-        finally:
-            free(output)
-
-    def decrypt(self, const unsigned char[:] message not None):
-        """Decrypt message (including padding if relevant).
-
-        Arguments:
-            message (bytes): Message to decrypt.
-
-        """
-        if message.size == 0:
-            message = b"\0"
-        cdef size_t olen = 0
-        cdef unsigned char* output = <unsigned char*>malloc(
-            _mpi.MBEDTLS_MPI_MAX_SIZE // 2 * sizeof(unsigned char))
-        if not output:
-            raise MemoryError()
-        try:
-            _exc.check_error(_pk.mbedtls_pk_decrypt(
-                &self._ctx, &message[0], message.size,
-                output, &olen, self.key_size,
-                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
-            return output[:olen]
-        finally:
-            free(output)
-
-    def generate(self):
-        """Generate a keypair.
-
-        Return:
-            (bytes): The private key in DER format.
-
-        """
-        raise NotImplementedError
-
-    def _private_to_DER(self):
-        if not self._has_private():
-            return b""
-        cdef int olen
-        cdef size_t osize = PRV_DER_MAX_BYTES
-        cdef unsigned char *output = <unsigned char *>malloc(
-            osize * sizeof(unsigned char))
-        if not output:
-            raise MemoryError()
-        try:
-            olen = _exc.check_error(
-                _pk.mbedtls_pk_write_key_der(&self._ctx, output, osize))
-            return output[osize - olen:osize]
-        finally:
-            free(output)
-
-    def _private_to_PEM(self):
-        if not self._has_private():
-            return ""
-        cdef size_t osize = PRV_DER_MAX_BYTES * 4 // 3 + 100
-        cdef unsigned char *output = <unsigned char *>malloc(
-            osize * sizeof(unsigned char))
-        if not output:
-            raise MemoryError()
-        memset(output, 0, osize)
-        try:
-            _exc.check_error(
-                _pk.mbedtls_pk_write_key_pem(&self._ctx, output, osize))
-            return output[0:osize].rstrip(b"\0").decode("ascii")
-        finally:
-            free(output)
-
-    def export_key(self, format="DER"):
-        """Return the private key.
-
-        If no key is present, return a falsy value.
-
-        Args:
-            format (str): One of "DER" or "PEM".
-
-        """
-        if format == "DER":
-            return self._private_to_DER()
-        if format == "PEM":
-            return self._private_to_PEM()
-        raise ValueError(format)
-
-    def _public_to_DER(self):
-        if not self._has_public():
-            return b""
-        cdef int olen
-        cdef size_t osize = PRV_DER_MAX_BYTES
-        cdef unsigned char *output = <unsigned char *>malloc(
-            osize * sizeof(unsigned char))
-        if not output:
-            raise MemoryError()
-        try:
-            olen = _exc.check_error(
-                _pk.mbedtls_pk_write_pubkey_der(&self._ctx, output, osize))
-            return output[osize - olen:osize]
-        finally:
-            free(output)
-
-    def _public_to_PEM(self):
-        if not self._has_public():
-            return ""
-        cdef size_t osize = PRV_DER_MAX_BYTES * 4 // 3 + 100
-        cdef unsigned char *output = <unsigned char *>malloc(
-            osize * sizeof(unsigned char))
-        if not output:
-            raise MemoryError()
-        memset(output, 0, osize)
-        try:
-            _exc.check_error(
-                _pk.mbedtls_pk_write_pubkey_pem(&self._ctx, output, osize))
-            return output[0:osize].rstrip(b"\0").decode("ascii")
-        finally:
-            free(output)
-
-    def export_public_key(self, format="DER"):
-        """Return the public key.
-
-        If no key is present, return a falsy value.
-
-        Args:
-            format (str): One of "DER" or "PEM".
-
-        """
-        if format == "DER":
-            return self._public_to_DER()
-        if format == "PEM":
-            return self._public_to_PEM()
-        raise ValueError(format)
-
-    def to_PEM(self):
-        """Return the RSA in PEM format.
-
-        Warning:
-            This function is obsolete.
-
-        Return:
-            tuple(str, str): The private key and the public key.
-
-        See Also:
-            export_key(), export_public_key()
-
-        """
-        return KeyPair(self.export_key("PEM"), self.export_public_key("PEM"))
-
-    def __str__(self):
-        return self.export_key(format="PEM")
-
-    def to_DER(self):
-        """Return the RSA in DER format.
-
-        Warning:
-            This function is obsolete.
-
-        Return:
-            tuple(bytes, bytes): The private key and the public key.
-
-        See Also:
-            export_key(), export_public_key()
-
-        """
-        return KeyPair(self.export_key("DER"), self.export_public_key("DER"))
-
-    def to_bytes(self):
-        """Return the private key in DER format."""
-        return self.export_key(format="DER")
-
-    def __bytes__(self):
-        return self.to_bytes()
-
-
-cdef class RSA(CipherBase):
-
-    """RSA public-key cryptosystem."""
-
-    def __init__(self,
-                 const unsigned char[:] key=None,
-                 const unsigned char[:] password=None):
-        super().__init__(b"RSA", key, password)
-
-    def _has_private(self):
-        """Return `True` if the key contains a valid private half."""
-        return _rsa.mbedtls_rsa_check_privkey(
-            _pk.mbedtls_pk_rsa(self._ctx)
-        ) == 0
-
-    def _has_public(self):
-        """Return `True` if the key contains a valid public half."""
-        return _rsa.mbedtls_rsa_check_pubkey(_pk.mbedtls_pk_rsa(self._ctx)) == 0
-
-    def generate(self, unsigned int key_size=2048, int exponent=65537):
-        """Generate an RSA keypair.
-
-        Arguments:
-            key_size (unsigned int): size in bits.
-            exponent (int): public RSA exponent.
-
-        Return:
-            (bytes): The private key in DER format.
-
-        """
-        _exc.check_error(_rsa.mbedtls_rsa_gen_key(
-            _pk.mbedtls_pk_rsa(self._ctx), &_rnd.mbedtls_ctr_drbg_random,
-            &__rng._ctx, key_size, exponent))
-        return self.export_key("DER")
-
-
-cdef class ECPoint:
-
-    """A point on the elliptic curve."""
-    def __init__(self, x, y, z):
-        cdef _mpi.MPI _x = _mpi.MPI(x)
-        cdef _mpi.MPI _y = _mpi.MPI(y)
-        cdef _mpi.MPI _z = _mpi.MPI(z)
-        _mpi.mbedtls_mpi_copy(&self._ctx.X, &_x._ctx)
-        _mpi.mbedtls_mpi_copy(&self._ctx.Y, &_y._ctx)
-        _mpi.mbedtls_mpi_copy(&self._ctx.Z, &_z._ctx)
-
-    def __cinit__(self):
-        """Initialize the context."""
-        _ecp.mbedtls_ecp_point_init(&self._ctx)
-
-    def __dealloc__(self):
-        """Free and clear the context."""
-        _ecp.mbedtls_ecp_point_free(&self._ctx)
-
-    def __reduce__(self):
-        return type(self), (self.x, self.y, self.z)
-
-    @property
-    def x(self):
-        """Return the X coordinate."""
-        try:
-            return _mpi.from_mpi_p(&self._ctx.X)
-        except ValueError:
-            return _mpi.MPI()
-
-    @property
-    def y(self):
-        """Return the Y coordinate."""
-        try:
-            return _mpi.from_mpi_p(&self._ctx.Y)
-        except ValueError:
-            return _mpi.MPI()
-
-    @property
-    def z(self):
-        """Return the Z coordinate."""
-        try:
-            return _mpi.from_mpi_p(&self._ctx.Z)
-        except ValueError:
-            return _mpi.MPI()
-
-    def __str__(self):
-        return "%s(%i, %i, %i)" % (
-            type(self).__name__, self.x, self.y, self.z
-        )
-
-    def __repr__(self):
-        return "%s(%r, %r, %r)" % (
-            type(self).__name__, self.x, self.y, self.z
-        )
-
-    def __eq__(self, other):
-        if other == 0:
-            return _ecp.mbedtls_ecp_is_zero(&self._ctx) == 1
-        elif type(other) is type(self):
-            c_other = <ECPoint> other
-            return _ecp.mbedtls_ecp_point_cmp(&self._ctx, &c_other._ctx) == 0
-        return NotImplemented
-
-    def __hash__(self):
-        return hash((self.x, self.y, self.z))
-
-    def __bool__(self):
-        return _ecp.mbedtls_ecp_is_zero(&self._ctx) == 0
-
-
-cdef class ECC(CipherBase):
-
-    """Elliptic-curve cryptosystems.
-
-    Args:
-        (Curve, optional): A curve returned by `get_supported_curves()`.
-
-    See Also:
-        get_supported_curves()
-
-    """
-    def __init__(self,
-                 curve=None,
-                 const unsigned char[:] key=None,
-                 const unsigned char[:] password=None):
-        super().__init__(b"EC", key, password)
-        if curve is None:
-            curve = get_supported_curves()[0]
-        self._curve = curve
-
-    @property
-    def curve(self):
-        return self._curve
-
-    def _has_private(self):
-        """Return `True` if the key contains a valid private half."""
-        cdef const _ecp.mbedtls_ecp_keypair* ecp = _pk.mbedtls_pk_ec(self._ctx)
-        return _mpi.mbedtls_mpi_cmp_mpi(&ecp.d, &_mpi.MPI()._ctx) != 0
-
-    def _has_public(self):
-        """Return `True` if the key contains a valid public half."""
-        cdef _ecp.mbedtls_ecp_keypair* ecp = _pk.mbedtls_pk_ec(self._ctx)
-        return not _ecp.mbedtls_ecp_is_zero(&ecp.Q)
-
-    def sign(self,
-             const unsigned char[:] message not None,
-             digestmod=None):
-        if self._curve in (Curve.CURVE25519, Curve.CURVE448):
-            raise ValueError("ECDSA does not support Curve25519 or Curve448.")
-        return super().sign(message, digestmod)
-
-    def generate(self):
-        """Generate an EC keypair.
-
-        Return:
-            (bytes): The private key in DER format.
-
-        """
-        grp_id = curve_name_to_grp_id(self.curve)
-        if grp_id is None:
-            raise ValueError(self.curve)
-        _exc.check_error(_ecp.mbedtls_ecp_gen_key(
-            grp_id, _pk.mbedtls_pk_ec(self._ctx),
-            &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
-        format = (
-            "NUM"
-            if self.curve in (Curve.CURVE25519, Curve.CURVE448)
-            else "DER"
-        )
-        return self.export_key(format)
-
-    def _private_to_num(self):
-        try:
-            return _mpi.from_mpi_p(&_pk.mbedtls_pk_ec(self._ctx).d)
-        except ValueError:
-            return _mpi.MPI()
-
-    def export_key(self, format=None):
-        """Return the private key.
-
-        If not key is present, return a falsy value.
-
-        Args:
-            format (str): One of "DER", "PEM", or "NUM".
-
-        """
-        if format is None:
-            format = (
-                "NUM"
-                if self.curve in (Curve.CURVE25519, Curve.CURVE448)
-                else "DER"
-            )
-        if format == "NUM":
-            return self._private_to_num()
-        elif self.curve in (Curve.CURVE25519, Curve.CURVE448):
-            raise ValueError(
-                "Curve25519 and Curve448 only support export as NUM"
-            )
-        return super().export_key(format)
-
-    def _public_to_point(self):
-        point = ECPoint(0, 0, 0)
-        _ecp.mbedtls_ecp_copy(&point._ctx, &_pk.mbedtls_pk_ec(self._ctx).Q)
-        return point
-
-    def export_public_key(self, format="DER"):
-        """Return the public key.
-
-        If no key is present, return a falsy value.
-
-        Args:
-            format (str): One of "DER", "PEM", or "POINT".
-
-        """
-        if format == "POINT":
-            return self._public_to_point()
-        elif self.curve in (Curve.CURVE25519, Curve.CURVE448):
-            raise ValueError(
-                "Curve25519 and Curve448 only support export as NUM"
-            )
-        return super().export_public_key(format)
-
-
-cdef class DHBase:
-
-    """Base class to DH key exchange: client and server.
-
-    Args:
-        modulus (int): The prime modulus P.
-        generator (int): The generator G, a primitive root modulo P.
-
-    See Also:
-        DHServer, DHClient: The derived classes.
-
-    """
-    def __init__(self, modulus, generator):
-        super().__init__()
-        _exc.check_error(_mpi.mbedtls_mpi_copy(
-            &self._ctx.P, &_mpi.MPI(modulus)._ctx))
-        _exc.check_error(_mpi.mbedtls_mpi_copy(
-            &self._ctx.G, &_mpi.MPI(generator)._ctx))
-
-    def __cinit__(self):
-        """Initialize the context."""
-        _dhm.mbedtls_dhm_init(&self._ctx)
-
-    def __dealloc__(self):
-        """Free and clear the context."""
-        _dhm.mbedtls_dhm_free(&self._ctx)
-
-    def __getstate__(self):
-        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
-
-    @property
-    def key_size(self):
-        """Return the size of the key, in bytes."""
-        return _mpi.mbedtls_mpi_size(&self._ctx.P)
-
-    @property
-    def modulus(self):
-        """Return the prime modulus, P."""
-        return _mpi.from_mpi_p(&self._ctx.P)
-
-    @property
-    def generator(self):
-        """Return the generator, G."""
-        return _mpi.from_mpi_p(&self._ctx.G)
-
-    @property
-    def _secret(self):
-        """Return the secret (int)."""
-        return _mpi.from_mpi_p(&self._ctx.X)
-
-    @property
-    def shared_secret(self):
-        """The shared secret (int).
-
-        The shared secret is 0 if the TLS handshake is not finished.
-
-        """
-        try:
-            return _mpi.from_mpi_p(&self._ctx.K)
-        except ValueError:
-            return _mpi.MPI()
-
-    def generate_secret(self):
-        """Generate the shared secret."""
-        cdef _mpi.MPI mpi
-        cdef unsigned char* output = <unsigned char*>malloc(
-            _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
-        cdef size_t olen = 0
-        if not output:
-            raise MemoryError()
-        try:
-            _exc.check_error(_dhm.mbedtls_dhm_calc_secret(
-                &self._ctx, &output[0], _mpi.MBEDTLS_MPI_MAX_SIZE, &olen,
-                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
-            mpi = _mpi.MPI()
-            _mpi.mbedtls_mpi_read_binary(&mpi._ctx, &output[0], olen)
-            return mpi
-        finally:
-            free(output)
-
-
-cdef class DHServer(DHBase):
-
-    """The server side of the DH key exchange."""
-
-    def generate(self):
-        """Generate a public key.
-
-        Return:
-            bytes: A TLS ServerKeyExchange payload.
-
-        """
-        cdef unsigned char* output = <unsigned char*>malloc(
-            _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
-        cdef size_t olen = 0
-        if not output:
-            raise MemoryError()
-        try:
-            _exc.check_error(_dhm.mbedtls_dhm_make_params(
-                &self._ctx, self.key_size, &output[0], &olen,
-                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
-            assert olen != 0
-            return output[:olen]
-        finally:
-            free(output)
-
-    def import_CKE(self, const unsigned char[:] buffer not None):
-        """Read the ClientKeyExchange payload."""
-        if buffer.size == 0:
-            buffer = b"\0"
-        _exc.check_error(_dhm.mbedtls_dhm_read_public(
-            &self._ctx, &buffer[0], buffer.size))
-
-
-cdef class DHClient(DHBase):
-
-    """The client side of the DH key exchange."""
-
-    def generate(self):
-        """Generate the public key.
-
-        Return:
-            bytes: The byte representation (big endian) of: G^X mod P.
-
-        """
-        cdef _mpi.MPI mpi
-        cdef unsigned char* output = <unsigned char*>malloc(
-            _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
-        if not output:
-            raise MemoryError()
-        try:
-            _exc.check_error(_dhm.mbedtls_dhm_make_public(
-                &self._ctx, self.key_size, &output[0], self.key_size,
-                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
-            mpi = _mpi.from_mpi_p(&self._ctx.GX)
-            return mpi.to_bytes(
-                _mpi.mbedtls_mpi_size(&mpi._ctx), "big")
-        finally:
-            free(output)
-
-    def import_SKE(self, const unsigned char[:] buffer not None):
-        """Read the ServerKeyExchange payload."""
-        if buffer.size == 0:
-            raise ValueError("SKE is empty")
-        # Const away cast is safe because the pointer is used as
-        # a read-only index in `dhm_read_bignum()`.
-        cdef unsigned char* first = <unsigned char*> &buffer[0]
-        cdef const unsigned char* end = &buffer[-1] + 1
-        _exc.check_error(_dhm.mbedtls_dhm_read_params(&self._ctx, &first, end))
-
-
-cdef class ECDHBase:
-
-    """Base class to ECDH(E) key exchange: client and server.
-
-    Args:
-        (Curve, optional): A curve returned by `get_supported_curves()`.
-
-    See Also:
-        ECDHServer, ECDHClient: The derived class.
-        get_supported_curves()
-
-    """
-    def __init__(self, curve=None):
-        super().__init__()
-        if curve is None:
-            curve = get_supported_curves()[0]
-        self.curve = Curve(curve)
-        _exc.check_error(_ecp.mbedtls_ecp_group_load(
-            &self._ctx.grp, curve_name_to_grp_id(self.curve)))
-
-    def __cinit__(self):
-        """Initialize the context."""
-        _ecdh.mbedtls_ecdh_init(&self._ctx)
-
-    def __dealloc__(self):
-        """Free and clear the context."""
-        _ecdh.mbedtls_ecdh_free(&self._ctx)
-
-    def __getstate__(self):
-        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
-
-    def _has_private(self):
-        """Return `True` if the key contains a valid private half."""
-        return _mpi.mbedtls_mpi_cmp_mpi(&self._ctx.d, &_mpi.MPI()._ctx) != 0
-
-    def _has_public(self):
-        """Return `True` if the key contains a valid public half."""
-        return not _ecp.mbedtls_ecp_is_zero(&self._ctx.Q)
-
-    def _has_peers_public(self):
-        """Return `True` if the peer's key is present."""
-        return not _ecp.mbedtls_ecp_is_zero(&self._ctx.Qp)
-
-    @property
-    def public_key(self):
-        """The public key (ECPoint)"""
-        ecp = ECPoint(0, 0, 0)
-        _exc.check_error(_ecp.mbedtls_ecp_copy(&ecp._ctx, &self._ctx.Q))
-        return ecp
-
-    @public_key.setter
-    def public_key(self, ECPoint ecp):
-        _exc.check_error(_ecp.mbedtls_ecp_copy(&self._ctx.Q, &ecp._ctx))
-
-    @property
-    def private_key(self):
-        """The private key (int)"""
-        return _mpi.from_mpi_p(&self._ctx.d)
-
-    @private_key.setter
-    def private_key(self, priv):
-        cdef _mpi.MPI c_priv = _mpi.MPI(priv)
-        _mpi.mbedtls_mpi_copy(&self._ctx.d, &c_priv._ctx)
-
-    @property
-    def peers_public_key(self):
-        """Peer's public key (ECPoint)"""
-        ecp = ECPoint(0, 0, 0)
-        _exc.check_error(_ecp.mbedtls_ecp_copy(&ecp._ctx, &self._ctx.Qp))
-        return ecp
-
-    @peers_public_key.setter
-    def peers_public_key(self, ECPoint ecp):
-        _exc.check_error(_ecp.mbedtls_ecp_copy(&self._ctx.Qp, &ecp._ctx))
-
-    @property
-    def shared_secret(self):
-        """The shared secret (int).
-
-        The shared secret is 0 if the TLS handshake is not finished.
-
-        """
-        try:
-            return _mpi.from_mpi_p(&self._ctx.z)
-        except ValueError:
-            return _mpi.MPI()
-
-    def generate_secret(self):
-        """Generate the shared secret."""
-        cdef _mpi.MPI mpi = _mpi.MPI()
-        cdef unsigned char* output = <unsigned char*>malloc(
-            _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
-        cdef size_t olen = 0
-        if not output:
-            raise MemoryError()
-        try:
-            _exc.check_error(_ecdh.mbedtls_ecdh_calc_secret(
-                &self._ctx, &olen, &output[0], _mpi.MBEDTLS_MPI_MAX_SIZE,
-                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
-            assert olen != 0
-            curve_type = _ecp.mbedtls_ecp_get_type(&self._ctx.grp)
-            if curve_type == _ecp.MBEDTLS_ECP_TYPE_MONTGOMERY:
-                _mpi.mbedtls_mpi_read_binary_le(&mpi._ctx, &output[0], olen)
-            else:
-                _mpi.mbedtls_mpi_read_binary(&mpi._ctx, &output[0], olen)
-            return mpi
-        finally:
-            free(output)
-
-    def generate_public_key(self):
-        """Generate public key from a private key."""
-        _exc.check_error(_ecp.mbedtls_ecp_mul(
-            &self._ctx.grp, &self._ctx.Q, &self._ctx.d, &self._ctx.grp.G,
-            &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
-
-
-cdef class ECDHServer(ECDHBase):
-
-    """The server side of the ECDH key exchange."""
-
-    def __init__(self, ecc: ECC):
-        super().__init__(ecc.curve)
-        if ecc.export_key():
-            _exc.check_error(_ecdh.mbedtls_ecdh_get_params(
-                &self._ctx, _pk.mbedtls_pk_ec(ecc._ctx), _ecdh.MBEDTLS_ECDH_OURS))
-
-    def generate(self):
-        """Generate a public key.
-
-        Return:
-            bytes: A TLS ServerKeyExchange payload.
-
-        """
-        cdef unsigned char* output = <unsigned char*>malloc(
-            _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
-        cdef size_t olen = 0
-        if not output:
-            raise MemoryError()
-        try:
-            _exc.check_error(_ecdh.mbedtls_ecdh_make_params(
-                &self._ctx, &olen, &output[0], _mpi.MBEDTLS_MPI_MAX_SIZE,
-                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
-            assert olen != 0
-            return output[:olen]
-        finally:
-            free(output)
-
-    def import_CKE(self, const unsigned char[:] buffer not None):
-        """Read the ClientKeyExchange payload."""
-        if buffer.size == 0:
-            buffer = b"\0"
-        _exc.check_error(_ecdh.mbedtls_ecdh_read_public(
-            &self._ctx, &buffer[0], buffer.size))
-
-
-cdef class ECDHClient(ECDHBase):
-
-    """The client side of the ephemeral ECDH key exchange."""
-
-    def __init__(self, ecc: ECC):
-        super().__init__(ecc.curve)
-        if ecc.export_key():
-            _exc.check_error(_ecdh.mbedtls_ecdh_get_params(
-                &self._ctx, _pk.mbedtls_pk_ec(ecc._ctx), _ecdh.MBEDTLS_ECDH_THEIRS))
-
-    def generate(self):
-        """Generate a public key.
-
-        Return:
-            bytes: A TLS ClientKeyExchange payload.
-
-        """
-        cdef unsigned char* output = <unsigned char*>malloc(
-            _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
-        cdef size_t olen = 0
-        if not output:
-            raise MemoryError()
-        try:
-            _exc.check_error(_ecdh.mbedtls_ecdh_make_public(
-                &self._ctx, &olen, &output[0], _mpi.MBEDTLS_MPI_MAX_SIZE,
-                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
-            assert olen != 0
-            return output[:olen]
-        finally:
-            free(output)
-
-    def import_SKE(self, const unsigned char[:] buffer not None):
-        """Read the ServerKeyExchange payload."""
-        if buffer.size == 0:
-            buffer = b"\0"
-        cdef const unsigned char* first = &buffer[0]
-        cdef const unsigned char* end = &buffer[-1] + 1
-        _exc.check_error(_ecdh.mbedtls_ecdh_read_params(
-            &self._ctx, &first, end))
-
-
-cdef class ECDHNaive(ECDHBase):
-
-    """Naive ECDH key exchange."""
-
-    def __init__(self, curve=None):
-        if curve is None:
-            curve = Curve.CURVE25519
-        curve = Curve(curve)
-        if curve not in {Curve.CURVE25519, Curve.CURVE448}:
-            raise ValueError("ECDHNaive only supports curve25519 and curve448")
-        super().__init__(curve)
-
-    def generate(self):
-        """Generate a public key.
-
-        Return:
-            ECPoint: public key.
-
-        """
-        _exc.check_error(_ecdh.mbedtls_ecdh_gen_public(
-            &self._ctx.grp, &self._ctx.d, &self._ctx.Q,
-            &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
-        return self.public_key
-
-    def import_peer_public(self, pubkey):
-        self.import_peers_public(pubkey.x)
-
-    def import_peers_public(self, _pk.ECPoint pubkey):
-        """Read peer public key."""
-        _exc.check_error(_ecp.mbedtls_ecp_copy(&self._ctx.Qp, &pubkey._ctx))
-
-    def generate_secret(self):
-        """Generate the shared secret."""
-        _exc.check_error(_ecdh.mbedtls_ecdh_compute_shared(
-            &self._ctx.grp, &self._ctx.z, &self._ctx.Qp, &self._ctx.d,
-            &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
-        return _mpi.from_mpi_p(&self._ctx.z)
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2016, Elaborated Networks GmbH
+# Copyright (c) 2018, Mathias Laurin
+
+"""Public key (PK) library.
+
+The library handles RSA certificates and ECC (elliptic curve
+cryptography).
+
+The RSA and ECC classes offer compatible APIs.  They may be used
+interchangeably.
+
+ECDHServer and ECDHClient should be used for ephemeral Elliptic Curve
+Diffie-Hellman exchange.
+
+"""
+
+
+from libc.stdlib cimport free, malloc
+from libc.string cimport memset
+
+cimport mbedtls._dhm as _dhm
+cimport mbedtls._ecdh as _ecdh
+cimport mbedtls._ecp as _ecp
+cimport mbedtls._random as _rnd
+cimport mbedtls._rsa as _rsa
+cimport mbedtls.mpi as _mpi
+cimport mbedtls.pk as _pk
+
+import enum
+import re
+from collections import namedtuple
+from functools import partial
+from pathlib import Path
+
+import mbedtls._random as _rnd
+import mbedtls.exceptions as _exc
+from mbedtls.hashlib import new as _new_hash
+
+__all__ = ("check_pair", "get_supported_ciphers", "get_supported_curves",
+           "Curve", "RSA", "ECC", "DHServer", "DHClient",
+           "ECDHServer", "ECDHClient", "ECDHNaive")
+
+
+CIPHER_NAME = (
+    b"NONE",
+    b"RSA",
+    b"EC",
+    b"EC_DH",
+    b"ECDSA",
+    # b"RSA_ALT",
+    # b"RSASSA_PSS",
+)
+
+
+class CipherType(enum.Enum):
+    NONE = _pk.MBEDTLS_PK_NONE
+    RSA = _pk.MBEDTLS_PK_RSA
+    ECKEY = _pk.MBEDTLS_PK_ECKEY
+    ECKEY_DH = _pk.MBEDTLS_PK_ECKEY_DH
+    ECDSA = _pk.MBEDTLS_PK_ECDSA
+    RSA_ALT = _pk.MBEDTLS_PK_RSA_ALT
+    RSASSA_PSS = _pk.MBEDTLS_PK_RSASSA_PSS
+
+
+KeyPair = namedtuple("KeyPair", ["private", "public"])
+
+
+class Curve(bytes, enum.Enum):
+
+    """Elliptic curves."""
+
+    SECP192R1 = b'secp192r1'
+    SECP224R1 = b'secp224r1'
+    SECP256R1 = b'secp256r1'
+    SECP384R1 = b'secp384r1'
+    SECP521R1 = b'secp521r1'
+    BRAINPOOLP256R1 = b'brainpoolP256r1'
+    BRAINPOOLP384R1 = b'brainpoolP384r1'
+    BRAINPOOLP512R1 = b'brainpoolP512r1'
+    SECP192K1 = b'secp192k1'
+    SECP224K1 = b'secp224k1'
+    SECP256K1 = b'secp256k1'
+    CURVE25519 = b'x25519'
+    CURVE448 = b'x448'
+
+
+# The following calculations come from mbedtls/library/pkwrite.c.
+RSA_PUB_DER_MAX_BYTES = 38 + 2 * _mpi.MBEDTLS_MPI_MAX_SIZE
+MPI_MAX_SIZE_2 = _mpi.MBEDTLS_MPI_MAX_SIZE // 2 + _mpi.MBEDTLS_MPI_MAX_SIZE % 2
+RSA_PRV_DER_MAX_BYTES = 47 + 3 * _mpi.MBEDTLS_MPI_MAX_SIZE + 5 * MPI_MAX_SIZE_2
+
+ECP_PUB_DER_MAX_BYTES = 30 + 2 * _ecp.MBEDTLS_ECP_MAX_BYTES
+ECP_PRV_DER_MAX_BYTES = 29 + 3 * _ecp.MBEDTLS_ECP_MAX_BYTES
+
+PUB_DER_MAX_BYTES = max(RSA_PUB_DER_MAX_BYTES, ECP_PUB_DER_MAX_BYTES)
+PRV_DER_MAX_BYTES = max(RSA_PRV_DER_MAX_BYTES, ECP_PRV_DER_MAX_BYTES)
+
+del RSA_PUB_DER_MAX_BYTES, MPI_MAX_SIZE_2, RSA_PRV_DER_MAX_BYTES
+del ECP_PUB_DER_MAX_BYTES, ECP_PRV_DER_MAX_BYTES
+
+
+cpdef check_pair(CipherBase pub, CipherBase pri):
+    """Check if a public-private pair of keys matches."""
+    return _pk.mbedtls_pk_check_pair(&pub._ctx, &pri._ctx) == 0
+
+
+def _type_from_name(name):
+    return {name: n for n, name in enumerate(CIPHER_NAME)}.get(name, 0)
+
+
+cpdef get_supported_ciphers():
+    return CIPHER_NAME
+
+
+def get_supported_curves():
+    """Return the list of supported curves in order of preference."""
+    cdef const _ecp.mbedtls_ecp_curve_info* info = _ecp.mbedtls_ecp_curve_list()
+    names, idx = [], 0
+    while info[idx].name != NULL:
+        names.append(Curve(bytes(info[idx].name)))
+        idx += 1
+    return names
+
+
+cdef curve_name_to_grp_id(curve):
+    cdef const _ecp.mbedtls_ecp_curve_info* info = _ecp.mbedtls_ecp_curve_list()
+    idx = 0
+    while info[idx].name != NULL:
+        if info[idx].name == curve:
+            return info[idx].grp_id
+        idx += 1
+    raise LookupError(curve.decode("ascii") + " not found")
+
+
+cdef _rnd.Random __rng = _rnd.default_rng()
+
+
+def _get_md_alg(digestmod):
+    """Return the hash object.
+
+    Arguments:
+        digestmod: The digest name or digest constructor for the
+            Cipher object to use.  It supports any name suitable to
+            `mbedtls.hash.new()`.
+
+    """
+    # `digestmod` handling below is adapted from CPython's
+    # `hmac.py`.
+    if callable(digestmod):
+        return digestmod
+    elif isinstance(digestmod, (str, unicode)):
+        return partial(_new_hash, digestmod)
+    else:
+        raise TypeError("a valid digestmod is required, got %r" % digestmod)
+
+
+cdef class CipherBase:
+    """Base class to RSA and ECC ciphers.
+
+    Parameters:
+        name (bytes): The cipher name known to mbed TLS.
+        key (bytes, optional): A key (public or private half).
+        password (bytes, optional): The password for the key.
+
+    """
+    def __init__(self,
+                 name,
+                 const unsigned char[:] key=None,
+                 const unsigned char[:] password=None):
+        _exc.check_error(_pk.mbedtls_pk_setup(
+            &self._ctx,
+            _pk.mbedtls_pk_info_from_type(
+                _type_from_name(name)
+            )
+        ))
+        if key is None or key.size == 0:
+            return
+        mbedtls_pk_free(&self._ctx)  # The context must be reset on entry.
+        try:
+            if password is None or password.size == 0:
+                _exc.check_error(_pk.mbedtls_pk_parse_key(
+                    &self._ctx, &key[0], key.size, NULL, 0
+                ))
+            else:
+                _exc.check_error(_pk.mbedtls_pk_parse_key(
+                    &self._ctx, &key[0], key.size, &password[0], password.size
+                ))
+        except _exc.TLSError:
+            _exc.check_error(_pk.mbedtls_pk_parse_public_key(
+                &self._ctx, &key[0], key.size))
+
+    def __cinit__(self):
+        """Initialize the context."""
+        _pk.mbedtls_pk_init(&self._ctx)
+
+    def __reduce__(self):
+        key = self.export_key()
+        if not key:
+            key = self.export_public_key()
+        return type(self).from_buffer, (key,)
+
+    def __dealloc__(self):
+        """Free and clear the context."""
+        _pk.mbedtls_pk_free(&self._ctx)
+
+    def __hash__(self):
+        if self._has_private():
+            return hash(self.export_key(format="DER"))
+        else:
+            return hash(self.export_public_key(format="DER"))
+
+    def __eq__(self, other):
+        if isinstance(other, str):
+            other = other.encode("ascii")
+        if isinstance(other, bytes):
+            try:
+                other = type(self).from_buffer(other)
+            except (_exc.TLSError, ValueError, TypeError):
+                return False
+        if type(other) is not type(self):
+            return False
+        if self._has_private() or other._has_private():
+            return other.export_key() == self.export_key()
+        elif not (self._has_private() and other._has_private()):
+            return other.export_public_key() == self.export_public_key()
+
+    @classmethod
+    def from_buffer(
+        cls,
+        const unsigned char[:] key not None,
+        password=None,
+    ):
+        """Import a key (public or private half).
+
+        The public half is generated upon importing a private key.
+
+        Arguments:
+            key (bytes): The key in PEM or DER format.
+            password (bytes, optional): The password for
+                password-protected private keys.
+
+        """
+        bkey = bytes(key)
+        if re.search(b"^-----BEGIN.+END.+-----\\s+$", bkey, re.DOTALL):
+            # PEM must be null-terminated.
+            bkey = bkey + b"\0"
+        if callable(password):
+            return cls(key=bkey, password=password())
+        return cls(key=bkey, password=password)
+
+    @classmethod
+    def from_file(cls, path, password=None):
+        return cls.from_buffer(Path(path).read_bytes(), password)
+
+    @classmethod
+    def from_DER(cls, const unsigned char[:] key not None):
+        return cls.from_buffer(key)
+
+    @classmethod
+    def from_PEM(cls, key):
+        """Import a key (public or private half)."""
+        return cls.from_buffer(key.encode("ascii"))
+
+    @property
+    def _type(self):
+        """Return the type of the cipher."""
+        return _pk.mbedtls_pk_get_type(&self._ctx)
+
+    @property
+    def name(self):
+        """Return the name of the cipher."""
+        return _pk.mbedtls_pk_get_name(&self._ctx)
+
+    @property
+    def _bitlen(self):
+        """Return the size of the key, in bits."""
+        return _pk.mbedtls_pk_get_bitlen(&self._ctx)
+
+    @property
+    def key_size(self):
+        """Return the size of the key, in bytes."""
+        return _pk.mbedtls_pk_get_len(&self._ctx)
+
+    def _has_private(self):
+        """Return `True` if the key contains a valid private half."""
+        raise NotImplementedError
+
+    def _has_public(self):
+        """Return `True` if the key contains a valid public half."""
+        raise NotImplementedError
+
+    def sign(self,
+             const unsigned char[:] message not None,
+             digestmod=None):
+        """Make signature, including padding if relevant.
+
+        Arguments:
+            message (bytes): The message to sign.
+            digestmod (optional): The digest name or digest constructor.
+
+        Return:
+            bytes or None: The signature or None if the cipher does not
+                contain a private key.
+
+        """
+        if digestmod is None:
+            digestmod = 'sha256'
+        if not self._has_private():
+            return None
+        md_alg = _get_md_alg(digestmod)(message)
+        cdef const unsigned char[:] hash_ = md_alg.digest()
+        cdef size_t sig_len = 0
+        cdef unsigned char* output = <unsigned char*>malloc(
+            _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
+        if not output:
+            raise MemoryError()
+        try:
+            _exc.check_error(_pk.mbedtls_pk_sign(
+                &self._ctx, md_alg._type,
+                &hash_[0], hash_.size,
+                &output[0], &sig_len,
+                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
+            assert sig_len != 0
+            return output[:sig_len]
+        finally:
+            free(output)
+
+    def verify(self,
+               const unsigned char[:] message not None,
+               const unsigned char[:] signature not None,
+               digestmod=None):
+        """Verify signature, including padding if relevant.
+
+        Arguments:
+            message (bytes): The message to sign.
+            signature (bytes): The signature to verify.
+            digestmod (optional): The digest name or digest constructor.
+
+        Return:
+            bool: True if the verification passed, False otherwise.
+
+        """
+        if signature.size == 0:
+            return False
+        if digestmod is None:
+            digestmod = 'sha256'
+        md_alg = _get_md_alg(digestmod)(message)
+        cdef const unsigned char[:] hash_ = md_alg.digest()
+        return _pk.mbedtls_pk_verify(
+            &self._ctx, md_alg._type,
+            &hash_[0], hash_.size,
+            &signature[0], signature.size) == 0
+
+    def encrypt(self, const unsigned char[:] message not None):
+        """Encrypt message (including padding if relevant).
+
+        Arguments:
+            message (bytes): Message to encrypt.
+
+        """
+        if message.size == 0:
+            message = b"\0"
+        cdef size_t olen = 0
+        cdef unsigned char* output = <unsigned char*>malloc(
+            _mpi.MBEDTLS_MPI_MAX_SIZE // 2 * sizeof(unsigned char))
+        if not output:
+            raise MemoryError()
+        try:
+            _exc.check_error(_pk.mbedtls_pk_encrypt(
+                &self._ctx, &message[0], message.size,
+                output, &olen, self.key_size,
+                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
+            return output[:olen]
+        finally:
+            free(output)
+
+    def decrypt(self, const unsigned char[:] message not None):
+        """Decrypt message (including padding if relevant).
+
+        Arguments:
+            message (bytes): Message to decrypt.
+
+        """
+        if message.size == 0:
+            message = b"\0"
+        cdef size_t olen = 0
+        cdef unsigned char* output = <unsigned char*>malloc(
+            _mpi.MBEDTLS_MPI_MAX_SIZE // 2 * sizeof(unsigned char))
+        if not output:
+            raise MemoryError()
+        try:
+            _exc.check_error(_pk.mbedtls_pk_decrypt(
+                &self._ctx, &message[0], message.size,
+                output, &olen, self.key_size,
+                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
+            return output[:olen]
+        finally:
+            free(output)
+
+    def generate(self):
+        """Generate a keypair.
+
+        Return:
+            (bytes): The private key in DER format.
+
+        """
+        raise NotImplementedError
+
+    def _private_to_DER(self):
+        if not self._has_private():
+            return b""
+        cdef int olen
+        cdef size_t osize = PRV_DER_MAX_BYTES
+        cdef unsigned char *output = <unsigned char *>malloc(
+            osize * sizeof(unsigned char))
+        if not output:
+            raise MemoryError()
+        try:
+            olen = _exc.check_error(
+                _pk.mbedtls_pk_write_key_der(&self._ctx, output, osize))
+            return output[osize - olen:osize]
+        finally:
+            free(output)
+
+    def _private_to_PEM(self):
+        if not self._has_private():
+            return ""
+        cdef size_t osize = PRV_DER_MAX_BYTES * 4 // 3 + 100
+        cdef unsigned char *output = <unsigned char *>malloc(
+            osize * sizeof(unsigned char))
+        if not output:
+            raise MemoryError()
+        memset(output, 0, osize)
+        try:
+            _exc.check_error(
+                _pk.mbedtls_pk_write_key_pem(&self._ctx, output, osize))
+            return output[0:osize].rstrip(b"\0").decode("ascii")
+        finally:
+            free(output)
+
+    def export_key(self, format="DER"):
+        """Return the private key.
+
+        If no key is present, return a falsy value.
+
+        Args:
+            format (str): One of "DER" or "PEM".
+
+        """
+        if format == "DER":
+            return self._private_to_DER()
+        if format == "PEM":
+            return self._private_to_PEM()
+        raise ValueError(format)
+
+    def _public_to_DER(self):
+        if not self._has_public():
+            return b""
+        cdef int olen
+        cdef size_t osize = PRV_DER_MAX_BYTES
+        cdef unsigned char *output = <unsigned char *>malloc(
+            osize * sizeof(unsigned char))
+        if not output:
+            raise MemoryError()
+        try:
+            olen = _exc.check_error(
+                _pk.mbedtls_pk_write_pubkey_der(&self._ctx, output, osize))
+            return output[osize - olen:osize]
+        finally:
+            free(output)
+
+    def _public_to_PEM(self):
+        if not self._has_public():
+            return ""
+        cdef size_t osize = PRV_DER_MAX_BYTES * 4 // 3 + 100
+        cdef unsigned char *output = <unsigned char *>malloc(
+            osize * sizeof(unsigned char))
+        if not output:
+            raise MemoryError()
+        memset(output, 0, osize)
+        try:
+            _exc.check_error(
+                _pk.mbedtls_pk_write_pubkey_pem(&self._ctx, output, osize))
+            return output[0:osize].rstrip(b"\0").decode("ascii")
+        finally:
+            free(output)
+
+    def export_public_key(self, format="DER"):
+        """Return the public key.
+
+        If no key is present, return a falsy value.
+
+        Args:
+            format (str): One of "DER" or "PEM".
+
+        """
+        if format == "DER":
+            return self._public_to_DER()
+        if format == "PEM":
+            return self._public_to_PEM()
+        raise ValueError(format)
+
+    def to_PEM(self):
+        """Return the RSA in PEM format.
+
+        Warning:
+            This function is obsolete.
+
+        Return:
+            tuple(str, str): The private key and the public key.
+
+        See Also:
+            export_key(), export_public_key()
+
+        """
+        return KeyPair(self.export_key("PEM"), self.export_public_key("PEM"))
+
+    def __str__(self):
+        return self.export_key(format="PEM")
+
+    def to_DER(self):
+        """Return the RSA in DER format.
+
+        Warning:
+            This function is obsolete.
+
+        Return:
+            tuple(bytes, bytes): The private key and the public key.
+
+        See Also:
+            export_key(), export_public_key()
+
+        """
+        return KeyPair(self.export_key("DER"), self.export_public_key("DER"))
+
+    def to_bytes(self):
+        """Return the private key in DER format."""
+        return self.export_key(format="DER")
+
+    def __bytes__(self):
+        return self.to_bytes()
+
+
+cdef class RSA(CipherBase):
+
+    """RSA public-key cryptosystem."""
+
+    def __init__(self,
+                 const unsigned char[:] key=None,
+                 const unsigned char[:] password=None):
+        super().__init__(b"RSA", key, password)
+
+    def _has_private(self):
+        """Return `True` if the key contains a valid private half."""
+        return _rsa.mbedtls_rsa_check_privkey(
+            _pk.mbedtls_pk_rsa(self._ctx)
+        ) == 0
+
+    def _has_public(self):
+        """Return `True` if the key contains a valid public half."""
+        return _rsa.mbedtls_rsa_check_pubkey(_pk.mbedtls_pk_rsa(self._ctx)) == 0
+
+    def generate(self, unsigned int key_size=2048, int exponent=65537):
+        """Generate an RSA keypair.
+
+        Arguments:
+            key_size (unsigned int): size in bits.
+            exponent (int): public RSA exponent.
+
+        Return:
+            (bytes): The private key in DER format.
+
+        """
+        _exc.check_error(_rsa.mbedtls_rsa_gen_key(
+            _pk.mbedtls_pk_rsa(self._ctx), &_rnd.mbedtls_ctr_drbg_random,
+            &__rng._ctx, key_size, exponent))
+        return self.export_key("DER")
+
+
+cdef class ECPoint:
+
+    """A point on the elliptic curve."""
+    def __init__(self, x, y, z):
+        cdef _mpi.MPI _x = _mpi.MPI(x)
+        cdef _mpi.MPI _y = _mpi.MPI(y)
+        cdef _mpi.MPI _z = _mpi.MPI(z)
+        _mpi.mbedtls_mpi_copy(&self._ctx.X, &_x._ctx)
+        _mpi.mbedtls_mpi_copy(&self._ctx.Y, &_y._ctx)
+        _mpi.mbedtls_mpi_copy(&self._ctx.Z, &_z._ctx)
+
+    def __cinit__(self):
+        """Initialize the context."""
+        _ecp.mbedtls_ecp_point_init(&self._ctx)
+
+    def __dealloc__(self):
+        """Free and clear the context."""
+        _ecp.mbedtls_ecp_point_free(&self._ctx)
+
+    def __reduce__(self):
+        return type(self), (self.x, self.y, self.z)
+
+    @property
+    def x(self):
+        """Return the X coordinate."""
+        try:
+            return _mpi.from_mpi_p(&self._ctx.X)
+        except ValueError:
+            return _mpi.MPI()
+
+    @property
+    def y(self):
+        """Return the Y coordinate."""
+        try:
+            return _mpi.from_mpi_p(&self._ctx.Y)
+        except ValueError:
+            return _mpi.MPI()
+
+    @property
+    def z(self):
+        """Return the Z coordinate."""
+        try:
+            return _mpi.from_mpi_p(&self._ctx.Z)
+        except ValueError:
+            return _mpi.MPI()
+
+    def __str__(self):
+        return "%s(%i, %i, %i)" % (
+            type(self).__name__, self.x, self.y, self.z
+        )
+
+    def __repr__(self):
+        return "%s(%r, %r, %r)" % (
+            type(self).__name__, self.x, self.y, self.z
+        )
+
+    def __eq__(self, other):
+        if other == 0:
+            return _ecp.mbedtls_ecp_is_zero(&self._ctx) == 1
+        elif type(other) is type(self):
+            c_other = <ECPoint> other
+            return _ecp.mbedtls_ecp_point_cmp(&self._ctx, &c_other._ctx) == 0
+        return NotImplemented
+
+    def __hash__(self):
+        return hash((self.x, self.y, self.z))
+
+    def __bool__(self):
+        return _ecp.mbedtls_ecp_is_zero(&self._ctx) == 0
+
+
+cdef class ECC(CipherBase):
+
+    """Elliptic-curve cryptosystems.
+
+    Args:
+        (Curve, optional): A curve returned by `get_supported_curves()`.
+
+    See Also:
+        get_supported_curves()
+
+    """
+    def __init__(self,
+                 curve=None,
+                 const unsigned char[:] key=None,
+                 const unsigned char[:] password=None):
+        super().__init__(b"EC", key, password)
+        if curve is None:
+            curve = get_supported_curves()[0]
+        self._curve = curve
+
+    @property
+    def curve(self):
+        return self._curve
+
+    def _has_private(self):
+        """Return `True` if the key contains a valid private half."""
+        cdef const _ecp.mbedtls_ecp_keypair* ecp = _pk.mbedtls_pk_ec(self._ctx)
+        return _mpi.mbedtls_mpi_cmp_mpi(&ecp.d, &_mpi.MPI()._ctx) != 0
+
+    def _has_public(self):
+        """Return `True` if the key contains a valid public half."""
+        cdef _ecp.mbedtls_ecp_keypair* ecp = _pk.mbedtls_pk_ec(self._ctx)
+        return not _ecp.mbedtls_ecp_is_zero(&ecp.Q)
+
+    def sign(self,
+             const unsigned char[:] message not None,
+             digestmod=None):
+        if self._curve in (Curve.CURVE25519, Curve.CURVE448):
+            raise ValueError("ECDSA does not support Curve25519 or Curve448.")
+        return super().sign(message, digestmod)
+
+    def generate(self):
+        """Generate an EC keypair.
+
+        Return:
+            (bytes): The private key in DER format.
+
+        """
+        grp_id = curve_name_to_grp_id(self.curve)
+        if grp_id is None:
+            raise ValueError(self.curve)
+        _exc.check_error(_ecp.mbedtls_ecp_gen_key(
+            grp_id, _pk.mbedtls_pk_ec(self._ctx),
+            &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
+        format = (
+            "NUM"
+            if self.curve in (Curve.CURVE25519, Curve.CURVE448)
+            else "DER"
+        )
+        return self.export_key(format)
+
+    def _private_to_num(self):
+        try:
+            return _mpi.from_mpi_p(&_pk.mbedtls_pk_ec(self._ctx).d)
+        except ValueError:
+            return _mpi.MPI()
+
+    def export_key(self, format=None):
+        """Return the private key.
+
+        If not key is present, return a falsy value.
+
+        Args:
+            format (str): One of "DER", "PEM", or "NUM".
+
+        """
+        if format is None:
+            format = (
+                "NUM"
+                if self.curve in (Curve.CURVE25519, Curve.CURVE448)
+                else "DER"
+            )
+        if format == "NUM":
+            return self._private_to_num()
+        elif self.curve in (Curve.CURVE25519, Curve.CURVE448):
+            raise ValueError(
+                "Curve25519 and Curve448 only support export as NUM"
+            )
+        return super().export_key(format)
+
+    def _public_to_point(self):
+        point = ECPoint(0, 0, 0)
+        _ecp.mbedtls_ecp_copy(&point._ctx, &_pk.mbedtls_pk_ec(self._ctx).Q)
+        return point
+
+    def export_public_key(self, format="DER"):
+        """Return the public key.
+
+        If no key is present, return a falsy value.
+
+        Args:
+            format (str): One of "DER", "PEM", or "POINT".
+
+        """
+        if format == "POINT":
+            return self._public_to_point()
+        elif self.curve in (Curve.CURVE25519, Curve.CURVE448):
+            raise ValueError(
+                "Curve25519 and Curve448 only support export as NUM"
+            )
+        return super().export_public_key(format)
+
+
+cdef class DHBase:
+
+    """Base class to DH key exchange: client and server.
+
+    Args:
+        modulus (int): The prime modulus P.
+        generator (int): The generator G, a primitive root modulo P.
+
+    See Also:
+        DHServer, DHClient: The derived classes.
+
+    """
+    def __init__(self, modulus, generator):
+        super().__init__()
+        _exc.check_error(_mpi.mbedtls_mpi_copy(
+            &self._ctx.P, &_mpi.MPI(modulus)._ctx))
+        _exc.check_error(_mpi.mbedtls_mpi_copy(
+            &self._ctx.G, &_mpi.MPI(generator)._ctx))
+
+    def __cinit__(self):
+        """Initialize the context."""
+        _dhm.mbedtls_dhm_init(&self._ctx)
+
+    def __dealloc__(self):
+        """Free and clear the context."""
+        _dhm.mbedtls_dhm_free(&self._ctx)
+
+    def __getstate__(self):
+        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
+
+    @property
+    def key_size(self):
+        """Return the size of the key, in bytes."""
+        return _mpi.mbedtls_mpi_size(&self._ctx.P)
+
+    @property
+    def modulus(self):
+        """Return the prime modulus, P."""
+        return _mpi.from_mpi_p(&self._ctx.P)
+
+    @property
+    def generator(self):
+        """Return the generator, G."""
+        return _mpi.from_mpi_p(&self._ctx.G)
+
+    @property
+    def _secret(self):
+        """Return the secret (int)."""
+        return _mpi.from_mpi_p(&self._ctx.X)
+
+    @property
+    def shared_secret(self):
+        """The shared secret (int).
+
+        The shared secret is 0 if the TLS handshake is not finished.
+
+        """
+        try:
+            return _mpi.from_mpi_p(&self._ctx.K)
+        except ValueError:
+            return _mpi.MPI()
+
+    def generate_secret(self):
+        """Generate the shared secret."""
+        cdef _mpi.MPI mpi
+        cdef unsigned char* output = <unsigned char*>malloc(
+            _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
+        cdef size_t olen = 0
+        if not output:
+            raise MemoryError()
+        try:
+            _exc.check_error(_dhm.mbedtls_dhm_calc_secret(
+                &self._ctx, &output[0], _mpi.MBEDTLS_MPI_MAX_SIZE, &olen,
+                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
+            mpi = _mpi.MPI()
+            _mpi.mbedtls_mpi_read_binary(&mpi._ctx, &output[0], olen)
+            return mpi
+        finally:
+            free(output)
+
+
+cdef class DHServer(DHBase):
+
+    """The server side of the DH key exchange."""
+
+    def generate(self):
+        """Generate a public key.
+
+        Return:
+            bytes: A TLS ServerKeyExchange payload.
+
+        """
+        cdef unsigned char* output = <unsigned char*>malloc(
+            _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
+        cdef size_t olen = 0
+        if not output:
+            raise MemoryError()
+        try:
+            _exc.check_error(_dhm.mbedtls_dhm_make_params(
+                &self._ctx, self.key_size, &output[0], &olen,
+                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
+            assert olen != 0
+            return output[:olen]
+        finally:
+            free(output)
+
+    def import_CKE(self, const unsigned char[:] buffer not None):
+        """Read the ClientKeyExchange payload."""
+        if buffer.size == 0:
+            buffer = b"\0"
+        _exc.check_error(_dhm.mbedtls_dhm_read_public(
+            &self._ctx, &buffer[0], buffer.size))
+
+
+cdef class DHClient(DHBase):
+
+    """The client side of the DH key exchange."""
+
+    def generate(self):
+        """Generate the public key.
+
+        Return:
+            bytes: The byte representation (big endian) of: G^X mod P.
+
+        """
+        cdef _mpi.MPI mpi
+        cdef unsigned char* output = <unsigned char*>malloc(
+            _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
+        if not output:
+            raise MemoryError()
+        try:
+            _exc.check_error(_dhm.mbedtls_dhm_make_public(
+                &self._ctx, self.key_size, &output[0], self.key_size,
+                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
+            mpi = _mpi.from_mpi_p(&self._ctx.GX)
+            return mpi.to_bytes(
+                _mpi.mbedtls_mpi_size(&mpi._ctx), "big")
+        finally:
+            free(output)
+
+    def import_SKE(self, const unsigned char[:] buffer not None):
+        """Read the ServerKeyExchange payload."""
+        if buffer.size == 0:
+            raise ValueError("SKE is empty")
+        # Const away cast is safe because the pointer is used as
+        # a read-only index in `dhm_read_bignum()`.
+        cdef unsigned char* first = <unsigned char*> &buffer[0]
+        cdef const unsigned char* end = &buffer[-1] + 1
+        _exc.check_error(_dhm.mbedtls_dhm_read_params(&self._ctx, &first, end))
+
+
+cdef class ECDHBase:
+
+    """Base class to ECDH(E) key exchange: client and server.
+
+    Args:
+        (Curve, optional): A curve returned by `get_supported_curves()`.
+
+    See Also:
+        ECDHServer, ECDHClient: The derived class.
+        get_supported_curves()
+
+    """
+    def __init__(self, curve=None):
+        super().__init__()
+        if curve is None:
+            curve = get_supported_curves()[0]
+        self.curve = Curve(curve)
+        _exc.check_error(_ecp.mbedtls_ecp_group_load(
+            &self._ctx.grp, curve_name_to_grp_id(self.curve)))
+
+    def __cinit__(self):
+        """Initialize the context."""
+        _ecdh.mbedtls_ecdh_init(&self._ctx)
+
+    def __dealloc__(self):
+        """Free and clear the context."""
+        _ecdh.mbedtls_ecdh_free(&self._ctx)
+
+    def __getstate__(self):
+        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
+
+    def _has_private(self):
+        """Return `True` if the key contains a valid private half."""
+        return _mpi.mbedtls_mpi_cmp_mpi(&self._ctx.d, &_mpi.MPI()._ctx) != 0
+
+    def _has_public(self):
+        """Return `True` if the key contains a valid public half."""
+        return not _ecp.mbedtls_ecp_is_zero(&self._ctx.Q)
+
+    def _has_peers_public(self):
+        """Return `True` if the peer's key is present."""
+        return not _ecp.mbedtls_ecp_is_zero(&self._ctx.Qp)
+
+    @property
+    def public_key(self):
+        """The public key (ECPoint)"""
+        ecp = ECPoint(0, 0, 0)
+        _exc.check_error(_ecp.mbedtls_ecp_copy(&ecp._ctx, &self._ctx.Q))
+        return ecp
+
+    @public_key.setter
+    def public_key(self, ECPoint ecp):
+        _exc.check_error(_ecp.mbedtls_ecp_copy(&self._ctx.Q, &ecp._ctx))
+
+    @property
+    def private_key(self):
+        """The private key (int)"""
+        return _mpi.from_mpi_p(&self._ctx.d)
+
+    @private_key.setter
+    def private_key(self, priv):
+        cdef _mpi.MPI c_priv = _mpi.MPI(priv)
+        _mpi.mbedtls_mpi_copy(&self._ctx.d, &c_priv._ctx)
+
+    @property
+    def peers_public_key(self):
+        """Peer's public key (ECPoint)"""
+        ecp = ECPoint(0, 0, 0)
+        _exc.check_error(_ecp.mbedtls_ecp_copy(&ecp._ctx, &self._ctx.Qp))
+        return ecp
+
+    @peers_public_key.setter
+    def peers_public_key(self, ECPoint ecp):
+        _exc.check_error(_ecp.mbedtls_ecp_copy(&self._ctx.Qp, &ecp._ctx))
+
+    @property
+    def shared_secret(self):
+        """The shared secret (int).
+
+        The shared secret is 0 if the TLS handshake is not finished.
+
+        """
+        try:
+            return _mpi.from_mpi_p(&self._ctx.z)
+        except ValueError:
+            return _mpi.MPI()
+
+    def generate_secret(self):
+        """Generate the shared secret."""
+        cdef _mpi.MPI mpi = _mpi.MPI()
+        cdef unsigned char* output = <unsigned char*>malloc(
+            _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
+        cdef size_t olen = 0
+        if not output:
+            raise MemoryError()
+        try:
+            _exc.check_error(_ecdh.mbedtls_ecdh_calc_secret(
+                &self._ctx, &olen, &output[0], _mpi.MBEDTLS_MPI_MAX_SIZE,
+                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
+            assert olen != 0
+            curve_type = _ecp.mbedtls_ecp_get_type(&self._ctx.grp)
+            if curve_type == _ecp.MBEDTLS_ECP_TYPE_MONTGOMERY:
+                _mpi.mbedtls_mpi_read_binary_le(&mpi._ctx, &output[0], olen)
+            else:
+                _mpi.mbedtls_mpi_read_binary(&mpi._ctx, &output[0], olen)
+            return mpi
+        finally:
+            free(output)
+
+    def generate_public_key(self):
+        """Generate public key from a private key."""
+        _exc.check_error(_ecp.mbedtls_ecp_mul(
+            &self._ctx.grp, &self._ctx.Q, &self._ctx.d, &self._ctx.grp.G,
+            &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
+
+
+cdef class ECDHServer(ECDHBase):
+
+    """The server side of the ECDH key exchange."""
+
+    def __init__(self, ecc: ECC):
+        super().__init__(ecc.curve)
+        if ecc.export_key():
+            _exc.check_error(_ecdh.mbedtls_ecdh_get_params(
+                &self._ctx, _pk.mbedtls_pk_ec(ecc._ctx), _ecdh.MBEDTLS_ECDH_OURS))
+
+    def generate(self):
+        """Generate a public key.
+
+        Return:
+            bytes: A TLS ServerKeyExchange payload.
+
+        """
+        cdef unsigned char* output = <unsigned char*>malloc(
+            _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
+        cdef size_t olen = 0
+        if not output:
+            raise MemoryError()
+        try:
+            _exc.check_error(_ecdh.mbedtls_ecdh_make_params(
+                &self._ctx, &olen, &output[0], _mpi.MBEDTLS_MPI_MAX_SIZE,
+                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
+            assert olen != 0
+            return output[:olen]
+        finally:
+            free(output)
+
+    def import_CKE(self, const unsigned char[:] buffer not None):
+        """Read the ClientKeyExchange payload."""
+        if buffer.size == 0:
+            buffer = b"\0"
+        _exc.check_error(_ecdh.mbedtls_ecdh_read_public(
+            &self._ctx, &buffer[0], buffer.size))
+
+
+cdef class ECDHClient(ECDHBase):
+
+    """The client side of the ephemeral ECDH key exchange."""
+
+    def __init__(self, ecc: ECC):
+        super().__init__(ecc.curve)
+        if ecc.export_key():
+            _exc.check_error(_ecdh.mbedtls_ecdh_get_params(
+                &self._ctx, _pk.mbedtls_pk_ec(ecc._ctx), _ecdh.MBEDTLS_ECDH_THEIRS))
+
+    def generate(self):
+        """Generate a public key.
+
+        Return:
+            bytes: A TLS ClientKeyExchange payload.
+
+        """
+        cdef unsigned char* output = <unsigned char*>malloc(
+            _mpi.MBEDTLS_MPI_MAX_SIZE * sizeof(unsigned char))
+        cdef size_t olen = 0
+        if not output:
+            raise MemoryError()
+        try:
+            _exc.check_error(_ecdh.mbedtls_ecdh_make_public(
+                &self._ctx, &olen, &output[0], _mpi.MBEDTLS_MPI_MAX_SIZE,
+                &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
+            assert olen != 0
+            return output[:olen]
+        finally:
+            free(output)
+
+    def import_SKE(self, const unsigned char[:] buffer not None):
+        """Read the ServerKeyExchange payload."""
+        if buffer.size == 0:
+            buffer = b"\0"
+        cdef const unsigned char* first = &buffer[0]
+        cdef const unsigned char* end = &buffer[-1] + 1
+        _exc.check_error(_ecdh.mbedtls_ecdh_read_params(
+            &self._ctx, &first, end))
+
+
+cdef class ECDHNaive(ECDHBase):
+
+    """Naive ECDH key exchange."""
+
+    def __init__(self, curve=None):
+        if curve is None:
+            curve = Curve.CURVE25519
+        curve = Curve(curve)
+        if curve not in {Curve.CURVE25519, Curve.CURVE448}:
+            raise ValueError("ECDHNaive only supports curve25519 and curve448")
+        super().__init__(curve)
+
+    def generate(self):
+        """Generate a public key.
+
+        Return:
+            ECPoint: public key.
+
+        """
+        _exc.check_error(_ecdh.mbedtls_ecdh_gen_public(
+            &self._ctx.grp, &self._ctx.d, &self._ctx.Q,
+            &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
+        return self.public_key
+
+    def import_peer_public(self, pubkey):
+        self.import_peers_public(pubkey.x)
+
+    def import_peers_public(self, _pk.ECPoint pubkey):
+        """Read peer public key."""
+        _exc.check_error(_ecp.mbedtls_ecp_copy(&self._ctx.Qp, &pubkey._ctx))
+
+    def generate_secret(self):
+        """Generate the shared secret."""
+        _exc.check_error(_ecdh.mbedtls_ecdh_compute_shared(
+            &self._ctx.grp, &self._ctx.z, &self._ctx.Qp, &self._ctx.d,
+            &_rnd.mbedtls_ctr_drbg_random, &__rng._ctx))
+        return _mpi.from_mpi_p(&self._ctx.z)
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/secrets.py` & `python-mbedtls-2.7.1/src/mbedtls/secrets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,61 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2019, Mathias Laurin
-
-"""Generate secure random numbers.
-
-This is an implementation of the PEP 506 API based on a
-CSPRNG (Cryptographically Strong Pseudo Random Number Generator).
-
-This module is compatibale with the standard `secrets` (PEP 506) module.
-
-"""
-
-from __future__ import annotations
-
-import base64 as _base64
-import binascii as _binascii
-import sys
-from typing import Callable, Sequence, TypeVar, cast
-
-import mbedtls._random as _rnd  # pylint: disable=no-name-in-module
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Final
-else:
-    from typing import Final
-
-
-__all__ = [
-    "randbits",
-    "choice",
-    "randbelow",
-    "token_bytes",
-    "token_hex",
-    "token_urlsafe",
-]
-
-
-DEFAULT_ENTROPY: Final = 32
-
-
-__rng = _rnd.default_rng()
-
-
-randbits: Callable[[int], int] = __rng.getrandbits
-
-T_co = TypeVar("T_co", covariant=True)
-choice: Callable[[Sequence[T_co]], T_co] = __rng.choice
-randbelow: Callable[[int], int] = __rng.randbelow
-
-
-def token_bytes(nbytes: int = DEFAULT_ENTROPY) -> bytes:
-    """Return a random byte string containing `nbytes` number of bytes.
-
-    If `nbytes` is ``None`` or not supplied, a reasonable default is used.
-
-    """
-    return cast(bytes, __rng.urandom(nbytes))
-
-
-def token_hex(nbytes: int = DEFAULT_ENTROPY) -> str:
-    """Return a random text string, in hexadecimal."""
-    return _binascii.hexlify(token_bytes(nbytes)).decode("ascii")
-
-
-def token_urlsafe(nbytes: int = DEFAULT_ENTROPY) -> str:
-    """Return a random URL-safe string."""
-    tok = token_bytes(nbytes)
-    return _base64.urlsafe_b64encode(tok).rstrip(b"=").decode("ascii")
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2019, Mathias Laurin
+
+"""Generate secure random numbers.
+
+This is an implementation of the PEP 506 API based on a
+CSPRNG (Cryptographically Strong Pseudo Random Number Generator).
+
+This module is compatibale with the standard `secrets` (PEP 506) module.
+
+"""
+
+from __future__ import annotations
+
+import base64 as _base64
+import binascii as _binascii
+from typing import Callable, Final, Sequence, TypeVar, cast
+
+import mbedtls._random as _rnd  # pylint: disable=no-name-in-module
+
+__all__ = [
+    "randbits",
+    "choice",
+    "randbelow",
+    "token_bytes",
+    "token_hex",
+    "token_urlsafe",
+]
+
+
+DEFAULT_ENTROPY: Final = 32
+
+
+__rng = _rnd.default_rng()
+
+
+randbits: Callable[[int], int] = __rng.getrandbits
+
+T_co = TypeVar("T_co", covariant=True)
+choice: Callable[[Sequence[T_co]], T_co] = __rng.choice
+randbelow: Callable[[int], int] = __rng.randbelow
+
+
+def token_bytes(nbytes: int = DEFAULT_ENTROPY) -> bytes:
+    """Return a random byte string containing `nbytes` number of bytes.
+
+    If `nbytes` is ``None`` or not supplied, a reasonable default is used.
+
+    """
+    return cast(bytes, __rng.urandom(nbytes))
+
+
+def token_hex(nbytes: int = DEFAULT_ENTROPY) -> str:
+    """Return a random text string, in hexadecimal."""
+    return _binascii.hexlify(token_bytes(nbytes)).decode("ascii")
+
+
+def token_urlsafe(nbytes: int = DEFAULT_ENTROPY) -> str:
+    """Return a random URL-safe string."""
+    tok = token_bytes(nbytes)
+    return _base64.urlsafe_b64encode(tok).rstrip(b"=").decode("ascii")
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/tls.py` & `python-mbedtls-2.7.1/src/mbedtls/tls.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,461 +1,463 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2018, Mathias Laurin
-
-from __future__ import annotations
-
-import enum
-import errno
-import os
-import socket as _pysocket
-import struct
-import sys
-from typing import Any, NoReturn, Optional, Tuple, Union, cast, overload
-
-from ._tls import HandshakeStep as HandshakeStep
-from ._tls import HelloVerifyRequest
-from ._tls import MbedTLSBuffer as TLSWrappedBuffer
-from ._tls import (
-    Purpose,
-    RaggedEOF,
-    TLSSession,
-    TrustStore,
-    WantReadError,
-    WantWriteError,
-    _BaseContext,
-    _tls_from_version,
-    _tls_to_version,
-    ciphers_available,
-)
-from ._tlsi import DTLSConfiguration as DTLSConfiguration
-from ._tlsi import DTLSVersion as DTLSVersion
-from ._tlsi import MaxFragmentLength as MaxFragmentLength
-from ._tlsi import NextProtocol as NextProtocol
-from ._tlsi import PrivateKey as PrivateKey
-from ._tlsi import ServerNameCallback as ServerNameCallback
-from ._tlsi import TLSConfiguration as TLSConfiguration
-from ._tlsi import TLSVersion as TLSVersion
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Final
-else:
-    from typing import Final
-
-if sys.version_info < (3, 10):
-    from typing_extensions import TypeAlias
-else:
-    from typing import TypeAlias
-
-
-__all__ = (
-    "ClientContext",
-    "DTLSConfiguration",
-    "DTLSVersion",
-    "HelloVerifyRequest",
-    "MaxFragmentLength",
-    "NextProtocol",
-    "PrivateKey",
-    "Purpose",
-    "RaggedEOF",
-    "ServerContext",
-    "ServerNameCallback",
-    "TLSConfiguration",
-    "TLSRecordHeader",
-    "TLSSession",
-    "TLSVersion",
-    "TLSWrappedBuffer",
-    "TLSWrappedSocket",
-    "TrustStore",
-    "WantReadError",
-    "WantWriteError",
-    "ciphers_available",
-)
-
-# `_Address` stolen from `_socket.pyi`.
-_Address: TypeAlias = Union[Tuple[Any, ...], str]
-_WriteableBuffer: TypeAlias = Union[memoryview, bytearray]
-
-
-class TLSRecordHeader:
-    """Encode/decode TLS record protocol format."""
-
-    __slots__ = ("record_type", "version", "length")
-    fmt = "!BHH"
-
-    class RecordType(enum.IntEnum):
-        CHANGE_CIPHER_SPEC = 0x14
-        ALERT = 0x15
-        HANDSHAKE = 0x16
-        APPLICATION_DATA = 0x17
-
-    def __init__(
-        self,
-        record_type: Union[int, TLSRecordHeader.RecordType],
-        version: Union[int, Tuple[int, int], TLSVersion],
-        length: int,
-    ) -> None:
-        def parse_version(
-            v: Union[int, Tuple[int, int], TLSVersion]
-        ) -> TLSVersion:
-            if isinstance(v, TLSVersion):
-                return v
-            if isinstance(v, int):
-                return TLSVersion(v)
-            return TLSVersion(((v[0] & 0xFF) << 8) + v[1] & 0xFF)
-
-        self.record_type: Final = TLSRecordHeader.RecordType(record_type)
-        self.version: Final = parse_version(version)
-        self.length: Final = length
-
-    def __str__(self) -> str:
-        return "{}({}, {}, {})".format(
-            type(self).__name__,
-            self.record_type,
-            self.version,
-            self.length,
-        )
-
-    def __repr__(self) -> str:
-        return "{}({!r}, {!r}, {!r})".format(
-            type(self).__name__,
-            self.record_type,
-            self.version,
-            self.length,
-        )
-
-    def __eq__(self, other: object) -> bool:
-        if not isinstance(other, TLSRecordHeader):
-            return NotImplemented
-        return (
-            self.record_type is other.record_type
-            and self.version is other.version
-            and self.length == other.length
-        )
-
-    def __hash__(self) -> int:
-        return 0x5AFE ^ self.record_type ^ self.version.value ^ self.length
-
-    def __len__(self) -> int:
-        return 5
-
-    def __bytes__(self) -> bytes:
-        maj, min_ = _tls_from_version(self.version)
-        version = ((maj & 0xFF) << 8) + (min_ & 0xFF)
-        return struct.pack(
-            TLSRecordHeader.fmt,
-            self.record_type,
-            version,
-            self.length,
-        )
-
-    @classmethod
-    def from_bytes(cls, header: bytes) -> TLSRecordHeader:
-        record_type, maj_min_version, length = struct.unpack(
-            TLSRecordHeader.fmt, header[:5]
-        )
-        maj, min_ = (maj_min_version >> 8) & 0xFF, maj_min_version & 0xFF
-        return cls(
-            TLSRecordHeader.RecordType(record_type),
-            _tls_to_version((maj, min_)),
-            length,
-        )
-
-
-class ClientContext(_BaseContext):
-    # _pep543.ClientContext
-
-    @property
-    def _purpose(self) -> Purpose:
-        return Purpose.CLIENT_AUTH
-
-    def wrap_socket(
-        self, socket: _pysocket.socket, server_hostname: Optional[str]
-    ) -> TLSWrappedSocket:
-        """Wrap an existing Python socket object ``socket`` and return a
-        ``TLSWrappedSocket`` object. ``socket`` must be a ``SOCK_STREAM``
-        socket: all other socket types are unsupported.
-
-        Args:
-            socket: The socket to wrap.
-            server_hostname: The hostname of the service
-                which we are connecting to.  Pass ``None`` if hostname
-                validation is not desired.  This parameter has no
-                default value because opting-out hostname validation is
-                dangerous and should not be the default behavior.
-
-        """
-        buffer = self.wrap_buffers(server_hostname)
-        return TLSWrappedSocket(socket, buffer)
-
-    def wrap_buffers(self, server_hostname: Optional[str]) -> TLSWrappedBuffer:
-        """Create an in-memory stream for TLS."""
-        # PEP 543
-        return TLSWrappedBuffer(self, server_hostname)
-
-
-class ServerContext(_BaseContext):
-    # _pep543.ServerContext
-
-    @property
-    def _purpose(self) -> Purpose:
-        return Purpose.SERVER_AUTH
-
-    def wrap_socket(self, socket: _pysocket.socket) -> TLSWrappedSocket:
-        """Wrap an existing Python socket object ``socket``."""
-        buffer = self.wrap_buffers()
-        return TLSWrappedSocket(socket, buffer)
-
-    def wrap_buffers(self) -> TLSWrappedBuffer:
-        # PEP 543
-        return TLSWrappedBuffer(self)
-
-
-class TLSWrappedSocket:
-    # pylint: disable=too-many-instance-attributes
-    # _pep543.TLSWrappedSocket
-    def __init__(
-        self, socket: _pysocket.socket, buffer: TLSWrappedBuffer
-    ) -> None:
-        super().__init__()
-        self._socket = socket
-        self._buffer = buffer
-        self._context = buffer.context
-        self._closed = False
-
-    @property
-    def context(self) -> _BaseContext:
-        return self._buffer.context
-
-    @property
-    def _buffer(self) -> TLSWrappedBuffer:
-        return cast(TLSWrappedBuffer, self.__dict__["_buffer"])
-
-    @_buffer.setter
-    def _buffer(self, __buffer: TLSWrappedBuffer) -> None:
-        self.__dict__["_buffer"] = __buffer
-        self.setcookieparam = __buffer.setcookieparam
-        self.cipher = __buffer.cipher
-        self.negotiated_protocol = __buffer.negotiated_protocol
-        self.negotiated_tls_version = __buffer.negotiated_tls_version
-
-    @property
-    def _socket(self) -> _pysocket.socket:
-        return cast(_pysocket.socket, self.__dict__["_socket"])
-
-    @_socket.setter
-    def _socket(self, __socket: _pysocket.socket) -> None:
-        self.__dict__["_socket"] = __socket
-        # PEP 543 requires the full socket API.
-        self.family = __socket.family
-        self.proto = __socket.proto
-        self.type = __socket.type
-        self.bind = __socket.bind
-        self.connect = __socket.connect
-        self.connect_ex = __socket.connect_ex
-        self.fileno = __socket.fileno
-        self.getpeername = __socket.getpeername
-        self.getsockname = __socket.getsockname
-        self.getsockopt = __socket.getsockopt
-        self.listen = __socket.listen
-        self.makefile = __socket.makefile
-        self.setblocking = __socket.setblocking
-        self.settimeout = __socket.settimeout
-        self.gettimeout = __socket.gettimeout
-        self.setsockopt = __socket.setsockopt
-
-    def __getstate__(self) -> NoReturn:
-        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
-
-    def __enter__(self) -> TLSWrappedSocket:
-        return self
-
-    def __exit__(self, *exc_info: object) -> None:
-        if not self._closed:
-            self.close()
-
-    def __str__(self) -> str:
-        return str(self._socket)
-
-    @property
-    def _handshake_state(self) -> HandshakeStep:
-        # pylint: disable=protected-access
-        return self._buffer._handshake_state
-
-    def setmtu(self, mtu: int) -> None:
-        """Set Maxiumum Transport Unit (MTU) for DTLS.
-
-        Set to zero to unset.
-
-        Raises:
-            OverflowError: If value cannot be converted to UInt16.
-
-        """
-        self._buffer.setmtu(mtu)
-
-    def accept(self) -> Tuple[TLSWrappedSocket, _Address]:
-        if self.type == _pysocket.SOCK_STREAM:
-            conn, address = self._socket.accept()
-        else:
-            _, address = self._socket.recvfrom(1024, _pysocket.MSG_PEEK)
-            # Use this socket to communicate with the client and bind
-            # another one for the next connection.  This procedure is
-            # adapted from `mbedtls_net_accept()`.
-            sockname = self.getsockname()
-            conn = _pysocket.fromfd(self.fileno(), self.family, self.type)
-            conn.connect(address)
-            # Closing the socket on Python 2.7 and 3.4 invalidates
-            # the accessors.  So we should get the values first.
-            family, type_, proto = self.family, self.type, self.proto
-            self.close()
-            self._socket = _pysocket.socket(family, type_, proto)
-            self.setsockopt(_pysocket.SOL_SOCKET, _pysocket.SO_REUSEADDR, 1)
-            self.bind(sockname)
-        if isinstance(self.context, ClientContext):
-            # pylint: disable=protected-access
-            # Probably not very useful but there is not reason to forbid it.
-            return (
-                self.context.wrap_socket(conn, self._buffer._server_hostname),
-                address,
-            )
-        assert isinstance(self.context, ServerContext)
-        return self.context.wrap_socket(conn), address
-
-    def close(self) -> None:
-        self._closed = True
-        self._buffer.shutdown()
-        self._socket.close()
-
-    def recv(self, bufsize: int, flags: int = 0) -> bytes:
-        encrypted = self._socket.recv(bufsize, flags)
-        if not encrypted:
-            return b""
-        self._buffer.receive_from_network(encrypted)
-        return self._buffer.read(bufsize)
-
-    def recv_into(
-        self,
-        buffer: _WriteableBuffer,
-        nbytes: Optional[int] = None,
-        flags: int = 0,
-    ) -> int:
-        if nbytes is None:
-            bufsize = len(buffer)
-        else:
-            bufsize = min(len(buffer), nbytes)
-        encrypted = self._socket.recv(bufsize, flags)
-        if not encrypted:
-            return 0
-        self._buffer.receive_from_network(encrypted)
-        return self._buffer.readinto(buffer, len(encrypted))
-
-    def recvfrom(self, bufsize: int, flags: int = 0) -> Tuple[bytes, _Address]:
-        encrypted, addr = self._socket.recvfrom(bufsize, flags)
-        if not encrypted:
-            return b"", addr
-        self._buffer.receive_from_network(encrypted)
-        return self._buffer.read(bufsize), addr
-
-    def recvfrom_into(
-        self,
-        buffer: _WriteableBuffer,
-        nbytes: Optional[int] = None,
-        flags: int = 0,
-    ) -> Tuple[int, _Address]:
-        encrypted, addr = self._socket.recvfrom(
-            nbytes if nbytes is not None else len(buffer), flags
-        )
-        if not encrypted:
-            return 0, addr
-        self._buffer.receive_from_network(encrypted)
-        return (
-            self._buffer.readinto(
-                buffer, nbytes if nbytes is not None else len(buffer)
-            ),
-            addr,
-        )
-
-    def send(self, message: bytes, flags: int = 0) -> int:
-        # Maximum size supported by TLS is 16K (encrypted).
-        # mbedTLS defines it in MBEDTLS_SSL_MAX_CONTENT_LEN and
-        # MBEDTLS_SSL_IN_CONTENT_LEN/MBEDTLS_SSL_OUT_CONTENT_LEN.
-        amt = self._buffer.write(message)
-        encrypted = self._buffer.peek_outgoing(amt)
-        self._socket.send(encrypted, flags)
-        self._buffer.consume_outgoing(amt)
-        return len(message)
-
-    def sendall(self, message: bytes, flags: int = 0) -> None:
-        amt = self._buffer.write(message)
-        encrypted = self._buffer.peek_outgoing(amt)
-        self._buffer.consume_outgoing(amt)
-        self._socket.sendall(encrypted, flags)
-
-    def sendto(self, message: bytes, *args: Any) -> int:
-        if not 1 <= len(args) <= 2:
-            raise TypeError(
-                "sendto() takes 2 or 3 arguments (%i given)" % (1 + len(args))
-            )
-
-        amt = self._buffer.write(message)
-        encrypted = self._buffer.peek_outgoing(amt)
-        self._socket.sendto(encrypted, *args)
-        self._buffer.consume_outgoing(amt)
-        return len(message)
-
-    def shutdown(self, how: int) -> None:
-        self._buffer.shutdown()
-        self._socket.shutdown(how)
-
-    # PEP 543 adds the following methods.
-    @overload
-    def do_handshake(self) -> None:
-        ...
-
-    @overload
-    def do_handshake(self, address: _Address) -> None:
-        ...
-
-    @overload
-    def do_handshake(self, flags: int, address: _Address) -> None:
-        ...
-
-    def do_handshake(self, *args):  # type: ignore[no-untyped-def]
-        # pylint: disable=too-many-branches
-        if args and self.type is not _pysocket.SOCK_DGRAM:
-            raise OSError(errno.ENOTCONN, os.strerror(errno.ENOTCONN))
-
-        if len(args) == 0:
-            flags, address = 0, None
-        elif len(args) == 1:
-            flags, address = 0, args[0]
-        elif len(args) == 2:
-            assert isinstance(args[0], int)
-            flags, address = args
-        else:
-            raise TypeError("do_handshake() takes 0, 1, or 2 arguments")
-
-        while self._handshake_state is not HandshakeStep.HANDSHAKE_OVER:
-            try:
-                self._buffer.do_handshake()
-            except WantReadError as exc:
-                if address is None:
-                    data = self._socket.recv(1024, flags)
-                else:
-                    data, addr = self._socket.recvfrom(1024, flags)
-                    if addr != address:
-                        # The error may not be the clearest but we'd better
-                        # bail out in any case.
-                        raise OSError(
-                            errno.ENOTCONN, os.strerror(errno.ENOTCONN)
-                        ) from exc
-                self._buffer.receive_from_network(data)
-            except WantWriteError:
-                in_transit = self._buffer.peek_outgoing(1024)
-                if address is None:
-                    amt = self._socket.send(in_transit, flags)
-                else:
-                    amt = self._socket.sendto(in_transit, flags, address)
-                self._buffer.consume_outgoing(amt)
-
-    def unwrap(self) -> _pysocket.socket:
-        self._buffer.shutdown()
-        return self._socket
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2018, Mathias Laurin
+
+from __future__ import annotations
+
+import enum
+import errno
+import os
+import socket as _pysocket
+import struct
+import sys
+from contextlib import suppress
+from typing import Any, Final, NoReturn, Optional, Tuple, Union, cast, overload
+
+from ._tls import HandshakeStep as HandshakeStep
+from ._tls import HelloVerifyRequest
+from ._tls import MbedTLSBuffer as TLSWrappedBuffer
+from ._tls import (
+    Purpose,
+    RaggedEOF,
+    TLSSession,
+    TrustStore,
+    WantReadError,
+    WantWriteError,
+    _BaseContext,
+    _tls_from_version,
+    _tls_to_version,
+    ciphers_available,
+)
+from ._tlsi import DTLSConfiguration as DTLSConfiguration
+from ._tlsi import DTLSVersion as DTLSVersion
+from ._tlsi import MaxFragmentLength as MaxFragmentLength
+from ._tlsi import NextProtocol as NextProtocol
+from ._tlsi import PrivateKey as PrivateKey
+from ._tlsi import ServerNameCallback as ServerNameCallback
+from ._tlsi import TLSConfiguration as TLSConfiguration
+from ._tlsi import TLSVersion as TLSVersion
+
+if sys.version_info < (3, 10):
+    from typing_extensions import TypeAlias
+else:
+    from typing import TypeAlias
+
+
+__all__ = (
+    "ClientContext",
+    "DTLSConfiguration",
+    "DTLSVersion",
+    "HelloVerifyRequest",
+    "MaxFragmentLength",
+    "NextProtocol",
+    "PrivateKey",
+    "Purpose",
+    "RaggedEOF",
+    "ServerContext",
+    "ServerNameCallback",
+    "TLSConfiguration",
+    "TLSRecordHeader",
+    "TLSSession",
+    "TLSVersion",
+    "TLSWrappedBuffer",
+    "TLSWrappedSocket",
+    "TrustStore",
+    "WantReadError",
+    "WantWriteError",
+    "ciphers_available",
+)
+
+# `_Address` stolen from `_socket.pyi`.
+_Address: TypeAlias = Union[Tuple[Any, ...], str]
+_WriteableBuffer: TypeAlias = Union[memoryview, bytearray]
+
+
+class TLSRecordHeader:
+    """Encode/decode TLS record protocol format."""
+
+    __slots__ = ("record_type", "version", "length")
+    fmt = "!BHH"
+
+    class RecordType(enum.IntEnum):
+        CHANGE_CIPHER_SPEC = 0x14
+        ALERT = 0x15
+        HANDSHAKE = 0x16
+        APPLICATION_DATA = 0x17
+
+    def __init__(
+        self,
+        record_type: Union[int, TLSRecordHeader.RecordType],
+        version: Union[int, Tuple[int, int], TLSVersion],
+        length: int,
+    ) -> None:
+        def parse_version(
+            v: Union[int, Tuple[int, int], TLSVersion]
+        ) -> TLSVersion:
+            if isinstance(v, TLSVersion):
+                return v
+            if isinstance(v, int):
+                return TLSVersion(v)
+            return TLSVersion(((v[0] & 0xFF) << 8) + v[1] & 0xFF)
+
+        self.record_type: Final = TLSRecordHeader.RecordType(record_type)
+        self.version: Final = parse_version(version)
+        self.length: Final = length
+
+    def __str__(self) -> str:
+        return "{}({}, {}, {})".format(
+            type(self).__name__,
+            self.record_type,
+            self.version,
+            self.length,
+        )
+
+    def __repr__(self) -> str:
+        return "{}({!r}, {!r}, {!r})".format(
+            type(self).__name__,
+            self.record_type,
+            self.version,
+            self.length,
+        )
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, TLSRecordHeader):
+            return NotImplemented
+        return (
+            self.record_type is other.record_type
+            and self.version is other.version
+            and self.length == other.length
+        )
+
+    def __hash__(self) -> int:
+        return 0x5AFE ^ self.record_type ^ self.version.value ^ self.length
+
+    def __len__(self) -> int:
+        return 5
+
+    def __bytes__(self) -> bytes:
+        maj, min_ = _tls_from_version(self.version)
+        version = ((maj & 0xFF) << 8) + (min_ & 0xFF)
+        return struct.pack(
+            TLSRecordHeader.fmt,
+            self.record_type,
+            version,
+            self.length,
+        )
+
+    @classmethod
+    def from_bytes(cls, header: bytes) -> TLSRecordHeader:
+        record_type, maj_min_version, length = struct.unpack(
+            TLSRecordHeader.fmt, header[:5]
+        )
+        maj, min_ = (maj_min_version >> 8) & 0xFF, maj_min_version & 0xFF
+        return cls(
+            TLSRecordHeader.RecordType(record_type),
+            _tls_to_version((maj, min_)),
+            length,
+        )
+
+
+class ClientContext(_BaseContext):
+    # _pep543.ClientContext
+
+    @property
+    def _purpose(self) -> Purpose:
+        return Purpose.CLIENT_AUTH
+
+    def wrap_socket(
+        self, socket: _pysocket.socket, server_hostname: Optional[str]
+    ) -> TLSWrappedSocket:
+        """Wrap an existing Python socket object ``socket`` and return a
+        ``TLSWrappedSocket`` object. ``socket`` must be a ``SOCK_STREAM``
+        socket: all other socket types are unsupported.
+
+        Args:
+            socket: The socket to wrap.
+            server_hostname: The hostname of the service
+                which we are connecting to.  Pass ``None`` if hostname
+                validation is not desired.  This parameter has no
+                default value because opting-out hostname validation is
+                dangerous and should not be the default behavior.
+
+        """
+        buffer = self.wrap_buffers(server_hostname)
+        return TLSWrappedSocket(socket, buffer)
+
+    def wrap_buffers(self, server_hostname: Optional[str]) -> TLSWrappedBuffer:
+        """Create an in-memory stream for TLS."""
+        # PEP 543
+        return TLSWrappedBuffer(self, server_hostname)
+
+
+class ServerContext(_BaseContext):
+    # _pep543.ServerContext
+
+    @property
+    def _purpose(self) -> Purpose:
+        return Purpose.SERVER_AUTH
+
+    def wrap_socket(self, socket: _pysocket.socket) -> TLSWrappedSocket:
+        """Wrap an existing Python socket object ``socket``."""
+        buffer = self.wrap_buffers()
+        return TLSWrappedSocket(socket, buffer)
+
+    def wrap_buffers(self) -> TLSWrappedBuffer:
+        # PEP 543
+        return TLSWrappedBuffer(self)
+
+
+class TLSWrappedSocket:
+    # pylint: disable=too-many-instance-attributes
+    # _pep543.TLSWrappedSocket
+    def __init__(
+        self, socket: _pysocket.socket, buffer: TLSWrappedBuffer
+    ) -> None:
+        super().__init__()
+        self._socket = socket
+        self._buffer = buffer
+        self._context = buffer.context
+        self._closed = False
+
+    @property
+    def context(self) -> _BaseContext:
+        return self._buffer.context
+
+    @property
+    def _buffer(self) -> TLSWrappedBuffer:
+        return cast(TLSWrappedBuffer, self.__dict__["_buffer"])
+
+    @_buffer.setter
+    def _buffer(self, __buffer: TLSWrappedBuffer) -> None:
+        self.__dict__["_buffer"] = __buffer
+        self.setcookieparam = __buffer.setcookieparam
+        self.cipher = __buffer.cipher
+        self.negotiated_protocol = __buffer.negotiated_protocol
+        self.negotiated_tls_version = __buffer.negotiated_tls_version
+
+    @property
+    def _socket(self) -> _pysocket.socket:
+        return cast(_pysocket.socket, self.__dict__["_socket"])
+
+    @_socket.setter
+    def _socket(self, __socket: _pysocket.socket) -> None:
+        self.__dict__["_socket"] = __socket
+        # PEP 543 requires the full socket API.
+        self.family = __socket.family
+        self.proto = __socket.proto
+        self.type = __socket.type
+        self.bind = __socket.bind
+        self.connect = __socket.connect
+        self.connect_ex = __socket.connect_ex
+        self.fileno = __socket.fileno
+        self.getpeername = __socket.getpeername
+        self.getsockname = __socket.getsockname
+        self.getsockopt = __socket.getsockopt
+        self.listen = __socket.listen
+        self.makefile = __socket.makefile
+        self.setblocking = __socket.setblocking
+        self.settimeout = __socket.settimeout
+        self.gettimeout = __socket.gettimeout
+        self.setsockopt = __socket.setsockopt
+
+    def __getstate__(self) -> NoReturn:
+        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
+
+    def __enter__(self) -> TLSWrappedSocket:
+        return self
+
+    def __exit__(self, *exc_info: object) -> None:
+        if not self._closed:
+            self.close()
+
+    def __str__(self) -> str:
+        return str(self._socket)
+
+    @property
+    def _handshake_state(self) -> HandshakeStep:
+        # pylint: disable=protected-access
+        return self._buffer._handshake_state
+
+    def setmtu(self, mtu: int) -> None:
+        """Set Maxiumum Transport Unit (MTU) for DTLS.
+
+        Set to zero to unset.
+
+        Raises:
+            OverflowError: If value cannot be converted to UInt16.
+
+        """
+        self._buffer.setmtu(mtu)
+
+    def accept(self) -> Tuple[TLSWrappedSocket, _Address]:
+        if self.type == _pysocket.SOCK_STREAM:
+            conn, address = self._socket.accept()
+        else:
+            _, address = self._socket.recvfrom(1024, _pysocket.MSG_PEEK)
+            # Use this socket to communicate with the client and bind
+            # another one for the next connection.  This procedure is
+            # adapted from `mbedtls_net_accept()`.
+            sockname = self.getsockname()
+            conn = _pysocket.fromfd(self.fileno(), self.family, self.type)
+            conn.connect(address)
+            # Closing the socket on Python 2.7 and 3.4 invalidates
+            # the accessors.  So we should get the values first.
+            family, type_, proto = self.family, self.type, self.proto
+            self.close()
+            self._socket = _pysocket.socket(family, type_, proto)
+            self.setsockopt(_pysocket.SOL_SOCKET, _pysocket.SO_REUSEADDR, 1)
+            self.bind(sockname)
+        if isinstance(self.context, ClientContext):
+            # pylint: disable=protected-access
+            # Probably not very useful but there is not reason to forbid it.
+            return (
+                self.context.wrap_socket(conn, self._buffer._server_hostname),
+                address,
+            )
+        assert isinstance(self.context, ServerContext)
+        return self.context.wrap_socket(conn), address
+
+    def close(self) -> None:
+        self._closed = True
+        self._buffer.shutdown()
+        self._socket.close()
+
+    def recv(self, bufsize: int, flags: int = 0) -> bytes:
+        encrypted = self._socket.recv(bufsize, flags)
+        if not encrypted:
+            return b""
+        self._buffer.receive_from_network(encrypted)
+        return self._buffer.read(bufsize)
+
+    def recv_into(
+        self,
+        buffer: _WriteableBuffer,
+        nbytes: Optional[int] = None,
+        flags: int = 0,
+    ) -> int:
+        if nbytes is None:
+            bufsize = len(buffer)
+        else:
+            bufsize = min(len(buffer), nbytes)
+        encrypted = self._socket.recv(bufsize, flags)
+        if not encrypted:
+            return 0
+        self._buffer.receive_from_network(encrypted)
+        return self._buffer.readinto(buffer, len(encrypted))
+
+    def recvfrom(self, bufsize: int, flags: int = 0) -> Tuple[bytes, _Address]:
+        encrypted, addr = self._socket.recvfrom(bufsize, flags)
+        if not encrypted:
+            return b"", addr
+        self._buffer.receive_from_network(encrypted)
+        return self._buffer.read(bufsize), addr
+
+    def recvfrom_into(
+        self,
+        buffer: _WriteableBuffer,
+        nbytes: Optional[int] = None,
+        flags: int = 0,
+    ) -> Tuple[int, _Address]:
+        encrypted, addr = self._socket.recvfrom(
+            nbytes if nbytes is not None else len(buffer), flags
+        )
+        if not encrypted:
+            return 0, addr
+        self._buffer.receive_from_network(encrypted)
+        return (
+            self._buffer.readinto(
+                buffer, nbytes if nbytes is not None else len(buffer)
+            ),
+            addr,
+        )
+
+    def send(self, message: bytes, flags: int = 0) -> int:
+        # Maximum size supported by TLS is 16K (encrypted).
+        # mbedTLS defines it in MBEDTLS_SSL_MAX_CONTENT_LEN and
+        # MBEDTLS_SSL_IN_CONTENT_LEN/MBEDTLS_SSL_OUT_CONTENT_LEN.
+        amt = self._buffer.write(message)
+        encrypted = self._buffer.peek_outgoing(amt)
+        self._socket.send(encrypted, flags)
+        self._buffer.consume_outgoing(amt)
+        return len(message)
+
+    def sendall(self, message: bytes, flags: int = 0) -> None:
+        amt = self._buffer.write(message)
+        encrypted = self._buffer.peek_outgoing(amt)
+        self._buffer.consume_outgoing(amt)
+        self._socket.sendall(encrypted, flags)
+
+    def sendto(self, message: bytes, *args: Any) -> int:
+        if not 1 <= len(args) <= 2:
+            raise TypeError(
+                "sendto() takes 2 or 3 arguments (%i given)" % (1 + len(args))
+            )
+
+        amt = self._buffer.write(message)
+        encrypted = self._buffer.peek_outgoing(amt)
+        self._socket.sendto(encrypted, *args)
+        self._buffer.consume_outgoing(amt)
+        return len(message)
+
+    def shutdown(self, how: int) -> None:
+        self._buffer.shutdown()
+        # Alerts are much smaller but it doesn't matter.
+        close_notify = self._buffer.peek_outgoing(4096)
+        with suppress(OSError):
+            # Do not raise if the socket is already closed.
+            amt = self._socket.send(close_notify)
+            self._buffer.consume_outgoing(amt)
+        self._socket.shutdown(how)
+
+    # PEP 543 adds the following methods.
+    @overload
+    def do_handshake(self) -> None:
+        ...
+
+    @overload
+    def do_handshake(self, address: _Address) -> None:
+        ...
+
+    @overload
+    def do_handshake(self, flags: int, address: _Address) -> None:
+        ...
+
+    def do_handshake(self, *args):  # type: ignore[no-untyped-def]
+        # pylint: disable=too-many-branches
+        if args and self.type is not _pysocket.SOCK_DGRAM:
+            raise OSError(errno.ENOTCONN, os.strerror(errno.ENOTCONN))
+
+        if len(args) == 0:
+            flags, address = 0, None
+        elif len(args) == 1:
+            flags, address = 0, args[0]
+        elif len(args) == 2:
+            assert isinstance(args[0], int)
+            flags, address = args
+        else:
+            raise TypeError("do_handshake() takes 0, 1, or 2 arguments")
+
+        while self._handshake_state is not HandshakeStep.HANDSHAKE_OVER:
+            try:
+                self._buffer.do_handshake()
+            except WantReadError as exc:
+                if address is None:
+                    data = self._socket.recv(1024, flags)
+                else:
+                    data, addr = self._socket.recvfrom(1024, flags)
+                    if addr != address:
+                        # The error may not be the clearest but we'd better
+                        # bail out in any case.
+                        raise OSError(
+                            errno.ENOTCONN, os.strerror(errno.ENOTCONN)
+                        ) from exc
+                self._buffer.receive_from_network(data)
+            except WantWriteError:
+                in_transit = self._buffer.peek_outgoing(1024)
+                if address is None:
+                    amt = self._socket.send(in_transit, flags)
+                else:
+                    amt = self._socket.sendto(in_transit, flags, address)
+                self._buffer.consume_outgoing(amt)
+
+    def unwrap(self) -> _pysocket.socket:
+        self._buffer.shutdown()
+        return self._socket
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/version.pyx` & `python-mbedtls-2.7.1/src/mbedtls/version.pyx`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2019, Mathias Laurin
-
-"""Run-time version information"""
-
-from libc.stdlib cimport free, malloc
-
-cimport mbedtls.version as _ver
-
-from collections import namedtuple
-
-mbedtls_version = namedtuple("mbedtls_version", "major minor micro")
-
-
-cdef __version_info():
-    """Returns the version as a tuple."""
-    cdef unsigned int version = _ver.mbedtls_version_get_number()
-    major = version >> 24 & 0xff
-    minor = version >> 16 & 0xff
-    micro = version >> 8 & 0xff
-    assert version & 0xff == 0
-    return mbedtls_version(major, minor, micro)
-
-
-cdef __version():
-    """Return the version as a string."""
-    cdef char *output = <char *>malloc(18 * sizeof(char))
-    cdef bytes buffer
-    if not output:
-        raise MemoryError()
-    try:
-        _ver.mbedtls_version_get_string_full(output)
-        buffer = output
-        return buffer.decode("ascii")
-    finally:
-        free(output)
-
-
-cdef _has_feature(feature):
-    feature_ = feature.encode("ascii")
-    cdef char *c_feature = feature_
-    cdef int result = _ver.mbedtls_version_check_feature(&c_feature[0])
-    if result == -2:
-        raise ValueError("%s not supported" % feature)
-    return result == 0
-
-
-def has_feature(feature):
-    feature = feature.upper()
-    if not feature.startswith("MBEDTLS_"):
-        feature = "MBEDTLS_" + feature
-    result = _has_feature(feature)
-    if result is True:
-        return result
-    elif not feature.endswith("_C"):
-        return _has_feature(feature + "_C")
-    else:
-        return False
-
-
-version_info = __version_info()
-version = __version()
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2019, Mathias Laurin
+
+"""Run-time version information"""
+
+from libc.stdlib cimport free, malloc
+
+cimport mbedtls.version as _ver
+
+from collections import namedtuple
+
+mbedtls_version = namedtuple("mbedtls_version", "major minor micro")
+
+
+cdef __version_info():
+    """Returns the version as a tuple."""
+    cdef unsigned int version = _ver.mbedtls_version_get_number()
+    major = version >> 24 & 0xff
+    minor = version >> 16 & 0xff
+    micro = version >> 8 & 0xff
+    assert version & 0xff == 0
+    return mbedtls_version(major, minor, micro)
+
+
+cdef __version():
+    """Return the version as a string."""
+    cdef char *output = <char *>malloc(18 * sizeof(char))
+    cdef bytes buffer
+    if not output:
+        raise MemoryError()
+    try:
+        _ver.mbedtls_version_get_string_full(output)
+        buffer = output
+        return buffer.decode("ascii")
+    finally:
+        free(output)
+
+
+cdef _has_feature(feature):
+    feature_ = feature.encode("ascii")
+    cdef char *c_feature = feature_
+    cdef int result = _ver.mbedtls_version_check_feature(&c_feature[0])
+    if result == -2:
+        raise ValueError("%s not supported" % feature)
+    return result == 0
+
+
+def has_feature(feature):
+    feature = feature.upper()
+    if not feature.startswith("MBEDTLS_"):
+        feature = "MBEDTLS_" + feature
+    result = _has_feature(feature)
+    if result is True:
+        return result
+    elif not feature.endswith("_C"):
+        return _has_feature(feature + "_C")
+    else:
+        return False
+
+
+version_info = __version_info()
+version = __version()
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/x509.pxd` & `python-mbedtls-2.7.1/src/mbedtls/x509.pxd`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,309 +1,309 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2018, Mathias Laurin
-
-"""Declarations from `mbedtls/x509*.h`.
-
- - CSR: Certificate signing request parsing and writing.
- - CRL: Certificate revocation list parsing.
- - CRT: Certificate parsing and writing.
-
-"""
-
-
-cimport mbedtls._asn1 as _asn1
-cimport mbedtls._md as _md
-cimport mbedtls.mpi as _mpi
-cimport mbedtls.pk as _pk
-
-
-cdef extern from "mbedtls/x509.h" nogil:
-    ctypedef _asn1.mbedtls_asn1_buf mbedtls_x509_buf
-    ctypedef _asn1.mbedtls_asn1_named_data mbedtls_x509_name
-    ctypedef _asn1.mbedtls_asn1_sequence mbedtls_x509_sequence
-    int mbedtls_x509_dn_gets(
-        char *buf, size_t size, const mbedtls_x509_name *dn)
-    cdef struct mbedtls_x509_time:
-        int year, mon, day
-        int hour, min, sec
-
-
-cdef extern from "mbedtls/x509_crt.h" nogil:
-    cdef struct mbedtls_x509_crt:
-        mbedtls_x509_buf raw
-        mbedtls_x509_buf tbs
-        int version
-        mbedtls_x509_buf serial
-        mbedtls_x509_buf sig_oid
-        # mbedtls_x509_buf issuer_raw
-        # mbedtls_x509_buf subject_raw
-        mbedtls_x509_name issuer
-        mbedtls_x509_name subject
-        mbedtls_x509_time valid_from
-        mbedtls_x509_time valid_to
-        _pk.mbedtls_pk_context pk  # public key
-        # mbedtls_x509_buf issuer_id
-        # mbedtls_x509_buf subject_id
-        # mbedtls_x509_buf v3_ext
-        mbedtls_x509_sequence subject_alt_names
-        # int ext_types
-        int ca_istrue  # 1 if this certificate belongs to a CA, 0 otherwise
-        int max_pathlen
-        unsigned int key_usage
-        # mbedtls_x509_sequence ext_key_usage
-        # unsigned char ns_cert_type
-
-        mbedtls_x509_buf sig
-        _md.mbedtls_md_type_t sig_md
-        # mbedtls_pk_type_t sig_pk
-        # void *sig_opts
-        mbedtls_x509_crt *next
-
-    ctypedef struct mbedtls_x509_crt_profile:
-        pass
-
-    ctypedef struct mbedtls_x509write_cert:
-        pass
-
-    # mbedtls_x509_crt
-    # ----------------
-    int mbedtls_x509_crt_parse_der(
-        mbedtls_x509_crt *chain,
-        const unsigned char *buf,
-        size_t buflen)
-    int mbedtls_x509_crt_parse(
-        mbedtls_x509_crt *chain,
-        const unsigned char *buf,
-        size_t buflen)
-    int mbedtls_x509_crt_parse_file(
-        mbedtls_x509_crt *chain,
-        const char *path)
-
-    # mbedtls_x509_crt_parse_path
-
-    int mbedtls_x509_crt_info(
-        char *buf,
-        size_t size,
-        const char* prefix,
-        const mbedtls_x509_crt *crt)
-
-    # mbedtls_x509_crt_verify_info
-    # mbedtls_x509_crt_verify
-    # mbedtls_x509_crt_verify_with_profile
-    # mbedtls_x509_crt_check_key_usage
-    # mbedtls_x509_crt_check_extended_key_usage
-
-    int mbedtls_x509_crt_is_revoked(
-        const mbedtls_x509_crt *crt,
-        const mbedtls_x509_crl *crl)
-
-    void mbedtls_x509_crt_init(mbedtls_x509_crt *crt)
-    void mbedtls_x509_crt_free(mbedtls_x509_crt *crt)
-
-    # mbedtls_x509write_cert
-    # ----------------------
-
-    void mbedtls_x509write_crt_init(mbedtls_x509write_cert *ctx)
-    void mbedtls_x509write_crt_set_version(
-        mbedtls_x509write_cert *ctx,
-        int version)
-    int mbedtls_x509write_crt_set_serial(
-        mbedtls_x509write_cert *ctx,
-        _mpi.mbedtls_mpi *serial)
-
-    int mbedtls_x509write_crt_set_validity(
-        mbedtls_x509write_cert *ctx,
-        const char *not_before,
-        const char *not_after)
-    int mbedtls_x509write_crt_set_issuer_name(
-        mbedtls_x509write_cert *ctx,
-        const char *issuer_name)
-    int mbedtls_x509write_crt_set_subject_name(
-        mbedtls_x509write_cert *ctx,
-        const char *subject_name)
-    void mbedtls_x509write_crt_set_subject_key(
-        mbedtls_x509write_cert *ctx,
-        _pk.mbedtls_pk_context *key)
-    void mbedtls_x509write_crt_set_issuer_key(
-        mbedtls_x509write_cert *ctx,
-        _pk.mbedtls_pk_context *key)
-    void mbedtls_x509write_crt_set_md_alg(
-        mbedtls_x509write_cert *ctx,
-        _md.mbedtls_md_type_t md_alg)
-
-    # mbedtls_x509write_crt_set_extension
-    int mbedtls_x509write_crt_set_basic_constraints(
-        mbedtls_x509write_cert *ctx,
-        int is_ca, int max_pathlen)
-
-    int mbedtls_x509write_crt_set_subject_key_identifier(
-        mbedtls_x509write_cert *ctx)
-    int mbedtls_x509write_crt_set_authority_key_identifier(
-        mbedtls_x509write_cert *ctx)
-
-    # mbedtls_x509write_crt_set_key_usage
-    # mbedtls_x509write_crt_set_ns_cert_type
-
-    void mbedtls_x509write_crt_free(mbedtls_x509write_cert *ctx)
-
-    int mbedtls_x509write_crt_der(
-        mbedtls_x509write_cert *ctx,
-        unsigned char *buf, size_t size,
-        int (*f_rng)(void *, unsigned char *, size_t),
-        void *p_rng)
-    int mbedtls_x509write_crt_pem(
-        mbedtls_x509write_cert *ctx,
-        unsigned char *buf, size_t size,
-        int (*f_rng)(void *, unsigned char *, size_t),
-        void *p_rng)
-
-
-cdef extern from "mbedtls/x509_csr.h" nogil:
-    # Certificate signing request parsing and writing
-    # -----------------------------------------------
-    cdef struct mbedtls_x509_csr:
-        mbedtls_x509_buf raw
-        # mbedtls_x509_buf cri
-        int version
-        # mbedtls_x509_buf subject_raw
-        mbedtls_x509_name subject
-        _pk.mbedtls_pk_context pk
-        mbedtls_x509_buf sig_oid
-        mbedtls_x509_buf sig
-        _md.mbedtls_md_type_t sig_md
-        # mbedtls_pk_type_t sig_pk
-        # void *sig_opts
-
-    ctypedef struct mbedtls_x509write_csr:
-        pass
-
-    # mbedtls_x509_csr
-    # ----------------
-    int mbedtls_x509_csr_parse_der(
-        mbedtls_x509_csr *csr,
-        const unsigned char *buf,
-        size_t buflen)
-    int mbedtls_x509_csr_parse(
-        mbedtls_x509_csr *csr,
-        const unsigned char *buf,
-        size_t buflen)
-    int mbedtls_x509_csr_parse_file(
-        mbedtls_x509_csr *csr,
-        const char *path)
-    int mbedtls_x509_csr_info(
-        char *buf,
-        size_t size,
-        const char* prefix,
-        const mbedtls_x509_csr *csr)
-    void mbedtls_x509_csr_init(mbedtls_x509_csr *csr)
-    void mbedtls_x509_csr_free(mbedtls_x509_csr *csr)
-
-    # mbedtls_x509write_csr
-    # ---------------------
-    void mbedtls_x509write_csr_init(mbedtls_x509write_csr *ctx)
-
-    int mbedtls_x509write_csr_set_subject_name(
-        mbedtls_x509write_csr *ctx,
-        const char *subject_name)
-    void mbedtls_x509write_csr_set_key(
-        mbedtls_x509write_csr *ctx,
-        _pk.mbedtls_pk_context *key)
-    void mbedtls_x509write_csr_set_md_alg(
-        mbedtls_x509write_csr *ctx,
-        _md.mbedtls_md_type_t md_alg)
-
-    # mbedtls_x509write_csr_set_key_usage
-    # mbedtls_x509write_csr_set_ns_cert_type
-    # mbedtls_x509write_csr_set_extension
-
-    void mbedtls_x509write_csr_free(mbedtls_x509write_csr *ctx)
-
-    int mbedtls_x509write_csr_der(
-        mbedtls_x509write_csr *ctx,
-        unsigned char *buf, size_t size,
-        int (*f_rng)(void *, unsigned char *, size_t),
-        void *p_rng)
-    int mbedtls_x509write_csr_pem(
-        mbedtls_x509write_csr *ctx,
-        unsigned char *buf, size_t size,
-        int (*f_rng)(void *, unsigned char *, size_t),
-        void *p_rng)
-
-
-cdef extern from "mbedtls/x509_crl.h" nogil:
-    # Certificate revocation list parsing
-    # -----------------------------------
-    ctypedef struct mbedtls_x509_crl_entry:
-        mbedtls_x509_buf raw
-        mbedtls_x509_buf serial
-        mbedtls_x509_time revocation_date
-        mbedtls_x509_buf entry_ext
-        mbedtls_x509_crl_entry *next
-
-    cdef struct mbedtls_x509_crl:
-        mbedtls_x509_buf raw
-        mbedtls_x509_buf tbs
-        int version
-        mbedtls_x509_buf sig_oid
-        mbedtls_x509_buf issuer_raw
-        mbedtls_x509_name issuer
-        mbedtls_x509_time this_update
-        mbedtls_x509_time next_update
-        mbedtls_x509_crl_entry entry
-        mbedtls_x509_buf crl_ext
-        mbedtls_x509_buf sig_oid2
-        mbedtls_x509_buf sig
-        _md.mbedtls_md_type_t sig_md
-        # mbedtls_pk_type_t sig_pk
-        # void *sig_opts
-        mbedtls_x509_crl *next
-
-    # mbedtls_x509_crl
-    # ----------------
-    int mbedtls_x509_crl_parse_der(
-        mbedtls_x509_crl *chain,
-        const unsigned char *buf,
-        size_t buflen)
-    int mbedtls_x509_crl_parse(
-        mbedtls_x509_crl *chain,
-        const unsigned char *buf,
-        size_t buflen)
-    int mbedtls_x509_crl_parse_file(
-        mbedtls_x509_crl *chain,
-        const char *path)
-    int mbedtls_x509_crl_info(
-        char *buf,
-        size_t size,
-        const char *prefix,
-        const mbedtls_x509_crl *crl)
-    void mbedtls_x509_crl_init(mbedtls_x509_crl *crl)
-    void mbedtls_x509_crl_free(mbedtls_x509_crl *crl)
-
-
-cdef class Certificate:
-    pass
-
-
-cdef class CRT(Certificate):
-    cdef mbedtls_x509_crt _ctx
-    cdef set_next(self, CRT crt)
-    cdef unset_next(self)
-    cdef CRT _next
-
-
-cdef class _CRTWriter:
-    cdef mbedtls_x509write_cert _ctx
-
-
-cdef class CSR(Certificate):
-    cdef mbedtls_x509_csr _ctx
-
-
-cdef class _CSRWriter:
-    cdef mbedtls_x509write_csr _ctx
-
-
-cdef class CRL(Certificate):
-    cdef mbedtls_x509_crl _ctx
-    cdef set_next(self, CRL crl)
-    cdef unset_next(self)
-    cdef CRL _next
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2018, Mathias Laurin
+
+"""Declarations from `mbedtls/x509*.h`.
+
+ - CSR: Certificate signing request parsing and writing.
+ - CRL: Certificate revocation list parsing.
+ - CRT: Certificate parsing and writing.
+
+"""
+
+
+cimport mbedtls._asn1 as _asn1
+cimport mbedtls._md as _md
+cimport mbedtls.mpi as _mpi
+cimport mbedtls.pk as _pk
+
+
+cdef extern from "mbedtls/x509.h" nogil:
+    ctypedef _asn1.mbedtls_asn1_buf mbedtls_x509_buf
+    ctypedef _asn1.mbedtls_asn1_named_data mbedtls_x509_name
+    ctypedef _asn1.mbedtls_asn1_sequence mbedtls_x509_sequence
+    int mbedtls_x509_dn_gets(
+        char *buf, size_t size, const mbedtls_x509_name *dn)
+    cdef struct mbedtls_x509_time:
+        int year, mon, day
+        int hour, min, sec
+
+
+cdef extern from "mbedtls/x509_crt.h" nogil:
+    cdef struct mbedtls_x509_crt:
+        mbedtls_x509_buf raw
+        mbedtls_x509_buf tbs
+        int version
+        mbedtls_x509_buf serial
+        mbedtls_x509_buf sig_oid
+        # mbedtls_x509_buf issuer_raw
+        # mbedtls_x509_buf subject_raw
+        mbedtls_x509_name issuer
+        mbedtls_x509_name subject
+        mbedtls_x509_time valid_from
+        mbedtls_x509_time valid_to
+        _pk.mbedtls_pk_context pk  # public key
+        # mbedtls_x509_buf issuer_id
+        # mbedtls_x509_buf subject_id
+        # mbedtls_x509_buf v3_ext
+        mbedtls_x509_sequence subject_alt_names
+        # int ext_types
+        int ca_istrue  # 1 if this certificate belongs to a CA, 0 otherwise
+        int max_pathlen
+        unsigned int key_usage
+        # mbedtls_x509_sequence ext_key_usage
+        # unsigned char ns_cert_type
+
+        mbedtls_x509_buf sig
+        _md.mbedtls_md_type_t sig_md
+        # mbedtls_pk_type_t sig_pk
+        # void *sig_opts
+        mbedtls_x509_crt *next
+
+    ctypedef struct mbedtls_x509_crt_profile:
+        pass
+
+    ctypedef struct mbedtls_x509write_cert:
+        pass
+
+    # mbedtls_x509_crt
+    # ----------------
+    int mbedtls_x509_crt_parse_der(
+        mbedtls_x509_crt *chain,
+        const unsigned char *buf,
+        size_t buflen)
+    int mbedtls_x509_crt_parse(
+        mbedtls_x509_crt *chain,
+        const unsigned char *buf,
+        size_t buflen)
+    int mbedtls_x509_crt_parse_file(
+        mbedtls_x509_crt *chain,
+        const char *path)
+
+    # mbedtls_x509_crt_parse_path
+
+    int mbedtls_x509_crt_info(
+        char *buf,
+        size_t size,
+        const char* prefix,
+        const mbedtls_x509_crt *crt)
+
+    # mbedtls_x509_crt_verify_info
+    # mbedtls_x509_crt_verify
+    # mbedtls_x509_crt_verify_with_profile
+    # mbedtls_x509_crt_check_key_usage
+    # mbedtls_x509_crt_check_extended_key_usage
+
+    int mbedtls_x509_crt_is_revoked(
+        const mbedtls_x509_crt *crt,
+        const mbedtls_x509_crl *crl)
+
+    void mbedtls_x509_crt_init(mbedtls_x509_crt *crt)
+    void mbedtls_x509_crt_free(mbedtls_x509_crt *crt)
+
+    # mbedtls_x509write_cert
+    # ----------------------
+
+    void mbedtls_x509write_crt_init(mbedtls_x509write_cert *ctx)
+    void mbedtls_x509write_crt_set_version(
+        mbedtls_x509write_cert *ctx,
+        int version)
+    int mbedtls_x509write_crt_set_serial(
+        mbedtls_x509write_cert *ctx,
+        _mpi.mbedtls_mpi *serial)
+
+    int mbedtls_x509write_crt_set_validity(
+        mbedtls_x509write_cert *ctx,
+        const char *not_before,
+        const char *not_after)
+    int mbedtls_x509write_crt_set_issuer_name(
+        mbedtls_x509write_cert *ctx,
+        const char *issuer_name)
+    int mbedtls_x509write_crt_set_subject_name(
+        mbedtls_x509write_cert *ctx,
+        const char *subject_name)
+    void mbedtls_x509write_crt_set_subject_key(
+        mbedtls_x509write_cert *ctx,
+        _pk.mbedtls_pk_context *key)
+    void mbedtls_x509write_crt_set_issuer_key(
+        mbedtls_x509write_cert *ctx,
+        _pk.mbedtls_pk_context *key)
+    void mbedtls_x509write_crt_set_md_alg(
+        mbedtls_x509write_cert *ctx,
+        _md.mbedtls_md_type_t md_alg)
+
+    # mbedtls_x509write_crt_set_extension
+    int mbedtls_x509write_crt_set_basic_constraints(
+        mbedtls_x509write_cert *ctx,
+        int is_ca, int max_pathlen)
+
+    int mbedtls_x509write_crt_set_subject_key_identifier(
+        mbedtls_x509write_cert *ctx)
+    int mbedtls_x509write_crt_set_authority_key_identifier(
+        mbedtls_x509write_cert *ctx)
+
+    # mbedtls_x509write_crt_set_key_usage
+    # mbedtls_x509write_crt_set_ns_cert_type
+
+    void mbedtls_x509write_crt_free(mbedtls_x509write_cert *ctx)
+
+    int mbedtls_x509write_crt_der(
+        mbedtls_x509write_cert *ctx,
+        unsigned char *buf, size_t size,
+        int (*f_rng)(void *, unsigned char *, size_t),
+        void *p_rng)
+    int mbedtls_x509write_crt_pem(
+        mbedtls_x509write_cert *ctx,
+        unsigned char *buf, size_t size,
+        int (*f_rng)(void *, unsigned char *, size_t),
+        void *p_rng)
+
+
+cdef extern from "mbedtls/x509_csr.h" nogil:
+    # Certificate signing request parsing and writing
+    # -----------------------------------------------
+    cdef struct mbedtls_x509_csr:
+        mbedtls_x509_buf raw
+        # mbedtls_x509_buf cri
+        int version
+        # mbedtls_x509_buf subject_raw
+        mbedtls_x509_name subject
+        _pk.mbedtls_pk_context pk
+        mbedtls_x509_buf sig_oid
+        mbedtls_x509_buf sig
+        _md.mbedtls_md_type_t sig_md
+        # mbedtls_pk_type_t sig_pk
+        # void *sig_opts
+
+    ctypedef struct mbedtls_x509write_csr:
+        pass
+
+    # mbedtls_x509_csr
+    # ----------------
+    int mbedtls_x509_csr_parse_der(
+        mbedtls_x509_csr *csr,
+        const unsigned char *buf,
+        size_t buflen)
+    int mbedtls_x509_csr_parse(
+        mbedtls_x509_csr *csr,
+        const unsigned char *buf,
+        size_t buflen)
+    int mbedtls_x509_csr_parse_file(
+        mbedtls_x509_csr *csr,
+        const char *path)
+    int mbedtls_x509_csr_info(
+        char *buf,
+        size_t size,
+        const char* prefix,
+        const mbedtls_x509_csr *csr)
+    void mbedtls_x509_csr_init(mbedtls_x509_csr *csr)
+    void mbedtls_x509_csr_free(mbedtls_x509_csr *csr)
+
+    # mbedtls_x509write_csr
+    # ---------------------
+    void mbedtls_x509write_csr_init(mbedtls_x509write_csr *ctx)
+
+    int mbedtls_x509write_csr_set_subject_name(
+        mbedtls_x509write_csr *ctx,
+        const char *subject_name)
+    void mbedtls_x509write_csr_set_key(
+        mbedtls_x509write_csr *ctx,
+        _pk.mbedtls_pk_context *key)
+    void mbedtls_x509write_csr_set_md_alg(
+        mbedtls_x509write_csr *ctx,
+        _md.mbedtls_md_type_t md_alg)
+
+    # mbedtls_x509write_csr_set_key_usage
+    # mbedtls_x509write_csr_set_ns_cert_type
+    # mbedtls_x509write_csr_set_extension
+
+    void mbedtls_x509write_csr_free(mbedtls_x509write_csr *ctx)
+
+    int mbedtls_x509write_csr_der(
+        mbedtls_x509write_csr *ctx,
+        unsigned char *buf, size_t size,
+        int (*f_rng)(void *, unsigned char *, size_t),
+        void *p_rng)
+    int mbedtls_x509write_csr_pem(
+        mbedtls_x509write_csr *ctx,
+        unsigned char *buf, size_t size,
+        int (*f_rng)(void *, unsigned char *, size_t),
+        void *p_rng)
+
+
+cdef extern from "mbedtls/x509_crl.h" nogil:
+    # Certificate revocation list parsing
+    # -----------------------------------
+    ctypedef struct mbedtls_x509_crl_entry:
+        mbedtls_x509_buf raw
+        mbedtls_x509_buf serial
+        mbedtls_x509_time revocation_date
+        mbedtls_x509_buf entry_ext
+        mbedtls_x509_crl_entry *next
+
+    cdef struct mbedtls_x509_crl:
+        mbedtls_x509_buf raw
+        mbedtls_x509_buf tbs
+        int version
+        mbedtls_x509_buf sig_oid
+        mbedtls_x509_buf issuer_raw
+        mbedtls_x509_name issuer
+        mbedtls_x509_time this_update
+        mbedtls_x509_time next_update
+        mbedtls_x509_crl_entry entry
+        mbedtls_x509_buf crl_ext
+        mbedtls_x509_buf sig_oid2
+        mbedtls_x509_buf sig
+        _md.mbedtls_md_type_t sig_md
+        # mbedtls_pk_type_t sig_pk
+        # void *sig_opts
+        mbedtls_x509_crl *next
+
+    # mbedtls_x509_crl
+    # ----------------
+    int mbedtls_x509_crl_parse_der(
+        mbedtls_x509_crl *chain,
+        const unsigned char *buf,
+        size_t buflen)
+    int mbedtls_x509_crl_parse(
+        mbedtls_x509_crl *chain,
+        const unsigned char *buf,
+        size_t buflen)
+    int mbedtls_x509_crl_parse_file(
+        mbedtls_x509_crl *chain,
+        const char *path)
+    int mbedtls_x509_crl_info(
+        char *buf,
+        size_t size,
+        const char *prefix,
+        const mbedtls_x509_crl *crl)
+    void mbedtls_x509_crl_init(mbedtls_x509_crl *crl)
+    void mbedtls_x509_crl_free(mbedtls_x509_crl *crl)
+
+
+cdef class Certificate:
+    pass
+
+
+cdef class CRT(Certificate):
+    cdef mbedtls_x509_crt _ctx
+    cdef set_next(self, CRT crt)
+    cdef unset_next(self)
+    cdef CRT _next
+
+
+cdef class _CRTWriter:
+    cdef mbedtls_x509write_cert _ctx
+
+
+cdef class CSR(Certificate):
+    cdef mbedtls_x509_csr _ctx
+
+
+cdef class _CSRWriter:
+    cdef mbedtls_x509write_csr _ctx
+
+
+cdef class CRL(Certificate):
+    cdef mbedtls_x509_crl _ctx
+    cdef set_next(self, CRL crl)
+    cdef unset_next(self)
+    cdef CRL _next
```

### Comparing `python-mbedtls-2.7.0/src/mbedtls/x509.pyx` & `python-mbedtls-2.7.1/src/mbedtls/x509.pyx`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,1042 +1,1042 @@
-# SPDX-License-Identifier: MIT
-# Copyright (c) 2018, Mathias Laurin
-
-"""Structure and functions for parsing and writing X.509 certificates."""
-
-
-from libc.stdlib cimport free, malloc
-
-cimport mbedtls.mpi as _mpi
-cimport mbedtls.pk as _pk
-cimport mbedtls.x509 as x509
-
-import base64
-import datetime as dt
-import enum
-from collections import namedtuple
-from pathlib import Path
-
-import mbedtls._md as _md
-import mbedtls.exceptions as _exc
-import mbedtls.mpi as _mpi
-import mbedtls.pk as _pk
-from mbedtls.hashlib import new as _new_hash
-
-
-@enum.unique
-class KeyUsage(enum.IntEnum):
-    """Key Usage Extension.
-
-    See Also:
-        RFC 5280 - 4.2.1.3 Key Usage.
-
-    """
-    DIGITAL_SIGNATURE = 0x80
-    NON_REPUDIATION = 0x40
-    KEY_ENCIPHERMENT = 0x20
-    DATA_ENCIPHERMENT = 0x10
-    KEY_AGREEMENT = 0x08
-    KEY_CERT_SIGN = 0x04
-    CRL_SIGN = 0x02
-    ENCIPHER_ONLY = 0x01
-    DECIPHER_ONLY = 0x8000
-
-
-def PEM_to_DER(pem):
-    return base64.b64decode(
-        b"".join(line.encode("ascii") for line in pem.splitlines()
-                 if not line.startswith("-----")))
-
-
-def DER_to_PEM(der, text):
-    chunk_size = 64
-    pem = base64.b64encode(der).decode("ascii")
-    return "\n".join((
-        "-----BEGIN %s-----" % text.upper(),
-        "\n".join(pem[n:n+chunk_size] for n in range(0, len(pem), chunk_size)),
-        "-----END %s-----" % text.upper(),
-        ""))
-
-
-cdef class Certificate:
-    @classmethod
-    def from_buffer(cls, buffer):
-        # PEP 543
-        return cls(buffer)
-
-    @classmethod
-    def from_file(cls, path):
-        # PEP 543
-        raise NotImplementedError
-
-    @classmethod
-    def from_DER(cls, der):
-        raise NotImplementedError
-
-    @classmethod
-    def from_PEM(cls, pem):
-        raise NotImplementedError
-
-    def __reduce__(self):
-        return type(self).from_DER, (bytes(self),)
-
-    def __hash__(self):
-        return hash(self.to_DER())
-
-    def __eq__(self, other):
-        if type(other) is type(self):
-            return self.to_DER() == other.to_DER()
-        else:
-            return other == self.to_DER() or other == self.to_PEM()
-
-    def __str__(self):
-        raise NotImplementedError
-
-    def __bytes__(self):
-        return self.to_DER()
-
-    def export(self, format="DER"):
-        if format == "DER":
-            return self.to_DER()
-        if format == "PEM":
-            return self.to_PEM()
-        raise ValueError(format)
-
-    def to_bytes(self):
-        return self.to_DER()
-
-    def to_DER(self):
-        raise NotImplementedError
-
-    def to_PEM(self):
-        raise NotImplementedError
-
-
-class BasicConstraints(
-        namedtuple("BasicConstraints", ["ca", "max_path_length"])):
-    """The basic constraints for the certificate."""
-
-    def __new__(cls, ca=False, max_path_length=0):
-        return super().__new__(cls, ca, max_path_length)
-
-
-cdef class CRT(Certificate):
-    """X.509 certificate."""
-
-    def __init__(self, const unsigned char[:] buffer):
-        super().__init__()
-        self._next = None
-        if buffer is None or buffer.size == 0:
-            return
-        _exc.check_error(x509.mbedtls_x509_crt_parse(
-            &self._ctx, &buffer[0], buffer.size))
-
-    def __cinit__(self):
-        """Initialize a certificate (chain)."""
-        x509.mbedtls_x509_crt_init(&self._ctx)
-
-    def __dealloc__(self):
-        """Unallocate all certificate data."""
-        self.unset_next()
-        x509.mbedtls_x509_crt_free(&self._ctx)
-
-    def __next__(self):
-        if self._next is None:
-            raise StopIteration
-        return self._next
-
-    def __str__(self):
-        cdef size_t osize = 2**24
-        cdef char *output = <char *>malloc(osize * sizeof(char))
-        cdef char *prefix = b""
-        if not output:
-            raise MemoryError()
-        try:
-            written = _exc.check_error(x509.mbedtls_x509_crt_info(
-                &output[0], osize, prefix, &self._ctx))
-            return output[:written].decode("utf8")
-        finally:
-            free(output)
-
-    # RFC 5280, Section 4.1 Basic Certificate Fields
-    # RFC 5280, Section 4.1.1 Certificate Fields
-
-    @property
-    def tbs_certificate(self):
-        """The TBS (to be signed) certificate in DER format.
-
-        See Also:
-            RFC 5280, Section 4.1.1.1 TBS Certificate
-
-        """
-        return bytes(self._ctx.tbs.p[:self._ctx.tbs.len])
-
-    @property
-    def _signature_algorithm(self):
-        """Cryptographic algorithm used by the CA to sign this CRT.
-
-        See Also:
-            RFC 5280, Section 4.1.1.2 Signature Algorithm
-
-        """
-        # The byte structure should be parsed according to RFC 5280.
-        return bytes(self._ctx.sig_oid.p[:self._ctx.sig_oid.len])
-
-    @property
-    def signature_value(self):
-        """Digital signature of the TBS certificate.
-
-        See Also:
-            RFC 5280, Section 4.1.1.3 Signature Value
-
-        """
-        return bytes(self._ctx.sig.p[:self._ctx.sig.len])
-
-    # RFC 5280, Section 4.1.2 TBS Certificate
-
-    @property
-    def version(self):
-        """The version of the encoded certificate.
-
-        See Also:
-            RF 5280, Section 4.1.2.1 Version
-
-        """
-        return int(self._ctx.version)
-
-    @property
-    def serial_number(self):
-        """The certificate serial number.
-
-        See Also:
-            RFC 5280, Section 4.1.2.2 Serial Number
-
-        """
-        return int(_mpi.MPI.from_bytes(
-            self._ctx.serial.p[:self._ctx.serial.len], "big"))
-
-    # RFC 4.1.2.3 Signature
-    @property
-    def digestmod(self):
-        return _new_hash(_md._digestmod(self._ctx.sig_md))
-
-    @property
-    def issuer(self):
-        """Entity that has signed and issued the certificate.
-
-        See Also:
-            RFC 5280, Section 4.1.2.4 Issuer
-
-        """
-        cdef size_t osize = 200
-        cdef char* c_buf = <char *>malloc(osize * sizeof(char))
-        if not c_buf:
-            raise MemoryError()
-        try:
-            written = x509.mbedtls_x509_dn_gets(
-                &c_buf[0], osize, &self._ctx.issuer)
-            return c_buf[:written].decode("utf8")
-        finally:
-            free(c_buf)
-
-    @property
-    def not_before(self):
-        """Beginning of the validity of the certificate (inclusive).
-
-        See Also:
-            RFC 5280, Section 4.1.2.5 Validity
-
-        """
-        cdef x509.mbedtls_x509_time *valid_from = &self._ctx.valid_from
-        return dt.datetime(
-            valid_from[0].year, valid_from[0].mon, valid_from[0].day,
-            valid_from[0].hour, valid_from[0].min, valid_from[0].sec)
-
-    @property
-    def not_after(self):
-        """End of the validity of the certificate (inclusive).
-
-        See Also:
-            RFC 5280, Section 4.1.2.5 Validity
-
-        """
-        cdef x509.mbedtls_x509_time *valid_to = &self._ctx.valid_to
-        return dt.datetime(
-            valid_to[0].year, valid_to[0].mon, valid_to[0].day,
-            valid_to[0].hour, valid_to[0].min, valid_to[0].sec)
-
-    @property
-    def subject(self):
-        """Entity associated with the public key.
-
-        See Also:
-            RFC 5280, Section 4.1.2.6 Subject
-
-        """
-        cdef size_t osize = 200
-        cdef char *c_buf = <char *>malloc(osize * sizeof(char))
-        if not c_buf:
-            raise MemoryError()
-        try:
-            written = x509.mbedtls_x509_dn_gets(
-                &c_buf[0], osize, &self._ctx.subject)
-            return c_buf[:written].decode("utf8")
-        finally:
-            free(c_buf)
-
-    @property
-    def subject_public_key(self):
-        """The public key.
-
-        See Also:
-            RFC 5280, Section 4.1.2.7 Subject Public Key Info
-
-        """
-        cipher_type = _pk.CipherType(_pk.mbedtls_pk_get_type(&self._ctx.pk))
-        cipher = {
-            _pk.CipherType.RSA: _pk.RSA,
-            _pk.CipherType.ECKEY: _pk.ECC,
-        }.get(cipher_type, None)
-        if cipher is None:
-            raise NotImplementedError("unsupported cipher %r" % cipher_type)
-
-        cdef size_t osize = _pk.PUB_DER_MAX_BYTES
-        cdef unsigned char *c_buf = <unsigned char *>malloc(
-            osize * sizeof(unsigned char))
-        if not c_buf:
-            raise MemoryError()
-        try:
-            ret = _exc.check_error(_pk.mbedtls_pk_write_pubkey_der(
-                &self._ctx.pk, &c_buf[0], osize))
-            return cipher.from_DER(c_buf[osize - ret:osize])
-        finally:
-            free(c_buf)
-
-    # RFC 5280, Section 4.1.2.8 Unique Identifiers
-    # RFC 5280, Section 4.1.2.9 Extensions
-    # RFC 5280, Section 4.2 Certificate Extensions
-    # RFC 5280, Section 4.2.1 Standard Extensions
-    # RFC 5280, Section 4.2.1.1 Authority Key Identifier
-    # RFC 5280, Section 4.2.1.2 Subject Key Identifier
-
-    @property
-    def key_usage(self):
-        """Key usage extension (bitfield).
-
-        See Also:
-            RFC 5280, Section 4.2.1.3 Key Usage
-
-        """
-        return KeyUsage(self._ctx.key_usage)
-
-    # RFC 5280, Section 4.2.1.4 Certificate Policies
-    # RFC 5280, Section 4.2.1.5 Policy Mappings
-
-    @property
-    def subject_alternative_names(self):
-        """Subject alternative name extension.
-
-        See Also:
-            RFC 5280, Section 4.2.1.6 Subject Alternative Name
-
-        """
-        cdef mbedtls_x509_sequence *item
-        item = &self._ctx.subject_alt_names
-        names = set()
-        while item != NULL:
-            names.add(item.buf.p[:item.buf.len].decode("utf8"))
-            item = item.next
-        return frozenset(names)
-
-    # RFC 5280, Section 4.2.1.7 Issuer Alternative Name
-    # RFC 5280, Section 4.2.1.8 Subject Directory Attributes
-
-    @property
-    def basic_constraints(self):
-        """ca is true if the certified public key may be used
-        to verify certificate signatures.
-
-        See Also:
-            - RFC 5280, Section 4.2.1.9 Basic Constraints
-            - RFC 5280, `max_path_length`
-
-        """
-        max_path_length = int(self._ctx.max_pathlen)
-        if max_path_length > 0:
-            max_path_length -= 1
-        ca = bool(self._ctx.ca_istrue)
-        return BasicConstraints(ca, max_path_length)
-
-    # RFC 5280, Section 4.2.1.10 Name Constraints
-    # RFC 5280, Section 4.2.1.11 Policy Constraints
-    # RFC 5280, Section 4.2.1.12 Extended Key Usage
-    # RFC 5280, Section 4.2.1.13 CRL Distribution Points
-    # RFC 5280, Section 4.2.1.14 Inhibit Any-Policy
-    # RFC 5280, Section 4.2.1.15 Freshest CRL
-
-    cdef set_next(self, CRT crt):
-        self._next = crt
-        self._ctx.next = &crt._ctx
-
-    cdef unset_next(self):
-        self._ctx.next = NULL
-        self._next = None
-
-    def check_revocation(self, CRL crl):
-        """Return True if the certificate is revoked, False otherwise."""
-        return bool(x509.mbedtls_x509_crt_is_revoked(&self._ctx, &crl._ctx))
-
-    @classmethod
-    def from_file(cls, path):
-        path_ = str(Path(path)).encode("utf8")
-        cdef const char* c_path = path_
-        cdef CRT self = cls(None)
-        _exc.check_error(x509.mbedtls_x509_crt_parse_file(&self._ctx, c_path))
-        return self
-
-    @classmethod
-    def from_DER(cls, const unsigned char[:] buffer not None):
-        if buffer.size == 0:
-            raise ValueError("Cannot create %s from an empty buffer"
-                             % cls.__name__)
-        cdef CRT self = cls(None)
-        _exc.check_error(x509.mbedtls_x509_crt_parse_der(
-            &self._ctx, &buffer[0], buffer.size))
-        return self
-
-    @classmethod
-    def from_PEM(cls, pem):
-        return cls.from_DER(PEM_to_DER(pem))
-
-    def to_DER(self):
-        return bytes(self._ctx.raw.p[0:self._ctx.raw.len])
-
-    def to_PEM(self):
-        return DER_to_PEM(self.to_DER(), "Certificate")
-
-    def sign(self, csr, issuer_key, not_before, not_after, serial_number,
-             basic_constraints=BasicConstraints()):
-        """Return a new, signed certificate for the CSR."""
-        if not _pk.check_pair(
-                self.subject_public_key,
-                issuer_key):
-            raise ValueError(
-                "The issuer_key does not correspond to this certificate")
-        cdef CRT crt = self.new(
-            not_before=not_before,
-            not_after=not_after,
-            issuer=self.subject,
-            issuer_key=issuer_key,
-            subject=csr.subject,
-            subject_key=csr.subject_public_key,
-            serial_number=serial_number,
-            digestmod=csr.digestmod,
-            basic_constraints=basic_constraints)
-        return crt
-
-    @classmethod
-    def selfsign(cls, csr, issuer_key, not_before, not_after, serial_number,
-                 basic_constraints=BasicConstraints()):
-        """Return a new, self-signed certificate for the CSR."""
-        return cls.new(
-            not_before=not_before,
-            not_after=not_after,
-            issuer=csr.subject,
-            issuer_key=issuer_key,
-            subject=csr.subject,
-            subject_key=csr.subject_public_key,
-            serial_number=serial_number,
-            digestmod=csr.digestmod,
-            basic_constraints=basic_constraints)
-
-    def verify(self, crt):
-        """Verify the certificate `crt`."""
-        return self.subject_public_key.verify(
-            crt.tbs_certificate, crt.signature_value, crt.digestmod.name)
-
-    @staticmethod
-    def new(not_before, not_after, issuer, issuer_key, subject, subject_key,
-            serial_number, digestmod, basic_constraints=BasicConstraints()):
-        """Return a new certificate."""
-        return _CRTWriter(
-            not_before, not_after, issuer, issuer_key,
-            subject, subject_key, serial_number, digestmod,
-            basic_constraints=basic_constraints).to_certificate()
-
-
-cdef class _CRTWriter:
-    """CRT writing context.
-
-    This class should not be used directly.
-    Use `CRT.new()` instead.
-
-    """
-    def __init__(self, not_before, not_after, issuer, issuer_key,
-                 subject, subject_key, serial_number, digestmod,
-                 basic_constraints=BasicConstraints()):
-        super().__init__()
-        self.set_validity(not_before, not_after)
-        self.set_issuer(issuer)
-        self.set_issuer_key(issuer_key)
-        self.set_subject(subject)
-        self.set_subject_key(subject_key)
-        self.set_serial_number(serial_number)
-        self.set_digestmod(digestmod)
-        self.set_basic_constraints(basic_constraints)
-
-    def __cinit__(self):
-        """Initialize a CRT write context."""
-        x509.mbedtls_x509write_crt_init(&self._ctx)
-
-    def __dealloc__(self):
-        """Free the contents of a CRT write context."""
-        x509.mbedtls_x509write_crt_free(&self._ctx)
-
-    def __getstate__(self):
-        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
-
-    def to_DER(self):
-        """Return the certificate in DER format.
-
-        Warning:
-            No RNG function is used.
-
-        """
-        cdef size_t osize = 4096
-        cdef unsigned char *output = <unsigned char *>malloc(
-            osize * sizeof(unsigned char))
-        if not output:
-            raise MemoryError()
-        try:
-            written = _exc.check_error(x509.mbedtls_x509write_crt_der(
-                &self._ctx, &output[0], osize, NULL, NULL))
-            return output[osize - written:osize]
-        finally:
-            free(output)
-
-    def to_bytes(self):
-        return self.to_DER()
-
-    def to_certificate(self):
-        """Return a Certificate object."""
-        return CRT.from_DER(self.to_DER())
-
-    def set_version(self, version=3):
-        """Set the version for a certificate.
-
-        Arg:
-           version (int): The version between 1 and 3.
-
-        """
-        if version not in range(1, 4):
-            raise ValueError("version not between 1 and 3")
-        x509.mbedtls_x509write_crt_set_version(&self._ctx, version - 1)
-
-    def set_serial_number(self, serial_number):
-        """Set the serial number for a certificate.
-
-        Arg:
-            serial_number (int or bytes): The serial number.
-
-        """
-        if not serial_number:
-            return
-        cdef _mpi.MPI ser = _mpi.MPI(serial_number)
-        x509.mbedtls_x509write_crt_set_serial(&self._ctx, &ser._ctx)
-
-    def set_validity(self, not_before, not_after):
-        """Set the validity period for a certificate.
-
-        Args:
-            not_before (datetime): Begin timestamp.
-            not_after (datetime): End timestamp.
-
-        """
-        fmt = "%Y%m%d%H%M%S"
-        # Keep reference to Python objects.
-        not_before = not_before.strftime(fmt).encode("ascii")
-        not_after = not_after.strftime(fmt).encode("ascii")
-        cdef const char* c_not_before = not_before
-        cdef const char* c_not_after = not_after
-        _exc.check_error(x509.mbedtls_x509write_crt_set_validity(
-            &self._ctx, c_not_before, c_not_after))
-
-    def set_issuer(self, issuer):
-        """Set the issuer name.
-
-        Args:
-            issuer (str): Comma-separated list of OID types and values:
-                e.g. "C=UK,I=ARM,CN=mbed TLS CA"
-
-        """
-        # Keep reference to Python object.
-        issuer_ = issuer.encode("utf8")
-        cdef const char* c_issuer = issuer_
-        _exc.check_error(x509.mbedtls_x509write_crt_set_issuer_name(
-            &self._ctx, c_issuer))
-
-    def set_subject(self, subject):
-        """Set the subject name for a certificate.
-
-        Args:
-            subject (str): Subject name as a comma-separated list
-                of OID types and values.
-                e.g. "C=UK,O=ARM,CN=mbed TLS Server 1"
-
-        """
-        if subject is None:
-            return
-        # Keep reference to Python object.
-        subject_ = subject.encode("utf8")
-        cdef const char* c_subject = subject_
-        _exc.check_error(x509.mbedtls_x509write_crt_set_subject_name(
-            &self._ctx, c_subject))
-
-    def set_digestmod(self, digestmod):
-        """Set MD algorithm to use for the signature.
-
-        Args:
-            digestmod (MDBase): MD algorithm, for ex. `hash.sha1()`.
-
-        """
-        x509.mbedtls_x509write_crt_set_md_alg(&self._ctx, digestmod._type)
-
-    def set_subject_key(self, _pk.CipherBase key):
-        """Set the subject key.
-
-        Args:
-            key (CipherBase): Subject key.
-
-        """
-        x509.mbedtls_x509write_crt_set_subject_key(&self._ctx, &key._ctx)
-        _exc.check_error(
-            x509.mbedtls_x509write_crt_set_subject_key_identifier(&self._ctx))
-
-    def set_issuer_key(self, _pk.CipherBase key):
-        """Set the issuer key.
-
-        Args:
-            key (CipherBase): Issuer key.
-
-        """
-        x509.mbedtls_x509write_crt_set_issuer_key(
-            &self._ctx, &key._ctx)
-        _exc.check_error(
-            x509.mbedtls_x509write_crt_set_authority_key_identifier(&self._ctx)
-        )
-
-    def set_basic_constraints(self, basic_constraints):
-        """Set the basic constraints extension for a CRT.
-
-        Args:
-            basic_constraints (BasicConstraints): The basic constraints.
-
-        """
-        if not basic_constraints:
-            return
-        _exc.check_error(x509.mbedtls_x509write_crt_set_basic_constraints(
-            &self._ctx, int(basic_constraints[0]), basic_constraints[1]))
-
-
-cdef class CSR(Certificate):
-    """X.509 certificate signing request parser."""
-
-    def __init__(self, const unsigned char[:] buffer):
-        super().__init__()
-        if buffer is None or buffer.size == 0:
-            return
-        _exc.check_error(x509.mbedtls_x509_csr_parse(
-            &self._ctx, &buffer[0], buffer.size))
-
-    def __cinit__(self):
-        """Initialize a CSR."""
-        x509.mbedtls_x509_csr_init(&self._ctx)
-
-    def __dealloc__(self):
-        """Unallocate all CSR data."""
-        x509.mbedtls_x509_csr_free(&self._ctx)
-
-    def __str__(self):
-        cdef size_t osize = 2**24
-        cdef char *output = <char *>malloc(osize * sizeof(char))
-        cdef char *prefix = b""
-        if not output:
-            raise MemoryError()
-        try:
-            written = _exc.check_error(x509.mbedtls_x509_csr_info(
-                &output[0], osize, prefix, &self._ctx))
-            return output[:written].decode("utf8")
-        finally:
-            free(output)
-
-    @property
-    def digestmod(self):
-        """Return the hash function used for the signature.
-
-        See Also:
-            RFC5280, Section 4.1.1.2 Signature Algorithm.
-
-        """
-        return _new_hash(_md._digestmod(self._ctx.sig_md))
-
-    @property
-    def version(self):
-        """The version of the encoded certificate.
-
-        See Also:
-            RF 5280, Section 4.1.2.1 Version
-
-        """
-        return int(self._ctx.version)
-
-    @property
-    def subject(self):
-        """Entity associated with the public key.
-
-        See Also:
-            RFC 5280, Section 4.1.2.6 Subject
-
-        """
-        cdef size_t osize = 200
-        cdef char *c_buf = <char *>malloc(osize * sizeof(char))
-        if not c_buf:
-            raise MemoryError()
-        try:
-            written = x509.mbedtls_x509_dn_gets(
-                &c_buf[0], osize, &self._ctx.subject)
-            return c_buf[:written].decode("utf8")
-        finally:
-            free(c_buf)
-
-    @property
-    def subject_public_key(self):
-        """The public key.
-
-        See Also:
-            RFC 5280, Section 4.1.2.7 Subject Public Key Info
-
-        """
-        cipher_type = _pk.CipherType(_pk.mbedtls_pk_get_type(&self._ctx.pk))
-        cipher = {
-            _pk.CipherType.RSA: _pk.RSA,
-            _pk.CipherType.ECKEY: _pk.ECC,
-        }.get(cipher_type, None)
-        if cipher is None:
-            raise ValueError("unsupported cipher %r" % cipher_type)
-
-        cdef size_t osize = _pk.PUB_DER_MAX_BYTES
-        cdef unsigned char *c_buf = <unsigned char *>malloc(
-            osize * sizeof(unsigned char))
-        if not c_buf:
-            raise MemoryError()
-        try:
-            ret = _exc.check_error(_pk.mbedtls_pk_write_pubkey_der(
-                &self._ctx.pk, &c_buf[0], osize))
-            return cipher.from_DER(c_buf[osize - ret:osize])
-        finally:
-            free(c_buf)
-
-    @classmethod
-    def from_file(cls, path):
-        path_ = str(Path(path)).encode("utf8")
-        cdef const char* c_path = path_
-        cdef CSR self = cls(None)
-        _exc.check_error(x509.mbedtls_x509_csr_parse_file(&self._ctx, c_path))
-        return self
-
-    @classmethod
-    def from_DER(cls, const unsigned char[:] buffer not None):
-        if buffer.size == 0:
-            raise ValueError("Cannot create %s from an empty buffer"
-                             % cls.__name__)
-        cdef CSR self = cls(None)
-        _exc.check_error(x509.mbedtls_x509_csr_parse_der(
-            &self._ctx, &buffer[0], buffer.size))
-        return self
-
-    @classmethod
-    def from_PEM(cls, pem):
-        return cls.from_DER(PEM_to_DER(pem))
-
-    def to_DER(self):
-        return bytes(self._ctx.raw.p[0:self._ctx.raw.len])
-
-    def to_PEM(self):
-        return DER_to_PEM(self.to_DER(), "Certificate Request")
-
-    @staticmethod
-    def new(subject_key, subject, digestmod):
-        """Return a new CSR."""
-        return _CSRWriter(subject_key, subject, digestmod).to_certificate()
-
-
-cdef class _CSRWriter:
-    """X.509 CSR writing context.
-
-    This class should not be used directly.  Use `CSR.new()` instead.
-
-    """
-    def __init__(self, subject_key, subject, digestmod):
-        super().__init__()
-        self.set_subject_key(subject_key)
-        self.set_subject(subject)
-        self.set_digestmod(digestmod)
-
-    def __cinit__(self):
-        """Initialize a CSR context."""
-        x509.mbedtls_x509write_csr_init(&self._ctx)
-
-    def __dealloc__(self):
-        """Free the contents of a CSR context."""
-        x509.mbedtls_x509write_csr_free(&self._ctx)
-
-    def __getstate__(self):
-        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
-
-    def set_subject(self, subject):
-        """Set the subject name for a CSR.
-
-        Args:
-            subject (str): Subject name as a comma-separated list
-                of OID types and values.
-                e.g. "C=UK,O=ARM,CN=mbed TLS Server 1"
-
-        """
-        if not subject:
-            return
-        # Keep reference to Python object.
-        subject_ = subject.encode("utf8")
-        cdef const char* c_subject = subject_
-        _exc.check_error(x509.mbedtls_x509write_csr_set_subject_name(
-            &self._ctx, c_subject))
-
-    def set_subject_key(self, _pk.CipherBase key):
-        """Set the key for the CSR.
-
-        Args:
-            key (CipherBase): Asymetric key to include.
-
-        """
-        x509.mbedtls_x509write_csr_set_key(&self._ctx, &key._ctx)
-
-    def set_digestmod(self, digestmod):
-        """Set MD algorithm to use for the signature.
-
-        Args:
-            digestmod (MDBase): MD algorithm, for ex. `hash.sha1()`.
-
-        """
-        x509.mbedtls_x509write_csr_set_md_alg(&self._ctx, digestmod._type)
-
-    def to_DER(self):
-        """Return the CSR in DER format.
-
-        Warning:
-            No RNG function is used.
-
-        """
-        cdef size_t osize = 4096
-        cdef unsigned char *output = <unsigned char *>malloc(
-            osize * sizeof(unsigned char))
-        if not output:
-            raise MemoryError()
-        try:
-            written = _exc.check_error(x509.mbedtls_x509write_csr_der(
-                &self._ctx, &output[0], osize, NULL, NULL))
-            return output[osize - written:osize]
-        finally:
-            free(output)
-
-    def to_bytes(self):
-        return self.to_DER()
-
-    def to_certificate(self):
-        """Return a CSR object."""
-        return CSR.from_DER(self.to_DER())
-
-
-class CRLEntry(namedtuple("CRLEntry", ["serial", "revocation_date"])):
-    """An entry in the revocation list."""
-
-
-cdef class CRL(Certificate):
-    """X.509 revocation list."""
-
-    def __init__(self, const unsigned char[:] buffer):
-        super().__init__()
-        self._next = None
-        if buffer is None or buffer.size == 0:
-            return
-        _exc.check_error(x509.mbedtls_x509_crl_parse(
-            &self._ctx, &buffer[0], buffer.size))
-
-    def __cinit__(self):
-        """Initialize a CRL (chain)."""
-        x509.mbedtls_x509_crl_init(&self._ctx)
-
-    def __dealloc__(self):
-        """Unallocate all CRL data."""
-        self.unset_next()
-        x509.mbedtls_x509_crl_free(&self._ctx)
-
-    def __next__(self):
-        if self._next is None:
-            raise StopIteration
-        return self._next
-
-    def __str__(self):
-        cdef size_t osize = 2**24
-        cdef char *output = <char *>malloc(osize * sizeof(char))
-        cdef char *prefix = b""
-        if not output:
-            raise MemoryError()
-        try:
-            written = _exc.check_error(x509.mbedtls_x509_crl_info(
-                &output[0], osize, prefix, &self._ctx))
-            return output[:written].decode("utf8")
-        finally:
-            free(output)
-
-    # RFC 5280, Section 5.1 CRL Fields
-    # RFC 5280, Section 5.1.1 Certificate List Fields
-    @property
-    def tbs_certificate(self):
-        """The TBS (to be signed) certificate in DER format.
-
-        See Also:
-            RFC 5280, Section 5.1.1.1 TBS Certificate
-
-        """
-        return bytes(self._ctx.tbs.p[:self._ctx.tbs.len])
-
-    # RFC 5280, Section 5.1.1.2 Signature Algorithm
-
-    @property
-    def signature_value(self):
-        """Cryptographic algorithm used by the CA to sign this CRL.
-
-        See Also:
-            RFC 5280, Section 5.1.1.3 Signature Algorithm
-
-        """
-        return bytes(self._ctx.sig.p[:self._ctx.sig.len])
-
-    # RFC 5280, Section 5.1.2 Certificate List "To Be Signed"
-
-    @property
-    def version(self):
-        """The version of the encoded certificate.
-
-        See Also:
-            RF 5280, Section 5.1.2.1 Version
-
-        """
-        return int(self._ctx.version)
-
-    # RFC 5280, Section 5.1.2.2 Signature
-
-    @property
-    def issuer_name(self):
-        """Entity that has signed and issued the certificate.
-
-        See Also:
-            RFC 5280, Section 5.1.2.3 Issuer Name
-
-        """
-        cdef size_t osize = 200
-        cdef char* c_buf = <char *>malloc(osize * sizeof(char))
-        if not c_buf:
-            raise MemoryError()
-        try:
-            written = x509.mbedtls_x509_dn_gets(
-                &c_buf[0], osize, &self._ctx.issuer)
-            return c_buf[:written].decode("utf8")
-        finally:
-            free(c_buf)
-
-    @property
-    def this_update(self):
-        """The issue date of this certificate.
-
-        See Also:
-            RFC 5280, Section 5.1.2.4 This Update
-
-        """
-        cdef x509.mbedtls_x509_time *this_update = &self._ctx.this_update
-        return dt.datetime(
-            this_update[0].year, this_update[0].mon, this_update[0].day,
-            this_update[0].hour, this_update[0].min, this_update[0].sec)
-
-    @property
-    def next_update(self):
-        """The date by which the next certificate will be issued.
-
-        See Also:
-            RFC 5280, Section 5.1.2.5 Next Update
-
-        """
-        cdef x509.mbedtls_x509_time *next_update = &self._ctx.next_update
-        return dt.datetime(
-            next_update[0].year, next_update[0].mon, next_update[0].day,
-            next_update[0].hour, next_update[0].min, next_update[0].sec)
-
-    @property
-    def revoked_certificates(self):
-        """The list of revoked certificates.
-
-        See Also:
-            RFC 5280, Section 5.1.2.6 Revoked Certificates
-
-        """
-        cdef x509.mbedtls_x509_crl_entry *item
-        item = &self._ctx.entry
-        revoked = []
-        while item != NULL:
-            revoked.append(CRLEntry(
-                int(_mpi.MPI.from_bytes(
-                    item.serial.p[:item.serial.len], "big")),
-                dt.datetime(
-                    item.revocation_date.year,
-                    item.revocation_date.mon,
-                    item.revocation_date.day,
-                    item.revocation_date.hour,
-                    item.revocation_date.min,
-                    item.revocation_date.sec)))
-            item = item.next
-        return tuple(revoked)
-
-    @classmethod
-    def from_file(cls, path):
-        path_ = str(Path(path)).encode("utf8")
-        cdef const char* c_path = path_
-        cdef CRL self = cls(None)
-        _exc.check_error(x509.mbedtls_x509_crl_parse_file(&self._ctx, c_path))
-        return self
-
-    @classmethod
-    def from_DER(cls, const unsigned char[:] buffer not None):
-        if buffer.size == 0:
-            raise ValueError("Cannot create %s from an empty buffer"
-                             % cls.__name__)
-        cdef CRL self = cls(None)
-        _exc.check_error(x509.mbedtls_x509_crl_parse_der(
-            &self._ctx, &buffer[0], buffer.size))
-        return self
-
-    @classmethod
-    def from_PEM(cls, pem):
-        return cls.from_DER(PEM_to_DER(pem))
-
-    def to_DER(self):
-        return bytes(self._ctx.raw.p[0:self._ctx.raw.len])
-
-    def to_PEM(self):
-        return DER_to_PEM(self.to_DER(), "X509 CRL")
-
-    cdef set_next(self, CRL crl):
-        self._next = crl
-        self._ctx.next = &crl._ctx
-
-    cdef unset_next(self):
-        self._ctx.next = NULL
-        self._next = None
+# SPDX-License-Identifier: MIT
+# Copyright (c) 2018, Mathias Laurin
+
+"""Structure and functions for parsing and writing X.509 certificates."""
+
+
+from libc.stdlib cimport free, malloc
+
+cimport mbedtls.mpi as _mpi
+cimport mbedtls.pk as _pk
+cimport mbedtls.x509 as x509
+
+import base64
+import datetime as dt
+import enum
+from collections import namedtuple
+from pathlib import Path
+
+import mbedtls._md as _md
+import mbedtls.exceptions as _exc
+import mbedtls.mpi as _mpi
+import mbedtls.pk as _pk
+from mbedtls.hashlib import new as _new_hash
+
+
+@enum.unique
+class KeyUsage(enum.IntEnum):
+    """Key Usage Extension.
+
+    See Also:
+        RFC 5280 - 4.2.1.3 Key Usage.
+
+    """
+    DIGITAL_SIGNATURE = 0x80
+    NON_REPUDIATION = 0x40
+    KEY_ENCIPHERMENT = 0x20
+    DATA_ENCIPHERMENT = 0x10
+    KEY_AGREEMENT = 0x08
+    KEY_CERT_SIGN = 0x04
+    CRL_SIGN = 0x02
+    ENCIPHER_ONLY = 0x01
+    DECIPHER_ONLY = 0x8000
+
+
+def PEM_to_DER(pem):
+    return base64.b64decode(
+        b"".join(line.encode("ascii") for line in pem.splitlines()
+                 if not line.startswith("-----")))
+
+
+def DER_to_PEM(der, text):
+    chunk_size = 64
+    pem = base64.b64encode(der).decode("ascii")
+    return "\n".join((
+        "-----BEGIN %s-----" % text.upper(),
+        "\n".join(pem[n:n+chunk_size] for n in range(0, len(pem), chunk_size)),
+        "-----END %s-----" % text.upper(),
+        ""))
+
+
+cdef class Certificate:
+    @classmethod
+    def from_buffer(cls, buffer):
+        # PEP 543
+        return cls(buffer)
+
+    @classmethod
+    def from_file(cls, path):
+        # PEP 543
+        raise NotImplementedError
+
+    @classmethod
+    def from_DER(cls, der):
+        raise NotImplementedError
+
+    @classmethod
+    def from_PEM(cls, pem):
+        raise NotImplementedError
+
+    def __reduce__(self):
+        return type(self).from_DER, (bytes(self),)
+
+    def __hash__(self):
+        return hash(self.to_DER())
+
+    def __eq__(self, other):
+        if type(other) is type(self):
+            return self.to_DER() == other.to_DER()
+        else:
+            return other == self.to_DER() or other == self.to_PEM()
+
+    def __str__(self):
+        raise NotImplementedError
+
+    def __bytes__(self):
+        return self.to_DER()
+
+    def export(self, format="DER"):
+        if format == "DER":
+            return self.to_DER()
+        if format == "PEM":
+            return self.to_PEM()
+        raise ValueError(format)
+
+    def to_bytes(self):
+        return self.to_DER()
+
+    def to_DER(self):
+        raise NotImplementedError
+
+    def to_PEM(self):
+        raise NotImplementedError
+
+
+class BasicConstraints(
+        namedtuple("BasicConstraints", ["ca", "max_path_length"])):
+    """The basic constraints for the certificate."""
+
+    def __new__(cls, ca=False, max_path_length=0):
+        return super().__new__(cls, ca, max_path_length)
+
+
+cdef class CRT(Certificate):
+    """X.509 certificate."""
+
+    def __init__(self, const unsigned char[:] buffer):
+        super().__init__()
+        self._next = None
+        if buffer is None or buffer.size == 0:
+            return
+        _exc.check_error(x509.mbedtls_x509_crt_parse(
+            &self._ctx, &buffer[0], buffer.size))
+
+    def __cinit__(self):
+        """Initialize a certificate (chain)."""
+        x509.mbedtls_x509_crt_init(&self._ctx)
+
+    def __dealloc__(self):
+        """Unallocate all certificate data."""
+        self.unset_next()
+        x509.mbedtls_x509_crt_free(&self._ctx)
+
+    def __next__(self):
+        if self._next is None:
+            raise StopIteration
+        return self._next
+
+    def __str__(self):
+        cdef size_t osize = 2**24
+        cdef char *output = <char *>malloc(osize * sizeof(char))
+        cdef char *prefix = b""
+        if not output:
+            raise MemoryError()
+        try:
+            written = _exc.check_error(x509.mbedtls_x509_crt_info(
+                &output[0], osize, prefix, &self._ctx))
+            return output[:written].decode("utf8")
+        finally:
+            free(output)
+
+    # RFC 5280, Section 4.1 Basic Certificate Fields
+    # RFC 5280, Section 4.1.1 Certificate Fields
+
+    @property
+    def tbs_certificate(self):
+        """The TBS (to be signed) certificate in DER format.
+
+        See Also:
+            RFC 5280, Section 4.1.1.1 TBS Certificate
+
+        """
+        return bytes(self._ctx.tbs.p[:self._ctx.tbs.len])
+
+    @property
+    def _signature_algorithm(self):
+        """Cryptographic algorithm used by the CA to sign this CRT.
+
+        See Also:
+            RFC 5280, Section 4.1.1.2 Signature Algorithm
+
+        """
+        # The byte structure should be parsed according to RFC 5280.
+        return bytes(self._ctx.sig_oid.p[:self._ctx.sig_oid.len])
+
+    @property
+    def signature_value(self):
+        """Digital signature of the TBS certificate.
+
+        See Also:
+            RFC 5280, Section 4.1.1.3 Signature Value
+
+        """
+        return bytes(self._ctx.sig.p[:self._ctx.sig.len])
+
+    # RFC 5280, Section 4.1.2 TBS Certificate
+
+    @property
+    def version(self):
+        """The version of the encoded certificate.
+
+        See Also:
+            RF 5280, Section 4.1.2.1 Version
+
+        """
+        return int(self._ctx.version)
+
+    @property
+    def serial_number(self):
+        """The certificate serial number.
+
+        See Also:
+            RFC 5280, Section 4.1.2.2 Serial Number
+
+        """
+        return int(_mpi.MPI.from_bytes(
+            self._ctx.serial.p[:self._ctx.serial.len], "big"))
+
+    # RFC 4.1.2.3 Signature
+    @property
+    def digestmod(self):
+        return _new_hash(_md._digestmod(self._ctx.sig_md))
+
+    @property
+    def issuer(self):
+        """Entity that has signed and issued the certificate.
+
+        See Also:
+            RFC 5280, Section 4.1.2.4 Issuer
+
+        """
+        cdef size_t osize = 200
+        cdef char* c_buf = <char *>malloc(osize * sizeof(char))
+        if not c_buf:
+            raise MemoryError()
+        try:
+            written = x509.mbedtls_x509_dn_gets(
+                &c_buf[0], osize, &self._ctx.issuer)
+            return c_buf[:written].decode("utf8")
+        finally:
+            free(c_buf)
+
+    @property
+    def not_before(self):
+        """Beginning of the validity of the certificate (inclusive).
+
+        See Also:
+            RFC 5280, Section 4.1.2.5 Validity
+
+        """
+        cdef x509.mbedtls_x509_time *valid_from = &self._ctx.valid_from
+        return dt.datetime(
+            valid_from[0].year, valid_from[0].mon, valid_from[0].day,
+            valid_from[0].hour, valid_from[0].min, valid_from[0].sec)
+
+    @property
+    def not_after(self):
+        """End of the validity of the certificate (inclusive).
+
+        See Also:
+            RFC 5280, Section 4.1.2.5 Validity
+
+        """
+        cdef x509.mbedtls_x509_time *valid_to = &self._ctx.valid_to
+        return dt.datetime(
+            valid_to[0].year, valid_to[0].mon, valid_to[0].day,
+            valid_to[0].hour, valid_to[0].min, valid_to[0].sec)
+
+    @property
+    def subject(self):
+        """Entity associated with the public key.
+
+        See Also:
+            RFC 5280, Section 4.1.2.6 Subject
+
+        """
+        cdef size_t osize = 200
+        cdef char *c_buf = <char *>malloc(osize * sizeof(char))
+        if not c_buf:
+            raise MemoryError()
+        try:
+            written = x509.mbedtls_x509_dn_gets(
+                &c_buf[0], osize, &self._ctx.subject)
+            return c_buf[:written].decode("utf8")
+        finally:
+            free(c_buf)
+
+    @property
+    def subject_public_key(self):
+        """The public key.
+
+        See Also:
+            RFC 5280, Section 4.1.2.7 Subject Public Key Info
+
+        """
+        cipher_type = _pk.CipherType(_pk.mbedtls_pk_get_type(&self._ctx.pk))
+        cipher = {
+            _pk.CipherType.RSA: _pk.RSA,
+            _pk.CipherType.ECKEY: _pk.ECC,
+        }.get(cipher_type, None)
+        if cipher is None:
+            raise NotImplementedError("unsupported cipher %r" % cipher_type)
+
+        cdef size_t osize = _pk.PUB_DER_MAX_BYTES
+        cdef unsigned char *c_buf = <unsigned char *>malloc(
+            osize * sizeof(unsigned char))
+        if not c_buf:
+            raise MemoryError()
+        try:
+            ret = _exc.check_error(_pk.mbedtls_pk_write_pubkey_der(
+                &self._ctx.pk, &c_buf[0], osize))
+            return cipher.from_DER(c_buf[osize - ret:osize])
+        finally:
+            free(c_buf)
+
+    # RFC 5280, Section 4.1.2.8 Unique Identifiers
+    # RFC 5280, Section 4.1.2.9 Extensions
+    # RFC 5280, Section 4.2 Certificate Extensions
+    # RFC 5280, Section 4.2.1 Standard Extensions
+    # RFC 5280, Section 4.2.1.1 Authority Key Identifier
+    # RFC 5280, Section 4.2.1.2 Subject Key Identifier
+
+    @property
+    def key_usage(self):
+        """Key usage extension (bitfield).
+
+        See Also:
+            RFC 5280, Section 4.2.1.3 Key Usage
+
+        """
+        return KeyUsage(self._ctx.key_usage)
+
+    # RFC 5280, Section 4.2.1.4 Certificate Policies
+    # RFC 5280, Section 4.2.1.5 Policy Mappings
+
+    @property
+    def subject_alternative_names(self):
+        """Subject alternative name extension.
+
+        See Also:
+            RFC 5280, Section 4.2.1.6 Subject Alternative Name
+
+        """
+        cdef mbedtls_x509_sequence *item
+        item = &self._ctx.subject_alt_names
+        names = set()
+        while item != NULL:
+            names.add(item.buf.p[:item.buf.len].decode("utf8"))
+            item = item.next
+        return frozenset(names)
+
+    # RFC 5280, Section 4.2.1.7 Issuer Alternative Name
+    # RFC 5280, Section 4.2.1.8 Subject Directory Attributes
+
+    @property
+    def basic_constraints(self):
+        """ca is true if the certified public key may be used
+        to verify certificate signatures.
+
+        See Also:
+            - RFC 5280, Section 4.2.1.9 Basic Constraints
+            - RFC 5280, `max_path_length`
+
+        """
+        max_path_length = int(self._ctx.max_pathlen)
+        if max_path_length > 0:
+            max_path_length -= 1
+        ca = bool(self._ctx.ca_istrue)
+        return BasicConstraints(ca, max_path_length)
+
+    # RFC 5280, Section 4.2.1.10 Name Constraints
+    # RFC 5280, Section 4.2.1.11 Policy Constraints
+    # RFC 5280, Section 4.2.1.12 Extended Key Usage
+    # RFC 5280, Section 4.2.1.13 CRL Distribution Points
+    # RFC 5280, Section 4.2.1.14 Inhibit Any-Policy
+    # RFC 5280, Section 4.2.1.15 Freshest CRL
+
+    cdef set_next(self, CRT crt):
+        self._next = crt
+        self._ctx.next = &crt._ctx
+
+    cdef unset_next(self):
+        self._ctx.next = NULL
+        self._next = None
+
+    def check_revocation(self, CRL crl):
+        """Return True if the certificate is revoked, False otherwise."""
+        return bool(x509.mbedtls_x509_crt_is_revoked(&self._ctx, &crl._ctx))
+
+    @classmethod
+    def from_file(cls, path):
+        path_ = str(Path(path)).encode("utf8")
+        cdef const char* c_path = path_
+        cdef CRT self = cls(None)
+        _exc.check_error(x509.mbedtls_x509_crt_parse_file(&self._ctx, c_path))
+        return self
+
+    @classmethod
+    def from_DER(cls, const unsigned char[:] buffer not None):
+        if buffer.size == 0:
+            raise ValueError("Cannot create %s from an empty buffer"
+                             % cls.__name__)
+        cdef CRT self = cls(None)
+        _exc.check_error(x509.mbedtls_x509_crt_parse_der(
+            &self._ctx, &buffer[0], buffer.size))
+        return self
+
+    @classmethod
+    def from_PEM(cls, pem):
+        return cls.from_DER(PEM_to_DER(pem))
+
+    def to_DER(self):
+        return bytes(self._ctx.raw.p[0:self._ctx.raw.len])
+
+    def to_PEM(self):
+        return DER_to_PEM(self.to_DER(), "Certificate")
+
+    def sign(self, csr, issuer_key, not_before, not_after, serial_number,
+             basic_constraints=BasicConstraints()):
+        """Return a new, signed certificate for the CSR."""
+        if not _pk.check_pair(
+                self.subject_public_key,
+                issuer_key):
+            raise ValueError(
+                "The issuer_key does not correspond to this certificate")
+        cdef CRT crt = self.new(
+            not_before=not_before,
+            not_after=not_after,
+            issuer=self.subject,
+            issuer_key=issuer_key,
+            subject=csr.subject,
+            subject_key=csr.subject_public_key,
+            serial_number=serial_number,
+            digestmod=csr.digestmod,
+            basic_constraints=basic_constraints)
+        return crt
+
+    @classmethod
+    def selfsign(cls, csr, issuer_key, not_before, not_after, serial_number,
+                 basic_constraints=BasicConstraints()):
+        """Return a new, self-signed certificate for the CSR."""
+        return cls.new(
+            not_before=not_before,
+            not_after=not_after,
+            issuer=csr.subject,
+            issuer_key=issuer_key,
+            subject=csr.subject,
+            subject_key=csr.subject_public_key,
+            serial_number=serial_number,
+            digestmod=csr.digestmod,
+            basic_constraints=basic_constraints)
+
+    def verify(self, crt):
+        """Verify the certificate `crt`."""
+        return self.subject_public_key.verify(
+            crt.tbs_certificate, crt.signature_value, crt.digestmod.name)
+
+    @staticmethod
+    def new(not_before, not_after, issuer, issuer_key, subject, subject_key,
+            serial_number, digestmod, basic_constraints=BasicConstraints()):
+        """Return a new certificate."""
+        return _CRTWriter(
+            not_before, not_after, issuer, issuer_key,
+            subject, subject_key, serial_number, digestmod,
+            basic_constraints=basic_constraints).to_certificate()
+
+
+cdef class _CRTWriter:
+    """CRT writing context.
+
+    This class should not be used directly.
+    Use `CRT.new()` instead.
+
+    """
+    def __init__(self, not_before, not_after, issuer, issuer_key,
+                 subject, subject_key, serial_number, digestmod,
+                 basic_constraints=BasicConstraints()):
+        super().__init__()
+        self.set_validity(not_before, not_after)
+        self.set_issuer(issuer)
+        self.set_issuer_key(issuer_key)
+        self.set_subject(subject)
+        self.set_subject_key(subject_key)
+        self.set_serial_number(serial_number)
+        self.set_digestmod(digestmod)
+        self.set_basic_constraints(basic_constraints)
+
+    def __cinit__(self):
+        """Initialize a CRT write context."""
+        x509.mbedtls_x509write_crt_init(&self._ctx)
+
+    def __dealloc__(self):
+        """Free the contents of a CRT write context."""
+        x509.mbedtls_x509write_crt_free(&self._ctx)
+
+    def __getstate__(self):
+        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
+
+    def to_DER(self):
+        """Return the certificate in DER format.
+
+        Warning:
+            No RNG function is used.
+
+        """
+        cdef size_t osize = 4096
+        cdef unsigned char *output = <unsigned char *>malloc(
+            osize * sizeof(unsigned char))
+        if not output:
+            raise MemoryError()
+        try:
+            written = _exc.check_error(x509.mbedtls_x509write_crt_der(
+                &self._ctx, &output[0], osize, NULL, NULL))
+            return output[osize - written:osize]
+        finally:
+            free(output)
+
+    def to_bytes(self):
+        return self.to_DER()
+
+    def to_certificate(self):
+        """Return a Certificate object."""
+        return CRT.from_DER(self.to_DER())
+
+    def set_version(self, version=3):
+        """Set the version for a certificate.
+
+        Arg:
+           version (int): The version between 1 and 3.
+
+        """
+        if version not in range(1, 4):
+            raise ValueError("version not between 1 and 3")
+        x509.mbedtls_x509write_crt_set_version(&self._ctx, version - 1)
+
+    def set_serial_number(self, serial_number):
+        """Set the serial number for a certificate.
+
+        Arg:
+            serial_number (int or bytes): The serial number.
+
+        """
+        if not serial_number:
+            return
+        cdef _mpi.MPI ser = _mpi.MPI(serial_number)
+        x509.mbedtls_x509write_crt_set_serial(&self._ctx, &ser._ctx)
+
+    def set_validity(self, not_before, not_after):
+        """Set the validity period for a certificate.
+
+        Args:
+            not_before (datetime): Begin timestamp.
+            not_after (datetime): End timestamp.
+
+        """
+        fmt = "%Y%m%d%H%M%S"
+        # Keep reference to Python objects.
+        not_before = not_before.strftime(fmt).encode("ascii")
+        not_after = not_after.strftime(fmt).encode("ascii")
+        cdef const char* c_not_before = not_before
+        cdef const char* c_not_after = not_after
+        _exc.check_error(x509.mbedtls_x509write_crt_set_validity(
+            &self._ctx, c_not_before, c_not_after))
+
+    def set_issuer(self, issuer):
+        """Set the issuer name.
+
+        Args:
+            issuer (str): Comma-separated list of OID types and values:
+                e.g. "C=UK,I=ARM,CN=mbed TLS CA"
+
+        """
+        # Keep reference to Python object.
+        issuer_ = issuer.encode("utf8")
+        cdef const char* c_issuer = issuer_
+        _exc.check_error(x509.mbedtls_x509write_crt_set_issuer_name(
+            &self._ctx, c_issuer))
+
+    def set_subject(self, subject):
+        """Set the subject name for a certificate.
+
+        Args:
+            subject (str): Subject name as a comma-separated list
+                of OID types and values.
+                e.g. "C=UK,O=ARM,CN=mbed TLS Server 1"
+
+        """
+        if subject is None:
+            return
+        # Keep reference to Python object.
+        subject_ = subject.encode("utf8")
+        cdef const char* c_subject = subject_
+        _exc.check_error(x509.mbedtls_x509write_crt_set_subject_name(
+            &self._ctx, c_subject))
+
+    def set_digestmod(self, digestmod):
+        """Set MD algorithm to use for the signature.
+
+        Args:
+            digestmod (MDBase): MD algorithm, for ex. `hash.sha1()`.
+
+        """
+        x509.mbedtls_x509write_crt_set_md_alg(&self._ctx, digestmod._type)
+
+    def set_subject_key(self, _pk.CipherBase key):
+        """Set the subject key.
+
+        Args:
+            key (CipherBase): Subject key.
+
+        """
+        x509.mbedtls_x509write_crt_set_subject_key(&self._ctx, &key._ctx)
+        _exc.check_error(
+            x509.mbedtls_x509write_crt_set_subject_key_identifier(&self._ctx))
+
+    def set_issuer_key(self, _pk.CipherBase key):
+        """Set the issuer key.
+
+        Args:
+            key (CipherBase): Issuer key.
+
+        """
+        x509.mbedtls_x509write_crt_set_issuer_key(
+            &self._ctx, &key._ctx)
+        _exc.check_error(
+            x509.mbedtls_x509write_crt_set_authority_key_identifier(&self._ctx)
+        )
+
+    def set_basic_constraints(self, basic_constraints):
+        """Set the basic constraints extension for a CRT.
+
+        Args:
+            basic_constraints (BasicConstraints): The basic constraints.
+
+        """
+        if not basic_constraints:
+            return
+        _exc.check_error(x509.mbedtls_x509write_crt_set_basic_constraints(
+            &self._ctx, int(basic_constraints[0]), basic_constraints[1]))
+
+
+cdef class CSR(Certificate):
+    """X.509 certificate signing request parser."""
+
+    def __init__(self, const unsigned char[:] buffer):
+        super().__init__()
+        if buffer is None or buffer.size == 0:
+            return
+        _exc.check_error(x509.mbedtls_x509_csr_parse(
+            &self._ctx, &buffer[0], buffer.size))
+
+    def __cinit__(self):
+        """Initialize a CSR."""
+        x509.mbedtls_x509_csr_init(&self._ctx)
+
+    def __dealloc__(self):
+        """Unallocate all CSR data."""
+        x509.mbedtls_x509_csr_free(&self._ctx)
+
+    def __str__(self):
+        cdef size_t osize = 2**24
+        cdef char *output = <char *>malloc(osize * sizeof(char))
+        cdef char *prefix = b""
+        if not output:
+            raise MemoryError()
+        try:
+            written = _exc.check_error(x509.mbedtls_x509_csr_info(
+                &output[0], osize, prefix, &self._ctx))
+            return output[:written].decode("utf8")
+        finally:
+            free(output)
+
+    @property
+    def digestmod(self):
+        """Return the hash function used for the signature.
+
+        See Also:
+            RFC5280, Section 4.1.1.2 Signature Algorithm.
+
+        """
+        return _new_hash(_md._digestmod(self._ctx.sig_md))
+
+    @property
+    def version(self):
+        """The version of the encoded certificate.
+
+        See Also:
+            RF 5280, Section 4.1.2.1 Version
+
+        """
+        return int(self._ctx.version)
+
+    @property
+    def subject(self):
+        """Entity associated with the public key.
+
+        See Also:
+            RFC 5280, Section 4.1.2.6 Subject
+
+        """
+        cdef size_t osize = 200
+        cdef char *c_buf = <char *>malloc(osize * sizeof(char))
+        if not c_buf:
+            raise MemoryError()
+        try:
+            written = x509.mbedtls_x509_dn_gets(
+                &c_buf[0], osize, &self._ctx.subject)
+            return c_buf[:written].decode("utf8")
+        finally:
+            free(c_buf)
+
+    @property
+    def subject_public_key(self):
+        """The public key.
+
+        See Also:
+            RFC 5280, Section 4.1.2.7 Subject Public Key Info
+
+        """
+        cipher_type = _pk.CipherType(_pk.mbedtls_pk_get_type(&self._ctx.pk))
+        cipher = {
+            _pk.CipherType.RSA: _pk.RSA,
+            _pk.CipherType.ECKEY: _pk.ECC,
+        }.get(cipher_type, None)
+        if cipher is None:
+            raise ValueError("unsupported cipher %r" % cipher_type)
+
+        cdef size_t osize = _pk.PUB_DER_MAX_BYTES
+        cdef unsigned char *c_buf = <unsigned char *>malloc(
+            osize * sizeof(unsigned char))
+        if not c_buf:
+            raise MemoryError()
+        try:
+            ret = _exc.check_error(_pk.mbedtls_pk_write_pubkey_der(
+                &self._ctx.pk, &c_buf[0], osize))
+            return cipher.from_DER(c_buf[osize - ret:osize])
+        finally:
+            free(c_buf)
+
+    @classmethod
+    def from_file(cls, path):
+        path_ = str(Path(path)).encode("utf8")
+        cdef const char* c_path = path_
+        cdef CSR self = cls(None)
+        _exc.check_error(x509.mbedtls_x509_csr_parse_file(&self._ctx, c_path))
+        return self
+
+    @classmethod
+    def from_DER(cls, const unsigned char[:] buffer not None):
+        if buffer.size == 0:
+            raise ValueError("Cannot create %s from an empty buffer"
+                             % cls.__name__)
+        cdef CSR self = cls(None)
+        _exc.check_error(x509.mbedtls_x509_csr_parse_der(
+            &self._ctx, &buffer[0], buffer.size))
+        return self
+
+    @classmethod
+    def from_PEM(cls, pem):
+        return cls.from_DER(PEM_to_DER(pem))
+
+    def to_DER(self):
+        return bytes(self._ctx.raw.p[0:self._ctx.raw.len])
+
+    def to_PEM(self):
+        return DER_to_PEM(self.to_DER(), "Certificate Request")
+
+    @staticmethod
+    def new(subject_key, subject, digestmod):
+        """Return a new CSR."""
+        return _CSRWriter(subject_key, subject, digestmod).to_certificate()
+
+
+cdef class _CSRWriter:
+    """X.509 CSR writing context.
+
+    This class should not be used directly.  Use `CSR.new()` instead.
+
+    """
+    def __init__(self, subject_key, subject, digestmod):
+        super().__init__()
+        self.set_subject_key(subject_key)
+        self.set_subject(subject)
+        self.set_digestmod(digestmod)
+
+    def __cinit__(self):
+        """Initialize a CSR context."""
+        x509.mbedtls_x509write_csr_init(&self._ctx)
+
+    def __dealloc__(self):
+        """Free the contents of a CSR context."""
+        x509.mbedtls_x509write_csr_free(&self._ctx)
+
+    def __getstate__(self):
+        raise TypeError(f"cannot pickle {self.__class__.__name__!r} object")
+
+    def set_subject(self, subject):
+        """Set the subject name for a CSR.
+
+        Args:
+            subject (str): Subject name as a comma-separated list
+                of OID types and values.
+                e.g. "C=UK,O=ARM,CN=mbed TLS Server 1"
+
+        """
+        if not subject:
+            return
+        # Keep reference to Python object.
+        subject_ = subject.encode("utf8")
+        cdef const char* c_subject = subject_
+        _exc.check_error(x509.mbedtls_x509write_csr_set_subject_name(
+            &self._ctx, c_subject))
+
+    def set_subject_key(self, _pk.CipherBase key):
+        """Set the key for the CSR.
+
+        Args:
+            key (CipherBase): Asymetric key to include.
+
+        """
+        x509.mbedtls_x509write_csr_set_key(&self._ctx, &key._ctx)
+
+    def set_digestmod(self, digestmod):
+        """Set MD algorithm to use for the signature.
+
+        Args:
+            digestmod (MDBase): MD algorithm, for ex. `hash.sha1()`.
+
+        """
+        x509.mbedtls_x509write_csr_set_md_alg(&self._ctx, digestmod._type)
+
+    def to_DER(self):
+        """Return the CSR in DER format.
+
+        Warning:
+            No RNG function is used.
+
+        """
+        cdef size_t osize = 4096
+        cdef unsigned char *output = <unsigned char *>malloc(
+            osize * sizeof(unsigned char))
+        if not output:
+            raise MemoryError()
+        try:
+            written = _exc.check_error(x509.mbedtls_x509write_csr_der(
+                &self._ctx, &output[0], osize, NULL, NULL))
+            return output[osize - written:osize]
+        finally:
+            free(output)
+
+    def to_bytes(self):
+        return self.to_DER()
+
+    def to_certificate(self):
+        """Return a CSR object."""
+        return CSR.from_DER(self.to_DER())
+
+
+class CRLEntry(namedtuple("CRLEntry", ["serial", "revocation_date"])):
+    """An entry in the revocation list."""
+
+
+cdef class CRL(Certificate):
+    """X.509 revocation list."""
+
+    def __init__(self, const unsigned char[:] buffer):
+        super().__init__()
+        self._next = None
+        if buffer is None or buffer.size == 0:
+            return
+        _exc.check_error(x509.mbedtls_x509_crl_parse(
+            &self._ctx, &buffer[0], buffer.size))
+
+    def __cinit__(self):
+        """Initialize a CRL (chain)."""
+        x509.mbedtls_x509_crl_init(&self._ctx)
+
+    def __dealloc__(self):
+        """Unallocate all CRL data."""
+        self.unset_next()
+        x509.mbedtls_x509_crl_free(&self._ctx)
+
+    def __next__(self):
+        if self._next is None:
+            raise StopIteration
+        return self._next
+
+    def __str__(self):
+        cdef size_t osize = 2**24
+        cdef char *output = <char *>malloc(osize * sizeof(char))
+        cdef char *prefix = b""
+        if not output:
+            raise MemoryError()
+        try:
+            written = _exc.check_error(x509.mbedtls_x509_crl_info(
+                &output[0], osize, prefix, &self._ctx))
+            return output[:written].decode("utf8")
+        finally:
+            free(output)
+
+    # RFC 5280, Section 5.1 CRL Fields
+    # RFC 5280, Section 5.1.1 Certificate List Fields
+    @property
+    def tbs_certificate(self):
+        """The TBS (to be signed) certificate in DER format.
+
+        See Also:
+            RFC 5280, Section 5.1.1.1 TBS Certificate
+
+        """
+        return bytes(self._ctx.tbs.p[:self._ctx.tbs.len])
+
+    # RFC 5280, Section 5.1.1.2 Signature Algorithm
+
+    @property
+    def signature_value(self):
+        """Cryptographic algorithm used by the CA to sign this CRL.
+
+        See Also:
+            RFC 5280, Section 5.1.1.3 Signature Algorithm
+
+        """
+        return bytes(self._ctx.sig.p[:self._ctx.sig.len])
+
+    # RFC 5280, Section 5.1.2 Certificate List "To Be Signed"
+
+    @property
+    def version(self):
+        """The version of the encoded certificate.
+
+        See Also:
+            RF 5280, Section 5.1.2.1 Version
+
+        """
+        return int(self._ctx.version)
+
+    # RFC 5280, Section 5.1.2.2 Signature
+
+    @property
+    def issuer_name(self):
+        """Entity that has signed and issued the certificate.
+
+        See Also:
+            RFC 5280, Section 5.1.2.3 Issuer Name
+
+        """
+        cdef size_t osize = 200
+        cdef char* c_buf = <char *>malloc(osize * sizeof(char))
+        if not c_buf:
+            raise MemoryError()
+        try:
+            written = x509.mbedtls_x509_dn_gets(
+                &c_buf[0], osize, &self._ctx.issuer)
+            return c_buf[:written].decode("utf8")
+        finally:
+            free(c_buf)
+
+    @property
+    def this_update(self):
+        """The issue date of this certificate.
+
+        See Also:
+            RFC 5280, Section 5.1.2.4 This Update
+
+        """
+        cdef x509.mbedtls_x509_time *this_update = &self._ctx.this_update
+        return dt.datetime(
+            this_update[0].year, this_update[0].mon, this_update[0].day,
+            this_update[0].hour, this_update[0].min, this_update[0].sec)
+
+    @property
+    def next_update(self):
+        """The date by which the next certificate will be issued.
+
+        See Also:
+            RFC 5280, Section 5.1.2.5 Next Update
+
+        """
+        cdef x509.mbedtls_x509_time *next_update = &self._ctx.next_update
+        return dt.datetime(
+            next_update[0].year, next_update[0].mon, next_update[0].day,
+            next_update[0].hour, next_update[0].min, next_update[0].sec)
+
+    @property
+    def revoked_certificates(self):
+        """The list of revoked certificates.
+
+        See Also:
+            RFC 5280, Section 5.1.2.6 Revoked Certificates
+
+        """
+        cdef x509.mbedtls_x509_crl_entry *item
+        item = &self._ctx.entry
+        revoked = []
+        while item != NULL:
+            revoked.append(CRLEntry(
+                int(_mpi.MPI.from_bytes(
+                    item.serial.p[:item.serial.len], "big")),
+                dt.datetime(
+                    item.revocation_date.year,
+                    item.revocation_date.mon,
+                    item.revocation_date.day,
+                    item.revocation_date.hour,
+                    item.revocation_date.min,
+                    item.revocation_date.sec)))
+            item = item.next
+        return tuple(revoked)
+
+    @classmethod
+    def from_file(cls, path):
+        path_ = str(Path(path)).encode("utf8")
+        cdef const char* c_path = path_
+        cdef CRL self = cls(None)
+        _exc.check_error(x509.mbedtls_x509_crl_parse_file(&self._ctx, c_path))
+        return self
+
+    @classmethod
+    def from_DER(cls, const unsigned char[:] buffer not None):
+        if buffer.size == 0:
+            raise ValueError("Cannot create %s from an empty buffer"
+                             % cls.__name__)
+        cdef CRL self = cls(None)
+        _exc.check_error(x509.mbedtls_x509_crl_parse_der(
+            &self._ctx, &buffer[0], buffer.size))
+        return self
+
+    @classmethod
+    def from_PEM(cls, pem):
+        return cls.from_DER(PEM_to_DER(pem))
+
+    def to_DER(self):
+        return bytes(self._ctx.raw.p[0:self._ctx.raw.len])
+
+    def to_PEM(self):
+        return DER_to_PEM(self.to_DER(), "X509 CRL")
+
+    cdef set_next(self, CRL crl):
+        self._next = crl
+        self._ctx.next = &crl._ctx
+
+    cdef unset_next(self):
+        self._ctx.next = NULL
+        self._next = None
```

### Comparing `python-mbedtls-2.7.0/src/python_mbedtls.egg-info/PKG-INFO` & `python-mbedtls-2.7.1/src/python_mbedtls.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,444 +1,444 @@
-Metadata-Version: 2.1
-Name: python-mbedtls
-Version: 2.7.0
-Summary: hash, hmac, RSA, ECC, X.509, TLS, DTLS, handshakes, and secrets with an mbed TLS back end
-Home-page: https://github.com/Synss/python-mbedtls
-Download-URL: https://github.com/Synss/python-mbedtls/tarball/2.7.0
-Author: Mathias Laurin
-Author-email: Mathias.Laurin@github.com
-License: MIT License
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Cython
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Security :: Cryptography
-Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-
-.. vim:tw=72
-
-=======================================================
-Cryptographic library for Python with Mbed TLS back end
-=======================================================
-
-.. image:: https://results.pre-commit.ci/badge/github/Synss/python-mbedtls/master.svg
-   :target: https://results.pre-commit.ci/latest/github/Synss/python-mbedtls/master
-   :alt: pre-commit.ci status
-
-.. image::
-   https://github.com/Synss/python-mbedtls/actions/workflows/main.yml/badge.svg?branch=master
-   :target: https://github.com/Synss/python-mbedtls/actions/
-
-.. image::
-   https://coveralls.io/repos/github/Synss/python-mbedtls/badge.svg?branch=master
-   :target: https://coveralls.io/github/Synss/python-mbedtls?branch=master
-
-
-`python-mbedtls`_ is a free cryptographic library for Python that uses
-`mbed TLS`_ for back end.
-
-   mbed TLS (formerly known as PolarSSL) makes it trivially easy for
-   developers to include cryptographic and SSL/TLS capabilities in their
-   (embedded) products, facilitating this functionality with a minimal
-   coding footprint.
-
-*python-mbedtls* API follows the recommendations from:
-
-* `PEP 272`_ -- API for Block Encryption Algorithms v1.0
-* `PEP 452`_ -- API for Cryptographic Hash Functions v2.0
-* `PEP 506`_ -- Adding a Secret Module to the Standard Library
-* `PEP 543`_ -- A Unified TLS API for Python (`completed and modernized`_)
-
-and therefore plays well with the `cryptographic services`_ from the
-Python standard library and many other cryptography libraries as well.
-
-.. _python-mbedtls: https://synss.github.io/python-mbedtls
-.. _mbed TLS: https://tls.mbed.org
-.. _PEP 272: https://www.python.org/dev/peps/pep-0272/
-.. _PEP 452: https://www.python.org/dev/peps/pep-0452/
-.. _PEP 506: https://www.python.org/dev/peps/pep-0506/
-.. _PEP 543: https://www.python.org/dev/peps/pep-0543/
-.. _cryptographic services: https://docs.python.org/3/library/crypto.html
-.. _PyCrypto: https://www.dlitz.net/software/pycrypto/
-.. _hashlib: https://docs.python.org/3.6/library/hashlib.html
-.. _hmac: https://docs.python.org/3.6/library/hmac.html
-.. _completed and modernized: https://github.com/Synss/python-mbedtls/blob/master/src/mbedtls/_tlsi.py
-
-
-License
-=======
-
-*python-mbedtls* is licensed under the MIT License (see LICENSE.txt).
-This enables the use of *python-mbedtls* in both open source and closed
-source projects.  The MIT License is compatible with both GPL and Apache
-2.0 license under which mbed TLS is distributed.
-
-
-API documentation
-=================
-
-https://synss.github.io/python-mbedtls/
-
-
-Installation
-============
-
-The bindings are tested with mbedTLS 2.28.3 for Python 3.7,
-3.8, 3.9, 3.10, and 3.11 on Linux, macOS, and Windows.
-
-`manylinux`_ wheels are available for 64-bit Linux systems.  Install
-with ``pip install python-mbedtls``.
-
-.. _manylinux: https://www.python.org/dev/peps/pep-0513/
-
-
-Usage and examples
-==================
-
-Now, let us see examples using the various parts of the library.
-
-
-Check which version of mbed TLS is being used by python-mbedtls
----------------------------------------------------------------
-
-The *mbedtls.version* module shows the run-time version
-information to mbed TLS.
-
->>> from mbedtls import version
->>> _ = version.version  # "mbed TLS 2.28.3"
->>> _ = version.version_info  # (2, 28, 3)
-
-
-Message digest
---------------
-
-The *mbedtls.hashlib* module supports MD2, MD4, MD5, SHA-1, SHA-2
-(in 224, 256, 384, and 512-bits), and RIPEMD-160 secure hashes
-and message digests.  Note that MD2 and MD4 are not included
-by default and are only present if they are compiled in mbedtls.
-
-Here are the examples from (standard) *hashlib* ported
-to *python-mbedtls*:
-
->>> from mbedtls import hashlib
->>> m = hashlib.md5()
->>> m.update(b"Nobody inspects")
->>> m.update(b" the spammish repetition")
->>> m.digest()
-b'\xbbd\x9c\x83\xdd\x1e\xa5\xc9\xd9\xde\xc9\xa1\x8d\xf0\xff\xe9'
->>> m.digest_size
-16
->>> m.block_size
-64
-
-More condensed:
-
->>> hashlib.sha224(b"Nobody inspects the spammish repetition").hexdigest()
-'a4337bc45a8fc544c03f52dc550cd6e1e87021bc896588bd79e901e2'
-
-Using ``new()``:
-
->>> h = hashlib.new('ripemd160')
->>> h.update(b"Nobody inspects the spammish repetition")
->>> h.hexdigest()
-'cc4a5ce1b3df48aec5d22d1f16b894a0b894eccc'
-
-
-HMAC algorithm
---------------
-
-The *mbedtls.hmac* module computes HMAC.
-
-Example:
-
->>> from mbedtls import hmac
->>> m = hmac.new(b"This is my secret key", digestmod="md5")
->>> m.update(b"Nobody inspects")
->>> m.update(b" the spammish repetition")
->>> m.digest()
-b'\x9d-/rj\\\x98\x80\xb1rG\x87\x0f\xe9\xe4\xeb'
-
-Warning:
-
-The message is cleared after calculation of the digest.  Only call
-``mbedtls.hmac.Hmac.digest()`` or ``mbedtls.hmac.Hmac.hexdigest()``
-once per message.
-
-
-HMAC-based key derivation function (HKDF)
------------------------------------------
-
-The *mbedtls.hkdf* module exposes extract-and-expand key derivation
-functions.  The main function is ``hkdf()`` but ``extract()`` and
-``expand()`` may be used as well.
-
-Example:
-
->>> from mbedtls import hkdf
->>> hkdf.hkdf(
-...     b"my secret key",
-...     length=42,
-...     info=b"my cool app",
-...     salt=b"and pepper",
-...     digestmod=hmac.sha256
-... )
-b'v,\xef\x90\xccU\x1d\x1b\xd7\\a\xaf\x92\xac\n\x90\xf9q\xf4)\xcd"\xf7\x1a\x94p\x03.\xa8e\x1e\xfb\x92\xe8l\x0cc\xf8e\rvj'
-
-where *info*, *salt*, and *digestmod* are optional, although providing
-(at least) *info* is highly recommended.
-
-
-Symmetric cipher
-----------------
-
-The *mbedtls.cipher* module provides symmetric encryption.  The API
-follows the recommendations from PEP 272 so that it can be used as a
-drop-in replacement to other libraries.
-
-*python-mbedtls* provides the following algorithms:
-
-- AES encryption/decryption (128, 192, and 256 bits) in ECB, CBC, CFB128,
-  CTR, OFB, or XTS mode;
-- AES AEAD (128, 192, and 256 bits) in GCM or CCM mode;
-- ARC4 encryption/decryption;
-- ARIA encryption/decryption (128, 192, and 256 bits) in ECB, CBC,
-  CTR, or GCM modes;
-- Blowfish encryption/decryption in ECB, CBC, CFB64, or CTR mode;
-- Camellia encryption/decryption (128, 192, and 256 bits) in ECB, CBC,
-  CFB128, CTR, or GCM mode;
-- DES, DES3, and double DES3 encryption/decryption in ECB or CBC mode;
-- CHACHA20 and CHACHA20/POLY1305 encryption/decryption.
-
-Example:
-
->>> from mbedtls import cipher
->>> c = cipher.AES.new(b"My 16-bytes key.", cipher.MODE_CBC, b"CBC needs an IV.")
->>> enc = c.encrypt(b"This is a super-secret message!!")
->>> enc
-b"*`k6\x98\x97=[\xdf\x7f\x88\x96\xf5\t\x19J\xf62h\xf4n\xca\xe8\xfe\xf5\xd7X'\xb1\x8c\xc9\x85"
->>> c.decrypt(enc)
-b'This is a super-secret message!!'
-
-
-RSA public key
---------------
-
-The *mbedtls.pk* module provides the RSA cryptosystem.  This includes:
-
-- Public-private key generation and key import/export in PEM and DER
-  formats;
-- asymmetric encryption and decryption;
-- message signature and verification.
-
-Key generation, the default size is 2048 bits:
-
->>> from mbedtls import pk
->>> rsa = pk.RSA()
->>> prv = rsa.generate()
->>> rsa.key_size
-256
-
-Message encryption and decryption:
-
->>> enc = rsa.encrypt(b"secret message")
->>> rsa.decrypt(enc)
-b'secret message'
-
-Message signature and verification:
-
->>> sig = rsa.sign(b"Please sign here.")
->>> rsa.verify(b"Please sign here.", sig)
-True
->>> rsa.verify(b"Sorry, wrong message.", sig)
-False
->>> pub = rsa.export_public_key(format="DER")
->>> other = pk.RSA.from_buffer(pub)
->>> other.verify(b"Please sign here.", sig)
-True
-
-
-Static and ephemeral elliptic curve Diffie-Hellman
---------------------------------------------------
-
-The *mbedtls.pk* module provides the ECC cryptosystem.  This includes:
-
-- Public-private key generation and key import/export in the PEM and DER
-  formats;
-- asymmetric encrypt and decryption;
-- message signature and verification;
-- ephemeral ECDH key exchange.
-
-``get_supported_curves()`` returns the list of supported curves.
-
-The API of the ECC class is the same as the API of the RSA class
-but ciphering (``encrypt()`` and ``decrypt()`` is not supported by
-Mbed TLS).
-
-Message signature and verification using elliptic a curve digital
-signature algorithm (ECDSA):
-
->>> from mbedtls import pk
->>> ecdsa = pk.ECC()
->>> prv = ecdsa.generate()
->>> sig = ecdsa.sign(b"Please sign here.")
->>> ecdsa.verify(b"Please sign here.", sig)
-True
->>> ecdsa.verify(b"Sorry, wrong message.", sig)
-False
->>> pub = ecdsa.export_public_key(format="DER")
->>> other = pk.ECC.from_buffer(pub)
->>> other.verify(b"Please sign here.", sig)
-True
-
-The classes ``ECDHServer`` and ``ECDHClient`` may be used for ephemeral
-ECDH.  The key exchange is as follows:
-
->>> ecdh_key = pk.ECC()
->>> ecdh_key.generate()
->>> ecdh_srv = pk.ECDHServer(ecdh_key)
->>> ecdh_cli = pk.ECDHClient(ecdh_key)
-
-The server generates the ServerKeyExchange encrypted payload and
-passes it to the client:
-
->>> ske = ecdh_srv.generate()
->>> ecdh_cli.import_SKE(ske)
-
-then the client generates the ClientKeyExchange encrypted payload and
-passes it back to the server:
-
->>> cke = ecdh_cli.generate()
->>> ecdh_srv.import_CKE(cke)
-
-Now, client and server may generate their shared secret:
-
->>> secret = ecdh_srv.generate_secret()
->>> ecdh_cli.generate_secret() == secret
-True
->>> ecdh_srv.shared_secret == ecdh_cli.shared_secret
-True
-
-
-Diffie-Hellman-Merkle key exchange
-----------------------------------
-
-The classes ``DHServer`` and ``DHClient`` may be used for DH Key
-exchange.  The classes have the same API as ``ECDHServer``
-and ``ECDHClient``, respectively.
-
-The key exchange is as follow:
-
->>> from mbedtls.mpi import MPI
->>> from mbedtls import pk
->>> dh_srv = pk.DHServer(MPI.prime(128), MPI.prime(96))
->>> dh_cli = pk.DHClient(MPI.prime(128), MPI.prime(96))
-
-The 128-bytes prime and the 96-bytes prime are the modulus ``P``
-and the generator ``G``.
-
-The server generates the ServerKeyExchange payload:
-
->>> ske = dh_srv.generate()
->>> dh_cli.import_SKE(ske)
-
-The payload ends with ``G^X mod P`` where ``X`` is the secret value of
-the server.
-
->>> cke = dh_cli.generate()
->>> dh_srv.import_CKE(cke)
-
-``cke`` is ``G^Y mod P`` (with ``Y`` the secret value from the client)
-returned as its representation in bytes so that it can be readily
-transported over the network.
-
-As in ECDH, client and server may now generate their shared secret:
-
->>> secret = dh_srv.generate_secret()
->>> dh_cli.generate_secret() == secret
-True
->>> dh_srv.shared_secret == dh_cli.shared_secret
-True
-
-
-X.509 certificate writing and parsing
--------------------------------------
-
-The *mbedtls.x509* module can be used to parse X.509 certificates
-or create and verify a certificate chain.
-
-Here, the trusted root is a self-signed CA certificate
-``ca0_crt`` signed by ``ca0_key``.
-
->>> import datetime as dt
->>>
->>> from mbedtls import hashlib
->>> from mbedtls import pk
->>> from mbedtls import x509
->>>
->>> now = dt.datetime.utcnow()
->>> ca0_key = pk.RSA()
->>> _ = ca0_key.generate()
->>> ca0_csr = x509.CSR.new(ca0_key, "CN=Trusted CA", hashlib.sha256())
->>> ca0_crt = x509.CRT.selfsign(
-...     ca0_csr, ca0_key,
-...     not_before=now, not_after=now + dt.timedelta(days=90),
-...     serial_number=0x123456,
-...     basic_constraints=x509.BasicConstraints(True, 1))
-...
-
-An intermediate then issues a Certificate Singing Request (CSR) that the
-root CA signs:
-
->>> ca1_key = pk.ECC()
->>> _ = ca1_key.generate()
->>> ca1_csr = x509.CSR.new(ca1_key, "CN=Intermediate CA", hashlib.sha256())
->>>
->>> ca1_crt = ca0_crt.sign(
-...     ca1_csr, ca0_key, now, now + dt.timedelta(days=90), 0x123456,
-...     basic_constraints=x509.BasicConstraints(ca=True, max_path_length=3))
-...
-
-And finally, the intermediate CA signs a certificate for the
-End Entity on the basis of a new CSR:
-
->>> ee0_key = pk.ECC()
->>> _ = ee0_key.generate()
->>> ee0_csr = x509.CSR.new(ee0_key, "CN=End Entity", hashlib.sha256())
->>>
->>> ee0_crt = ca1_crt.sign(
-...     ee0_csr, ca1_key, now, now + dt.timedelta(days=90), 0x987654)
-...
-
-The emitting certificate can be used to verify the next certificate in
-the chain:
-
->>> ca1_crt.verify(ee0_crt)
-True
->>> ca0_crt.verify(ca1_crt)
-True
-
-Note, however, that this verification is only one step in a private key
-infrastructure and does not take CRLs, path length, etc. into account.
-
-
-TLS and DTLS client and server
-------------------------------
-
-The *mbedtls.tls* module provides TLS clients and servers.  The API
-follows the recommendations of `PEP 543`_.  Note, however, that the
-Python standard SSL library does not follow the PEP so that this
-library may not be a drop-in replacement.
-
-.. _PEP 543: https://www.python.org/dev/peps/pep-0543/
-
-Connectionless DTLS is supported as well.
-
-See examples in the `programs/`_ directory of the repository
-and `tests/test_tls.py`_.
-
-.. _programs/: https://github.com/Synss/python-mbedtls/tree/master/programs
-.. _tests/test_tls.py: https://github.com/Synss/python-mbedtls/blob/master/tests/test_tls.py
+Metadata-Version: 2.1
+Name: python-mbedtls
+Version: 2.7.1
+Summary: hash, hmac, RSA, ECC, X.509, TLS, DTLS, handshakes, and secrets with an mbed TLS back end
+Home-page: https://github.com/Synss/python-mbedtls
+Download-URL: https://github.com/Synss/python-mbedtls/tarball/2.7.1
+Author: Mathias Laurin
+Author-email: Mathias.Laurin@github.com
+License: MIT License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Cython
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Security :: Cryptography
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+.. vim:tw=72
+
+=======================================================
+Cryptographic library for Python with Mbed TLS back end
+=======================================================
+
+.. image:: https://results.pre-commit.ci/badge/github/Synss/python-mbedtls/master.svg
+   :target: https://results.pre-commit.ci/latest/github/Synss/python-mbedtls/master
+   :alt: pre-commit.ci status
+
+.. image::
+   https://github.com/Synss/python-mbedtls/actions/workflows/main.yml/badge.svg?branch=master
+   :target: https://github.com/Synss/python-mbedtls/actions/
+
+.. image::
+   https://coveralls.io/repos/github/Synss/python-mbedtls/badge.svg?branch=master
+   :target: https://coveralls.io/github/Synss/python-mbedtls?branch=master
+
+
+`python-mbedtls`_ is a free cryptographic library for Python that uses
+`mbed TLS`_ for back end.
+
+   mbed TLS (formerly known as PolarSSL) makes it trivially easy for
+   developers to include cryptographic and SSL/TLS capabilities in their
+   (embedded) products, facilitating this functionality with a minimal
+   coding footprint.
+
+*python-mbedtls* API follows the recommendations from:
+
+* `PEP 272`_ -- API for Block Encryption Algorithms v1.0
+* `PEP 452`_ -- API for Cryptographic Hash Functions v2.0
+* `PEP 506`_ -- Adding a Secret Module to the Standard Library
+* `PEP 543`_ -- A Unified TLS API for Python (`completed and modernized`_)
+
+and therefore plays well with the `cryptographic services`_ from the
+Python standard library and many other cryptography libraries as well.
+
+.. _python-mbedtls: https://synss.github.io/python-mbedtls
+.. _mbed TLS: https://tls.mbed.org
+.. _PEP 272: https://www.python.org/dev/peps/pep-0272/
+.. _PEP 452: https://www.python.org/dev/peps/pep-0452/
+.. _PEP 506: https://www.python.org/dev/peps/pep-0506/
+.. _PEP 543: https://www.python.org/dev/peps/pep-0543/
+.. _cryptographic services: https://docs.python.org/3/library/crypto.html
+.. _PyCrypto: https://www.dlitz.net/software/pycrypto/
+.. _hashlib: https://docs.python.org/3.6/library/hashlib.html
+.. _hmac: https://docs.python.org/3.6/library/hmac.html
+.. _completed and modernized: https://github.com/Synss/python-mbedtls/blob/master/src/mbedtls/_tlsi.py
+
+
+License
+=======
+
+*python-mbedtls* is licensed under the MIT License (see LICENSE.txt).
+This enables the use of *python-mbedtls* in both open source and closed
+source projects.  The MIT License is compatible with both GPL and Apache
+2.0 license under which mbed TLS is distributed.
+
+
+API documentation
+=================
+
+https://synss.github.io/python-mbedtls/
+
+
+Installation
+============
+
+The bindings are tested with mbedTLS 2.28.3 for Python 3.8,
+3.9, 3.10, and 3.11 on Linux, macOS, and Windows.
+
+`manylinux`_ wheels are available for 64-bit Linux systems.  Install
+with ``pip install python-mbedtls``.
+
+.. _manylinux: https://www.python.org/dev/peps/pep-0513/
+
+
+Usage and examples
+==================
+
+Now, let us see examples using the various parts of the library.
+
+
+Check which version of mbed TLS is being used by python-mbedtls
+---------------------------------------------------------------
+
+The *mbedtls.version* module shows the run-time version
+information to mbed TLS.
+
+>>> from mbedtls import version
+>>> _ = version.version  # "mbed TLS 2.28.3"
+>>> _ = version.version_info  # (2, 28, 3)
+
+
+Message digest
+--------------
+
+The *mbedtls.hashlib* module supports MD2, MD4, MD5, SHA-1, SHA-2
+(in 224, 256, 384, and 512-bits), and RIPEMD-160 secure hashes
+and message digests.  Note that MD2 and MD4 are not included
+by default and are only present if they are compiled in mbedtls.
+
+Here are the examples from (standard) *hashlib* ported
+to *python-mbedtls*:
+
+>>> from mbedtls import hashlib
+>>> m = hashlib.md5()
+>>> m.update(b"Nobody inspects")
+>>> m.update(b" the spammish repetition")
+>>> m.digest()
+b'\xbbd\x9c\x83\xdd\x1e\xa5\xc9\xd9\xde\xc9\xa1\x8d\xf0\xff\xe9'
+>>> m.digest_size
+16
+>>> m.block_size
+64
+
+More condensed:
+
+>>> hashlib.sha224(b"Nobody inspects the spammish repetition").hexdigest()
+'a4337bc45a8fc544c03f52dc550cd6e1e87021bc896588bd79e901e2'
+
+Using ``new()``:
+
+>>> h = hashlib.new('ripemd160')
+>>> h.update(b"Nobody inspects the spammish repetition")
+>>> h.hexdigest()
+'cc4a5ce1b3df48aec5d22d1f16b894a0b894eccc'
+
+
+HMAC algorithm
+--------------
+
+The *mbedtls.hmac* module computes HMAC.
+
+Example:
+
+>>> from mbedtls import hmac
+>>> m = hmac.new(b"This is my secret key", digestmod="md5")
+>>> m.update(b"Nobody inspects")
+>>> m.update(b" the spammish repetition")
+>>> m.digest()
+b'\x9d-/rj\\\x98\x80\xb1rG\x87\x0f\xe9\xe4\xeb'
+
+Warning:
+
+The message is cleared after calculation of the digest.  Only call
+``mbedtls.hmac.Hmac.digest()`` or ``mbedtls.hmac.Hmac.hexdigest()``
+once per message.
+
+
+HMAC-based key derivation function (HKDF)
+-----------------------------------------
+
+The *mbedtls.hkdf* module exposes extract-and-expand key derivation
+functions.  The main function is ``hkdf()`` but ``extract()`` and
+``expand()`` may be used as well.
+
+Example:
+
+>>> from mbedtls import hkdf
+>>> hkdf.hkdf(
+...     b"my secret key",
+...     length=42,
+...     info=b"my cool app",
+...     salt=b"and pepper",
+...     digestmod=hmac.sha256
+... )
+b'v,\xef\x90\xccU\x1d\x1b\xd7\\a\xaf\x92\xac\n\x90\xf9q\xf4)\xcd"\xf7\x1a\x94p\x03.\xa8e\x1e\xfb\x92\xe8l\x0cc\xf8e\rvj'
+
+where *info*, *salt*, and *digestmod* are optional, although providing
+(at least) *info* is highly recommended.
+
+
+Symmetric cipher
+----------------
+
+The *mbedtls.cipher* module provides symmetric encryption.  The API
+follows the recommendations from PEP 272 so that it can be used as a
+drop-in replacement to other libraries.
+
+*python-mbedtls* provides the following algorithms:
+
+- AES encryption/decryption (128, 192, and 256 bits) in ECB, CBC, CFB128,
+  CTR, OFB, or XTS mode;
+- AES AEAD (128, 192, and 256 bits) in GCM or CCM mode;
+- ARC4 encryption/decryption;
+- ARIA encryption/decryption (128, 192, and 256 bits) in ECB, CBC,
+  CTR, or GCM modes;
+- Blowfish encryption/decryption in ECB, CBC, CFB64, or CTR mode;
+- Camellia encryption/decryption (128, 192, and 256 bits) in ECB, CBC,
+  CFB128, CTR, or GCM mode;
+- DES, DES3, and double DES3 encryption/decryption in ECB or CBC mode;
+- CHACHA20 and CHACHA20/POLY1305 encryption/decryption.
+
+Example:
+
+>>> from mbedtls import cipher
+>>> c = cipher.AES.new(b"My 16-bytes key.", cipher.MODE_CBC, b"CBC needs an IV.")
+>>> enc = c.encrypt(b"This is a super-secret message!!")
+>>> enc
+b"*`k6\x98\x97=[\xdf\x7f\x88\x96\xf5\t\x19J\xf62h\xf4n\xca\xe8\xfe\xf5\xd7X'\xb1\x8c\xc9\x85"
+>>> c.decrypt(enc)
+b'This is a super-secret message!!'
+
+
+RSA public key
+--------------
+
+The *mbedtls.pk* module provides the RSA cryptosystem.  This includes:
+
+- Public-private key generation and key import/export in PEM and DER
+  formats;
+- asymmetric encryption and decryption;
+- message signature and verification.
+
+Key generation, the default size is 2048 bits:
+
+>>> from mbedtls import pk
+>>> rsa = pk.RSA()
+>>> prv = rsa.generate()
+>>> rsa.key_size
+256
+
+Message encryption and decryption:
+
+>>> enc = rsa.encrypt(b"secret message")
+>>> rsa.decrypt(enc)
+b'secret message'
+
+Message signature and verification:
+
+>>> sig = rsa.sign(b"Please sign here.")
+>>> rsa.verify(b"Please sign here.", sig)
+True
+>>> rsa.verify(b"Sorry, wrong message.", sig)
+False
+>>> pub = rsa.export_public_key(format="DER")
+>>> other = pk.RSA.from_buffer(pub)
+>>> other.verify(b"Please sign here.", sig)
+True
+
+
+Static and ephemeral elliptic curve Diffie-Hellman
+--------------------------------------------------
+
+The *mbedtls.pk* module provides the ECC cryptosystem.  This includes:
+
+- Public-private key generation and key import/export in the PEM and DER
+  formats;
+- asymmetric encrypt and decryption;
+- message signature and verification;
+- ephemeral ECDH key exchange.
+
+``get_supported_curves()`` returns the list of supported curves.
+
+The API of the ECC class is the same as the API of the RSA class
+but ciphering (``encrypt()`` and ``decrypt()`` is not supported by
+Mbed TLS).
+
+Message signature and verification using elliptic a curve digital
+signature algorithm (ECDSA):
+
+>>> from mbedtls import pk
+>>> ecdsa = pk.ECC()
+>>> prv = ecdsa.generate()
+>>> sig = ecdsa.sign(b"Please sign here.")
+>>> ecdsa.verify(b"Please sign here.", sig)
+True
+>>> ecdsa.verify(b"Sorry, wrong message.", sig)
+False
+>>> pub = ecdsa.export_public_key(format="DER")
+>>> other = pk.ECC.from_buffer(pub)
+>>> other.verify(b"Please sign here.", sig)
+True
+
+The classes ``ECDHServer`` and ``ECDHClient`` may be used for ephemeral
+ECDH.  The key exchange is as follows:
+
+>>> ecdh_key = pk.ECC()
+>>> ecdh_key.generate()
+>>> ecdh_srv = pk.ECDHServer(ecdh_key)
+>>> ecdh_cli = pk.ECDHClient(ecdh_key)
+
+The server generates the ServerKeyExchange encrypted payload and
+passes it to the client:
+
+>>> ske = ecdh_srv.generate()
+>>> ecdh_cli.import_SKE(ske)
+
+then the client generates the ClientKeyExchange encrypted payload and
+passes it back to the server:
+
+>>> cke = ecdh_cli.generate()
+>>> ecdh_srv.import_CKE(cke)
+
+Now, client and server may generate their shared secret:
+
+>>> secret = ecdh_srv.generate_secret()
+>>> ecdh_cli.generate_secret() == secret
+True
+>>> ecdh_srv.shared_secret == ecdh_cli.shared_secret
+True
+
+
+Diffie-Hellman-Merkle key exchange
+----------------------------------
+
+The classes ``DHServer`` and ``DHClient`` may be used for DH Key
+exchange.  The classes have the same API as ``ECDHServer``
+and ``ECDHClient``, respectively.
+
+The key exchange is as follow:
+
+>>> from mbedtls.mpi import MPI
+>>> from mbedtls import pk
+>>> dh_srv = pk.DHServer(MPI.prime(128), MPI.prime(96))
+>>> dh_cli = pk.DHClient(MPI.prime(128), MPI.prime(96))
+
+The 128-bytes prime and the 96-bytes prime are the modulus ``P``
+and the generator ``G``.
+
+The server generates the ServerKeyExchange payload:
+
+>>> ske = dh_srv.generate()
+>>> dh_cli.import_SKE(ske)
+
+The payload ends with ``G^X mod P`` where ``X`` is the secret value of
+the server.
+
+>>> cke = dh_cli.generate()
+>>> dh_srv.import_CKE(cke)
+
+``cke`` is ``G^Y mod P`` (with ``Y`` the secret value from the client)
+returned as its representation in bytes so that it can be readily
+transported over the network.
+
+As in ECDH, client and server may now generate their shared secret:
+
+>>> secret = dh_srv.generate_secret()
+>>> dh_cli.generate_secret() == secret
+True
+>>> dh_srv.shared_secret == dh_cli.shared_secret
+True
+
+
+X.509 certificate writing and parsing
+-------------------------------------
+
+The *mbedtls.x509* module can be used to parse X.509 certificates
+or create and verify a certificate chain.
+
+Here, the trusted root is a self-signed CA certificate
+``ca0_crt`` signed by ``ca0_key``.
+
+>>> import datetime as dt
+>>>
+>>> from mbedtls import hashlib
+>>> from mbedtls import pk
+>>> from mbedtls import x509
+>>>
+>>> now = dt.datetime.utcnow()
+>>> ca0_key = pk.RSA()
+>>> _ = ca0_key.generate()
+>>> ca0_csr = x509.CSR.new(ca0_key, "CN=Trusted CA", hashlib.sha256())
+>>> ca0_crt = x509.CRT.selfsign(
+...     ca0_csr, ca0_key,
+...     not_before=now, not_after=now + dt.timedelta(days=90),
+...     serial_number=0x123456,
+...     basic_constraints=x509.BasicConstraints(True, 1))
+...
+
+An intermediate then issues a Certificate Singing Request (CSR) that the
+root CA signs:
+
+>>> ca1_key = pk.ECC()
+>>> _ = ca1_key.generate()
+>>> ca1_csr = x509.CSR.new(ca1_key, "CN=Intermediate CA", hashlib.sha256())
+>>>
+>>> ca1_crt = ca0_crt.sign(
+...     ca1_csr, ca0_key, now, now + dt.timedelta(days=90), 0x123456,
+...     basic_constraints=x509.BasicConstraints(ca=True, max_path_length=3))
+...
+
+And finally, the intermediate CA signs a certificate for the
+End Entity on the basis of a new CSR:
+
+>>> ee0_key = pk.ECC()
+>>> _ = ee0_key.generate()
+>>> ee0_csr = x509.CSR.new(ee0_key, "CN=End Entity", hashlib.sha256())
+>>>
+>>> ee0_crt = ca1_crt.sign(
+...     ee0_csr, ca1_key, now, now + dt.timedelta(days=90), 0x987654)
+...
+
+The emitting certificate can be used to verify the next certificate in
+the chain:
+
+>>> ca1_crt.verify(ee0_crt)
+True
+>>> ca0_crt.verify(ca1_crt)
+True
+
+Note, however, that this verification is only one step in a private key
+infrastructure and does not take CRLs, path length, etc. into account.
+
+
+TLS and DTLS client and server
+------------------------------
+
+The *mbedtls.tls* module provides TLS clients and servers.  The API
+follows the recommendations of `PEP 543`_.  Note, however, that the
+Python standard SSL library does not follow the PEP so that this
+library may not be a drop-in replacement.
+
+.. _PEP 543: https://www.python.org/dev/peps/pep-0543/
+
+Connectionless DTLS is supported as well.
+
+See examples in the `programs/`_ directory of the repository
+and `tests/test_tls.py`_.
+
+.. _programs/: https://github.com/Synss/python-mbedtls/tree/master/programs
+.. _tests/test_tls.py: https://github.com/Synss/python-mbedtls/blob/master/tests/test_tls.py
```

### Comparing `python-mbedtls-2.7.0/src/python_mbedtls.egg-info/SOURCES.txt` & `python-mbedtls-2.7.1/src/python_mbedtls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-mbedtls-2.7.0/tests/conftest.py` & `python-mbedtls-2.7.1/tests/conftest.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-# SPDX-License-Identifier: MIT
-
-from __future__ import annotations
-
-import random
-import reprlib
-import sys
-from typing import Callable, Optional, Sequence
-
-import pytest
-
-import mbedtls
-
-
-def pytest_report_header(
-    # pylint: disable=unused-argument
-    config: object,
-    startdir: object,
-) -> None:
-    sys.stdout.write(
-        f"python-mbedtls {mbedtls.__version__}, {mbedtls.version.version}\n"
-    )
-
-
-class _Repr(reprlib.Repr):
-    """Repr with support for memoryview."""
-
-    def repr_memoryview(self, obj: memoryview, _level: object) -> str:
-        return f"{type(obj).__name__}({self.repr(obj.tobytes())})"
-
-
-_repr_instance = _Repr()
-_repr = _repr_instance.repr
-
-
-def _compare_memoryviews(
-    _config: object, _op: object, left: object, right: object
-) -> Sequence[str]:
-    # Adapted from pytest.
-    summary = [f"{_repr(left)} != {_repr(right)}"]
-    explanation = []
-    if isinstance(left, Sequence) and isinstance(right, Sequence):
-        for i in range(min(len(left), len(right))):
-            if left[i] != right[i]:
-                left_value = left[i : i + 1]
-                right_value = right[i : i + 1]
-                explanation += [
-                    f"At index {i} diff: {_repr(left_value)} != {_repr(right_value)}"
-                ]
-                break
-    return summary + explanation
-
-
-def pytest_assertrepr_compare(
-    config: object, op: object, left: object, right: object
-) -> Optional[Sequence[str]]:
-    if op == "==" and any(
-        (isinstance(left, memoryview), isinstance(right, memoryview))
-    ):
-        return _compare_memoryviews(config, op, left, right)
-    return None
-
-
-@pytest.fixture()
-def randbytes() -> Callable[[int], bytes]:
-    def function(length: int) -> bytes:
-        return bytes(
-            bytearray(random.randrange(0, 256) for _ in range(length))
-        )
-
-    return function
+# SPDX-License-Identifier: MIT
+
+from __future__ import annotations
+
+import random
+import reprlib
+import sys
+from typing import Callable, Optional, Sequence
+
+import pytest
+
+import mbedtls
+
+
+def pytest_report_header(
+    # pylint: disable=unused-argument
+    config: object,
+    startdir: object,
+) -> None:
+    sys.stdout.write(
+        f"python-mbedtls {mbedtls.__version__}, {mbedtls.version.version}\n"
+    )
+
+
+class _Repr(reprlib.Repr):
+    """Repr with support for memoryview."""
+
+    def repr_memoryview(self, obj: memoryview, _level: object) -> str:
+        return f"{type(obj).__name__}({self.repr(obj.tobytes())})"
+
+
+_repr_instance = _Repr()
+_repr = _repr_instance.repr
+
+
+def _compare_memoryviews(
+    _config: object, _op: object, left: object, right: object
+) -> Sequence[str]:
+    # Adapted from pytest.
+    summary = [f"{_repr(left)} != {_repr(right)}"]
+    explanation = []
+    if isinstance(left, Sequence) and isinstance(right, Sequence):
+        for i in range(min(len(left), len(right))):
+            if left[i] != right[i]:
+                left_value = left[i : i + 1]
+                right_value = right[i : i + 1]
+                explanation += [
+                    f"At index {i} diff: {_repr(left_value)} != {_repr(right_value)}"
+                ]
+                break
+    return summary + explanation
+
+
+def pytest_assertrepr_compare(
+    config: object, op: object, left: object, right: object
+) -> Optional[Sequence[str]]:
+    if op == "==" and any(
+        (isinstance(left, memoryview), isinstance(right, memoryview))
+    ):
+        return _compare_memoryviews(config, op, left, right)
+    return None
+
+
+@pytest.fixture()
+def randbytes() -> Callable[[int], bytes]:
+    def function(length: int) -> bytes:
+        return bytes(
+            bytearray(random.randrange(0, 256) for _ in range(length))
+        )
+
+    return function
```

### Comparing `python-mbedtls-2.7.0/tests/test_assertion_rewriting.py` & `python-mbedtls-2.7.1/tests/test_assertion_rewriting.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# SPDX-License-Identifier: MIT
-
-from __future__ import annotations
-
-import pytest
-
-
-@pytest.mark.xfail(reason="Test assertion rewriting")
-class TestMemoryviewAssertion:
-    @pytest.fixture()
-    def value(self) -> bytes:
-        return bytes(_ % 256 for _ in range(10000))
-
-    def test_memview_and_memview(self, value: bytes) -> None:
-        view = memoryview(value)
-        assert view == view[::-1]
-
-    def test_bytes_and_shorter_memview(self, value: bytes) -> None:
-        view = memoryview(value)
-        assert value == view[:-1]
-
-    def test_shorter_memview_and_bytes(self, value: bytes) -> None:
-        view = memoryview(value)
-        assert view[:-1] == value
-
-    def test_bytes_and_longer_memview(self, value: bytes) -> None:
-        view = memoryview(value)
-        assert value[:-1] == view
-
-    def test_longer_memview_and_bytes(self, value: bytes) -> None:
-        view = memoryview(value)
-        assert view == value[:-1]
-
-    def test_memview_and_str(self, value: bytes) -> None:
-        text = value.decode("latin1")
-        view = memoryview(value)
-        assert view == text  # type: ignore[comparison-overlap]
-
-    def test_str_and_memview(self, value: bytes) -> None:
-        text = value.decode("latin1")
-        view = memoryview(value)
-        assert text == view  # type: ignore[comparison-overlap]
+# SPDX-License-Identifier: MIT
+
+from __future__ import annotations
+
+import pytest
+
+
+@pytest.mark.xfail(reason="Test assertion rewriting")
+class TestMemoryviewAssertion:
+    @pytest.fixture()
+    def value(self) -> bytes:
+        return bytes(_ % 256 for _ in range(10000))
+
+    def test_memview_and_memview(self, value: bytes) -> None:
+        view = memoryview(value)
+        assert view == view[::-1]
+
+    def test_bytes_and_shorter_memview(self, value: bytes) -> None:
+        view = memoryview(value)
+        assert value == view[:-1]
+
+    def test_shorter_memview_and_bytes(self, value: bytes) -> None:
+        view = memoryview(value)
+        assert view[:-1] == value
+
+    def test_bytes_and_longer_memview(self, value: bytes) -> None:
+        view = memoryview(value)
+        assert value[:-1] == view
+
+    def test_longer_memview_and_bytes(self, value: bytes) -> None:
+        view = memoryview(value)
+        assert view == value[:-1]
+
+    def test_memview_and_str(self, value: bytes) -> None:
+        text = value.decode("latin1")
+        view = memoryview(value)
+        assert view == text  # type: ignore[comparison-overlap]
+
+    def test_str_and_memview(self, value: bytes) -> None:
+        text = value.decode("latin1")
+        view = memoryview(value)
+        assert text == view  # type: ignore[comparison-overlap]
```

### Comparing `python-mbedtls-2.7.0/tests/test_error.py` & `python-mbedtls-2.7.1/tests/test_error.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# SPDX-License-Identifier: MIT
-
-"""Unit test mbedtls.exceptions."""
-
-from __future__ import annotations
-
-from typing import Tuple
-
-import pytest
-
-from mbedtls.exceptions import check_error  # type: ignore
-from mbedtls.exceptions import TLSError
-
-
-@pytest.mark.parametrize(
-    "err_msg", [(0x003C, "ENTROPY"), (0x1080, "PEM"), (0x2200, "X509")]
-)
-def test_mbedtls_error(err_msg: Tuple[int, str]) -> None:
-    err, msg = err_msg
-    with pytest.raises(TLSError, match=r"%s - .+" % msg):
-        check_error(-err)
-
-
-def test_other_error() -> None:
-    with pytest.raises(TLSError, match="error message"):
-        raise TLSError(msg="error message")
+# SPDX-License-Identifier: MIT
+
+"""Unit test mbedtls.exceptions."""
+
+from __future__ import annotations
+
+from typing import Tuple
+
+import pytest
+
+from mbedtls.exceptions import check_error  # type: ignore
+from mbedtls.exceptions import TLSError
+
+
+@pytest.mark.parametrize(
+    "err_msg", [(0x003C, "ENTROPY"), (0x1080, "PEM"), (0x2200, "X509")]
+)
+def test_mbedtls_error(err_msg: Tuple[int, str]) -> None:
+    err, msg = err_msg
+    with pytest.raises(TLSError, match=r"%s - .+" % msg):
+        check_error(-err)
+
+
+def test_other_error() -> None:
+    with pytest.raises(TLSError, match="error message"):
+        raise TLSError(msg="error message")
```

### Comparing `python-mbedtls-2.7.0/tests/test_hkdf.py` & `python-mbedtls-2.7.1/tests/test_hkdf.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,336 +1,336 @@
-# SPDX-License-Identifier: MIT
-
-from __future__ import annotations
-
-from typing import Any, Callable, cast
-
-import pytest
-
-import mbedtls
-import mbedtls.hkdf as _hkdf
-import mbedtls.hmac as _hmac
-from mbedtls.hmac import Algorithm
-
-
-@pytest.mark.skipif(
-    not mbedtls.has_feature("HKDF"),
-    reason="requires HKDF support in libmbedtls",
-)
-class TestHKDF:
-    @pytest.fixture(
-        params=[
-            _hmac.md2,
-            _hmac.md4,
-            _hmac.md5,
-            _hmac.sha1,
-            _hmac.sha224,
-            _hmac.sha256,
-            _hmac.sha384,
-            _hmac.sha512,
-            _hmac.ripemd160,
-        ]
-    )
-    def hmac(self, request: Any) -> Algorithm:
-        feature = request.param.__name__
-        if not mbedtls.has_feature(
-            {"sha224": "sha256", "sha384": "sha512"}.get(feature, feature)
-        ):
-            return pytest.skip(f"requires {feature} support in mbedtls")
-        return cast(Algorithm, request.param)
-
-    @pytest.mark.parametrize("key_length", [0, 128])
-    def test_hkdf(
-        self, key_length: int, randbytes: Callable[[int], bytes]
-    ) -> None:
-        key = randbytes(key_length)
-        okm = _hkdf.hkdf(key, 32, b"")
-        assert len(okm) == 32
-
-    @pytest.mark.parametrize("key_length", [0, 128])
-    @pytest.mark.parametrize("info_length", [16, 128, 500, 1000])
-    @pytest.mark.parametrize("output_length", [16, 200, 500])
-    def test_hkdf_with_options(
-        self,
-        key_length: int,
-        info_length: int,
-        output_length: int,
-        hmac: Algorithm,
-        randbytes: Callable[[int], bytes],
-    ) -> None:
-        key = randbytes(key_length)
-        info = randbytes(info_length)
-        salt = randbytes(hmac(key).digest_size)
-
-        okm = _hkdf.hkdf(key, output_length, info, salt, hmac)
-        assert len(okm) == output_length
-
-    @pytest.mark.parametrize("key_length", [0, 128])
-    def test_extract_and_expand(
-        self, key_length: int, randbytes: Callable[[int], bytes]
-    ) -> None:
-        key = randbytes(key_length)
-        prk = _hkdf.extract(key)
-        assert len(prk) == _hmac.sha256(b"").digest_size
-
-        okm = _hkdf.expand(prk, 32, b"")
-        assert len(okm) == 32
-
-    @pytest.mark.parametrize("key_length", [0, 128])
-    @pytest.mark.parametrize("info_length", [16, 128, 500, 1000])
-    @pytest.mark.parametrize("output_length", [16, 200, 500])
-    def test_extract_and_expand_with_options(
-        self,
-        key_length: int,
-        info_length: int,
-        output_length: int,
-        hmac: Algorithm,
-        randbytes: Callable[[int], bytes],
-    ) -> None:
-        key = randbytes(key_length)
-        info = randbytes(info_length)
-        salt = randbytes(hmac(key).digest_size)
-
-        prk = _hkdf.extract(key, salt, hmac)
-        assert len(prk) == hmac(b"").digest_size
-
-        okm = _hkdf.expand(prk, output_length, info, hmac)
-        assert len(okm) == output_length
-
-
-def to_bytes(number: int, size: int) -> bytes:
-    return number.to_bytes(size, byteorder="big")
-
-
-class TestHKDF_RFC5869_TestVectors:
-    def test_case_1(self) -> None:
-        algorithm = _hmac.sha256
-        ikm = to_bytes(0x0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B, 22)
-        salt = to_bytes(0x000102030405060708090A0B0C, 13)
-        info = to_bytes(0xF0F1F2F3F4F5F6F7F8F9, 10)
-        length = 42
-        prk = to_bytes(
-            int(
-                "0x077709362c2e32df0ddc3f0dc47bba63"
-                "90b6c73bb50f9c3122ec844ad7c2b3e5",
-                0,
-            ),
-            32,
-        )
-        okm = to_bytes(
-            int(
-                "0x3cb25f25faacd57a90434f64d0362f2a"
-                "2d2d0a90cf1a5a4c5db02d56ecc4c5bf"
-                "34007208d5b887185865",
-                0,
-            ),
-            42,
-        )
-
-        assert _hkdf.extract(ikm, salt, algorithm) == prk
-        assert _hkdf.expand(prk, length, info, algorithm) == okm
-        assert _hkdf.hkdf(ikm, length, info, salt, algorithm) == okm
-
-    def test_case_2(self) -> None:
-        algorithm = _hmac.sha256
-        ikm = to_bytes(
-            int(
-                "0x000102030405060708090a0b0c0d0e0f"
-                "101112131415161718191a1b1c1d1e1f"
-                "202122232425262728292a2b2c2d2e2f"
-                "303132333435363738393a3b3c3d3e3f"
-                "404142434445464748494a4b4c4d4e4f",
-                0,
-            ),
-            80,
-        )
-        salt = to_bytes(
-            int(
-                "0x606162636465666768696a6b6c6d6e6f"
-                "707172737475767778797a7b7c7d7e7f"
-                "808182838485868788898a8b8c8d8e8f"
-                "909192939495969798999a9b9c9d9e9f"
-                "a0a1a2a3a4a5a6a7a8a9aaabacadaeaf",
-                0,
-            ),
-            80,
-        )
-        info = to_bytes(
-            int(
-                "0xb0b1b2b3b4b5b6b7b8b9babbbcbdbebf"
-                "c0c1c2c3c4c5c6c7c8c9cacbcccdcecf"
-                "d0d1d2d3d4d5d6d7d8d9dadbdcdddedf"
-                "e0e1e2e3e4e5e6e7e8e9eaebecedeeef"
-                "f0f1f2f3f4f5f6f7f8f9fafbfcfdfeff",
-                0,
-            ),
-            80,
-        )
-        length = 82
-        prk = to_bytes(
-            int(
-                "0x06a6b88c5853361a06104c9ceb35b45c"
-                "ef760014904671014a193f40c15fc244",
-                0,
-            ),
-            32,
-        )
-        okm = to_bytes(
-            int(
-                "0xb11e398dc80327a1c8e7f78c596a4934"
-                "4f012eda2d4efad8a050cc4c19afa97c"
-                "59045a99cac7827271cb41c65e590e09"
-                "da3275600c2f09b8367793a9aca3db71"
-                "cc30c58179ec3e87c14c01d5c1f3434f"
-                "1d87",
-                0,
-            ),
-            82,
-        )
-
-        assert _hkdf.extract(ikm, salt, algorithm) == prk
-        assert _hkdf.expand(prk, length, info, algorithm) == okm
-        assert _hkdf.hkdf(ikm, length, info, salt, algorithm) == okm
-
-    def test_case_3(self) -> None:
-        algorithm = _hmac.sha256
-        ikm = to_bytes(0x0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B, 22)
-        salt = b""
-        info = b""
-        length = 42
-        prk = to_bytes(
-            int(
-                "0x19ef24a32c717b167f33a91d6f648bdf"
-                "96596776afdb6377ac434c1c293ccb04",
-                0,
-            ),
-            32,
-        )
-        okm = to_bytes(
-            int(
-                "0x8da4e775a563c18f715f802a063c5a31"
-                "b8a11f5c5ee1879ec3454e5f3c738d2d"
-                "9d201395faa4b61a96c8",
-                0,
-            ),
-            42,
-        )
-
-        assert _hkdf.extract(ikm, salt, algorithm) == prk
-        assert _hkdf.expand(prk, length, info, algorithm) == okm
-        assert _hkdf.hkdf(ikm, length, info, salt, algorithm) == okm
-
-    def test_case_4(self) -> None:
-        algorithm = _hmac.sha1
-        ikm = to_bytes(0x0B0B0B0B0B0B0B0B0B0B0B, 11)
-        salt = to_bytes(0x000102030405060708090A0B0C, 13)
-        info = to_bytes(0xF0F1F2F3F4F5F6F7F8F9, 10)
-        length = 42
-        prk = to_bytes(0x9B6C18C432A7BF8F0E71C8EB88F4B30BAA2BA243, 20)
-        okm = to_bytes(
-            int(
-                "0x085a01ea1b10f36933068b56efa5ad81"
-                "a4f14b822f5b091568a9cdd4f155fda2"
-                "c22e422478d305f3f896",
-                0,
-            ),
-            42,
-        )
-
-        assert _hkdf.extract(ikm, salt, algorithm) == prk
-        assert _hkdf.expand(prk, length, info, algorithm) == okm
-        assert _hkdf.hkdf(ikm, length, info, salt, algorithm) == okm
-
-    def test_case_5(self) -> None:
-        algorithm = _hmac.sha1
-        ikm = to_bytes(
-            int(
-                "0x000102030405060708090a0b0c0d0e0f"
-                "101112131415161718191a1b1c1d1e1f"
-                "202122232425262728292a2b2c2d2e2f"
-                "303132333435363738393a3b3c3d3e3f"
-                "404142434445464748494a4b4c4d4e4f",
-                0,
-            ),
-            80,
-        )
-        salt = to_bytes(
-            int(
-                "0x606162636465666768696a6b6c6d6e6f"
-                "707172737475767778797a7b7c7d7e7f"
-                "808182838485868788898a8b8c8d8e8f"
-                "909192939495969798999a9b9c9d9e9f"
-                "a0a1a2a3a4a5a6a7a8a9aaabacadaeaf",
-                0,
-            ),
-            80,
-        )
-        info = to_bytes(
-            int(
-                "0xb0b1b2b3b4b5b6b7b8b9babbbcbdbebf"
-                "c0c1c2c3c4c5c6c7c8c9cacbcccdcecf"
-                "d0d1d2d3d4d5d6d7d8d9dadbdcdddedf"
-                "e0e1e2e3e4e5e6e7e8e9eaebecedeeef"
-                "f0f1f2f3f4f5f6f7f8f9fafbfcfdfeff",
-                0,
-            ),
-            80,
-        )
-        length = 82
-        prk = to_bytes(0x8ADAE09A2A307059478D309B26C4115A224CFAF6, 20)
-        okm = to_bytes(
-            int(
-                "0x0bd770a74d1160f7c9f12cd5912a06eb"
-                "ff6adcae899d92191fe4305673ba2ffe"
-                "8fa3f1a4e5ad79f3f334b3b202b2173c"
-                "486ea37ce3d397ed034c7f9dfeb15c5e"
-                "927336d0441f4c4300e2cff0d0900b52"
-                "d3b4",
-                0,
-            ),
-            82,
-        )
-
-        assert _hkdf.extract(ikm, salt, algorithm) == prk
-        assert _hkdf.expand(prk, length, info, algorithm) == okm
-        assert _hkdf.hkdf(ikm, length, info, salt, algorithm) == okm
-
-    def test_case_6(self) -> None:
-        algorithm = _hmac.sha1
-        ikm = to_bytes(0x0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B, 22)
-        salt = b""
-        info = b""
-        length = 42
-        prk = to_bytes(0xDA8C8A73C7FA77288EC6F5E7C297786AA0D32D01, 20)
-        okm = to_bytes(
-            int(
-                "0x0ac1af7002b3d761d1e55298da9d0506"
-                "b9ae52057220a306e07b6b87e8df21d0"
-                "ea00033de03984d34918",
-                0,
-            ),
-            42,
-        )
-
-        assert _hkdf.extract(ikm, salt, algorithm) == prk
-        assert _hkdf.expand(prk, length, info, algorithm) == okm
-        assert _hkdf.hkdf(ikm, length, info, salt, algorithm) == okm
-
-    def test_case_7(self) -> None:
-        algorithm = _hmac.sha1
-        ikm = to_bytes(0x0C0C0C0C0C0C0C0C0C0C0C0C0C0C0C0C0C0C0C0C0C0C, 22)
-        info = b""
-        length = 42
-        prk = to_bytes(0x2ADCCADA18779E7C2077AD2EB19D3F3E731385DD, 20)
-        okm = to_bytes(
-            int(
-                "0x2c91117204d745f3500d636a62f64f0a"
-                "b3bae548aa53d423b0d1f27ebba6f5e5"
-                "673a081d70cce7acfc48",
-                0,
-            ),
-            42,
-        )
-
-        assert _hkdf.extract(ikm, digestmod=algorithm) == prk
-        assert _hkdf.expand(prk, length, info, algorithm) == okm
-        assert _hkdf.hkdf(ikm, length, info, digestmod=algorithm) == okm
+# SPDX-License-Identifier: MIT
+
+from __future__ import annotations
+
+from typing import Any, Callable, cast
+
+import pytest
+
+import mbedtls
+import mbedtls.hkdf as _hkdf
+import mbedtls.hmac as _hmac
+from mbedtls.hmac import Algorithm
+
+
+@pytest.mark.skipif(
+    not mbedtls.has_feature("HKDF"),
+    reason="requires HKDF support in libmbedtls",
+)
+class TestHKDF:
+    @pytest.fixture(
+        params=[
+            _hmac.md2,
+            _hmac.md4,
+            _hmac.md5,
+            _hmac.sha1,
+            _hmac.sha224,
+            _hmac.sha256,
+            _hmac.sha384,
+            _hmac.sha512,
+            _hmac.ripemd160,
+        ]
+    )
+    def hmac(self, request: Any) -> Algorithm:
+        feature = request.param.__name__
+        if not mbedtls.has_feature(
+            {"sha224": "sha256", "sha384": "sha512"}.get(feature, feature)
+        ):
+            return pytest.skip(f"requires {feature} support in mbedtls")
+        return cast(Algorithm, request.param)
+
+    @pytest.mark.parametrize("key_length", [0, 128])
+    def test_hkdf(
+        self, key_length: int, randbytes: Callable[[int], bytes]
+    ) -> None:
+        key = randbytes(key_length)
+        okm = _hkdf.hkdf(key, 32, b"")
+        assert len(okm) == 32
+
+    @pytest.mark.parametrize("key_length", [0, 128])
+    @pytest.mark.parametrize("info_length", [16, 128, 500, 1000])
+    @pytest.mark.parametrize("output_length", [16, 200, 500])
+    def test_hkdf_with_options(
+        self,
+        key_length: int,
+        info_length: int,
+        output_length: int,
+        hmac: Algorithm,
+        randbytes: Callable[[int], bytes],
+    ) -> None:
+        key = randbytes(key_length)
+        info = randbytes(info_length)
+        salt = randbytes(hmac(key).digest_size)
+
+        okm = _hkdf.hkdf(key, output_length, info, salt, hmac)
+        assert len(okm) == output_length
+
+    @pytest.mark.parametrize("key_length", [0, 128])
+    def test_extract_and_expand(
+        self, key_length: int, randbytes: Callable[[int], bytes]
+    ) -> None:
+        key = randbytes(key_length)
+        prk = _hkdf.extract(key)
+        assert len(prk) == _hmac.sha256(b"").digest_size
+
+        okm = _hkdf.expand(prk, 32, b"")
+        assert len(okm) == 32
+
+    @pytest.mark.parametrize("key_length", [0, 128])
+    @pytest.mark.parametrize("info_length", [16, 128, 500, 1000])
+    @pytest.mark.parametrize("output_length", [16, 200, 500])
+    def test_extract_and_expand_with_options(
+        self,
+        key_length: int,
+        info_length: int,
+        output_length: int,
+        hmac: Algorithm,
+        randbytes: Callable[[int], bytes],
+    ) -> None:
+        key = randbytes(key_length)
+        info = randbytes(info_length)
+        salt = randbytes(hmac(key).digest_size)
+
+        prk = _hkdf.extract(key, salt, hmac)
+        assert len(prk) == hmac(b"").digest_size
+
+        okm = _hkdf.expand(prk, output_length, info, hmac)
+        assert len(okm) == output_length
+
+
+def to_bytes(number: int, size: int) -> bytes:
+    return number.to_bytes(size, byteorder="big")
+
+
+class TestHKDF_RFC5869_TestVectors:
+    def test_case_1(self) -> None:
+        algorithm = _hmac.sha256
+        ikm = to_bytes(0x0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B, 22)
+        salt = to_bytes(0x000102030405060708090A0B0C, 13)
+        info = to_bytes(0xF0F1F2F3F4F5F6F7F8F9, 10)
+        length = 42
+        prk = to_bytes(
+            int(
+                "0x077709362c2e32df0ddc3f0dc47bba63"
+                "90b6c73bb50f9c3122ec844ad7c2b3e5",
+                0,
+            ),
+            32,
+        )
+        okm = to_bytes(
+            int(
+                "0x3cb25f25faacd57a90434f64d0362f2a"
+                "2d2d0a90cf1a5a4c5db02d56ecc4c5bf"
+                "34007208d5b887185865",
+                0,
+            ),
+            42,
+        )
+
+        assert _hkdf.extract(ikm, salt, algorithm) == prk
+        assert _hkdf.expand(prk, length, info, algorithm) == okm
+        assert _hkdf.hkdf(ikm, length, info, salt, algorithm) == okm
+
+    def test_case_2(self) -> None:
+        algorithm = _hmac.sha256
+        ikm = to_bytes(
+            int(
+                "0x000102030405060708090a0b0c0d0e0f"
+                "101112131415161718191a1b1c1d1e1f"
+                "202122232425262728292a2b2c2d2e2f"
+                "303132333435363738393a3b3c3d3e3f"
+                "404142434445464748494a4b4c4d4e4f",
+                0,
+            ),
+            80,
+        )
+        salt = to_bytes(
+            int(
+                "0x606162636465666768696a6b6c6d6e6f"
+                "707172737475767778797a7b7c7d7e7f"
+                "808182838485868788898a8b8c8d8e8f"
+                "909192939495969798999a9b9c9d9e9f"
+                "a0a1a2a3a4a5a6a7a8a9aaabacadaeaf",
+                0,
+            ),
+            80,
+        )
+        info = to_bytes(
+            int(
+                "0xb0b1b2b3b4b5b6b7b8b9babbbcbdbebf"
+                "c0c1c2c3c4c5c6c7c8c9cacbcccdcecf"
+                "d0d1d2d3d4d5d6d7d8d9dadbdcdddedf"
+                "e0e1e2e3e4e5e6e7e8e9eaebecedeeef"
+                "f0f1f2f3f4f5f6f7f8f9fafbfcfdfeff",
+                0,
+            ),
+            80,
+        )
+        length = 82
+        prk = to_bytes(
+            int(
+                "0x06a6b88c5853361a06104c9ceb35b45c"
+                "ef760014904671014a193f40c15fc244",
+                0,
+            ),
+            32,
+        )
+        okm = to_bytes(
+            int(
+                "0xb11e398dc80327a1c8e7f78c596a4934"
+                "4f012eda2d4efad8a050cc4c19afa97c"
+                "59045a99cac7827271cb41c65e590e09"
+                "da3275600c2f09b8367793a9aca3db71"
+                "cc30c58179ec3e87c14c01d5c1f3434f"
+                "1d87",
+                0,
+            ),
+            82,
+        )
+
+        assert _hkdf.extract(ikm, salt, algorithm) == prk
+        assert _hkdf.expand(prk, length, info, algorithm) == okm
+        assert _hkdf.hkdf(ikm, length, info, salt, algorithm) == okm
+
+    def test_case_3(self) -> None:
+        algorithm = _hmac.sha256
+        ikm = to_bytes(0x0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B, 22)
+        salt = b""
+        info = b""
+        length = 42
+        prk = to_bytes(
+            int(
+                "0x19ef24a32c717b167f33a91d6f648bdf"
+                "96596776afdb6377ac434c1c293ccb04",
+                0,
+            ),
+            32,
+        )
+        okm = to_bytes(
+            int(
+                "0x8da4e775a563c18f715f802a063c5a31"
+                "b8a11f5c5ee1879ec3454e5f3c738d2d"
+                "9d201395faa4b61a96c8",
+                0,
+            ),
+            42,
+        )
+
+        assert _hkdf.extract(ikm, salt, algorithm) == prk
+        assert _hkdf.expand(prk, length, info, algorithm) == okm
+        assert _hkdf.hkdf(ikm, length, info, salt, algorithm) == okm
+
+    def test_case_4(self) -> None:
+        algorithm = _hmac.sha1
+        ikm = to_bytes(0x0B0B0B0B0B0B0B0B0B0B0B, 11)
+        salt = to_bytes(0x000102030405060708090A0B0C, 13)
+        info = to_bytes(0xF0F1F2F3F4F5F6F7F8F9, 10)
+        length = 42
+        prk = to_bytes(0x9B6C18C432A7BF8F0E71C8EB88F4B30BAA2BA243, 20)
+        okm = to_bytes(
+            int(
+                "0x085a01ea1b10f36933068b56efa5ad81"
+                "a4f14b822f5b091568a9cdd4f155fda2"
+                "c22e422478d305f3f896",
+                0,
+            ),
+            42,
+        )
+
+        assert _hkdf.extract(ikm, salt, algorithm) == prk
+        assert _hkdf.expand(prk, length, info, algorithm) == okm
+        assert _hkdf.hkdf(ikm, length, info, salt, algorithm) == okm
+
+    def test_case_5(self) -> None:
+        algorithm = _hmac.sha1
+        ikm = to_bytes(
+            int(
+                "0x000102030405060708090a0b0c0d0e0f"
+                "101112131415161718191a1b1c1d1e1f"
+                "202122232425262728292a2b2c2d2e2f"
+                "303132333435363738393a3b3c3d3e3f"
+                "404142434445464748494a4b4c4d4e4f",
+                0,
+            ),
+            80,
+        )
+        salt = to_bytes(
+            int(
+                "0x606162636465666768696a6b6c6d6e6f"
+                "707172737475767778797a7b7c7d7e7f"
+                "808182838485868788898a8b8c8d8e8f"
+                "909192939495969798999a9b9c9d9e9f"
+                "a0a1a2a3a4a5a6a7a8a9aaabacadaeaf",
+                0,
+            ),
+            80,
+        )
+        info = to_bytes(
+            int(
+                "0xb0b1b2b3b4b5b6b7b8b9babbbcbdbebf"
+                "c0c1c2c3c4c5c6c7c8c9cacbcccdcecf"
+                "d0d1d2d3d4d5d6d7d8d9dadbdcdddedf"
+                "e0e1e2e3e4e5e6e7e8e9eaebecedeeef"
+                "f0f1f2f3f4f5f6f7f8f9fafbfcfdfeff",
+                0,
+            ),
+            80,
+        )
+        length = 82
+        prk = to_bytes(0x8ADAE09A2A307059478D309B26C4115A224CFAF6, 20)
+        okm = to_bytes(
+            int(
+                "0x0bd770a74d1160f7c9f12cd5912a06eb"
+                "ff6adcae899d92191fe4305673ba2ffe"
+                "8fa3f1a4e5ad79f3f334b3b202b2173c"
+                "486ea37ce3d397ed034c7f9dfeb15c5e"
+                "927336d0441f4c4300e2cff0d0900b52"
+                "d3b4",
+                0,
+            ),
+            82,
+        )
+
+        assert _hkdf.extract(ikm, salt, algorithm) == prk
+        assert _hkdf.expand(prk, length, info, algorithm) == okm
+        assert _hkdf.hkdf(ikm, length, info, salt, algorithm) == okm
+
+    def test_case_6(self) -> None:
+        algorithm = _hmac.sha1
+        ikm = to_bytes(0x0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B0B, 22)
+        salt = b""
+        info = b""
+        length = 42
+        prk = to_bytes(0xDA8C8A73C7FA77288EC6F5E7C297786AA0D32D01, 20)
+        okm = to_bytes(
+            int(
+                "0x0ac1af7002b3d761d1e55298da9d0506"
+                "b9ae52057220a306e07b6b87e8df21d0"
+                "ea00033de03984d34918",
+                0,
+            ),
+            42,
+        )
+
+        assert _hkdf.extract(ikm, salt, algorithm) == prk
+        assert _hkdf.expand(prk, length, info, algorithm) == okm
+        assert _hkdf.hkdf(ikm, length, info, salt, algorithm) == okm
+
+    def test_case_7(self) -> None:
+        algorithm = _hmac.sha1
+        ikm = to_bytes(0x0C0C0C0C0C0C0C0C0C0C0C0C0C0C0C0C0C0C0C0C0C0C, 22)
+        info = b""
+        length = 42
+        prk = to_bytes(0x2ADCCADA18779E7C2077AD2EB19D3F3E731385DD, 20)
+        okm = to_bytes(
+            int(
+                "0x2c91117204d745f3500d636a62f64f0a"
+                "b3bae548aa53d423b0d1f27ebba6f5e5"
+                "673a081d70cce7acfc48",
+                0,
+            ),
+            42,
+        )
+
+        assert _hkdf.extract(ikm, digestmod=algorithm) == prk
+        assert _hkdf.expand(prk, length, info, algorithm) == okm
+        assert _hkdf.hkdf(ikm, length, info, digestmod=algorithm) == okm
```

### Comparing `python-mbedtls-2.7.0/tests/test_md.py` & `python-mbedtls-2.7.1/tests/test_md.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,227 +1,219 @@
-# SPDX-License-Identifier: MIT
-
-"""Unit tests for mbedtls.md."""
-
-from __future__ import annotations
-
-import pickle
-from collections.abc import Collection
-from typing import Any, Callable, Mapping, NamedTuple, cast
-
-import pytest
-
-from mbedtls import hashlib, hmac
-from mbedtls._md import Hash
-
-
-class Size(NamedTuple):
-    digest_size: int
-    block_size: int
-
-
-SUPPORTED_SIZES: Mapping[str, Size] = {
-    "md2": Size(digest_size=16, block_size=16),
-    "md4": Size(digest_size=16, block_size=64),
-    "md5": Size(digest_size=16, block_size=64),
-    "sha1": Size(digest_size=20, block_size=64),
-    "sha224": Size(digest_size=28, block_size=64),
-    "sha256": Size(digest_size=32, block_size=64),
-    "sha384": Size(digest_size=48, block_size=128),
-    "sha512": Size(digest_size=64, block_size=128),
-    "ripemd160": Size(digest_size=20, block_size=64),
-}
-
-
-def test_algorithms() -> None:
-    assert isinstance(hashlib.algorithms_guaranteed, Collection)
-    assert hashlib.algorithms_guaranteed
-
-    assert isinstance(hashlib.algorithms_available, Collection)
-    assert hashlib.algorithms_available
-
-    assert frozenset(hashlib.algorithms_guaranteed).issubset(
-        hashlib.algorithms_available
-    )
-
-
-def test_invalid_name_raises_TypeError() -> None:
-    with pytest.raises(TypeError):
-        Hash(42)  # type: ignore[arg-type]
-
-
-def test_unavailable_cipher_raises_ValueError() -> None:
-    with pytest.raises(ValueError):
-        Hash("unavailable")
-
-
-class TestHash:
-    @pytest.fixture(params=tuple(hashlib.algorithms_available))
-    def algorithm_str(self, request: Any) -> str:
-        assert isinstance(request.param, str)
-        return request.param
-
-    @pytest.fixture()
-    def algorithm(self, algorithm_str: str) -> hashlib.Algorithm:
-        return cast(hashlib.Algorithm, getattr(hashlib, algorithm_str))
-
-    @pytest.mark.parametrize(
-        "repr_",
-        [repr, str],
-        ids=lambda f: f.__name__,  # type: ignore[no-any-return]
-    )
-    def test_repr(
-        self, repr_: Callable[[object], str], algorithm: hashlib.Algorithm
-    ) -> None:
-        assert isinstance(repr_(algorithm(b"")), str)
-
-    def test_pickle(self, algorithm: hashlib.Algorithm) -> None:
-        with pytest.raises(TypeError) as excinfo:
-            pickle.dumps(algorithm(b""))
-
-        assert str(excinfo.value).startswith("cannot pickle")
-
-    def test_accessors(
-        self, algorithm: hashlib.Algorithm, algorithm_str: str
-    ) -> None:
-        obj = algorithm(b"")
-
-        assert obj.digest_size == SUPPORTED_SIZES[algorithm_str].digest_size
-        assert obj.block_size == SUPPORTED_SIZES[algorithm_str].block_size
-
-    def test_update(
-        self, algorithm: hashlib.Algorithm, randbytes: Callable[[int], bytes]
-    ) -> None:
-        buffer = randbytes(512)
-
-        obj = algorithm(b"")
-        obj.update(buffer)
-        other = algorithm(buffer)
-
-        assert obj.digest() == other.digest()
-        assert obj.hexdigest() == other.hexdigest()
-
-    def test_new(
-        self,
-        algorithm: hashlib.Algorithm,
-        algorithm_str: str,
-        randbytes: Callable[[int], bytes],
-    ) -> None:
-        buffer = randbytes(512)
-
-        obj = algorithm(buffer)
-        other = hashlib.new(algorithm_str, buffer)
-
-        assert obj.digest() == other.digest()
-        assert obj.hexdigest() == other.hexdigest()
-
-    def test_update_and_copy(
-        self, algorithm: hashlib.Algorithm, randbytes: Callable[[int], bytes]
-    ) -> None:
-        buffer = randbytes(512)
-
-        obj = algorithm(buffer)
-        other = obj.copy()
-
-        assert obj.digest() == other.digest()
-        assert obj.hexdigest() == other.hexdigest()
-
-    def test_copy_and_update(
-        self, algorithm: hashlib.Algorithm, randbytes: Callable[[int], bytes]
-    ) -> None:
-        buffer = randbytes(512)
-
-        obj = algorithm(buffer)
-        other = obj.copy()
-        obj.update(buffer)
-        other.update(buffer)
-
-        assert obj.digest() == other.digest()
-        assert obj.hexdigest() == other.hexdigest()
-
-    def test_copy_and_update_nothing(
-        self, algorithm: hashlib.Algorithm, randbytes: Callable[[int], bytes]
-    ) -> None:
-        buffer = randbytes(512)
-
-        obj = algorithm(buffer)
-        other = obj.copy()
-        obj.update(b"")
-
-        assert obj.digest() == other.digest()
-        assert obj.hexdigest() == other.hexdigest()
-
-
-class TestHmac:
-    @pytest.fixture(params=tuple(hmac.algorithms_available))
-    def algorithm_str(self, request: Any) -> str:
-        assert isinstance(request.param, str)
-        return request.param
-
-    @pytest.fixture()
-    def algorithm(self, algorithm_str: str) -> hmac.Algorithm:
-        return cast(hmac.Algorithm, getattr(hmac, algorithm_str))
-
-    @pytest.mark.parametrize(
-        "repr_",
-        [repr, str],
-        ids=lambda f: f.__name__,  # type: ignore[no-any-return]
-    )
-    def test_repr(
-        self, repr_: Callable[[object], str], algorithm: hmac.Algorithm
-    ) -> None:
-        assert isinstance(repr_(algorithm(b"")), str)
-
-    def test_pickle(self, algorithm: hmac.Algorithm) -> None:
-        with pytest.raises(TypeError) as excinfo:
-            pickle.dumps(algorithm(b""))
-
-        assert str(excinfo.value).startswith("cannot pickle")
-
-    def test_accessors(
-        self, algorithm: hmac.Algorithm, algorithm_str: str
-    ) -> None:
-        obj = algorithm(b"")
-
-        assert obj.digest_size == SUPPORTED_SIZES[algorithm_str].digest_size
-        assert obj.block_size == SUPPORTED_SIZES[algorithm_str].block_size
-
-    def test_update(
-        self, algorithm: hmac.Algorithm, randbytes: Callable[[int], bytes]
-    ) -> None:
-        key = b"key"
-        buffer = randbytes(512)
-
-        obj = algorithm(key, b"")
-        obj.update(buffer)
-        other = algorithm(key, buffer)
-
-        assert obj.digest() == other.digest()
-        assert obj.hexdigest() == other.hexdigest()
-
-    def test_new(
-        self,
-        algorithm: hmac.Algorithm,
-        algorithm_str: str,
-        randbytes: Callable[[int], bytes],
-    ) -> None:
-        key = b"key"
-        buffer = randbytes(512)
-
-        obj = algorithm(key, buffer)
-        other = hmac.new(key, buffer, digestmod=algorithm_str)
-
-        assert obj.digest() == other.digest()
-        assert obj.hexdigest() == other.hexdigest()
-
-    def test_copy_and_update_nothing(
-        self, algorithm: hmac.Algorithm, randbytes: Callable[[int], bytes]
-    ) -> None:
-        key = b"key"
-        buffer = randbytes(512)
-
-        obj = algorithm(key, buffer)
-        other = algorithm(key, buffer)
-        obj.update(b"")
-
-        assert obj.digest() == other.digest()
-        assert obj.hexdigest() == other.hexdigest()
+# SPDX-License-Identifier: MIT
+
+"""Unit tests for mbedtls.md."""
+
+from __future__ import annotations
+
+import pickle
+from collections.abc import Collection
+from typing import Any, Callable, Mapping, NamedTuple, cast
+
+import pytest
+
+from mbedtls import hashlib, hmac
+from mbedtls._md import Hash
+
+
+class Size(NamedTuple):
+    digest_size: int
+    block_size: int
+
+
+SUPPORTED_SIZES: Mapping[str, Size] = {
+    "md2": Size(digest_size=16, block_size=16),
+    "md4": Size(digest_size=16, block_size=64),
+    "md5": Size(digest_size=16, block_size=64),
+    "sha1": Size(digest_size=20, block_size=64),
+    "sha224": Size(digest_size=28, block_size=64),
+    "sha256": Size(digest_size=32, block_size=64),
+    "sha384": Size(digest_size=48, block_size=128),
+    "sha512": Size(digest_size=64, block_size=128),
+    "ripemd160": Size(digest_size=20, block_size=64),
+}
+
+
+def test_algorithms() -> None:
+    assert isinstance(hashlib.algorithms_guaranteed, Collection)
+    assert hashlib.algorithms_guaranteed
+
+    assert isinstance(hashlib.algorithms_available, Collection)
+    assert hashlib.algorithms_available
+
+    assert frozenset(hashlib.algorithms_guaranteed).issubset(
+        hashlib.algorithms_available
+    )
+
+
+def test_invalid_name_raises_TypeError() -> None:
+    with pytest.raises(TypeError):
+        Hash(42)  # type: ignore[arg-type]
+
+
+def test_unavailable_cipher_raises_ValueError() -> None:
+    with pytest.raises(ValueError):
+        Hash("unavailable")
+
+
+class TestHash:
+    @pytest.fixture(params=tuple(hashlib.algorithms_available))
+    def algorithm_str(self, request: Any) -> str:
+        assert isinstance(request.param, str)
+        return request.param
+
+    @pytest.fixture()
+    def algorithm(self, algorithm_str: str) -> hashlib.Algorithm:
+        return cast(hashlib.Algorithm, getattr(hashlib, algorithm_str))
+
+    @pytest.mark.parametrize("repr_", [repr, str], ids=lambda f: f.__name__)
+    def test_repr(
+        self, repr_: Callable[[object], str], algorithm: hashlib.Algorithm
+    ) -> None:
+        assert isinstance(repr_(algorithm(b"")), str)
+
+    def test_pickle(self, algorithm: hashlib.Algorithm) -> None:
+        with pytest.raises(TypeError) as excinfo:
+            pickle.dumps(algorithm(b""))
+
+        assert str(excinfo.value).startswith("cannot pickle")
+
+    def test_accessors(
+        self, algorithm: hashlib.Algorithm, algorithm_str: str
+    ) -> None:
+        obj = algorithm(b"")
+
+        assert obj.digest_size == SUPPORTED_SIZES[algorithm_str].digest_size
+        assert obj.block_size == SUPPORTED_SIZES[algorithm_str].block_size
+
+    def test_update(
+        self, algorithm: hashlib.Algorithm, randbytes: Callable[[int], bytes]
+    ) -> None:
+        buffer = randbytes(512)
+
+        obj = algorithm(b"")
+        obj.update(buffer)
+        other = algorithm(buffer)
+
+        assert obj.digest() == other.digest()
+        assert obj.hexdigest() == other.hexdigest()
+
+    def test_new(
+        self,
+        algorithm: hashlib.Algorithm,
+        algorithm_str: str,
+        randbytes: Callable[[int], bytes],
+    ) -> None:
+        buffer = randbytes(512)
+
+        obj = algorithm(buffer)
+        other = hashlib.new(algorithm_str, buffer)
+
+        assert obj.digest() == other.digest()
+        assert obj.hexdigest() == other.hexdigest()
+
+    def test_update_and_copy(
+        self, algorithm: hashlib.Algorithm, randbytes: Callable[[int], bytes]
+    ) -> None:
+        buffer = randbytes(512)
+
+        obj = algorithm(buffer)
+        other = obj.copy()
+
+        assert obj.digest() == other.digest()
+        assert obj.hexdigest() == other.hexdigest()
+
+    def test_copy_and_update(
+        self, algorithm: hashlib.Algorithm, randbytes: Callable[[int], bytes]
+    ) -> None:
+        buffer = randbytes(512)
+
+        obj = algorithm(buffer)
+        other = obj.copy()
+        obj.update(buffer)
+        other.update(buffer)
+
+        assert obj.digest() == other.digest()
+        assert obj.hexdigest() == other.hexdigest()
+
+    def test_copy_and_update_nothing(
+        self, algorithm: hashlib.Algorithm, randbytes: Callable[[int], bytes]
+    ) -> None:
+        buffer = randbytes(512)
+
+        obj = algorithm(buffer)
+        other = obj.copy()
+        obj.update(b"")
+
+        assert obj.digest() == other.digest()
+        assert obj.hexdigest() == other.hexdigest()
+
+
+class TestHmac:
+    @pytest.fixture(params=tuple(hmac.algorithms_available))
+    def algorithm_str(self, request: Any) -> str:
+        assert isinstance(request.param, str)
+        return request.param
+
+    @pytest.fixture()
+    def algorithm(self, algorithm_str: str) -> hmac.Algorithm:
+        return cast(hmac.Algorithm, getattr(hmac, algorithm_str))
+
+    @pytest.mark.parametrize("repr_", [repr, str], ids=lambda f: f.__name__)
+    def test_repr(
+        self, repr_: Callable[[object], str], algorithm: hmac.Algorithm
+    ) -> None:
+        assert isinstance(repr_(algorithm(b"")), str)
+
+    def test_pickle(self, algorithm: hmac.Algorithm) -> None:
+        with pytest.raises(TypeError) as excinfo:
+            pickle.dumps(algorithm(b""))
+
+        assert str(excinfo.value).startswith("cannot pickle")
+
+    def test_accessors(
+        self, algorithm: hmac.Algorithm, algorithm_str: str
+    ) -> None:
+        obj = algorithm(b"")
+
+        assert obj.digest_size == SUPPORTED_SIZES[algorithm_str].digest_size
+        assert obj.block_size == SUPPORTED_SIZES[algorithm_str].block_size
+
+    def test_update(
+        self, algorithm: hmac.Algorithm, randbytes: Callable[[int], bytes]
+    ) -> None:
+        key = b"key"
+        buffer = randbytes(512)
+
+        obj = algorithm(key, b"")
+        obj.update(buffer)
+        other = algorithm(key, buffer)
+
+        assert obj.digest() == other.digest()
+        assert obj.hexdigest() == other.hexdigest()
+
+    def test_new(
+        self,
+        algorithm: hmac.Algorithm,
+        algorithm_str: str,
+        randbytes: Callable[[int], bytes],
+    ) -> None:
+        key = b"key"
+        buffer = randbytes(512)
+
+        obj = algorithm(key, buffer)
+        other = hmac.new(key, buffer, digestmod=algorithm_str)
+
+        assert obj.digest() == other.digest()
+        assert obj.hexdigest() == other.hexdigest()
+
+    def test_copy_and_update_nothing(
+        self, algorithm: hmac.Algorithm, randbytes: Callable[[int], bytes]
+    ) -> None:
+        key = b"key"
+        buffer = randbytes(512)
+
+        obj = algorithm(key, buffer)
+        other = algorithm(key, buffer)
+        obj.update(b"")
+
+        assert obj.digest() == other.digest()
+        assert obj.hexdigest() == other.hexdigest()
```

### Comparing `python-mbedtls-2.7.0/tests/test_mpi.py` & `python-mbedtls-2.7.1/tests/test_mpi.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,308 +1,304 @@
-# SPDX-License-Identifier: MIT
-
-from __future__ import annotations
-
-import math
-import numbers
-import pickle
-from binascii import hexlify, unhexlify
-from typing import Callable
-
-import pytest
-
-from mbedtls.mpi import MPI
-
-
-@pytest.mark.parametrize("value", [12, 2**32 - 1, 10**100])
-def test_from_int(value: int) -> None:
-    mpi = MPI.from_int(value)
-    assert mpi == value
-    assert value == mpi
-
-
-@pytest.mark.parametrize(
-    "repr_",
-    [repr, str],
-    ids=lambda f: f.__name__,  # type: ignore[no-any-return]
-)
-def test_repr(repr_: Callable[[object], str]) -> None:
-    assert isinstance(repr_(MPI(69)), str)
-
-
-def test_pickle() -> None:
-    value = MPI(1337)
-    assert value == pickle.loads(pickle.dumps(value))
-
-
-def test_hash() -> None:
-    assert isinstance(hash(MPI(1337)), int)
-
-
-def test_is_integral() -> None:
-    assert isinstance(MPI(42), numbers.Integral)
-
-
-def test_add() -> None:
-    assert MPI(12) + MPI(12) == 24
-    assert isinstance(MPI(12) + MPI(12), MPI)
-
-    assert MPI(12) + 12 == 24
-    assert isinstance(MPI(12) + 12, MPI)
-
-    assert 12 + MPI(12) == 24
-    assert isinstance(12 + MPI(12), MPI)
-
-
-def test_sub() -> None:
-    assert MPI(12) - MPI(5) == 7
-    assert isinstance(MPI(12) - MPI(5), MPI)
-
-    assert MPI(12) - 5 == 7
-    assert isinstance(MPI(12) - 5, MPI)
-
-    assert 12 - MPI(5) == 7
-    assert isinstance(12 - MPI(5), MPI)
-
-
-def test_mul() -> None:
-    assert MPI(12) * MPI(2) == 24
-    assert isinstance(MPI(12) * MPI(2), MPI)
-
-    assert MPI(12) * 2 == 24
-    assert isinstance(MPI(12) * 2, MPI)
-
-    assert 12 * MPI(2) == 24
-    assert isinstance(12 * MPI(2), MPI)
-
-
-def test_pow() -> None:
-    assert pow(MPI(12), 5, 12**5 + 1) == 248832
-    assert pow(MPI(12), 5, 7) == 3
-
-
-def test_eq() -> None:
-    assert MPI(12) == MPI(12)
-    assert MPI(12) == 12
-    assert 12 == MPI(12)
-
-
-def test_eq_no_implicit_conversion() -> None:
-    assert MPI(12) != 12.0
-    assert 12.0 != MPI(12)
-
-
-def test_neq() -> None:
-    assert MPI(12) != MPI(42)
-    assert MPI(12) != 42
-    assert 12 != MPI(42)
-    assert MPI(12) != 42.0
-    assert 12.0 != MPI(42)
-
-
-def test_lt() -> None:
-    assert MPI(12) < MPI(42)
-    assert MPI(12) < 42
-    assert 12 < MPI(42)
-
-    assert MPI(42) >= MPI(12)
-    assert MPI(42) >= 12
-    assert 42 >= MPI(12)
-
-    assert not MPI(12) < MPI(12)
-    assert not MPI(12) < 12
-    assert not 12 < MPI(12)
-
-
-def test_lt_no_implicit_converstions() -> None:
-    with pytest.raises(TypeError):
-        assert MPI(12) < 42.0  # type: ignore[operator]
-
-    with pytest.raises(TypeError):
-        assert 12.0 < MPI(42)  # type: ignore[operator]
-
-
-def test_gt_larger_number_is_false() -> None:
-    assert (MPI(12) > MPI(42)) is False
-    assert (MPI(12) > 42) is False
-    assert (12 > MPI(42)) is False
-
-
-def test_gt_smaller_number_is_true() -> None:
-    assert (MPI(42) > MPI(12)) is True
-    assert (MPI(42) > 12) is True
-    assert (42 > MPI(12)) is True
-
-
-def test_gt_same_number_is_false() -> None:
-    assert (MPI(12) > MPI(12)) is False
-    assert (MPI(12) > 12) is False
-    assert (12 > MPI(12)) is False
-
-
-def test_le() -> None:
-    assert (MPI(12) <= MPI(42)) is True
-    assert (MPI(12) <= MPI(12)) is True
-    assert (MPI(42) <= MPI(12)) is False
-
-
-def test_ge() -> None:
-    assert (MPI(42) >= MPI(12)) is True
-    assert (MPI(42) >= MPI(42)) is True
-    assert (MPI(12) >= MPI(42)) is False
-
-
-def test_bool() -> None:
-    assert bool(MPI(0)) is False
-
-
-def test_float() -> None:
-    assert isinstance(float(MPI(12)), float)
-    assert not isinstance(float(MPI(12)), numbers.Integral)
-    assert isinstance(float(MPI(12)), numbers.Real)
-    assert float(MPI(12)) == 12.0
-
-
-def test_trunc() -> None:
-    assert isinstance(math.trunc(MPI(12)), numbers.Integral)
-    assert math.trunc(MPI(12)) == 12
-
-
-def test_floor() -> None:
-    assert isinstance(math.floor(MPI(12)), numbers.Integral)
-    assert math.floor(MPI(12)) == 12
-
-
-def test_ceil() -> None:
-    assert isinstance(math.ceil(MPI(12)), numbers.Integral)
-    assert math.ceil(MPI(12)) == 12
-
-
-def test_round() -> None:
-    assert isinstance(round(MPI(12)), numbers.Integral)
-    assert round(MPI(12)) == 12
-    assert round(MPI(12), 0) == 12
-
-
-def test_rshift() -> None:
-    assert MPI(12) >> MPI(2) == 3
-    assert isinstance(MPI(12) >> MPI(2), MPI)
-
-    assert MPI(12) >> 2 == 3
-    assert isinstance(MPI(12) >> 2, MPI)
-
-    with pytest.raises(TypeError):
-        assert 12 >> MPI(2) == 3
-
-
-def test_lshift() -> None:
-    assert MPI(12) << MPI(2) == 48
-    assert isinstance(MPI(12) << MPI(2), MPI)
-
-    assert MPI(12) << 2 == 48
-    assert isinstance(MPI(12) << 2, MPI)
-
-    with pytest.raises(TypeError):
-        assert 12 << MPI(2) == 48
-
-
-def test_and() -> None:
-    assert MPI(12) & MPI(12) == 12
-    assert isinstance(MPI(12) & MPI(12), MPI)
-
-    assert MPI(12) & MPI(3) == 0
-    assert isinstance(MPI(12) & MPI(3), MPI)
-
-    assert MPI(15) & MPI(4) == 4
-    assert isinstance(MPI(15) & MPI(4), MPI)
-
-    assert MPI(15) & 4 == 4
-    assert isinstance(MPI(15) & 4, MPI)
-
-    with pytest.raises(TypeError):
-        assert 15 & MPI(4) == 4
-
-
-def test_or() -> None:
-    assert MPI(12) | MPI(12) == 12
-    assert isinstance(MPI(12) | MPI(12), MPI)
-
-    assert MPI(12) | MPI(3) == 15
-    assert isinstance(MPI(12) | MPI(3), MPI)
-
-    assert MPI(15) | MPI(4) == 15
-    assert isinstance(MPI(15) | MPI(4), MPI)
-
-    assert MPI(15) | 4 == 15
-    assert isinstance(MPI(15) | 4, MPI)
-
-    with pytest.raises(TypeError):
-        assert 15 | MPI(4) == 15
-
-
-def test_xor() -> None:
-    assert MPI(12) ^ MPI(12) == 0
-    assert isinstance(MPI(12) ^ MPI(12), MPI)
-
-    assert MPI(12) ^ MPI(3) == 15
-    assert isinstance(MPI(12) ^ MPI(3), MPI)
-
-    assert MPI(15) ^ MPI(4) == 11
-    assert isinstance(MPI(15) ^ MPI(4), MPI)
-
-    assert MPI(15) ^ 4 == 11
-    assert isinstance(MPI(15) ^ 4, MPI)
-
-    with pytest.raises(TypeError):
-        assert 15 ^ MPI(4) == 11
-
-
-def test_floordiv() -> None:
-    assert MPI(24) // MPI(2) == 12
-    assert isinstance(MPI(24) // MPI(2), MPI)
-
-    assert MPI(24) // 2 == 12
-    assert isinstance(MPI(24) // 2, MPI)
-
-    assert 24 // MPI(2) == 12
-    assert isinstance(24 // MPI(2), MPI)
-
-
-def test_mod() -> None:
-    assert MPI(12) % MPI(10) == 2
-    assert isinstance(MPI(12) % MPI(10), MPI)
-
-    assert MPI(12) % 10 == 2
-    assert isinstance(MPI(12) % 10, MPI)
-
-    assert 12 % MPI(10) == 2
-    assert isinstance(12 % MPI(10), MPI)
-
-
-@pytest.mark.parametrize("value", [12, 2**32 - 1, 10**100])
-def test_bit_length(value: int) -> None:
-    mpi = MPI(value)
-    assert mpi == value
-    assert mpi.bit_length() == value.bit_length()
-
-
-def test_from_empty_bytes() -> None:
-    value = b""
-    big = MPI.from_bytes(value, byteorder="big")
-    little = MPI.from_bytes(value, byteorder="little")
-    assert big == little == 0
-    assert big.bit_length() == little.bit_length() == 0
-
-
-def test_from_bytes() -> None:
-    value = unhexlify(b"DEADBEEF")
-    mpi = MPI.from_bytes(value, byteorder="big")
-    assert mpi.to_bytes(4, byteorder="big") == unhexlify(b"DEADBEEF")
-    assert mpi.to_bytes(4, byteorder="little") == unhexlify(b"EFBEADDE")
-    assert mpi == int(hexlify(value), 16)
-
-
-def test_to_bytes_overflow() -> None:
-    value = unhexlify(b"DEEADBEEFF")
-    mpi = MPI.from_bytes(value, byteorder="big")
-    with pytest.raises(OverflowError):
-        mpi.to_bytes(2, byteorder="big")
+# SPDX-License-Identifier: MIT
+
+from __future__ import annotations
+
+import math
+import numbers
+import pickle
+from binascii import hexlify, unhexlify
+from typing import Callable
+
+import pytest
+
+from mbedtls.mpi import MPI
+
+
+@pytest.mark.parametrize("value", [12, 2**32 - 1, 10**100])
+def test_from_int(value: int) -> None:
+    mpi = MPI.from_int(value)
+    assert mpi == value
+    assert value == mpi
+
+
+@pytest.mark.parametrize("repr_", [repr, str], ids=lambda f: f.__name__)
+def test_repr(repr_: Callable[[object], str]) -> None:
+    assert isinstance(repr_(MPI(69)), str)
+
+
+def test_pickle() -> None:
+    value = MPI(1337)
+    assert value == pickle.loads(pickle.dumps(value))
+
+
+def test_hash() -> None:
+    assert isinstance(hash(MPI(1337)), int)
+
+
+def test_is_integral() -> None:
+    assert isinstance(MPI(42), numbers.Integral)
+
+
+def test_add() -> None:
+    assert MPI(12) + MPI(12) == 24
+    assert isinstance(MPI(12) + MPI(12), MPI)
+
+    assert MPI(12) + 12 == 24
+    assert isinstance(MPI(12) + 12, MPI)
+
+    assert 12 + MPI(12) == 24
+    assert isinstance(12 + MPI(12), MPI)
+
+
+def test_sub() -> None:
+    assert MPI(12) - MPI(5) == 7
+    assert isinstance(MPI(12) - MPI(5), MPI)
+
+    assert MPI(12) - 5 == 7
+    assert isinstance(MPI(12) - 5, MPI)
+
+    assert 12 - MPI(5) == 7
+    assert isinstance(12 - MPI(5), MPI)
+
+
+def test_mul() -> None:
+    assert MPI(12) * MPI(2) == 24
+    assert isinstance(MPI(12) * MPI(2), MPI)
+
+    assert MPI(12) * 2 == 24
+    assert isinstance(MPI(12) * 2, MPI)
+
+    assert 12 * MPI(2) == 24
+    assert isinstance(12 * MPI(2), MPI)
+
+
+def test_pow() -> None:
+    assert pow(MPI(12), 5, 12**5 + 1) == 248832
+    assert pow(MPI(12), 5, 7) == 3
+
+
+def test_eq() -> None:
+    assert MPI(12) == MPI(12)
+    assert MPI(12) == 12
+    assert 12 == MPI(12)
+
+
+def test_eq_no_implicit_conversion() -> None:
+    assert MPI(12) != 12.0
+    assert 12.0 != MPI(12)
+
+
+def test_neq() -> None:
+    assert MPI(12) != MPI(42)
+    assert MPI(12) != 42
+    assert 12 != MPI(42)
+    assert MPI(12) != 42.0
+    assert 12.0 != MPI(42)
+
+
+def test_lt() -> None:
+    assert MPI(12) < MPI(42)
+    assert MPI(12) < 42
+    assert 12 < MPI(42)
+
+    assert MPI(42) >= MPI(12)
+    assert MPI(42) >= 12
+    assert 42 >= MPI(12)
+
+    assert not MPI(12) < MPI(12)
+    assert not MPI(12) < 12
+    assert not 12 < MPI(12)
+
+
+def test_lt_no_implicit_converstions() -> None:
+    with pytest.raises(TypeError):
+        assert MPI(12) < 42.0  # type: ignore[operator]
+
+    with pytest.raises(TypeError):
+        assert 12.0 < MPI(42)  # type: ignore[operator]
+
+
+def test_gt_larger_number_is_false() -> None:
+    assert (MPI(12) > MPI(42)) is False
+    assert (MPI(12) > 42) is False
+    assert (12 > MPI(42)) is False
+
+
+def test_gt_smaller_number_is_true() -> None:
+    assert (MPI(42) > MPI(12)) is True
+    assert (MPI(42) > 12) is True
+    assert (42 > MPI(12)) is True
+
+
+def test_gt_same_number_is_false() -> None:
+    assert (MPI(12) > MPI(12)) is False
+    assert (MPI(12) > 12) is False
+    assert (12 > MPI(12)) is False
+
+
+def test_le() -> None:
+    assert (MPI(12) <= MPI(42)) is True
+    assert (MPI(12) <= MPI(12)) is True
+    assert (MPI(42) <= MPI(12)) is False
+
+
+def test_ge() -> None:
+    assert (MPI(42) >= MPI(12)) is True
+    assert (MPI(42) >= MPI(42)) is True
+    assert (MPI(12) >= MPI(42)) is False
+
+
+def test_bool() -> None:
+    assert bool(MPI(0)) is False
+
+
+def test_float() -> None:
+    assert isinstance(float(MPI(12)), float)
+    assert not isinstance(float(MPI(12)), numbers.Integral)
+    assert isinstance(float(MPI(12)), numbers.Real)
+    assert float(MPI(12)) == 12.0
+
+
+def test_trunc() -> None:
+    assert isinstance(math.trunc(MPI(12)), numbers.Integral)
+    assert math.trunc(MPI(12)) == 12
+
+
+def test_floor() -> None:
+    assert isinstance(math.floor(MPI(12)), numbers.Integral)
+    assert math.floor(MPI(12)) == 12
+
+
+def test_ceil() -> None:
+    assert isinstance(math.ceil(MPI(12)), numbers.Integral)
+    assert math.ceil(MPI(12)) == 12
+
+
+def test_round() -> None:
+    assert isinstance(round(MPI(12)), numbers.Integral)
+    assert round(MPI(12)) == 12
+    assert round(MPI(12), 0) == 12
+
+
+def test_rshift() -> None:
+    assert MPI(12) >> MPI(2) == 3
+    assert isinstance(MPI(12) >> MPI(2), MPI)
+
+    assert MPI(12) >> 2 == 3
+    assert isinstance(MPI(12) >> 2, MPI)
+
+    with pytest.raises(TypeError):
+        assert 12 >> MPI(2) == 3
+
+
+def test_lshift() -> None:
+    assert MPI(12) << MPI(2) == 48
+    assert isinstance(MPI(12) << MPI(2), MPI)
+
+    assert MPI(12) << 2 == 48
+    assert isinstance(MPI(12) << 2, MPI)
+
+    with pytest.raises(TypeError):
+        assert 12 << MPI(2) == 48
+
+
+def test_and() -> None:
+    assert MPI(12) & MPI(12) == 12
+    assert isinstance(MPI(12) & MPI(12), MPI)
+
+    assert MPI(12) & MPI(3) == 0
+    assert isinstance(MPI(12) & MPI(3), MPI)
+
+    assert MPI(15) & MPI(4) == 4
+    assert isinstance(MPI(15) & MPI(4), MPI)
+
+    assert MPI(15) & 4 == 4
+    assert isinstance(MPI(15) & 4, MPI)
+
+    with pytest.raises(TypeError):
+        assert 15 & MPI(4) == 4
+
+
+def test_or() -> None:
+    assert MPI(12) | MPI(12) == 12
+    assert isinstance(MPI(12) | MPI(12), MPI)
+
+    assert MPI(12) | MPI(3) == 15
+    assert isinstance(MPI(12) | MPI(3), MPI)
+
+    assert MPI(15) | MPI(4) == 15
+    assert isinstance(MPI(15) | MPI(4), MPI)
+
+    assert MPI(15) | 4 == 15
+    assert isinstance(MPI(15) | 4, MPI)
+
+    with pytest.raises(TypeError):
+        assert 15 | MPI(4) == 15
+
+
+def test_xor() -> None:
+    assert MPI(12) ^ MPI(12) == 0
+    assert isinstance(MPI(12) ^ MPI(12), MPI)
+
+    assert MPI(12) ^ MPI(3) == 15
+    assert isinstance(MPI(12) ^ MPI(3), MPI)
+
+    assert MPI(15) ^ MPI(4) == 11
+    assert isinstance(MPI(15) ^ MPI(4), MPI)
+
+    assert MPI(15) ^ 4 == 11
+    assert isinstance(MPI(15) ^ 4, MPI)
+
+    with pytest.raises(TypeError):
+        assert 15 ^ MPI(4) == 11
+
+
+def test_floordiv() -> None:
+    assert MPI(24) // MPI(2) == 12
+    assert isinstance(MPI(24) // MPI(2), MPI)
+
+    assert MPI(24) // 2 == 12
+    assert isinstance(MPI(24) // 2, MPI)
+
+    assert 24 // MPI(2) == 12
+    assert isinstance(24 // MPI(2), MPI)
+
+
+def test_mod() -> None:
+    assert MPI(12) % MPI(10) == 2
+    assert isinstance(MPI(12) % MPI(10), MPI)
+
+    assert MPI(12) % 10 == 2
+    assert isinstance(MPI(12) % 10, MPI)
+
+    assert 12 % MPI(10) == 2
+    assert isinstance(12 % MPI(10), MPI)
+
+
+@pytest.mark.parametrize("value", [12, 2**32 - 1, 10**100])
+def test_bit_length(value: int) -> None:
+    mpi = MPI(value)
+    assert mpi == value
+    assert mpi.bit_length() == value.bit_length()
+
+
+def test_from_empty_bytes() -> None:
+    value = b""
+    big = MPI.from_bytes(value, byteorder="big")
+    little = MPI.from_bytes(value, byteorder="little")
+    assert big == little == 0
+    assert big.bit_length() == little.bit_length() == 0
+
+
+def test_from_bytes() -> None:
+    value = unhexlify(b"DEADBEEF")
+    mpi = MPI.from_bytes(value, byteorder="big")
+    assert mpi.to_bytes(4, byteorder="big") == unhexlify(b"DEADBEEF")
+    assert mpi.to_bytes(4, byteorder="little") == unhexlify(b"EFBEADDE")
+    assert mpi == int(hexlify(value), 16)
+
+
+def test_to_bytes_overflow() -> None:
+    value = unhexlify(b"DEEADBEEFF")
+    mpi = MPI.from_bytes(value, byteorder="big")
+    with pytest.raises(OverflowError):
+        mpi.to_bytes(2, byteorder="big")
```

### Comparing `python-mbedtls-2.7.0/tests/test_pk.py` & `python-mbedtls-2.7.1/tests/test_pk.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,591 +1,583 @@
-# SPDX-License-Identifier: MIT
-
-"""Unit tests for mbedtls.pk."""
-
-from __future__ import annotations
-
-import pickle
-import sys
-from pathlib import Path
-from typing import Any, Callable, List, Tuple, Type, Union, cast
-
-import pytest
-
-from mbedtls import hashlib
-from mbedtls.exceptions import TLSError
-from mbedtls.mpi import MPI
-from mbedtls.pk import _get_md_alg  # type: ignore
-from mbedtls.pk import (
-    ECC,
-    RSA,
-    Curve,
-    DHClient,
-    DHServer,
-    ECDHClient,
-    ECDHNaive,
-    ECDHServer,
-    ECPoint,
-    check_pair,
-    get_supported_ciphers,
-    get_supported_curves,
-)
-
-if sys.version_info < (3, 11):
-    from typing_extensions import assert_never
-else:
-    from typing import assert_never
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Literal
-else:
-    from typing import Literal
-
-
-_CipherType = Union[RSA, ECC]
-
-
-def test_supported_curves() -> None:
-    assert sorted(get_supported_curves()) == [
-        Curve.BRAINPOOLP256R1,
-        Curve.BRAINPOOLP384R1,
-        Curve.BRAINPOOLP512R1,
-        Curve.SECP192K1,
-        Curve.SECP192R1,
-        Curve.SECP224K1,
-        Curve.SECP224R1,
-        Curve.SECP256K1,
-        Curve.SECP256R1,
-        Curve.SECP384R1,
-        Curve.SECP521R1,
-        Curve.CURVE25519,
-        Curve.CURVE448,
-    ]
-
-
-def test_get_supported_ciphers() -> None:
-    assert list(get_supported_ciphers()) == [
-        b"NONE",
-        b"RSA",
-        b"EC",
-        b"EC_DH",
-        b"ECDSA",
-    ]
-
-
-def test_rsa_encryp_decrypt(randbytes: Callable[[int], bytes]) -> None:
-    rsa = RSA()
-    rsa.generate(1024)
-    msg = randbytes(rsa.key_size - 11)
-    assert rsa.decrypt(rsa.encrypt(msg)) == msg
-
-
-def do_generate(cipher: _CipherType) -> bytes:
-    if isinstance(cipher, RSA):
-        return cipher.generate(1024)
-    if isinstance(cipher, ECC):
-        return cipher.generate()
-    assert_never(cipher)
-
-
-class TestECPoint:
-    @pytest.fixture(params=[(MPI(1), MPI(2), MPI(3)), (1, 2, 3)])
-    def xyz(self, request: Any) -> Tuple[int, int, int]:
-        return request.param  # type: ignore[no-any-return]
-
-    @pytest.fixture()
-    def point(self, xyz: Tuple[int, int, int]) -> ECPoint:
-        return ECPoint(*xyz)
-
-    @pytest.mark.parametrize(
-        "repr_",
-        [repr, str],
-        ids=lambda f: f.__name__,  # type: ignore[no-any-return]
-    )
-    def test_repr(
-        self, repr_: Callable[[object], str], point: ECPoint
-    ) -> None:
-        assert isinstance(repr_(point), str)
-
-    def test_pickle(self, point: ECPoint) -> None:
-        assert point == pickle.loads(pickle.dumps(point))
-
-    def test_hash(self, point: ECPoint) -> None:
-        assert isinstance(hash(point), int)
-
-    def test_accessors(
-        self, point: ECPoint, xyz: Tuple[int, int, int]
-    ) -> None:
-        x, y, z = xyz
-        assert point.x == x
-        assert point.y == y
-        assert point.z == z
-
-    def test_eq_point(self, point: ECPoint, xyz: Tuple[int, int, int]) -> None:
-        assert (point == ECPoint(*xyz)) is True
-        assert (point == ECPoint(0, 0, 0)) is False
-
-    def test_eq_zero(self) -> None:
-        zero = ECPoint(0, 0, 0)
-        assert (zero == 1) is False
-        assert (zero == 0) is True
-        assert (zero == ECPoint(0, 0, 0)) is True
-
-    def test_bool(self, point: ECPoint) -> None:
-        assert bool(point) is True
-        assert bool(ECPoint(0, 0, 0)) is False
-
-
-class TestCipher:
-    @pytest.fixture(
-        params=[cast(object, RSA)]
-        + cast(
-            List[object],
-            [
-                curve
-                for curve in get_supported_curves()
-                if curve not in (Curve.CURVE25519, Curve.CURVE448)
-            ],
-        )
-    )
-    def cipher(self, request: Any) -> _CipherType:
-        if request.param is RSA:
-            return cast(RSA, request.param())
-        return ECC(request.param)
-
-    def test_pickle(self, cipher: _CipherType) -> None:
-        assert cipher == pickle.loads(pickle.dumps(cipher))
-
-    def test_hash(self, cipher: _CipherType) -> None:
-        assert isinstance(hash(cipher), int)
-
-    def test_export_private_key(
-        self, cipher: _CipherType, tmp_path: Path
-    ) -> None:
-        cipher_tag = {RSA: "RSA", ECC: "EC"}[type(cipher)]
-
-        assert cipher.export_key("DER") == b""
-        assert cipher.export_key("PEM") == ""
-        assert cipher.key_size == 0
-
-        der = do_generate(cipher)
-        assert der
-        assert cipher.key_size > 0
-
-        assert der == cipher.export_key()
-        assert der == cipher.export_key("DER")
-        assert der == bytes(cipher)
-        assert der == cipher
-        assert cipher == type(cipher).from_DER(der)
-
-        pem = cipher.export_key("PEM")
-        assert pem.startswith(f"-----BEGIN {cipher_tag} PRIVATE KEY-----\n")
-        assert pem.endswith(f"-----END {cipher_tag} PRIVATE KEY-----\n")
-        assert pem == str(cipher)
-        assert pem == cipher.to_PEM().private
-        assert cipher == type(cipher).from_PEM(pem)
-
-    @pytest.mark.parametrize(
-        "copy",
-        [
-            lambda cipher: type(cipher).from_DER(cipher.export_key("DER")),
-            lambda cipher: type(cipher).from_PEM(cipher.export_key("PEM")),
-        ],
-    )
-    def test_import_private_key(
-        self, cipher: _CipherType, copy: Callable[[_CipherType], _CipherType]
-    ) -> None:
-        assert not cipher.export_key()
-        assert not cipher.export_public_key()
-
-        key = do_generate(cipher)
-        assert key
-
-        other = copy(cipher)
-        other = type(cipher).from_buffer(key)
-        assert other == cipher
-        assert other.export_key() == cipher.export_key() == key
-        assert other.export_public_key() == cipher.export_public_key()
-        assert check_pair(cipher, other) is True  # Test private half.
-        assert check_pair(other, cipher) is True  # Test public half.
-        assert check_pair(other, other) is True
-
-    def test_import_from_file(
-        self, cipher: _CipherType, tmp_path: Path
-    ) -> None:
-        do_generate(cipher)
-
-        prv_der_file = tmp_path / "crt.prv.der"
-        prv_der_file.write_bytes(cipher.export_key("DER"))
-        assert cipher == type(cipher).from_file(prv_der_file)
-        prv_der_file.unlink()
-
-        pub_der_file = tmp_path / "crt.pub.der"
-        pub_der = cipher.export_public_key("DER")
-        pub_der_file.write_bytes(pub_der)
-        assert pub_der == type(cipher).from_file(pub_der_file)
-        pub_der_file.unlink()
-
-        prv_pem_file = tmp_path / "crt.prv.pem"
-        prv_pem_file.write_text(cipher.export_key("PEM"))
-        assert cipher == type(cipher).from_file(prv_pem_file)
-        prv_pem_file.unlink()
-
-        pub_pem_file = tmp_path / "crt.pub.pem"
-        pub_pem = cipher.export_public_key("PEM")
-        pub_pem_file.write_text(pub_pem)
-        assert pub_pem == type(cipher).from_file(pub_pem_file)
-        pub_pem_file.unlink()
-
-    def test_export_public_key(self, cipher: _CipherType) -> None:
-        assert cipher.export_public_key("DER") == b""
-        assert cipher.export_public_key("PEM") == ""
-
-        do_generate(cipher)
-        der = cipher.export_public_key("DER")
-        assert der
-        assert der == type(cipher).from_DER(der).export_public_key("DER")
-
-        pem = cipher.export_public_key("PEM")
-        assert pem.startswith("-----BEGIN PUBLIC KEY-----\n")
-        assert pem.endswith("-----END PUBLIC KEY-----\n")
-        assert pem == type(cipher).from_PEM(pem).export_public_key("PEM")
-
-    def test_import_public_key(self, cipher: _CipherType) -> None:
-        assert not cipher.export_key()
-        assert not cipher.export_public_key()
-
-        do_generate(cipher)
-
-        pub = cipher.export_public_key("DER")
-        other = type(cipher).from_buffer(pub)
-        assert not other.export_key()
-        assert other.export_public_key()
-        assert check_pair(cipher, other) is False  # Test private half.
-        assert check_pair(other, cipher) is True  # Test public half.
-        assert check_pair(other, other) is False
-        assert cipher != other
-
-    @pytest.mark.parametrize(
-        "digestmod",
-        [_get_md_alg(name) for name in hashlib.algorithms_guaranteed],
-        ids=lambda dm: dm().name,  # type: ignore[no-any-return]
-    )
-    def test_sign_verify(
-        self,
-        cipher: _CipherType,
-        digestmod: str,
-        randbytes: Callable[[int], bytes],
-    ) -> None:
-        msg = randbytes(4096)
-        assert cipher.sign(msg, digestmod) is None
-
-        do_generate(cipher)
-
-        sig = cipher.sign(msg, digestmod)
-        assert sig is not None
-        assert cipher.verify(msg, sig, digestmod) is True
-        assert cipher.verify(msg + b"\0", sig, digestmod) is False
-
-
-class TestECCExportKey:
-    @pytest.fixture(params=get_supported_curves())
-    def curve(self, request: Any) -> Curve:
-        assert isinstance(request.param, Curve)
-        return request.param
-
-    def test_export_private_key(self, curve: Curve) -> None:
-        ecc = ECC(curve)
-        assert ecc.export_key("NUM") == 0
-
-        ecc.generate()
-        assert ecc.export_key("NUM") != 0
-
-        if curve in (Curve.CURVE25519, Curve.CURVE448):
-            with pytest.raises(ValueError):
-                ecc.export_key("DER")
-        else:
-            der = ecc.export_key("DER")
-            assert der
-            assert ECC(curve).from_DER(der) == der
-
-        if curve in (Curve.CURVE25519, Curve.CURVE448):
-            with pytest.raises(ValueError):
-                ecc.export_key("PEM")
-        else:
-            pem = ecc.export_key("PEM")
-            assert pem
-            assert pem.startswith("-----BEGIN EC PRIVATE KEY-----\n")
-            assert pem.endswith("-----END EC PRIVATE KEY-----\n")
-
-    def test_export_public(self, curve: Curve) -> None:
-        ecc = ECC(curve)
-        assert ecc.export_public_key("POINT") == 0
-        assert ecc.export_public_key("POINT") == ECPoint(0, 0, 0)
-
-        ecc.generate()
-
-        pub = ecc.export_public_key("POINT")
-        assert isinstance(pub, ECPoint)
-        assert pub.x not in (0, pub.y, pub.z)
-        if curve in (Curve.CURVE25519, Curve.CURVE448):
-            assert pub.y == 0
-        else:
-            assert pub.y not in (0, pub.x, pub.z)
-        assert pub.z in (0, 1)
-
-        if curve in (Curve.CURVE25519, Curve.CURVE448):
-            with pytest.raises(ValueError):
-                ecc.export_public_key("DER")
-        else:
-            der = ecc.export_public_key("DER")
-            assert der
-
-        if curve in (Curve.CURVE25519, Curve.CURVE448):
-            with pytest.raises(ValueError):
-                ecc.export_public_key("PEM")
-        else:
-            pem = ecc.export_public_key("PEM")
-            assert pem
-            assert pem.startswith("-----BEGIN PUBLIC KEY-----\n")
-            assert pem.endswith("-----END PUBLIC KEY-----\n")
-
-
-class TestECCtoECDH:
-    # pylint: disable=protected-access
-
-    @pytest.mark.parametrize("curve", get_supported_curves())
-    def test_exchange(self, curve: Curve) -> None:
-        ecp = ECC(curve)
-        ecp.generate()
-
-        srv, cli = ECDHServer(ecp), ECDHClient(ecp)
-
-        cke = cli.generate()
-        assert cli._has_public()
-
-        srv.import_CKE(cke)
-        assert srv._has_peers_public() is True
-
-        srv_sec = srv.generate_secret()
-        cli_sec = cli.generate_secret()
-        assert srv_sec == cli_sec
-
-
-class TestDH:
-    @pytest.mark.parametrize("dh_cls", [DHServer, DHClient])
-    def test_pickle(
-        self, dh_cls: Union[Type[DHServer], Type[DHClient]]
-    ) -> None:
-        dhentity = dh_cls(MPI.prime(64), MPI.prime(20))
-
-        with pytest.raises(TypeError) as excinfo:
-            pickle.dumps(dhentity)
-
-        assert str(excinfo.value).startswith("cannot pickle")
-
-    @pytest.mark.parametrize("dh_cls", [DHServer, DHClient])
-    def test_accessors(
-        self, dh_cls: Union[Type[DHServer], Type[DHClient]]
-    ) -> None:
-        modulus = MPI.prime(64)
-        generator = MPI.prime(20)
-
-        dhentity = dh_cls(modulus, generator)
-
-        assert dhentity.modulus == modulus
-        assert dhentity.generator == generator
-        assert dhentity.key_size == 8
-        assert dhentity.shared_secret == 0
-
-    def test_exchange(self) -> None:
-        cli = DHClient(MPI.prime(64), MPI.prime(20))
-        srv = DHServer(MPI.prime(64), MPI.prime(20))
-
-        ske = srv.generate()
-        cli.import_SKE(ske)
-        cke = cli.generate()
-        srv.import_CKE(cke)
-
-        srv_sec = srv.generate_secret()
-        cli_sec = cli.generate_secret()
-        assert srv_sec == cli_sec
-        assert srv_sec == srv.shared_secret
-        assert cli_sec == cli.shared_secret
-
-
-class TestECDH:
-    # pylint: disable=protected-access
-
-    @pytest.fixture(params=get_supported_curves())
-    def key(self, request: Any) -> ECC:
-        key = ECC(request.param)
-        return key
-
-    @pytest.mark.parametrize("peer_cls", [ECDHServer, ECDHClient])
-    def test_pickle(
-        self, key: ECC, peer_cls: Union[Type[ECDHServer], Type[ECDHClient]]
-    ) -> None:
-        key.generate()
-        peer = peer_cls(key)
-
-        with pytest.raises(TypeError) as excinfo:
-            pickle.dumps(peer)
-
-        assert str(excinfo.value).startswith("cannot pickle")
-
-    @pytest.mark.parametrize("peer_cls", [ECDHServer, ECDHClient])
-    def test_key_accessors_without_key(
-        self, key: ECC, peer_cls: Union[Type[ECDHServer], Type[ECDHClient]]
-    ) -> None:
-        peer = peer_cls(key)
-
-        assert not peer._has_private()
-        assert not peer._has_public()
-        assert not peer._has_peers_public()
-        assert peer.private_key == 0
-        assert peer.public_key == 0
-        assert peer.peers_public_key == 0
-        assert peer.shared_secret == 0
-
-    def test_client_accessors_with_key(self, key: ECC) -> None:
-        der = key.generate()
-        fmt: Literal["NUM", "DER"] = (
-            "NUM" if key.curve in (Curve.CURVE25519, Curve.CURVE448) else "DER"
-        )
-        assert der == key.export_key(fmt)
-
-        peer = ECDHClient(key)
-
-        assert not peer._has_private()
-        assert not peer._has_public()
-        assert peer._has_peers_public()
-        assert peer.private_key == 0
-        assert peer.public_key == 0
-        assert peer.peers_public_key == key.export_public_key("POINT")
-        assert peer.shared_secret == 0
-
-    def test_server_accessors_with_key(self, key: ECC) -> None:
-        der = key.generate()
-        fmt: Literal["NUM", "DER"] = (
-            "NUM" if key.curve in (Curve.CURVE25519, Curve.CURVE448) else "DER"
-        )
-        assert der == key.export_key(fmt)
-
-        peer = ECDHServer(key)
-
-        assert peer._has_private()
-        assert peer._has_public()
-        assert not peer._has_peers_public()
-        assert peer.private_key == key.export_key("NUM")
-        assert peer.public_key == key.export_public_key("POINT")
-        assert peer.peers_public_key == 0
-        assert peer.shared_secret == 0
-
-    def test_exchange(self, key: ECC) -> None:
-        srv, cli = ECDHServer(key), ECDHClient(key)
-
-        ske = srv.generate()
-        assert srv._has_public()
-
-        cli.import_SKE(ske)
-        assert cli._has_peers_public() is True
-
-        cke = cli.generate()
-        assert cli._has_public()
-
-        srv.import_CKE(cke)
-        assert srv._has_peers_public() is True
-
-        srv_sec = srv.generate_secret()
-        cli_sec = cli.generate_secret()
-        assert srv_sec == srv.shared_secret
-        assert cli_sec == cli.shared_secret
-        assert srv_sec == cli_sec
-        assert srv.shared_secret == cli.shared_secret
-
-    def test_generate_public(self, key: ECC) -> None:
-        srv, cli = ECDHServer(key), ECDHClient(key)
-
-        srv.generate()
-        cli.private_key = srv.private_key
-        assert cli.public_key != srv.public_key
-        cli.generate_public_key()
-        assert cli.public_key == srv.public_key
-
-
-def do_exchange(alice: ECDHNaive, bob: ECDHNaive) -> None:
-    alice_to_bob = alice.generate()
-    bob_to_alice = bob.generate()
-    alice.import_peers_public(bob_to_alice)
-    bob.import_peers_public(alice_to_bob)
-    alice.generate_secret()
-    bob.generate_secret()
-
-
-class TestECDHNaive:
-    # pylint: disable=protected-access
-
-    @pytest.fixture(params=[Curve.CURVE448, Curve.CURVE25519])
-    def curve(self, request: Any) -> Curve:
-        assert isinstance(request.param, Curve)
-        return request.param
-
-    def test_key_accessors_without_key(self, curve: Curve) -> None:
-        peer = ECDHNaive(curve)
-
-        assert not peer._has_private()
-        assert not peer._has_public()
-        assert peer.shared_secret == 0
-        assert peer.private_key == 0
-        assert peer.public_key == 0
-        assert peer.peers_public_key == 0
-
-    def test_exchange(self, curve: Curve) -> None:
-        alice, bob = ECDHNaive(curve), ECDHNaive(curve)
-
-        alice_to_bob = alice.generate()
-        assert alice._has_public()
-
-        bob_to_alice = bob.generate()
-        assert bob._has_public()
-
-        assert alice.private_key != 0
-        assert bob.private_key != 0
-        assert alice.private_key != bob.private_key
-
-        assert alice.public_key != 0
-        assert bob.public_key != 0
-        assert alice.public_key != bob.public_key
-
-        alice.import_peers_public(bob_to_alice)
-        assert alice._has_peers_public() is True
-        assert alice.peers_public_key == bob.public_key
-
-        bob.import_peers_public(alice_to_bob)
-        assert bob._has_peers_public() is True
-        assert bob.peers_public_key == alice.public_key
-
-        alice_secret = alice.generate_secret()
-        bob_secret = bob.generate_secret()
-        assert alice_secret == bob_secret
-        assert alice_secret == alice.shared_secret
-        assert bob_secret == bob.shared_secret
-
-    def test_attacker_fails_with_public_keys(self, curve: Curve) -> None:
-        alice, bob = ECDHNaive(curve), ECDHNaive(curve)
-        do_exchange(alice, bob)
-
-        eve = ECDHNaive(curve)
-        eve.public_key = alice.public_key
-        eve.peers_public_key = bob.public_key
-        with pytest.raises(TLSError):
-            eve.generate_secret()
-
-    def test_attacker_succeeds_with_private_key(self, curve: Curve) -> None:
-        alice, bob = ECDHNaive(curve), ECDHNaive(curve)
-        do_exchange(alice, bob)
-
-        eve = ECDHNaive(curve)
-        eve.peers_public_key = bob.public_key
-        eve.private_key = alice.private_key
-        assert eve.generate_secret() == alice.shared_secret
+# SPDX-License-Identifier: MIT
+
+"""Unit tests for mbedtls.pk."""
+
+from __future__ import annotations
+
+import pickle
+import sys
+from pathlib import Path
+from typing import Any, Callable, List, Tuple, Type, Union, cast
+
+import pytest
+
+from mbedtls import hashlib
+from mbedtls.exceptions import TLSError
+from mbedtls.mpi import MPI
+from mbedtls.pk import _get_md_alg  # type: ignore
+from mbedtls.pk import (
+    ECC,
+    RSA,
+    Curve,
+    DHClient,
+    DHServer,
+    ECDHClient,
+    ECDHNaive,
+    ECDHServer,
+    ECPoint,
+    check_pair,
+    get_supported_ciphers,
+    get_supported_curves,
+)
+
+if sys.version_info < (3, 11):
+    from typing_extensions import assert_never
+else:
+    from typing import assert_never
+
+from typing import Literal
+
+_CipherType = Union[RSA, ECC]
+
+
+def test_supported_curves() -> None:
+    assert sorted(get_supported_curves()) == [
+        Curve.BRAINPOOLP256R1,
+        Curve.BRAINPOOLP384R1,
+        Curve.BRAINPOOLP512R1,
+        Curve.SECP192K1,
+        Curve.SECP192R1,
+        Curve.SECP224K1,
+        Curve.SECP224R1,
+        Curve.SECP256K1,
+        Curve.SECP256R1,
+        Curve.SECP384R1,
+        Curve.SECP521R1,
+        Curve.CURVE25519,
+        Curve.CURVE448,
+    ]
+
+
+def test_get_supported_ciphers() -> None:
+    assert list(get_supported_ciphers()) == [
+        b"NONE",
+        b"RSA",
+        b"EC",
+        b"EC_DH",
+        b"ECDSA",
+    ]
+
+
+def test_rsa_encryp_decrypt(randbytes: Callable[[int], bytes]) -> None:
+    rsa = RSA()
+    rsa.generate(1024)
+    msg = randbytes(rsa.key_size - 11)
+    assert rsa.decrypt(rsa.encrypt(msg)) == msg
+
+
+def do_generate(cipher: _CipherType) -> bytes:
+    if isinstance(cipher, RSA):
+        return cipher.generate(1024)
+    if isinstance(cipher, ECC):
+        return cipher.generate()
+    assert_never(cipher)
+
+
+class TestECPoint:
+    @pytest.fixture(params=[(MPI(1), MPI(2), MPI(3)), (1, 2, 3)])
+    def xyz(self, request: Any) -> Tuple[int, int, int]:
+        return request.param  # type: ignore[no-any-return]
+
+    @pytest.fixture()
+    def point(self, xyz: Tuple[int, int, int]) -> ECPoint:
+        return ECPoint(*xyz)
+
+    @pytest.mark.parametrize("repr_", [repr, str], ids=lambda f: f.__name__)
+    def test_repr(
+        self, repr_: Callable[[object], str], point: ECPoint
+    ) -> None:
+        assert isinstance(repr_(point), str)
+
+    def test_pickle(self, point: ECPoint) -> None:
+        assert point == pickle.loads(pickle.dumps(point))
+
+    def test_hash(self, point: ECPoint) -> None:
+        assert isinstance(hash(point), int)
+
+    def test_accessors(
+        self, point: ECPoint, xyz: Tuple[int, int, int]
+    ) -> None:
+        x, y, z = xyz
+        assert point.x == x
+        assert point.y == y
+        assert point.z == z
+
+    def test_eq_point(self, point: ECPoint, xyz: Tuple[int, int, int]) -> None:
+        assert (point == ECPoint(*xyz)) is True
+        assert (point == ECPoint(0, 0, 0)) is False
+
+    def test_eq_zero(self) -> None:
+        zero = ECPoint(0, 0, 0)
+        assert (zero == 1) is False
+        assert (zero == 0) is True
+        assert (zero == ECPoint(0, 0, 0)) is True
+
+    def test_bool(self, point: ECPoint) -> None:
+        assert bool(point) is True
+        assert bool(ECPoint(0, 0, 0)) is False
+
+
+class TestCipher:
+    @pytest.fixture(
+        params=[cast(object, RSA)]
+        + cast(
+            List[object],
+            [
+                curve
+                for curve in get_supported_curves()
+                if curve not in (Curve.CURVE25519, Curve.CURVE448)
+            ],
+        )
+    )
+    def cipher(self, request: Any) -> _CipherType:
+        if request.param is RSA:
+            return cast(RSA, request.param())
+        return ECC(request.param)
+
+    def test_pickle(self, cipher: _CipherType) -> None:
+        assert cipher == pickle.loads(pickle.dumps(cipher))
+
+    def test_hash(self, cipher: _CipherType) -> None:
+        assert isinstance(hash(cipher), int)
+
+    def test_export_private_key(
+        self, cipher: _CipherType, tmp_path: Path
+    ) -> None:
+        cipher_tag = {RSA: "RSA", ECC: "EC"}[type(cipher)]
+
+        assert cipher.export_key("DER") == b""
+        assert cipher.export_key("PEM") == ""
+        assert cipher.key_size == 0
+
+        der = do_generate(cipher)
+        assert der
+        assert cipher.key_size > 0
+
+        assert der == cipher.export_key()
+        assert der == cipher.export_key("DER")
+        assert der == bytes(cipher)
+        assert der == cipher
+        assert cipher == type(cipher).from_DER(der)
+
+        pem = cipher.export_key("PEM")
+        assert pem.startswith(f"-----BEGIN {cipher_tag} PRIVATE KEY-----\n")
+        assert pem.endswith(f"-----END {cipher_tag} PRIVATE KEY-----\n")
+        assert pem == str(cipher)
+        assert pem == cipher.to_PEM().private
+        assert cipher == type(cipher).from_PEM(pem)
+
+    @pytest.mark.parametrize(
+        "copy",
+        [
+            lambda cipher: type(cipher).from_DER(cipher.export_key("DER")),
+            lambda cipher: type(cipher).from_PEM(cipher.export_key("PEM")),
+        ],
+    )
+    def test_import_private_key(
+        self, cipher: _CipherType, copy: Callable[[_CipherType], _CipherType]
+    ) -> None:
+        assert not cipher.export_key()
+        assert not cipher.export_public_key()
+
+        key = do_generate(cipher)
+        assert key
+
+        other = copy(cipher)
+        other = type(cipher).from_buffer(key)
+        assert other == cipher
+        assert other.export_key() == cipher.export_key() == key
+        assert other.export_public_key() == cipher.export_public_key()
+        assert check_pair(cipher, other) is True  # Test private half.
+        assert check_pair(other, cipher) is True  # Test public half.
+        assert check_pair(other, other) is True
+
+    def test_import_from_file(
+        self, cipher: _CipherType, tmp_path: Path
+    ) -> None:
+        do_generate(cipher)
+
+        prv_der_file = tmp_path / "crt.prv.der"
+        prv_der_file.write_bytes(cipher.export_key("DER"))
+        assert cipher == type(cipher).from_file(prv_der_file)
+        prv_der_file.unlink()
+
+        pub_der_file = tmp_path / "crt.pub.der"
+        pub_der = cipher.export_public_key("DER")
+        pub_der_file.write_bytes(pub_der)
+        assert pub_der == type(cipher).from_file(pub_der_file)
+        pub_der_file.unlink()
+
+        prv_pem_file = tmp_path / "crt.prv.pem"
+        prv_pem_file.write_text(cipher.export_key("PEM"))
+        assert cipher == type(cipher).from_file(prv_pem_file)
+        prv_pem_file.unlink()
+
+        pub_pem_file = tmp_path / "crt.pub.pem"
+        pub_pem = cipher.export_public_key("PEM")
+        pub_pem_file.write_text(pub_pem)
+        assert pub_pem == type(cipher).from_file(pub_pem_file)
+        pub_pem_file.unlink()
+
+    def test_export_public_key(self, cipher: _CipherType) -> None:
+        assert cipher.export_public_key("DER") == b""
+        assert cipher.export_public_key("PEM") == ""
+
+        do_generate(cipher)
+        der = cipher.export_public_key("DER")
+        assert der
+        assert der == type(cipher).from_DER(der).export_public_key("DER")
+
+        pem = cipher.export_public_key("PEM")
+        assert pem.startswith("-----BEGIN PUBLIC KEY-----\n")
+        assert pem.endswith("-----END PUBLIC KEY-----\n")
+        assert pem == type(cipher).from_PEM(pem).export_public_key("PEM")
+
+    def test_import_public_key(self, cipher: _CipherType) -> None:
+        assert not cipher.export_key()
+        assert not cipher.export_public_key()
+
+        do_generate(cipher)
+
+        pub = cipher.export_public_key("DER")
+        other = type(cipher).from_buffer(pub)
+        assert not other.export_key()
+        assert other.export_public_key()
+        assert check_pair(cipher, other) is False  # Test private half.
+        assert check_pair(other, cipher) is True  # Test public half.
+        assert check_pair(other, other) is False
+        assert cipher != other
+
+    @pytest.mark.parametrize(
+        "digestmod",
+        [_get_md_alg(name) for name in hashlib.algorithms_guaranteed],
+        ids=lambda dm: dm().name,
+    )
+    def test_sign_verify(
+        self,
+        cipher: _CipherType,
+        digestmod: str,
+        randbytes: Callable[[int], bytes],
+    ) -> None:
+        msg = randbytes(4096)
+        assert cipher.sign(msg, digestmod) is None
+
+        do_generate(cipher)
+
+        sig = cipher.sign(msg, digestmod)
+        assert sig is not None
+        assert cipher.verify(msg, sig, digestmod) is True
+        assert cipher.verify(msg + b"\0", sig, digestmod) is False
+
+
+class TestECCExportKey:
+    @pytest.fixture(params=get_supported_curves())
+    def curve(self, request: Any) -> Curve:
+        assert isinstance(request.param, Curve)
+        return request.param
+
+    def test_export_private_key(self, curve: Curve) -> None:
+        ecc = ECC(curve)
+        assert ecc.export_key("NUM") == 0
+
+        ecc.generate()
+        assert ecc.export_key("NUM") != 0
+
+        if curve in (Curve.CURVE25519, Curve.CURVE448):
+            with pytest.raises(ValueError):
+                ecc.export_key("DER")
+        else:
+            der = ecc.export_key("DER")
+            assert der
+            assert ECC(curve).from_DER(der) == der
+
+        if curve in (Curve.CURVE25519, Curve.CURVE448):
+            with pytest.raises(ValueError):
+                ecc.export_key("PEM")
+        else:
+            pem = ecc.export_key("PEM")
+            assert pem
+            assert pem.startswith("-----BEGIN EC PRIVATE KEY-----\n")
+            assert pem.endswith("-----END EC PRIVATE KEY-----\n")
+
+    def test_export_public(self, curve: Curve) -> None:
+        ecc = ECC(curve)
+        assert ecc.export_public_key("POINT") == 0
+        assert ecc.export_public_key("POINT") == ECPoint(0, 0, 0)
+
+        ecc.generate()
+
+        pub = ecc.export_public_key("POINT")
+        assert isinstance(pub, ECPoint)
+        assert pub.x not in (0, pub.y, pub.z)
+        if curve in (Curve.CURVE25519, Curve.CURVE448):
+            assert pub.y == 0
+        else:
+            assert pub.y not in (0, pub.x, pub.z)
+        assert pub.z in (0, 1)
+
+        if curve in (Curve.CURVE25519, Curve.CURVE448):
+            with pytest.raises(ValueError):
+                ecc.export_public_key("DER")
+        else:
+            der = ecc.export_public_key("DER")
+            assert der
+
+        if curve in (Curve.CURVE25519, Curve.CURVE448):
+            with pytest.raises(ValueError):
+                ecc.export_public_key("PEM")
+        else:
+            pem = ecc.export_public_key("PEM")
+            assert pem
+            assert pem.startswith("-----BEGIN PUBLIC KEY-----\n")
+            assert pem.endswith("-----END PUBLIC KEY-----\n")
+
+
+class TestECCtoECDH:
+    # pylint: disable=protected-access
+
+    @pytest.mark.parametrize("curve", get_supported_curves())
+    def test_exchange(self, curve: Curve) -> None:
+        ecp = ECC(curve)
+        ecp.generate()
+
+        srv, cli = ECDHServer(ecp), ECDHClient(ecp)
+
+        cke = cli.generate()
+        assert cli._has_public()
+
+        srv.import_CKE(cke)
+        assert srv._has_peers_public() is True
+
+        srv_sec = srv.generate_secret()
+        cli_sec = cli.generate_secret()
+        assert srv_sec == cli_sec
+
+
+class TestDH:
+    @pytest.mark.parametrize("dh_cls", [DHServer, DHClient])
+    def test_pickle(
+        self, dh_cls: Union[Type[DHServer], Type[DHClient]]
+    ) -> None:
+        dhentity = dh_cls(MPI.prime(64), MPI.prime(20))
+
+        with pytest.raises(TypeError) as excinfo:
+            pickle.dumps(dhentity)
+
+        assert str(excinfo.value).startswith("cannot pickle")
+
+    @pytest.mark.parametrize("dh_cls", [DHServer, DHClient])
+    def test_accessors(
+        self, dh_cls: Union[Type[DHServer], Type[DHClient]]
+    ) -> None:
+        modulus = MPI.prime(64)
+        generator = MPI.prime(20)
+
+        dhentity = dh_cls(modulus, generator)
+
+        assert dhentity.modulus == modulus
+        assert dhentity.generator == generator
+        assert dhentity.key_size == 8
+        assert dhentity.shared_secret == 0
+
+    def test_exchange(self) -> None:
+        cli = DHClient(MPI.prime(64), MPI.prime(20))
+        srv = DHServer(MPI.prime(64), MPI.prime(20))
+
+        ske = srv.generate()
+        cli.import_SKE(ske)
+        cke = cli.generate()
+        srv.import_CKE(cke)
+
+        srv_sec = srv.generate_secret()
+        cli_sec = cli.generate_secret()
+        assert srv_sec == cli_sec
+        assert srv_sec == srv.shared_secret
+        assert cli_sec == cli.shared_secret
+
+
+class TestECDH:
+    # pylint: disable=protected-access
+
+    @pytest.fixture(params=get_supported_curves())
+    def key(self, request: Any) -> ECC:
+        key = ECC(request.param)
+        return key
+
+    @pytest.mark.parametrize("peer_cls", [ECDHServer, ECDHClient])
+    def test_pickle(
+        self, key: ECC, peer_cls: Union[Type[ECDHServer], Type[ECDHClient]]
+    ) -> None:
+        key.generate()
+        peer = peer_cls(key)
+
+        with pytest.raises(TypeError) as excinfo:
+            pickle.dumps(peer)
+
+        assert str(excinfo.value).startswith("cannot pickle")
+
+    @pytest.mark.parametrize("peer_cls", [ECDHServer, ECDHClient])
+    def test_key_accessors_without_key(
+        self, key: ECC, peer_cls: Union[Type[ECDHServer], Type[ECDHClient]]
+    ) -> None:
+        peer = peer_cls(key)
+
+        assert not peer._has_private()
+        assert not peer._has_public()
+        assert not peer._has_peers_public()
+        assert peer.private_key == 0
+        assert peer.public_key == 0
+        assert peer.peers_public_key == 0
+        assert peer.shared_secret == 0
+
+    def test_client_accessors_with_key(self, key: ECC) -> None:
+        der = key.generate()
+        fmt: Literal["NUM", "DER"] = (
+            "NUM" if key.curve in (Curve.CURVE25519, Curve.CURVE448) else "DER"
+        )
+        assert der == key.export_key(fmt)
+
+        peer = ECDHClient(key)
+
+        assert not peer._has_private()
+        assert not peer._has_public()
+        assert peer._has_peers_public()
+        assert peer.private_key == 0
+        assert peer.public_key == 0
+        assert peer.peers_public_key == key.export_public_key("POINT")
+        assert peer.shared_secret == 0
+
+    def test_server_accessors_with_key(self, key: ECC) -> None:
+        der = key.generate()
+        fmt: Literal["NUM", "DER"] = (
+            "NUM" if key.curve in (Curve.CURVE25519, Curve.CURVE448) else "DER"
+        )
+        assert der == key.export_key(fmt)
+
+        peer = ECDHServer(key)
+
+        assert peer._has_private()
+        assert peer._has_public()
+        assert not peer._has_peers_public()
+        assert peer.private_key == key.export_key("NUM")
+        assert peer.public_key == key.export_public_key("POINT")
+        assert peer.peers_public_key == 0
+        assert peer.shared_secret == 0
+
+    def test_exchange(self, key: ECC) -> None:
+        srv, cli = ECDHServer(key), ECDHClient(key)
+
+        ske = srv.generate()
+        assert srv._has_public()
+
+        cli.import_SKE(ske)
+        assert cli._has_peers_public() is True
+
+        cke = cli.generate()
+        assert cli._has_public()
+
+        srv.import_CKE(cke)
+        assert srv._has_peers_public() is True
+
+        srv_sec = srv.generate_secret()
+        cli_sec = cli.generate_secret()
+        assert srv_sec == srv.shared_secret
+        assert cli_sec == cli.shared_secret
+        assert srv_sec == cli_sec
+        assert srv.shared_secret == cli.shared_secret
+
+    def test_generate_public(self, key: ECC) -> None:
+        srv, cli = ECDHServer(key), ECDHClient(key)
+
+        srv.generate()
+        cli.private_key = srv.private_key
+        assert cli.public_key != srv.public_key
+        cli.generate_public_key()
+        assert cli.public_key == srv.public_key
+
+
+def do_exchange(alice: ECDHNaive, bob: ECDHNaive) -> None:
+    alice_to_bob = alice.generate()
+    bob_to_alice = bob.generate()
+    alice.import_peers_public(bob_to_alice)
+    bob.import_peers_public(alice_to_bob)
+    alice.generate_secret()
+    bob.generate_secret()
+
+
+class TestECDHNaive:
+    # pylint: disable=protected-access
+
+    @pytest.fixture(params=[Curve.CURVE448, Curve.CURVE25519])
+    def curve(self, request: Any) -> Curve:
+        assert isinstance(request.param, Curve)
+        return request.param
+
+    def test_key_accessors_without_key(self, curve: Curve) -> None:
+        peer = ECDHNaive(curve)
+
+        assert not peer._has_private()
+        assert not peer._has_public()
+        assert peer.shared_secret == 0
+        assert peer.private_key == 0
+        assert peer.public_key == 0
+        assert peer.peers_public_key == 0
+
+    def test_exchange(self, curve: Curve) -> None:
+        alice, bob = ECDHNaive(curve), ECDHNaive(curve)
+
+        alice_to_bob = alice.generate()
+        assert alice._has_public()
+
+        bob_to_alice = bob.generate()
+        assert bob._has_public()
+
+        assert alice.private_key != 0
+        assert bob.private_key != 0
+        assert alice.private_key != bob.private_key
+
+        assert alice.public_key != 0
+        assert bob.public_key != 0
+        assert alice.public_key != bob.public_key
+
+        alice.import_peers_public(bob_to_alice)
+        assert alice._has_peers_public() is True
+        assert alice.peers_public_key == bob.public_key
+
+        bob.import_peers_public(alice_to_bob)
+        assert bob._has_peers_public() is True
+        assert bob.peers_public_key == alice.public_key
+
+        alice_secret = alice.generate_secret()
+        bob_secret = bob.generate_secret()
+        assert alice_secret == bob_secret
+        assert alice_secret == alice.shared_secret
+        assert bob_secret == bob.shared_secret
+
+    def test_attacker_fails_with_public_keys(self, curve: Curve) -> None:
+        alice, bob = ECDHNaive(curve), ECDHNaive(curve)
+        do_exchange(alice, bob)
+
+        eve = ECDHNaive(curve)
+        eve.public_key = alice.public_key
+        eve.peers_public_key = bob.public_key
+        with pytest.raises(TLSError):
+            eve.generate_secret()
+
+    def test_attacker_succeeds_with_private_key(self, curve: Curve) -> None:
+        alice, bob = ECDHNaive(curve), ECDHNaive(curve)
+        do_exchange(alice, bob)
+
+        eve = ECDHNaive(curve)
+        eve.peers_public_key = bob.public_key
+        eve.private_key = alice.private_key
+        assert eve.generate_secret() == alice.shared_secret
```

### Comparing `python-mbedtls-2.7.0/tests/test_random.py` & `python-mbedtls-2.7.1/tests/test_random.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-# SPDX-License-Identifier: MIT
-
-"""Unit tests for mbedtls.random."""
-
-from __future__ import annotations
-
-import pickle
-import random
-from collections import defaultdict
-from typing import Callable, MutableMapping, Sequence
-
-import pytest
-
-import mbedtls._random as _drbg
-import mbedtls.mpi as _mpi
-from mbedtls.exceptions import TLSError
-
-
-def sample(start: int, end: int, k: int = 20) -> Sequence[int]:
-    return random.sample(range(start, end), k)
-
-
-class TestEntropy:
-    # pylint: disable=protected-access, no-member
-    def test_pickle(self) -> None:
-        entropy = _drbg.Random()._entropy
-        with pytest.raises(TypeError) as excinfo:
-            pickle.dumps(entropy)
-
-        assert str(excinfo.value).startswith("cannot pickle")
-
-    def test_gather(self) -> None:
-        # Only test that this does not raise.
-        _drbg.Random()._entropy.gather()
-
-    @pytest.mark.parametrize("length", range(64))
-    def test_retrieve(self, length: int) -> None:
-        entropy = _drbg.Random()._entropy
-        assert len(entropy.retrieve(length)) == length
-
-    @pytest.mark.parametrize("length", [100])
-    def test_retrieve_long_block_raises_exception(self, length: int) -> None:
-        entropy = _drbg.Random()._entropy
-        with pytest.raises(TLSError):
-            entropy.retrieve(length)
-
-    def test_update(self, randbytes: Callable[[int], bytes]) -> None:
-        # Only test that this does not raise.
-        buf = randbytes(64)
-        _drbg.Random()._entropy.update(buf)
-
-    def test_not_reproducible(self) -> None:
-        entropy = _drbg.Random()._entropy
-        assert entropy.retrieve(8) != entropy.retrieve(8)
-
-    def test_random_retrieve(self) -> None:
-        size = 4
-        entropy = _drbg.Random()._entropy
-        number = entropy.retrieve(size)
-        result: MutableMapping[bool, int] = defaultdict(int)
-        for _ in range(250):
-            result[entropy.retrieve(size) == number] += 1
-        assert result[True] <= 1
-
-
-class TestRandom:
-    def test_pickle(self) -> None:
-        random = _drbg.Random()
-        with pytest.raises(TypeError) as excinfo:
-            pickle.dumps(random)
-
-        assert str(excinfo.value).startswith("cannot pickle")
-
-    def test_reseed(self) -> None:
-        _drbg.Random()._reseed()
-
-    @pytest.mark.repeat(100)
-    def test_random(self) -> None:
-        value = _drbg.Random().random()
-        assert isinstance(value, float)
-        assert 0 <= value < 1
-
-    @pytest.mark.repeat(100)
-    def test_random_not_reproducible(self) -> None:
-        random = _drbg.Random()
-        assert random.random() != random.random()
-
-    @pytest.mark.repeat(100)
-    def test_getrandbits_not_reproducible(self) -> None:
-        random = _drbg.Random()
-        assert random.getrandbits(64) != random.getrandbits(64)
-
-    @pytest.mark.repeat(100)
-    def test_random_initial_values(self) -> None:
-        random = _drbg.Random()
-        other = _drbg.Random()
-        assert random.random() != other.random()
-
-    @pytest.mark.repeat(100)
-    def test_getrandbits_initial_values(self) -> None:
-        random = _drbg.Random()
-        other = _drbg.Random()
-        assert random.getrandbits(64) != other.getrandbits(64)
-
-    @pytest.mark.parametrize("nbits", [1, 5, 10, 50, 100, 300, 500])
-    def test_getrandbits_size(self, nbits: int) -> None:
-        random = _drbg.Random()
-        value = random.getrandbits(nbits)
-        assert isinstance(value, _mpi.MPI)
-        assert value.bit_length() == pytest.approx(nbits, abs=8)
-        assert value.bit_length() <= nbits
-
-    @pytest.mark.parametrize("nbits", [-1, 0])
-    def test_getrandbits_negative_k_raises_value_error(
-        self, nbits: int
-    ) -> None:
-        random = _drbg.Random()
-        with pytest.raises(ValueError):
-            random.getrandbits(nbits)
-
-    def test_getrandbits_nonint_k_raises_type_error(self) -> None:
-        random = _drbg.Random()
-        with pytest.raises(TypeError):
-            random.getrandbits("a")  # type: ignore[arg-type]
+# SPDX-License-Identifier: MIT
+
+"""Unit tests for mbedtls.random."""
+
+from __future__ import annotations
+
+import pickle
+import random
+from collections import defaultdict
+from typing import Callable, MutableMapping, Sequence
+
+import pytest
+
+import mbedtls._random as _drbg
+import mbedtls.mpi as _mpi
+from mbedtls.exceptions import TLSError
+
+
+def sample(start: int, end: int, k: int = 20) -> Sequence[int]:
+    return random.sample(range(start, end), k)
+
+
+class TestEntropy:
+    # pylint: disable=protected-access, no-member
+    def test_pickle(self) -> None:
+        entropy = _drbg.Random()._entropy
+        with pytest.raises(TypeError) as excinfo:
+            pickle.dumps(entropy)
+
+        assert str(excinfo.value).startswith("cannot pickle")
+
+    def test_gather(self) -> None:
+        # Only test that this does not raise.
+        _drbg.Random()._entropy.gather()
+
+    @pytest.mark.parametrize("length", range(64))
+    def test_retrieve(self, length: int) -> None:
+        entropy = _drbg.Random()._entropy
+        assert len(entropy.retrieve(length)) == length
+
+    @pytest.mark.parametrize("length", [100])
+    def test_retrieve_long_block_raises_exception(self, length: int) -> None:
+        entropy = _drbg.Random()._entropy
+        with pytest.raises(TLSError):
+            entropy.retrieve(length)
+
+    def test_update(self, randbytes: Callable[[int], bytes]) -> None:
+        # Only test that this does not raise.
+        buf = randbytes(64)
+        _drbg.Random()._entropy.update(buf)
+
+    def test_not_reproducible(self) -> None:
+        entropy = _drbg.Random()._entropy
+        assert entropy.retrieve(8) != entropy.retrieve(8)
+
+    def test_random_retrieve(self) -> None:
+        size = 4
+        entropy = _drbg.Random()._entropy
+        number = entropy.retrieve(size)
+        result: MutableMapping[bool, int] = defaultdict(int)
+        for _ in range(250):
+            result[entropy.retrieve(size) == number] += 1
+        assert result[True] <= 1
+
+
+class TestRandom:
+    def test_pickle(self) -> None:
+        random = _drbg.Random()
+        with pytest.raises(TypeError) as excinfo:
+            pickle.dumps(random)
+
+        assert str(excinfo.value).startswith("cannot pickle")
+
+    def test_reseed(self) -> None:
+        _drbg.Random()._reseed()
+
+    @pytest.mark.repeat(100)
+    def test_random(self) -> None:
+        value = _drbg.Random().random()
+        assert isinstance(value, float)
+        assert 0 <= value < 1
+
+    @pytest.mark.repeat(100)
+    def test_random_not_reproducible(self) -> None:
+        random = _drbg.Random()
+        assert random.random() != random.random()
+
+    @pytest.mark.repeat(100)
+    def test_getrandbits_not_reproducible(self) -> None:
+        random = _drbg.Random()
+        assert random.getrandbits(64) != random.getrandbits(64)
+
+    @pytest.mark.repeat(100)
+    def test_random_initial_values(self) -> None:
+        random = _drbg.Random()
+        other = _drbg.Random()
+        assert random.random() != other.random()
+
+    @pytest.mark.repeat(100)
+    def test_getrandbits_initial_values(self) -> None:
+        random = _drbg.Random()
+        other = _drbg.Random()
+        assert random.getrandbits(64) != other.getrandbits(64)
+
+    @pytest.mark.parametrize("nbits", [1, 5, 10, 50, 100, 300, 500])
+    def test_getrandbits_size(self, nbits: int) -> None:
+        random = _drbg.Random()
+        value = random.getrandbits(nbits)
+        assert isinstance(value, _mpi.MPI)
+        assert value.bit_length() == pytest.approx(nbits, abs=8)
+        assert value.bit_length() <= nbits
+
+    @pytest.mark.parametrize("nbits", [-1, 0])
+    def test_getrandbits_negative_k_raises_value_error(
+        self, nbits: int
+    ) -> None:
+        random = _drbg.Random()
+        with pytest.raises(ValueError):
+            random.getrandbits(nbits)
+
+    def test_getrandbits_nonint_k_raises_type_error(self) -> None:
+        random = _drbg.Random()
+        with pytest.raises(TypeError):
+            random.getrandbits("a")  # type: ignore[arg-type]
```

### Comparing `python-mbedtls-2.7.0/tests/test_ringbuf.py` & `python-mbedtls-2.7.1/tests/test_ringbuf.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,288 +1,288 @@
-# SPDX-License-Identifier: MIT
-
-from __future__ import annotations
-
-import pickle
-from random import randint
-from typing import Any, Callable
-
-import pytest
-
-from mbedtls._ringbuf import RingBuffer  # type: ignore
-
-
-@pytest.fixture()
-def randomize_start(
-    randbytes: Callable[[int], bytes]
-) -> Callable[[bytes], None]:
-    def impl(buffer: RingBuffer) -> None:
-        # Randomize start of the buffer.
-        size = randint(0, buffer.maxlen)
-        buffer.write(randbytes(size))
-        consumed = buffer.consume(size)
-        assert buffer.empty()
-        assert consumed == size
-
-    return impl
-
-
-class TestRingBuf:
-    @pytest.fixture(params=[2000, 16384])
-    def maxlen(self, request: Any) -> int:
-        assert isinstance(request.param, int)
-        return request.param
-
-    def test_initial_conditions(self, maxlen: int) -> None:
-        buffer = RingBuffer(maxlen)
-
-        assert not buffer
-        assert len(buffer) == 0
-        assert buffer.maxlen == maxlen
-        assert buffer.empty()
-        assert not buffer.full()
-
-        assert buffer == b""
-
-    def test_clear(
-        self,
-        maxlen: int,
-        randomize_start: Callable[[bytes], None],
-        randbytes: Callable[[int], bytes],
-    ) -> None:
-        buffer = RingBuffer(maxlen)
-        randomize_start(buffer)
-
-        data = randbytes(maxlen)
-        written = buffer.write(data)
-        buffer.clear()
-
-        assert written == maxlen
-        assert not buffer
-        assert len(buffer) == 0
-        assert buffer.maxlen == maxlen
-        assert buffer.empty()
-        assert not buffer.full()
-
-        assert buffer == b""
-
-    def test_write_empty(
-        self, maxlen: int, randomize_start: Callable[[bytes], None]
-    ) -> None:
-        buffer = RingBuffer(maxlen)
-        randomize_start(buffer)
-
-        written = buffer.write(b"")
-        assert not written
-        assert not buffer
-        assert len(buffer) == 0
-        assert buffer.empty()
-        assert not buffer.full()
-
-        assert buffer == b""
-
-    def test_pickle(
-        self,
-        maxlen: int,
-        randomize_start: Callable[[bytes], None],
-        randbytes: Callable[[int], bytes],
-    ) -> None:
-        buffer = RingBuffer(maxlen)
-        randomize_start(buffer)
-
-        data = randbytes(maxlen // 2)
-        assert buffer.write(data) == len(data)
-
-        other = pickle.loads(pickle.dumps(buffer))
-        assert other
-        assert other == buffer
-
-    def test_consume_zero(
-        self,
-        maxlen: int,
-        randomize_start: Callable[[bytes], None],
-        randbytes: Callable[[int], bytes],
-    ) -> None:
-        buffer = RingBuffer(maxlen)
-        randomize_start(buffer)
-
-        data = randbytes(maxlen)
-        assert buffer.write(data) == len(data)
-        buffer.consume(0)
-
-        assert buffer.full()
-        assert buffer == data
-
-    def test_peek_zero(
-        self,
-        maxlen: int,
-        randomize_start: Callable[[bytes], None],
-        randbytes: Callable[[int], bytes],
-    ) -> None:
-        buffer = RingBuffer(maxlen)
-        randomize_start(buffer)
-
-        data = randbytes(maxlen)
-        assert buffer.write(data) == len(data)
-
-        peeked = buffer.peek(0)
-        assert peeked == b""
-
-        assert buffer.full()
-        assert buffer == data
-
-    def test_read_zero(
-        self,
-        maxlen: int,
-        randomize_start: Callable[[bytes], None],
-        randbytes: Callable[[int], bytes],
-    ) -> None:
-        buffer = RingBuffer(maxlen)
-        randomize_start(buffer)
-
-        data = randbytes(maxlen)
-        written = buffer.write(data)
-
-        assert written == maxlen
-        assert buffer.read(0) == b""
-
-    def test_write_full(
-        self,
-        maxlen: int,
-        randomize_start: Callable[[bytes], None],
-        randbytes: Callable[[int], bytes],
-    ) -> None:
-        buffer = RingBuffer(maxlen)
-        randomize_start(buffer)
-
-        data = randbytes(maxlen)
-        written = buffer.write(data)
-        assert written == maxlen
-        assert buffer
-        assert len(buffer) == maxlen
-        assert buffer.maxlen == maxlen
-        assert not buffer.empty()
-        assert buffer.full()
-
-        assert buffer == data
-
-    @pytest.mark.parametrize(
-        "chunk_size", [10, 100, 1000, 1997, 1998, 1999, 2000]
-    )
-    def test_write_chunks(
-        self,
-        maxlen: int,
-        chunk_size: int,
-        randomize_start: Callable[[bytes], None],
-        randbytes: Callable[[int], bytes],
-    ) -> None:
-        buffer = RingBuffer(maxlen)
-        randomize_start(buffer)
-
-        data = randbytes(maxlen)
-        written = 0
-        for index in range(0, maxlen, chunk_size):
-            written += buffer.write(data[index : index + chunk_size])
-
-        assert written == maxlen
-        assert buffer.full()
-        assert buffer == data
-
-    @pytest.mark.parametrize(
-        "chunk_size", [10, 100, 1000, 1997, 1998, 1999, 2000]
-    )
-    def test_peek(
-        self,
-        maxlen: int,
-        chunk_size: int,
-        randomize_start: Callable[[bytes], None],
-        randbytes: Callable[[int], bytes],
-    ) -> None:
-        buffer = RingBuffer(maxlen)
-        randomize_start(buffer)
-
-        data = randbytes(maxlen)
-        written = buffer.write(data)
-        for index in range(0, maxlen, chunk_size):
-            assert buffer.peek(index) == data[0:index]
-
-        assert written == maxlen
-        assert buffer == data
-
-    @pytest.mark.parametrize(
-        "chunk_size", [10, 100, 1000, 1997, 1998, 1999, 2000]
-    )
-    def test_read_chunks(
-        self,
-        maxlen: int,
-        chunk_size: int,
-        randomize_start: Callable[[bytes], None],
-        randbytes: Callable[[int], bytes],
-    ) -> None:
-        buffer = RingBuffer(maxlen)
-        randomize_start(buffer)
-
-        data = randbytes(maxlen)
-        written = buffer.write(data)
-        for index in range(0, maxlen, chunk_size):
-            assert len(buffer) == maxlen - index
-            assert buffer.read(chunk_size) == data[index : index + chunk_size]
-        assert written == maxlen
-        assert buffer.empty()
-
-    @pytest.mark.parametrize(
-        "chunk_size", [10, 100, 1000, 1997, 1998, 1999, 2000]
-    )
-    def test_read_write_with_wraparound(
-        self,
-        maxlen: int,
-        chunk_size: int,
-        randomize_start: Callable[[bytes], None],
-        randbytes: Callable[[int], bytes],
-    ) -> None:
-        buffer = RingBuffer(maxlen)
-        randomize_start(buffer)
-
-        wraparound = 5
-        written = 0
-        for _ in range(wraparound * maxlen // chunk_size):
-            data = randbytes(chunk_size)
-            written += buffer.write(data)
-            assert buffer.read(chunk_size) == data
-            assert buffer.empty()
-        assert written >= maxlen * (wraparound - 1)
-
-    def test_read_write_with_wraparound_long(
-        self,
-        maxlen: int,
-        randomize_start: Callable[[bytes], None],
-        randbytes: Callable[[int], bytes],
-    ) -> None:
-        buffer = RingBuffer(maxlen)
-        randomize_start(buffer)
-
-        size = randint(2, 42) * maxlen
-        step = randint(1, maxlen)
-        written = 0
-        for _ in range(0, size, step):
-            data = randbytes(step)
-            amt = buffer.write(data)
-            written += amt
-            assert amt == step
-            assert amt == len(data)
-            assert written % step == 0
-            assert buffer.read(len(data)) == data
-            assert buffer.empty()
-
-    def test_write_overflow_raises_buffererror(
-        self,
-        maxlen: int,
-        randomize_start: Callable[[bytes], None],
-        randbytes: Callable[[int], bytes],
-    ) -> None:
-        buffer = RingBuffer(maxlen)
-        randomize_start(buffer)
-
-        data = randbytes(maxlen + 1)
-        with pytest.raises(BufferError):
-            buffer.write(data)
-        assert not buffer
+# SPDX-License-Identifier: MIT
+
+from __future__ import annotations
+
+import pickle
+from random import randint
+from typing import Any, Callable
+
+import pytest
+
+from mbedtls._ringbuf import RingBuffer  # type: ignore
+
+
+@pytest.fixture()
+def randomize_start(
+    randbytes: Callable[[int], bytes]
+) -> Callable[[bytes], None]:
+    def impl(buffer: RingBuffer) -> None:
+        # Randomize start of the buffer.
+        size = randint(0, buffer.maxlen)
+        buffer.write(randbytes(size))
+        consumed = buffer.consume(size)
+        assert buffer.empty()
+        assert consumed == size
+
+    return impl
+
+
+class TestRingBuf:
+    @pytest.fixture(params=[2000, 16384])
+    def maxlen(self, request: Any) -> int:
+        assert isinstance(request.param, int)
+        return request.param
+
+    def test_initial_conditions(self, maxlen: int) -> None:
+        buffer = RingBuffer(maxlen)
+
+        assert not buffer
+        assert len(buffer) == 0
+        assert buffer.maxlen == maxlen
+        assert buffer.empty()
+        assert not buffer.full()
+
+        assert buffer == b""
+
+    def test_clear(
+        self,
+        maxlen: int,
+        randomize_start: Callable[[bytes], None],
+        randbytes: Callable[[int], bytes],
+    ) -> None:
+        buffer = RingBuffer(maxlen)
+        randomize_start(buffer)
+
+        data = randbytes(maxlen)
+        written = buffer.write(data)
+        buffer.clear()
+
+        assert written == maxlen
+        assert not buffer
+        assert len(buffer) == 0
+        assert buffer.maxlen == maxlen
+        assert buffer.empty()
+        assert not buffer.full()
+
+        assert buffer == b""
+
+    def test_write_empty(
+        self, maxlen: int, randomize_start: Callable[[bytes], None]
+    ) -> None:
+        buffer = RingBuffer(maxlen)
+        randomize_start(buffer)
+
+        written = buffer.write(b"")
+        assert not written
+        assert not buffer
+        assert len(buffer) == 0
+        assert buffer.empty()
+        assert not buffer.full()
+
+        assert buffer == b""
+
+    def test_pickle(
+        self,
+        maxlen: int,
+        randomize_start: Callable[[bytes], None],
+        randbytes: Callable[[int], bytes],
+    ) -> None:
+        buffer = RingBuffer(maxlen)
+        randomize_start(buffer)
+
+        data = randbytes(maxlen // 2)
+        assert buffer.write(data) == len(data)
+
+        other = pickle.loads(pickle.dumps(buffer))
+        assert other
+        assert other == buffer
+
+    def test_consume_zero(
+        self,
+        maxlen: int,
+        randomize_start: Callable[[bytes], None],
+        randbytes: Callable[[int], bytes],
+    ) -> None:
+        buffer = RingBuffer(maxlen)
+        randomize_start(buffer)
+
+        data = randbytes(maxlen)
+        assert buffer.write(data) == len(data)
+        buffer.consume(0)
+
+        assert buffer.full()
+        assert buffer == data
+
+    def test_peek_zero(
+        self,
+        maxlen: int,
+        randomize_start: Callable[[bytes], None],
+        randbytes: Callable[[int], bytes],
+    ) -> None:
+        buffer = RingBuffer(maxlen)
+        randomize_start(buffer)
+
+        data = randbytes(maxlen)
+        assert buffer.write(data) == len(data)
+
+        peeked = buffer.peek(0)
+        assert peeked == b""
+
+        assert buffer.full()
+        assert buffer == data
+
+    def test_read_zero(
+        self,
+        maxlen: int,
+        randomize_start: Callable[[bytes], None],
+        randbytes: Callable[[int], bytes],
+    ) -> None:
+        buffer = RingBuffer(maxlen)
+        randomize_start(buffer)
+
+        data = randbytes(maxlen)
+        written = buffer.write(data)
+
+        assert written == maxlen
+        assert buffer.read(0) == b""
+
+    def test_write_full(
+        self,
+        maxlen: int,
+        randomize_start: Callable[[bytes], None],
+        randbytes: Callable[[int], bytes],
+    ) -> None:
+        buffer = RingBuffer(maxlen)
+        randomize_start(buffer)
+
+        data = randbytes(maxlen)
+        written = buffer.write(data)
+        assert written == maxlen
+        assert buffer
+        assert len(buffer) == maxlen
+        assert buffer.maxlen == maxlen
+        assert not buffer.empty()
+        assert buffer.full()
+
+        assert buffer == data
+
+    @pytest.mark.parametrize(
+        "chunk_size", [10, 100, 1000, 1997, 1998, 1999, 2000]
+    )
+    def test_write_chunks(
+        self,
+        maxlen: int,
+        chunk_size: int,
+        randomize_start: Callable[[bytes], None],
+        randbytes: Callable[[int], bytes],
+    ) -> None:
+        buffer = RingBuffer(maxlen)
+        randomize_start(buffer)
+
+        data = randbytes(maxlen)
+        written = 0
+        for index in range(0, maxlen, chunk_size):
+            written += buffer.write(data[index : index + chunk_size])
+
+        assert written == maxlen
+        assert buffer.full()
+        assert buffer == data
+
+    @pytest.mark.parametrize(
+        "chunk_size", [10, 100, 1000, 1997, 1998, 1999, 2000]
+    )
+    def test_peek(
+        self,
+        maxlen: int,
+        chunk_size: int,
+        randomize_start: Callable[[bytes], None],
+        randbytes: Callable[[int], bytes],
+    ) -> None:
+        buffer = RingBuffer(maxlen)
+        randomize_start(buffer)
+
+        data = randbytes(maxlen)
+        written = buffer.write(data)
+        for index in range(0, maxlen, chunk_size):
+            assert buffer.peek(index) == data[0:index]
+
+        assert written == maxlen
+        assert buffer == data
+
+    @pytest.mark.parametrize(
+        "chunk_size", [10, 100, 1000, 1997, 1998, 1999, 2000]
+    )
+    def test_read_chunks(
+        self,
+        maxlen: int,
+        chunk_size: int,
+        randomize_start: Callable[[bytes], None],
+        randbytes: Callable[[int], bytes],
+    ) -> None:
+        buffer = RingBuffer(maxlen)
+        randomize_start(buffer)
+
+        data = randbytes(maxlen)
+        written = buffer.write(data)
+        for index in range(0, maxlen, chunk_size):
+            assert len(buffer) == maxlen - index
+            assert buffer.read(chunk_size) == data[index : index + chunk_size]
+        assert written == maxlen
+        assert buffer.empty()
+
+    @pytest.mark.parametrize(
+        "chunk_size", [10, 100, 1000, 1997, 1998, 1999, 2000]
+    )
+    def test_read_write_with_wraparound(
+        self,
+        maxlen: int,
+        chunk_size: int,
+        randomize_start: Callable[[bytes], None],
+        randbytes: Callable[[int], bytes],
+    ) -> None:
+        buffer = RingBuffer(maxlen)
+        randomize_start(buffer)
+
+        wraparound = 5
+        written = 0
+        for _ in range(wraparound * maxlen // chunk_size):
+            data = randbytes(chunk_size)
+            written += buffer.write(data)
+            assert buffer.read(chunk_size) == data
+            assert buffer.empty()
+        assert written >= maxlen * (wraparound - 1)
+
+    def test_read_write_with_wraparound_long(
+        self,
+        maxlen: int,
+        randomize_start: Callable[[bytes], None],
+        randbytes: Callable[[int], bytes],
+    ) -> None:
+        buffer = RingBuffer(maxlen)
+        randomize_start(buffer)
+
+        size = randint(2, 42) * maxlen
+        step = randint(1, maxlen)
+        written = 0
+        for _ in range(0, size, step):
+            data = randbytes(step)
+            amt = buffer.write(data)
+            written += amt
+            assert amt == step
+            assert amt == len(data)
+            assert written % step == 0
+            assert buffer.read(len(data)) == data
+            assert buffer.empty()
+
+    def test_write_overflow_raises_buffererror(
+        self,
+        maxlen: int,
+        randomize_start: Callable[[bytes], None],
+        randbytes: Callable[[int], bytes],
+    ) -> None:
+        buffer = RingBuffer(maxlen)
+        randomize_start(buffer)
+
+        data = randbytes(maxlen + 1)
+        with pytest.raises(BufferError):
+            buffer.write(data)
+        assert not buffer
```

### Comparing `python-mbedtls-2.7.0/tests/test_secrets.py` & `python-mbedtls-2.7.1/tests/test_secrets.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-# SPDX-License-Identifier: MIT
-
-from __future__ import annotations
-
-import pytest
-
-from mbedtls import secrets
-
-
-def test_token_bytes_default_entropy() -> None:
-    token = secrets.token_bytes()
-    assert len(token) == secrets.DEFAULT_ENTROPY
-    assert isinstance(token, bytes)
-
-
-@pytest.mark.parametrize("nbytes", [0, 32, 256, 500])
-def test_token_bytes(nbytes: int) -> None:
-    token = secrets.token_bytes(nbytes)
-    assert len(token) == nbytes
-    assert isinstance(token, bytes)
-
-
-def test_token_hex() -> None:
-    token = secrets.token_hex()
-    assert len(token) == 2 * secrets.DEFAULT_ENTROPY
-    assert isinstance(token, str)
-
-
-def test_token_urlsafe() -> None:
-    token = secrets.token_urlsafe()
-    assert len(token) == pytest.approx(1.3 * secrets.DEFAULT_ENTROPY, rel=0.1)
-    assert isinstance(token, str)
-
-
-@pytest.mark.repeat(100)
-def test_choice() -> None:
-    seq = tuple(range(100))
-    chosen = secrets.choice(seq)
-    assert chosen in seq
-
-
-def test_choice_from_empty_sequence_raises_indexerror() -> None:
-    with pytest.raises(IndexError):
-        secrets.choice([])
-
-
-def test_randbits() -> None:
-    assert 0 <= secrets.randbits(32) < (1 << 32)
-
-
-@pytest.mark.parametrize("upper_bound", [0, -1])
-def test_randbelow_zero_raises_valueerror(upper_bound: int) -> None:
-    with pytest.raises(ValueError):
-        secrets.randbelow(upper_bound)
-
-
-@pytest.mark.repeat(100)
-@pytest.mark.parametrize("upper_bound", [1, 1 << 32, 1 << 128, 1 << 1024])
-def test_randbelow(upper_bound: int) -> None:
-    assert 0 <= secrets.randbelow(upper_bound) < upper_bound
+# SPDX-License-Identifier: MIT
+
+from __future__ import annotations
+
+import pytest
+
+from mbedtls import secrets
+
+
+def test_token_bytes_default_entropy() -> None:
+    token = secrets.token_bytes()
+    assert len(token) == secrets.DEFAULT_ENTROPY
+    assert isinstance(token, bytes)
+
+
+@pytest.mark.parametrize("nbytes", [0, 32, 256, 500])
+def test_token_bytes(nbytes: int) -> None:
+    token = secrets.token_bytes(nbytes)
+    assert len(token) == nbytes
+    assert isinstance(token, bytes)
+
+
+def test_token_hex() -> None:
+    token = secrets.token_hex()
+    assert len(token) == 2 * secrets.DEFAULT_ENTROPY
+    assert isinstance(token, str)
+
+
+def test_token_urlsafe() -> None:
+    token = secrets.token_urlsafe()
+    assert len(token) == pytest.approx(1.3 * secrets.DEFAULT_ENTROPY, rel=0.1)
+    assert isinstance(token, str)
+
+
+@pytest.mark.repeat(100)
+def test_choice() -> None:
+    seq = tuple(range(100))
+    chosen = secrets.choice(seq)
+    assert chosen in seq
+
+
+def test_choice_from_empty_sequence_raises_indexerror() -> None:
+    with pytest.raises(IndexError):
+        secrets.choice([])
+
+
+def test_randbits() -> None:
+    assert 0 <= secrets.randbits(32) < (1 << 32)
+
+
+@pytest.mark.parametrize("upper_bound", [0, -1])
+def test_randbelow_zero_raises_valueerror(upper_bound: int) -> None:
+    with pytest.raises(ValueError):
+        secrets.randbelow(upper_bound)
+
+
+@pytest.mark.repeat(100)
+@pytest.mark.parametrize("upper_bound", [1, 1 << 32, 1 << 128, 1 << 1024])
+def test_randbelow(upper_bound: int) -> None:
+    assert 0 <= secrets.randbelow(upper_bound) < upper_bound
```

### Comparing `python-mbedtls-2.7.0/tests/test_tls.py` & `python-mbedtls-2.7.1/tests/test_tls.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,1171 +1,1159 @@
-# SPDX-License-Identifier: MIT
-
-# pylint: disable=too-many-lines
-
-from __future__ import annotations
-
-import datetime as dt
-import errno
-import pickle
-import socket
-import subprocess
-import sys
-import time
-from contextlib import suppress
-from pathlib import Path
-from typing import (
-    Any,
-    Callable,
-    Iterator,
-    Mapping,
-    Optional,
-    Sequence,
-    Tuple,
-    Union,
-)
-
-import pytest
-
-from mbedtls import hashlib
-from mbedtls._tls import (
-    _SUPPORTED_DTLS_VERSION,
-    _SUPPORTED_TLS_VERSION,
-    _dtls_from_version,
-    _dtls_to_version,
-)
-from mbedtls._tls import _DTLSCookie as DTLSCookie  # type: ignore
-from mbedtls._tls import _PSKSToreProxy as PSKStoreProxy  # type: ignore
-from mbedtls._tls import _tls_from_version, _tls_to_version
-from mbedtls.pk import ECC, RSA
-from mbedtls.tls import (
-    ClientContext,
-    DTLSConfiguration,
-    DTLSVersion,
-    HandshakeStep,
-    HelloVerifyRequest,
-    MaxFragmentLength,
-    NextProtocol,
-    Purpose,
-    ServerContext,
-    TLSConfiguration,
-    TLSRecordHeader,
-    TLSSession,
-    TLSVersion,
-    TLSWrappedBuffer,
-    TLSWrappedSocket,
-    TrustStore,
-    WantReadError,
-    WantWriteError,
-    ciphers_available,
-)
-from mbedtls.x509 import CRT, CSR, BasicConstraints
-
-_Key = Union[RSA, ECC]
-_HostName = str
-
-
-@pytest.fixture(scope="module")
-def rootpath() -> Path:
-    return Path(__file__).parent.parent
-
-
-def make_root_ca(
-    # pylint: disable=too-many-arguments
-    subject: Optional[str] = None,
-    not_before: Optional[dt.datetime] = None,
-    not_after: Optional[dt.datetime] = None,
-    serial_number: Optional[int] = None,
-    basic_constraints: Optional[BasicConstraints] = None,
-    digestmod: Optional[hashlib.Algorithm] = None,
-) -> Tuple[CRT, _Key]:
-    if subject is None:
-        subject = "OU=test, CN=Trusted CA"
-    if not_before is None:
-        not_before = dt.datetime.utcnow()
-    if not_after is None:
-        not_after = not_before + dt.timedelta(days=90)
-    if serial_number is None:
-        serial_number = 0x123456
-    if basic_constraints is None:
-        basic_constraints = BasicConstraints(True, -1)
-    if digestmod is None:
-        digestmod = hashlib.sha256
-
-    key = RSA()
-    key.generate()
-    crt = CRT.selfsign(
-        csr=CSR.new(key, subject, digestmod()),
-        issuer_key=key,
-        not_before=not_before,
-        not_after=not_after,
-        serial_number=serial_number,
-        basic_constraints=basic_constraints,
-    )
-    return crt, key
-
-
-def make_crt(
-    # pylint: disable=too-many-arguments
-    issuer_crt: CRT,
-    issuer_key: _Key,
-    subject: Optional[str] = None,
-    not_before: Optional[dt.datetime] = None,
-    not_after: Optional[dt.datetime] = None,
-    serial_number: Optional[int] = None,
-    basic_constraints: Optional[BasicConstraints] = None,
-    digestmod: Optional[hashlib.Algorithm] = None,
-) -> Tuple[CRT, _Key]:
-    if subject is None:
-        subject = "OU=test, CN=hostname"
-    if not_before is None:
-        not_before = issuer_crt.not_before
-    if not_after is None:
-        not_after = issuer_crt.not_after
-    if serial_number is None:
-        serial_number = 0x123456
-    if basic_constraints is None:
-        basic_constraints = BasicConstraints()
-    if digestmod is None:
-        # TODO: issuer_crt.digestmod should work but doesn't.
-        digestmod = hashlib.sha256
-
-    key = RSA()
-    key.generate()
-    crt = issuer_crt.sign(
-        csr=CSR.new(key, subject, digestmod()),
-        issuer_key=issuer_key,
-        not_before=not_before,
-        not_after=not_after,
-        serial_number=serial_number,
-        basic_constraints=basic_constraints,
-    )
-    return crt, key
-
-
-class TestPickle:
-    @pytest.mark.parametrize(
-        "obj",
-        [
-            TLSConfiguration(),
-            DTLSConfiguration(),
-            ClientContext(TLSConfiguration()),
-            ClientContext(DTLSConfiguration()),
-            ServerContext(TLSConfiguration()),
-            ServerContext(DTLSConfiguration()),
-        ],
-        ids=type,
-    )
-    def test_picklable(self, obj: object) -> None:
-        assert obj == pickle.loads(pickle.dumps(obj))
-
-    @pytest.mark.parametrize(
-        "obj",
-        [
-            TLSSession(),
-            TLSWrappedBuffer(ClientContext(DTLSConfiguration())),
-            TLSWrappedBuffer(ClientContext(TLSConfiguration())),
-            TLSWrappedBuffer(ServerContext(DTLSConfiguration())),
-            TLSWrappedBuffer(ServerContext(TLSConfiguration())),
-            TLSWrappedSocket(
-                socket.socket(),
-                TLSWrappedBuffer(ClientContext(DTLSConfiguration())),
-            ),
-            TLSWrappedSocket(
-                socket.socket(),
-                TLSWrappedBuffer(ClientContext(TLSConfiguration())),
-            ),
-            TLSWrappedSocket(
-                socket.socket(),
-                TLSWrappedBuffer(ServerContext(DTLSConfiguration())),
-            ),
-            TLSWrappedSocket(
-                socket.socket(),
-                TLSWrappedBuffer(ServerContext(TLSConfiguration())),
-            ),
-        ],
-        ids=type,
-    )
-    def test_unpicklable(self, obj: object) -> None:
-        with pytest.raises(TypeError) as excinfo:
-            pickle.dumps(obj)
-
-        assert str(excinfo.value).startswith("cannot pickle")
-
-
-class TestPSKStoreProxy:
-    @pytest.fixture()
-    def psk_store(self) -> Mapping[str, bytes]:
-        return {"client": b"the secret key"}
-
-    @pytest.fixture()
-    def proxy(self, psk_store: Mapping[str, bytes]) -> PSKStoreProxy:
-        return PSKStoreProxy(psk_store)
-
-    @pytest.mark.parametrize(
-        "repr_",
-        [repr, str],
-        ids=lambda f: f.__name__,  # type: ignore[no-any-return]
-    )
-    def test_repr(
-        self, repr_: Callable[[object], str], psk_store: Mapping[str, bytes]
-    ) -> None:
-        assert isinstance(repr_(psk_store), str)
-
-    def test_unwrap(
-        self, proxy: PSKStoreProxy, psk_store: Mapping[str, bytes]
-    ) -> None:
-        assert proxy.unwrap() == psk_store
-
-    def test_eq(
-        self, proxy: PSKStoreProxy, psk_store: Mapping[str, bytes]
-    ) -> None:
-        for k, v in psk_store.items():
-            assert proxy[k] == v
-
-    def test_len(
-        self, proxy: PSKStoreProxy, psk_store: Mapping[str, bytes]
-    ) -> None:
-        assert len(proxy) == len(psk_store)
-
-
-class TestVersion:
-    @pytest.mark.parametrize("version", _SUPPORTED_TLS_VERSION)
-    def test_tls_enum_to_protocol_version(self, version: TLSVersion) -> None:
-        assert _tls_to_version(_tls_from_version(version)) is version
-
-    @pytest.mark.parametrize("version", _SUPPORTED_DTLS_VERSION)
-    def test_dtls_enum_to_protocol_version(self, version: DTLSVersion) -> None:
-        assert _dtls_to_version(_dtls_from_version(version)) is version
-
-
-class TestTLSRecordHeader:
-    @pytest.fixture(params=TLSRecordHeader.RecordType)
-    def record_type(self, request: Any) -> TLSRecordHeader.RecordType:
-        assert isinstance(request.param, TLSRecordHeader.RecordType)
-        return request.param
-
-    @pytest.fixture(params=_SUPPORTED_TLS_VERSION)
-    def version(self, request: Any) -> TLSVersion:
-        assert isinstance(request.param, TLSVersion)
-        return request.param
-
-    @pytest.fixture()
-    def length(self) -> int:
-        return 42
-
-    @pytest.fixture()
-    def header(
-        self,
-        record_type: TLSRecordHeader.RecordType,
-        version: TLSVersion,
-        length: int,
-    ) -> TLSRecordHeader:
-        return TLSRecordHeader(record_type, version, length)
-
-    @pytest.mark.parametrize(
-        "repr_",
-        [repr, str],
-        ids=lambda f: f.__name__,  # type: ignore[no-any-return]
-    )
-    def test_repr(
-        self,
-        repr_: Callable[[object], str],
-        record_type: TLSRecordHeader.RecordType,
-    ) -> None:
-        assert isinstance(repr_(record_type), str)
-
-    def test_hash(self, record_type: TLSRecordHeader.RecordType) -> None:
-        assert isinstance(hash(record_type), int)
-
-    def test_accessors(
-        self,
-        header: TLSRecordHeader,
-        record_type: TLSRecordHeader.RecordType,
-        version: TLSVersion,
-        length: int,
-    ) -> None:
-        assert len(header) == 5
-        assert header.record_type is record_type
-        assert header.version is version
-        assert header.length == length
-
-    def test_serialization(self, header: TLSRecordHeader) -> None:
-        serialized = bytes(header)
-        assert isinstance(serialized, bytes)
-        assert len(serialized) == 5
-        assert TLSRecordHeader.from_bytes(serialized) == header
-
-
-class TestTLSSession:
-    @pytest.fixture()
-    def session(self) -> TLSSession:
-        return TLSSession()
-
-    def test_repr(self, session: TLSSession) -> None:
-        assert isinstance(repr(session), str)
-
-
-class TestTrustStore:
-    @pytest.fixture()
-    def store(self) -> TrustStore:
-        return TrustStore.system()
-
-    @pytest.mark.parametrize(
-        "repr_",
-        [repr, str],
-        ids=lambda f: f.__name__,  # type: ignore[no-any-return]
-    )
-    def test_repr(
-        self, repr_: Callable[[object], str], store: TrustStore
-    ) -> None:
-        assert isinstance(repr_(store), str)
-
-    def test_eq(self, store: TrustStore) -> None:
-        other = TrustStore(store)
-        assert store is not other
-        assert store == other
-
-    def test_bool(self, store: TrustStore) -> None:
-        assert not TrustStore()
-        assert store
-
-    def test_len(self, store: TrustStore) -> None:
-        assert len(store) != 0
-
-    def test_iter(self, store: TrustStore) -> None:
-        assert store[0] != store[1]
-        n = 0
-        for n, crt in enumerate(store, start=1):
-            assert crt in store
-        assert n == len(store)
-
-    def test_add_existing_certificate(self, store: TrustStore) -> None:
-        length = len(store)
-        store.add(store[0])
-        assert len(store) == length
-
-    def test_add_new_certificate(self, store: TrustStore) -> None:
-        root_ca = make_root_ca()[0]
-        length = len(store)
-        store.add(root_ca)
-        assert len(store) == length + 1
-
-
-class TestDTLSCookie:
-    @pytest.fixture()
-    def cookie(self) -> DTLSCookie:
-        return DTLSCookie()
-
-    def test_generate_does_not_raise(self, cookie: DTLSCookie) -> None:
-        cookie.generate()
-
-    def test_timeout(self, cookie: DTLSCookie) -> None:
-        assert cookie.timeout == 60
-        cookie.timeout = 1000
-        assert cookie.timeout == 1000
-
-
-def assert_conf_invariant(
-    conf: Union[TLSConfiguration, DTLSConfiguration],
-    **elem: Any,
-) -> None:
-    # For the context, the configuration is converted into an
-    # internal MbedTLSConfiguration and the accessors then
-    # converts the MbedTLSConfiguration back into a
-    # TLSConfiguration (or DTLSConfiguration).  These conversions
-    # are what we actually check here.
-    __tracebackhide__ = True  # pylint: disable=unused-variable
-    assert len(elem) == 1
-
-    key, value = next(iter(elem.items()))
-    assert (
-        getattr(ServerContext(conf.update(**elem)).configuration, key) == value
-    )
-
-
-class TestConfiguration:
-    @pytest.fixture(params=[DTLSConfiguration, TLSConfiguration])
-    def conf(self, request: Any) -> Union[TLSConfiguration, DTLSConfiguration]:
-        conf = request.param()
-        assert isinstance(conf, (TLSConfiguration, DTLSConfiguration))
-        return conf
-
-    @pytest.mark.parametrize("validate", [True, False])
-    def test_set_validate_certificates(
-        self, conf: Union[TLSConfiguration, DTLSConfiguration], validate: bool
-    ) -> None:
-        assert_conf_invariant(conf, validate_certificates=validate)
-
-    def test_set_empty_certificate_chain(
-        self, conf: Union[TLSConfiguration, DTLSConfiguration]
-    ) -> None:
-        assert_conf_invariant(conf, certificate_chain=None)
-
-    def test_set_certificate_chain(
-        self, conf: Union[TLSConfiguration, DTLSConfiguration]
-    ) -> None:
-        root_crt, root_key = make_root_ca()
-        ee_crt, ee_key = make_crt(root_crt, root_key)
-        chain = (ee_crt, root_crt), ee_key
-        assert_conf_invariant(conf, certificate_chain=chain)
-
-    def test_set_ciphers(
-        self, conf: Union[TLSConfiguration, DTLSConfiguration]
-    ) -> None:
-        assert_conf_invariant(conf, ciphers=tuple(ciphers_available()))
-
-    @pytest.mark.parametrize(
-        "inner_protocols",
-        [
-            (),
-            (NextProtocol.H2, NextProtocol.H2C),
-            (NextProtocol.H2, NextProtocol.H2C, NextProtocol.FTP),
-        ],
-    )
-    def test_set_inner_protocols(
-        self,
-        conf: Union[TLSConfiguration, DTLSConfiguration],
-        inner_protocols: Tuple[Union[NextProtocol, bytes]],
-    ) -> None:
-        assert_conf_invariant(
-            conf,
-            inner_protocols=inner_protocols,
-        )
-
-    @pytest.mark.parametrize("trust_store", [TrustStore.system()])
-    def test_trust_store(
-        self,
-        conf: Union[TLSConfiguration, DTLSConfiguration],
-        trust_store: TrustStore,
-    ) -> None:
-        assert trust_store
-        assert_conf_invariant(conf, trust_store=trust_store)
-
-    @pytest.mark.parametrize("mfl", MaxFragmentLength)
-    def test_max_fragmentation_length(
-        self,
-        conf: Union[TLSConfiguration, DTLSConfiguration],
-        mfl: MaxFragmentLength,
-    ) -> None:
-        assert_conf_invariant(conf, max_fragmentation_length=mfl)
-
-    def test_set_sni_callback(
-        self,
-        conf: Union[TLSConfiguration, DTLSConfiguration],
-    ) -> None:
-        assert conf.sni_callback is None
-
-    @pytest.mark.parametrize("psk", [None, ("client", b"the secret key")])
-    def test_psk(
-        self,
-        conf: Union[TLSConfiguration, DTLSConfiguration],
-        psk: Tuple[str, bytes],
-    ) -> None:
-        assert conf.pre_shared_key is None
-        assert_conf_invariant(conf, pre_shared_key=psk)
-
-    @pytest.mark.parametrize("psk_store", [{}, {"client": b"the secret key"}])
-    def test_psk_store(
-        self,
-        conf: Union[TLSConfiguration, DTLSConfiguration],
-        psk_store: Mapping[str, bytes],
-    ) -> None:
-        assert not conf.pre_shared_key_store
-        assert_conf_invariant(conf, pre_shared_key_store=psk_store)
-
-
-class TestTLSConfiguration:
-    @pytest.fixture()
-    def conf(self) -> TLSConfiguration:
-        return TLSConfiguration()
-
-    def test_default_supported_versions(self, conf: TLSConfiguration) -> None:
-        assert conf.lowest_supported_version is TLSVersion.TLSv1
-        assert conf.highest_supported_version is TLSVersion.MAXIMUM_SUPPORTED
-
-    @pytest.mark.parametrize("version", _SUPPORTED_TLS_VERSION)
-    def test_lowest_supported_version(
-        self, conf: TLSConfiguration, version: TLSVersion
-    ) -> None:
-        assert_conf_invariant(conf, lowest_supported_version=version)
-
-    @pytest.mark.parametrize("version", _SUPPORTED_TLS_VERSION)
-    def test_highest_supported_version(
-        self, conf: TLSConfiguration, version: TLSVersion
-    ) -> None:
-        assert_conf_invariant(conf, highest_supported_version=version)
-
-
-class TestDTLSConfiguration:
-    @pytest.fixture()
-    def conf(self) -> DTLSConfiguration:
-        return DTLSConfiguration()
-
-    def test_default_supported_versions(self, conf: DTLSConfiguration) -> None:
-        assert conf.lowest_supported_version is DTLSVersion.DTLSv1_0
-        assert conf.highest_supported_version is DTLSVersion.MAXIMUM_SUPPORTED
-
-    @pytest.mark.parametrize("version", _SUPPORTED_DTLS_VERSION)
-    def test_lowest_supported_version(
-        self, conf: DTLSConfiguration, version: DTLSVersion
-    ) -> None:
-        assert_conf_invariant(conf, lowest_supported_version=version)
-
-    @pytest.mark.parametrize("version", _SUPPORTED_DTLS_VERSION)
-    def test_highest_supported_version(
-        self, conf: DTLSConfiguration, version: DTLSVersion
-    ) -> None:
-        assert_conf_invariant(conf, highest_supported_version=version)
-
-    @pytest.mark.parametrize("anti_replay", [True, False])
-    def test_set_anti_replay(
-        self, conf: DTLSConfiguration, anti_replay: bool
-    ) -> None:
-        assert conf.anti_replay is True
-        assert_conf_invariant(conf, anti_replay=anti_replay)
-
-    @pytest.mark.parametrize(
-        "hs_min_max", [(1, 60), (42, 69), (4.2, 6.9), (42.0, 69.0)]
-    )
-    def test_handshake_timeout_minmax(
-        self,
-        conf: DTLSConfiguration,
-        hs_min_max: Tuple[float, float],
-    ) -> None:
-        hs_min, hs_max = hs_min_max
-        assert conf.handshake_timeout_min == 1.0
-        assert conf.handshake_timeout_max == 60.0
-        conf_ = conf.update(
-            handshake_timeout_min=hs_min,
-            handshake_timeout_max=hs_max,
-        )
-        assert conf_.handshake_timeout_min == hs_min
-        assert conf_.handshake_timeout_max == hs_max
-
-        assert_conf_invariant(conf, handshake_timeout_min=hs_min)
-        assert_conf_invariant(conf, handshake_timeout_max=hs_max)
-
-    @pytest.mark.parametrize("hs_min_max", [(1, 60), (42, 69), (4.2, 6.9)])
-    def test_handshake_timeout_default(
-        self,
-        conf: DTLSConfiguration,
-        hs_min_max: Tuple[float, float],
-    ) -> None:
-        assert conf.handshake_timeout_min == 1.0
-        assert conf.handshake_timeout_max == 60.0
-
-        hs_min, hs_max = hs_min_max
-        conf_ = conf.update(
-            handshake_timeout_min=hs_min,
-            handshake_timeout_max=hs_max,
-        )
-        assert conf_.handshake_timeout_min == hs_min
-        assert conf_.handshake_timeout_max == hs_max
-
-        assert_conf_invariant(conf, handshake_timeout_min=hs_min)
-        assert_conf_invariant(conf, handshake_timeout_max=hs_max)
-
-
-class TestContext:
-    @pytest.fixture(params=[Purpose.SERVER_AUTH, Purpose.CLIENT_AUTH])
-    def purpose(self, request: Any) -> Purpose:
-        assert isinstance(request.param, Purpose)
-        return request.param
-
-    @pytest.fixture(params=[TLSConfiguration, DTLSConfiguration])
-    def conf(self, request: Any) -> Union[TLSConfiguration, DTLSConfiguration]:
-        conf = request.param()
-        assert isinstance(conf, (TLSConfiguration, DTLSConfiguration))
-        return conf
-
-    @pytest.fixture(params=[ServerContext, ClientContext])
-    def context(
-        self, conf: Union[TLSConfiguration, DTLSConfiguration], request: Any
-    ) -> Union[ServerContext, ClientContext]:
-        ctx = request.param(conf)
-        assert isinstance(ctx, (ServerContext, ClientContext))
-        return ctx
-
-    def test_repr(self, context: Union[ServerContext, ClientContext]) -> None:
-        assert isinstance(repr(context), str)
-
-    def test_get_configuration(
-        self,
-        context: Union[ServerContext, ClientContext],
-        conf: Union[TLSConfiguration, DTLSConfiguration],
-    ) -> None:
-        assert context.configuration == conf
-
-
-CLIENT_HELLO = (HandshakeStep.CLIENT_HELLO,)
-SERVER_HELLO = (
-    HandshakeStep.SERVER_HELLO,
-    HandshakeStep.SERVER_CERTIFICATE,
-    HandshakeStep.SERVER_KEY_EXCHANGE,
-    HandshakeStep.CERTIFICATE_REQUEST,
-    HandshakeStep.SERVER_HELLO_DONE,
-)
-CLIENT_KEY_EXCHANGE = (
-    HandshakeStep.CLIENT_CERTIFICATE,
-    HandshakeStep.CLIENT_KEY_EXCHANGE,
-    HandshakeStep.CERTIFICATE_VERIFY,
-    HandshakeStep.CLIENT_CHANGE_CIPHER_SPEC,
-    HandshakeStep.CLIENT_FINISHED,
-)
-SERVER_CHANGE_CIPHER_SPEC = (
-    HandshakeStep.SERVER_CHANGE_CIPHER_SPEC,
-    HandshakeStep.SERVER_FINISHED,
-)
-HANDSHAKE_OVER = (
-    HandshakeStep.FLUSH_BUFFERS,
-    HandshakeStep.HANDSHAKE_WRAPUP,
-    HandshakeStep.HANDSHAKE_OVER,
-)
-
-
-def do_io(
-    *, src: TLSWrappedBuffer, dst: TLSWrappedBuffer, amt: int = 1024
-) -> None:
-    # pylint: disable=protected-access
-    __tracebackhide__ = True  # pylint: disable=unused-variable
-    assert src._output_buffer, "nothing to do"
-    while src._output_buffer:
-        in_transit = src.peek_outgoing(amt)
-        src.consume_outgoing(len(in_transit))
-        dst.receive_from_network(in_transit)
-
-
-def do_send(
-    data: bytes, *, src: TLSWrappedBuffer, dst: TLSWrappedBuffer
-) -> bytes:
-    amt = src.write(data)
-    do_io(src=src, dst=dst)
-    return dst.read(amt)
-
-
-def do_handshake(
-    end: TLSWrappedBuffer, states: Sequence[HandshakeStep]
-) -> None:
-    # pylint: disable=protected-access
-    __tracebackhide__ = True  # pylint: disable=unused-variable
-    while end._handshake_state is not states[0]:
-        # The backend goes through every state for both
-        # ends.  This is not relevant.
-        try:
-            end.do_handshake()
-        except (WantReadError, WantWriteError) as exc:
-            raise AssertionError(
-                f"{type(end.context).__name__} wants {end._handshake_state}"
-            ) from exc
-
-    for state in states:
-        assert end._handshake_state is state
-        if state is HandshakeStep.HANDSHAKE_OVER:
-            break
-        with suppress(WantWriteError):
-            end.do_handshake()
-
-
-def make_full_handshake(
-    *, client: TLSWrappedBuffer, server: TLSWrappedBuffer
-) -> None:
-    do_handshake(client, CLIENT_HELLO)
-    do_io(src=client, dst=server)
-
-    do_handshake(server, SERVER_HELLO)
-    do_io(src=server, dst=client)
-    assert client.negotiated_protocol() == server.negotiated_protocol()
-
-    do_handshake(client, CLIENT_KEY_EXCHANGE)
-    do_io(src=client, dst=server)
-    assert client.negotiated_tls_version() == server.negotiated_tls_version()
-
-    do_handshake(server, SERVER_CHANGE_CIPHER_SPEC)
-    do_io(src=server, dst=client)
-
-    do_handshake(server, HANDSHAKE_OVER)
-    do_handshake(client, HANDSHAKE_OVER)
-    assert client.cipher() == server.cipher()
-
-
-def make_hello_verify_request(
-    *, client: TLSWrappedBuffer, server: TLSWrappedBuffer, cookie: bytes
-) -> None:
-    do_handshake(client, CLIENT_HELLO)
-    do_io(src=client, dst=server)
-    server.setcookieparam(cookie)
-    with pytest.raises(HelloVerifyRequest):
-        do_handshake(
-            server,
-            (
-                HandshakeStep.SERVER_HELLO,
-                HandshakeStep.SERVER_HELLO_VERIFY_REQUEST_SENT,
-            ),
-        )
-
-    do_handshake(server, (HandshakeStep.HELLO_REQUEST,))
-    server.setcookieparam(cookie)
-    do_io(src=server, dst=client)
-
-
-def do_communicate(args: Any) -> str:
-    while True:
-        with subprocess.Popen(
-            args,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-            text=True,
-            encoding="utf8",
-        ) as proc:
-            out, err = proc.communicate()
-            if "ConnectionRefusedError" in err:
-                time.sleep(0.01)  # Avoid tight CPU loop.
-                continue
-            return out
-
-
-class TestTLSHandshake:
-    @pytest.fixture(scope="class")
-    def hostname(self) -> _HostName:
-        return "www.example.com"
-
-    @pytest.fixture(scope="class")
-    def certificate_chain(
-        self, hostname: _HostName
-    ) -> Tuple[Tuple[CRT, ...], _Key]:
-        root_crt, root_key = make_root_ca()
-        ee_crt, ee_key = make_crt(
-            root_crt, root_key, subject=f"OU=test, CN={hostname}"
-        )
-        return (ee_crt, root_crt), ee_key
-
-    def test_cert_without_validation(
-        self, certificate_chain: Tuple[Tuple[CRT, ...], _Key]
-    ) -> None:
-        server = ServerContext(
-            TLSConfiguration(
-                certificate_chain=certificate_chain,
-                validate_certificates=False,
-            )
-        ).wrap_buffers()
-        client = ClientContext(
-            TLSConfiguration(validate_certificates=False)
-        ).wrap_buffers("hostname")
-        make_full_handshake(client=client, server=server)
-
-        secret = b"a very secret message"
-        assert do_send(secret, src=client, dst=server) == secret
-        assert do_send(secret, src=server, dst=client) == secret
-
-    def test_cert_with_validation(
-        self,
-        hostname: _HostName,
-        certificate_chain: Tuple[Tuple[CRT, ...], _Key],
-    ) -> None:
-        trust_store = TrustStore()
-        crt: CRT
-        for crt in certificate_chain[0][1:]:
-            trust_store.add(crt)
-        server = ServerContext(
-            TLSConfiguration(
-                certificate_chain=certificate_chain,
-                validate_certificates=False,
-            )
-        ).wrap_buffers()
-        # Host name must now be the common name (CN) of the leaf certificate.
-        client = ClientContext(
-            TLSConfiguration(trust_store=trust_store)
-        ).wrap_buffers(hostname)
-        make_full_handshake(client=client, server=server)
-
-        secret = b"a very secret message"
-        assert do_send(secret, src=client, dst=server) == secret
-        assert do_send(secret, src=server, dst=client) == secret
-
-    def test_psk(self) -> None:
-        psk = ("cli", b"secret")
-        server = ServerContext(
-            TLSConfiguration(
-                pre_shared_key_store=dict((psk,)),
-                validate_certificates=False,
-            )
-        ).wrap_buffers()
-        client = ClientContext(
-            TLSConfiguration(
-                pre_shared_key=psk,
-                validate_certificates=False,
-            ),
-        ).wrap_buffers("hostname")
-        make_full_handshake(client=client, server=server)
-
-        secret = b"a very secret message"
-        assert do_send(secret, src=client, dst=server) == secret
-        assert do_send(secret, src=server, dst=client) == secret
-
-
-class TestDTLSHandshake:
-    def test_psk(self) -> None:
-        psk = ("cli", b"secret")
-        server = ServerContext(
-            DTLSConfiguration(
-                pre_shared_key_store=dict((psk,)),
-                validate_certificates=False,
-            )
-        ).wrap_buffers()
-        client = ClientContext(
-            DTLSConfiguration(
-                pre_shared_key=psk,
-                validate_certificates=False,
-            ),
-        ).wrap_buffers("hostname")
-        make_hello_verify_request(
-            client=client, server=server, cookie="🍪🍪🍪".encode()
-        )
-        make_full_handshake(client=client, server=server)
-
-        secret = b"a very secret message"
-        assert do_send(secret, src=client, dst=server) == secret
-        assert do_send(secret, src=server, dst=client) == secret
-
-    @pytest.mark.parametrize("mtu_cli", [0, 128, 380, 500, (1 << 16) - 1])
-    @pytest.mark.parametrize("mtu_srv", [0, 128, 380, 500, (1 << 16) - 1])
-    def test_psk_set_mtu(self, mtu_cli: int, mtu_srv: int) -> None:
-        psk = ("cli", b"secret")
-        server = ServerContext(
-            DTLSConfiguration(
-                pre_shared_key_store=dict((psk,)),
-                validate_certificates=False,
-            )
-        ).wrap_buffers()
-        server.setmtu(mtu_srv)
-        client = ClientContext(
-            DTLSConfiguration(
-                pre_shared_key=psk,
-                validate_certificates=False,
-            ),
-        ).wrap_buffers("hostname")
-        client.setmtu(mtu_cli)
-        make_hello_verify_request(
-            client=client, server=server, cookie="🍪🍪🍪".encode()
-        )
-        make_full_handshake(client=client, server=server)
-
-        secret = b"a very secret message"
-        assert do_send(secret, src=client, dst=server) == secret
-        assert do_send(secret, src=server, dst=client) == secret
-
-    def test_resume_from_pickle(self) -> None:
-        psk = ("cli", b"secret")
-        server = ServerContext(
-            DTLSConfiguration(
-                pre_shared_key_store=dict((psk,)),
-                validate_certificates=False,
-            )
-        ).wrap_buffers()
-        client = ClientContext(
-            DTLSConfiguration(
-                pre_shared_key=psk,
-                ciphers=("TLS-ECDHE-PSK-WITH-CHACHA20-POLY1305-SHA256",),
-                lowest_supported_version=DTLSVersion.DTLSv1_2,
-                validate_certificates=False,
-            ),
-        ).wrap_buffers("hostname")
-        make_hello_verify_request(
-            client=client, server=server, cookie="🍪🍪🍪".encode()
-        )
-        make_full_handshake(client=client, server=server)
-
-        secret = b"a very secret message"
-        do_send(secret, src=client, dst=server)
-        do_send(secret, src=server, dst=client)
-
-        client = pickle.loads(pickle.dumps(client))
-        do_send(secret, src=client, dst=server)
-        do_send(secret, src=server, dst=client)
-
-
-class TestWrappedSocket_SmokeTests:
-    @pytest.mark.parametrize("conf", [TLSConfiguration(), DTLSConfiguration()])
-    def test_wrap_unwrap_client(
-        self, conf: Union[TLSConfiguration, DTLSConfiguration]
-    ) -> None:
-        with ClientContext(conf).wrap_socket(socket.socket(), None):
-            pass
-
-    @pytest.mark.parametrize("conf", [TLSConfiguration(), DTLSConfiguration()])
-    def test_wrap_unwrap_server(
-        self, conf: Union[TLSConfiguration, DTLSConfiguration]
-    ) -> None:
-        with ServerContext(conf).wrap_socket(socket.socket()):
-            pass
-
-
-@pytest.mark.e2e()
-@pytest.mark.skipif(sys.platform == "win32", reason="Flaky under Windows")
-class TestProgramsTLS:
-    @pytest.fixture(scope="class")
-    def port(self) -> int:
-        """Return a free port
-
-        Note:
-            Not 100% race condition free.
-
-        """
-        port = 0
-        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
-            sock.bind(("localhost", port))
-            port = sock.getsockname()[1]
-        return port
-
-    @pytest.fixture(scope="class")
-    def server(
-        self, rootpath: Path, port: int
-    ) -> Iterator[subprocess.Popen[str]]:
-        args = [
-            sys.executable,
-            str(rootpath / "programs" / "server.py"),
-            "--port",
-            f"{port}",
-            "--tls",
-            "--psk-store",
-            "cli=secret",
-        ]
-        with subprocess.Popen(args, text=True, encoding="utf8") as proc:
-            yield proc
-            proc.kill()
-            proc.wait(1.0)
-
-    @pytest.mark.repeat(3)
-    @pytest.mark.usefixtures("server")
-    @pytest.mark.timeout(30)
-    def test_client(self, rootpath: Path, port: int) -> None:
-        secret = "a very secret message"
-        args = [
-            sys.executable,
-            str(rootpath / "programs" / "client.py"),
-            "--port",
-            f"{port}",
-            "--tls",
-            "--psk",
-            "cli=secret",
-            secret,
-        ]
-        for _ in range(3):
-            assert do_communicate(args) == secret + "\n"
-
-    @pytest.mark.usefixtures("server")
-    @pytest.mark.timeout(30)
-    def test_raw_socket_send_recv(self, port: int) -> None:
-        secret = b"a very secret message"
-        with ClientContext(
-            TLSConfiguration(
-                pre_shared_key=("cli", b"secret"),
-                validate_certificates=False,
-            ),
-        ).wrap_socket(
-            socket.socket(socket.AF_INET, socket.SOCK_STREAM), "localhost"
-        ) as client:
-            client.connect(("127.0.0.1", port))
-            client.do_handshake()
-            sent = client.send(secret)
-            assert sent == len(secret)
-
-            data = client.recv(1024)
-        assert data == secret
-
-    @pytest.mark.usefixtures("server")
-    @pytest.mark.timeout(30)
-    def test_raw_socket_send_recv_into(self, port: int) -> None:
-        secret = b"a very secret message"
-        buffer = bytearray(b"\0" * 256)
-        with ClientContext(
-            TLSConfiguration(
-                pre_shared_key=("cli", b"secret"),
-                validate_certificates=False,
-            ),
-        ).wrap_socket(
-            socket.socket(socket.AF_INET, socket.SOCK_STREAM), "localhost"
-        ) as client:
-            client.connect(("127.0.0.1", port))
-            client.do_handshake()
-            sent = client.send(secret)
-            assert sent == len(secret)
-
-            received = client.recv_into(buffer, 1024)
-        assert buffer[:received] == secret
-
-    @pytest.mark.usefixtures("server")
-    @pytest.mark.timeout(30)
-    def test_raw_socket_sendall_recv(self, port: int) -> None:
-        secret = b"a very secret message"
-        with ClientContext(
-            TLSConfiguration(
-                pre_shared_key=("cli", b"secret"),
-                validate_certificates=False,
-            ),
-        ).wrap_socket(
-            socket.socket(socket.AF_INET, socket.SOCK_STREAM), "localhost"
-        ) as client:
-            client.connect(("127.0.0.1", port))
-            client.do_handshake()
-            client.sendall(secret)
-            data = client.recv(1024)
-        assert data == secret
-
-    @pytest.mark.usefixtures("server")
-    @pytest.mark.timeout(30)
-    def test_raw_socket_connectionless_unavailable(self, port: int) -> None:
-        address = ("127.0.0.1", port)
-        with ClientContext(
-            TLSConfiguration(
-                pre_shared_key=("cli", b"secret"),
-                validate_certificates=False,
-            ),
-        ).wrap_socket(
-            socket.socket(socket.AF_INET, socket.SOCK_STREAM), "localhost"
-        ) as client:
-            with pytest.raises(OSError) as excinfo:
-                client.do_handshake(address)
-
-        assert excinfo.value.errno is errno.ENOTCONN
-
-
-@pytest.mark.e2e()
-@pytest.mark.skipif(sys.platform == "win32", reason="Flaky under Windows")
-class TestProgramsDTLS:
-    @pytest.fixture(scope="class")
-    def port(self) -> int:
-        """Return a free port
-
-        Note:
-            Not 100% race condition free.
-
-        """
-        port = 0
-        with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as sock:
-            sock.bind(("localhost", port))
-            port = sock.getsockname()[1]
-        return port
-
-    @pytest.fixture(scope="class")
-    def server(
-        self, rootpath: Path, port: int
-    ) -> Iterator[subprocess.Popen[str]]:
-        args = [
-            sys.executable,
-            str(rootpath / "programs" / "server.py"),
-            "--port",
-            f"{port}",
-            "--dtls",
-            "--psk-store",
-            "cli=secret",
-        ]
-        with subprocess.Popen(args, text=True, encoding="utf8") as proc:
-            yield proc
-            proc.kill()
-            proc.wait(1.0)
-
-    @pytest.mark.repeat(3)
-    @pytest.mark.usefixtures("server")
-    @pytest.mark.timeout(30)
-    def test_client(self, rootpath: Path, port: int) -> None:
-        secret = "a very secret message"
-        args = [
-            sys.executable,
-            str(rootpath / "programs" / "client.py"),
-            "--port",
-            f"{port}",
-            "--dtls",
-            "--psk",
-            "cli=secret",
-            secret,
-        ]
-        for _ in range(3):
-            assert do_communicate(args) == secret + "\n"
-
-    @pytest.mark.usefixtures("server")
-    @pytest.mark.timeout(30)
-    def test_raw_socket_send_recv(self, port: int) -> None:
-        address = ("127.0.0.1", port)
-        secret = b"a very secret message"
-        with ClientContext(
-            DTLSConfiguration(
-                pre_shared_key=("cli", b"secret"),
-                validate_certificates=False,
-            ),
-        ).wrap_socket(
-            socket.socket(socket.AF_INET, socket.SOCK_DGRAM), "localhost"
-        ) as client:
-            client.connect(address)
-            client.do_handshake()
-            sent = client.send(secret)
-            assert sent == len(secret)
-
-            data = client.recv(1024)
-        assert data == secret
-
-    @pytest.mark.usefixtures("server")
-    @pytest.mark.timeout(30)
-    def test_raw_socket_sendto_recvfrom(self, port: int) -> None:
-        address = ("127.0.0.1", port)
-        secret = b"a very secret message"
-        with ClientContext(
-            DTLSConfiguration(
-                pre_shared_key=("cli", b"secret"),
-                validate_certificates=False,
-            ),
-        ).wrap_socket(
-            socket.socket(socket.AF_INET, socket.SOCK_DGRAM), "localhost"
-        ) as client:
-            client.do_handshake(address)
-            sent = client.sendto(secret, address)
-            assert sent == len(secret)
-
-            data, addr = client.recvfrom(1024)
-            assert addr == address
-        assert data == secret
-
-    @pytest.mark.usefixtures("server")
-    @pytest.mark.timeout(30)
-    def test_raw_socket_sendto_recvfrom_with_flags(self, port: int) -> None:
-        # Note that flags is always 0 (noop) here because we are only
-        # interested in testing the API.  See also issue #62.
-        address = ("127.0.0.1", port)
-        secret = b"a very secret message"
-        with ClientContext(
-            DTLSConfiguration(
-                pre_shared_key=("cli", b"secret"),
-                validate_certificates=False,
-            ),
-        ).wrap_socket(
-            socket.socket(socket.AF_INET, socket.SOCK_DGRAM), "localhost"
-        ) as client:
-            client.do_handshake(0, address)
-            sent = client.sendto(secret, 0, address)
-            assert sent == len(secret)
-
-            data, addr = client.recvfrom(1024, 0)
-            assert addr == address
-        assert data == secret
-
-    @pytest.mark.usefixtures("server")
-    @pytest.mark.timeout(30)
-    def test_raw_socket_sendto_recvfrom_into(self, port: int) -> None:
-        address = ("127.0.0.1", port)
-        secret = b"a very secret message"
-        buffer = bytearray(b"\0" * 256)
-        with ClientContext(
-            DTLSConfiguration(
-                pre_shared_key=("cli", b"secret"),
-                validate_certificates=False,
-            ),
-        ).wrap_socket(
-            socket.socket(socket.AF_INET, socket.SOCK_DGRAM), "localhost"
-        ) as client:
-            client.do_handshake(address)
-            sent = client.sendto(secret, address)
-            assert sent == len(secret)
-
-            received, addr = client.recvfrom_into(buffer, 1024)
-            assert addr == address
-        assert buffer[:received] == secret
+# SPDX-License-Identifier: MIT
+
+# pylint: disable=too-many-lines
+
+from __future__ import annotations
+
+import datetime as dt
+import errno
+import pickle
+import socket
+import subprocess
+import sys
+import time
+from contextlib import suppress
+from pathlib import Path
+from typing import (
+    Any,
+    Callable,
+    Iterator,
+    Mapping,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
+
+import pytest
+
+from mbedtls import hashlib
+from mbedtls._tls import (
+    _SUPPORTED_DTLS_VERSION,
+    _SUPPORTED_TLS_VERSION,
+    _dtls_from_version,
+    _dtls_to_version,
+)
+from mbedtls._tls import _DTLSCookie as DTLSCookie  # type: ignore
+from mbedtls._tls import _PSKSToreProxy as PSKStoreProxy  # type: ignore
+from mbedtls._tls import _tls_from_version, _tls_to_version
+from mbedtls.pk import ECC, RSA
+from mbedtls.tls import (
+    ClientContext,
+    DTLSConfiguration,
+    DTLSVersion,
+    HandshakeStep,
+    HelloVerifyRequest,
+    MaxFragmentLength,
+    NextProtocol,
+    Purpose,
+    ServerContext,
+    TLSConfiguration,
+    TLSRecordHeader,
+    TLSSession,
+    TLSVersion,
+    TLSWrappedBuffer,
+    TLSWrappedSocket,
+    TrustStore,
+    WantReadError,
+    WantWriteError,
+    ciphers_available,
+)
+from mbedtls.x509 import CRT, CSR, BasicConstraints
+
+_Key = Union[RSA, ECC]
+_HostName = str
+
+
+@pytest.fixture(scope="module")
+def rootpath() -> Path:
+    return Path(__file__).parent.parent
+
+
+def make_root_ca(
+    # pylint: disable=too-many-arguments
+    subject: Optional[str] = None,
+    not_before: Optional[dt.datetime] = None,
+    not_after: Optional[dt.datetime] = None,
+    serial_number: Optional[int] = None,
+    basic_constraints: Optional[BasicConstraints] = None,
+    digestmod: Optional[hashlib.Algorithm] = None,
+) -> Tuple[CRT, _Key]:
+    if subject is None:
+        subject = "OU=test, CN=Trusted CA"
+    if not_before is None:
+        not_before = dt.datetime.utcnow()
+    if not_after is None:
+        not_after = not_before + dt.timedelta(days=90)
+    if serial_number is None:
+        serial_number = 0x123456
+    if basic_constraints is None:
+        basic_constraints = BasicConstraints(True, -1)
+    if digestmod is None:
+        digestmod = hashlib.sha256
+
+    key = RSA()
+    key.generate()
+    crt = CRT.selfsign(
+        csr=CSR.new(key, subject, digestmod()),
+        issuer_key=key,
+        not_before=not_before,
+        not_after=not_after,
+        serial_number=serial_number,
+        basic_constraints=basic_constraints,
+    )
+    return crt, key
+
+
+def make_crt(
+    # pylint: disable=too-many-arguments
+    issuer_crt: CRT,
+    issuer_key: _Key,
+    subject: Optional[str] = None,
+    not_before: Optional[dt.datetime] = None,
+    not_after: Optional[dt.datetime] = None,
+    serial_number: Optional[int] = None,
+    basic_constraints: Optional[BasicConstraints] = None,
+    digestmod: Optional[hashlib.Algorithm] = None,
+) -> Tuple[CRT, _Key]:
+    if subject is None:
+        subject = "OU=test, CN=hostname"
+    if not_before is None:
+        not_before = issuer_crt.not_before
+    if not_after is None:
+        not_after = issuer_crt.not_after
+    if serial_number is None:
+        serial_number = 0x123456
+    if basic_constraints is None:
+        basic_constraints = BasicConstraints()
+    if digestmod is None:
+        # TODO: issuer_crt.digestmod should work but doesn't.
+        digestmod = hashlib.sha256
+
+    key = RSA()
+    key.generate()
+    crt = issuer_crt.sign(
+        csr=CSR.new(key, subject, digestmod()),
+        issuer_key=issuer_key,
+        not_before=not_before,
+        not_after=not_after,
+        serial_number=serial_number,
+        basic_constraints=basic_constraints,
+    )
+    return crt, key
+
+
+class TestPickle:
+    @pytest.mark.parametrize(
+        "obj",
+        [
+            TLSConfiguration(),
+            DTLSConfiguration(),
+            ClientContext(TLSConfiguration()),
+            ClientContext(DTLSConfiguration()),
+            ServerContext(TLSConfiguration()),
+            ServerContext(DTLSConfiguration()),
+        ],
+        ids=type,
+    )
+    def test_picklable(self, obj: object) -> None:
+        assert obj == pickle.loads(pickle.dumps(obj))
+
+    @pytest.mark.parametrize(
+        "obj",
+        [
+            TLSSession(),
+            TLSWrappedBuffer(ClientContext(DTLSConfiguration())),
+            TLSWrappedBuffer(ClientContext(TLSConfiguration())),
+            TLSWrappedBuffer(ServerContext(DTLSConfiguration())),
+            TLSWrappedBuffer(ServerContext(TLSConfiguration())),
+            TLSWrappedSocket(
+                socket.socket(),
+                TLSWrappedBuffer(ClientContext(DTLSConfiguration())),
+            ),
+            TLSWrappedSocket(
+                socket.socket(),
+                TLSWrappedBuffer(ClientContext(TLSConfiguration())),
+            ),
+            TLSWrappedSocket(
+                socket.socket(),
+                TLSWrappedBuffer(ServerContext(DTLSConfiguration())),
+            ),
+            TLSWrappedSocket(
+                socket.socket(),
+                TLSWrappedBuffer(ServerContext(TLSConfiguration())),
+            ),
+        ],
+        ids=type,
+    )
+    def test_unpicklable(self, obj: object) -> None:
+        with pytest.raises(TypeError) as excinfo:
+            pickle.dumps(obj)
+
+        assert str(excinfo.value).startswith("cannot pickle")
+
+
+class TestPSKStoreProxy:
+    @pytest.fixture()
+    def psk_store(self) -> Mapping[str, bytes]:
+        return {"client": b"the secret key"}
+
+    @pytest.fixture()
+    def proxy(self, psk_store: Mapping[str, bytes]) -> PSKStoreProxy:
+        return PSKStoreProxy(psk_store)
+
+    @pytest.mark.parametrize("repr_", [repr, str], ids=lambda f: f.__name__)
+    def test_repr(
+        self, repr_: Callable[[object], str], psk_store: Mapping[str, bytes]
+    ) -> None:
+        assert isinstance(repr_(psk_store), str)
+
+    def test_unwrap(
+        self, proxy: PSKStoreProxy, psk_store: Mapping[str, bytes]
+    ) -> None:
+        assert proxy.unwrap() == psk_store
+
+    def test_eq(
+        self, proxy: PSKStoreProxy, psk_store: Mapping[str, bytes]
+    ) -> None:
+        for k, v in psk_store.items():
+            assert proxy[k] == v
+
+    def test_len(
+        self, proxy: PSKStoreProxy, psk_store: Mapping[str, bytes]
+    ) -> None:
+        assert len(proxy) == len(psk_store)
+
+
+class TestVersion:
+    @pytest.mark.parametrize("version", _SUPPORTED_TLS_VERSION)
+    def test_tls_enum_to_protocol_version(self, version: TLSVersion) -> None:
+        assert _tls_to_version(_tls_from_version(version)) is version
+
+    @pytest.mark.parametrize("version", _SUPPORTED_DTLS_VERSION)
+    def test_dtls_enum_to_protocol_version(self, version: DTLSVersion) -> None:
+        assert _dtls_to_version(_dtls_from_version(version)) is version
+
+
+class TestTLSRecordHeader:
+    @pytest.fixture(params=TLSRecordHeader.RecordType)
+    def record_type(self, request: Any) -> TLSRecordHeader.RecordType:
+        assert isinstance(request.param, TLSRecordHeader.RecordType)
+        return request.param
+
+    @pytest.fixture(params=_SUPPORTED_TLS_VERSION)
+    def version(self, request: Any) -> TLSVersion:
+        assert isinstance(request.param, TLSVersion)
+        return request.param
+
+    @pytest.fixture()
+    def length(self) -> int:
+        return 42
+
+    @pytest.fixture()
+    def header(
+        self,
+        record_type: TLSRecordHeader.RecordType,
+        version: TLSVersion,
+        length: int,
+    ) -> TLSRecordHeader:
+        return TLSRecordHeader(record_type, version, length)
+
+    @pytest.mark.parametrize("repr_", [repr, str], ids=lambda f: f.__name__)
+    def test_repr(
+        self,
+        repr_: Callable[[object], str],
+        record_type: TLSRecordHeader.RecordType,
+    ) -> None:
+        assert isinstance(repr_(record_type), str)
+
+    def test_hash(self, record_type: TLSRecordHeader.RecordType) -> None:
+        assert isinstance(hash(record_type), int)
+
+    def test_accessors(
+        self,
+        header: TLSRecordHeader,
+        record_type: TLSRecordHeader.RecordType,
+        version: TLSVersion,
+        length: int,
+    ) -> None:
+        assert len(header) == 5
+        assert header.record_type is record_type
+        assert header.version is version
+        assert header.length == length
+
+    def test_serialization(self, header: TLSRecordHeader) -> None:
+        serialized = bytes(header)
+        assert isinstance(serialized, bytes)
+        assert len(serialized) == 5
+        assert TLSRecordHeader.from_bytes(serialized) == header
+
+
+class TestTLSSession:
+    @pytest.fixture()
+    def session(self) -> TLSSession:
+        return TLSSession()
+
+    def test_repr(self, session: TLSSession) -> None:
+        assert isinstance(repr(session), str)
+
+
+class TestTrustStore:
+    @pytest.fixture()
+    def store(self) -> TrustStore:
+        return TrustStore.system()
+
+    @pytest.mark.parametrize("repr_", [repr, str], ids=lambda f: f.__name__)
+    def test_repr(
+        self, repr_: Callable[[object], str], store: TrustStore
+    ) -> None:
+        assert isinstance(repr_(store), str)
+
+    def test_eq(self, store: TrustStore) -> None:
+        other = TrustStore(store)
+        assert store is not other
+        assert store == other
+
+    def test_bool(self, store: TrustStore) -> None:
+        assert not TrustStore()
+        assert store
+
+    def test_len(self, store: TrustStore) -> None:
+        assert len(store) != 0
+
+    def test_iter(self, store: TrustStore) -> None:
+        assert store[0] != store[1]
+        n = 0
+        for n, crt in enumerate(store, start=1):
+            assert crt in store
+        assert n == len(store)
+
+    def test_add_existing_certificate(self, store: TrustStore) -> None:
+        length = len(store)
+        store.add(store[0])
+        assert len(store) == length
+
+    def test_add_new_certificate(self, store: TrustStore) -> None:
+        root_ca = make_root_ca()[0]
+        length = len(store)
+        store.add(root_ca)
+        assert len(store) == length + 1
+
+
+class TestDTLSCookie:
+    @pytest.fixture()
+    def cookie(self) -> DTLSCookie:
+        return DTLSCookie()
+
+    def test_generate_does_not_raise(self, cookie: DTLSCookie) -> None:
+        cookie.generate()
+
+    def test_timeout(self, cookie: DTLSCookie) -> None:
+        assert cookie.timeout == 60
+        cookie.timeout = 1000
+        assert cookie.timeout == 1000
+
+
+def assert_conf_invariant(
+    conf: Union[TLSConfiguration, DTLSConfiguration],
+    **elem: Any,
+) -> None:
+    # For the context, the configuration is converted into an
+    # internal MbedTLSConfiguration and the accessors then
+    # converts the MbedTLSConfiguration back into a
+    # TLSConfiguration (or DTLSConfiguration).  These conversions
+    # are what we actually check here.
+    __tracebackhide__ = True  # pylint: disable=unused-variable
+    assert len(elem) == 1
+
+    key, value = next(iter(elem.items()))
+    assert (
+        getattr(ServerContext(conf.update(**elem)).configuration, key) == value
+    )
+
+
+class TestConfiguration:
+    @pytest.fixture(params=[DTLSConfiguration, TLSConfiguration])
+    def conf(self, request: Any) -> Union[TLSConfiguration, DTLSConfiguration]:
+        conf = request.param()
+        assert isinstance(conf, (TLSConfiguration, DTLSConfiguration))
+        return conf
+
+    @pytest.mark.parametrize("validate", [True, False])
+    def test_set_validate_certificates(
+        self, conf: Union[TLSConfiguration, DTLSConfiguration], validate: bool
+    ) -> None:
+        assert_conf_invariant(conf, validate_certificates=validate)
+
+    def test_set_empty_certificate_chain(
+        self, conf: Union[TLSConfiguration, DTLSConfiguration]
+    ) -> None:
+        assert_conf_invariant(conf, certificate_chain=None)
+
+    def test_set_certificate_chain(
+        self, conf: Union[TLSConfiguration, DTLSConfiguration]
+    ) -> None:
+        root_crt, root_key = make_root_ca()
+        ee_crt, ee_key = make_crt(root_crt, root_key)
+        chain = (ee_crt, root_crt), ee_key
+        assert_conf_invariant(conf, certificate_chain=chain)
+
+    def test_set_ciphers(
+        self, conf: Union[TLSConfiguration, DTLSConfiguration]
+    ) -> None:
+        assert_conf_invariant(conf, ciphers=tuple(ciphers_available()))
+
+    @pytest.mark.parametrize(
+        "inner_protocols",
+        [
+            (),
+            (NextProtocol.H2, NextProtocol.H2C),
+            (NextProtocol.H2, NextProtocol.H2C, NextProtocol.FTP),
+        ],
+    )
+    def test_set_inner_protocols(
+        self,
+        conf: Union[TLSConfiguration, DTLSConfiguration],
+        inner_protocols: Tuple[Union[NextProtocol, bytes]],
+    ) -> None:
+        assert_conf_invariant(
+            conf,
+            inner_protocols=inner_protocols,
+        )
+
+    @pytest.mark.parametrize("trust_store", [TrustStore.system()])
+    def test_trust_store(
+        self,
+        conf: Union[TLSConfiguration, DTLSConfiguration],
+        trust_store: TrustStore,
+    ) -> None:
+        assert trust_store
+        assert_conf_invariant(conf, trust_store=trust_store)
+
+    @pytest.mark.parametrize("mfl", MaxFragmentLength)
+    def test_max_fragmentation_length(
+        self,
+        conf: Union[TLSConfiguration, DTLSConfiguration],
+        mfl: MaxFragmentLength,
+    ) -> None:
+        assert_conf_invariant(conf, max_fragmentation_length=mfl)
+
+    def test_set_sni_callback(
+        self,
+        conf: Union[TLSConfiguration, DTLSConfiguration],
+    ) -> None:
+        assert conf.sni_callback is None
+
+    @pytest.mark.parametrize("psk", [None, ("client", b"the secret key")])
+    def test_psk(
+        self,
+        conf: Union[TLSConfiguration, DTLSConfiguration],
+        psk: Tuple[str, bytes],
+    ) -> None:
+        assert conf.pre_shared_key is None
+        assert_conf_invariant(conf, pre_shared_key=psk)
+
+    @pytest.mark.parametrize("psk_store", [{}, {"client": b"the secret key"}])
+    def test_psk_store(
+        self,
+        conf: Union[TLSConfiguration, DTLSConfiguration],
+        psk_store: Mapping[str, bytes],
+    ) -> None:
+        assert not conf.pre_shared_key_store
+        assert_conf_invariant(conf, pre_shared_key_store=psk_store)
+
+
+class TestTLSConfiguration:
+    @pytest.fixture()
+    def conf(self) -> TLSConfiguration:
+        return TLSConfiguration()
+
+    def test_default_supported_versions(self, conf: TLSConfiguration) -> None:
+        assert conf.lowest_supported_version is TLSVersion.TLSv1
+        assert conf.highest_supported_version is TLSVersion.MAXIMUM_SUPPORTED
+
+    @pytest.mark.parametrize("version", _SUPPORTED_TLS_VERSION)
+    def test_lowest_supported_version(
+        self, conf: TLSConfiguration, version: TLSVersion
+    ) -> None:
+        assert_conf_invariant(conf, lowest_supported_version=version)
+
+    @pytest.mark.parametrize("version", _SUPPORTED_TLS_VERSION)
+    def test_highest_supported_version(
+        self, conf: TLSConfiguration, version: TLSVersion
+    ) -> None:
+        assert_conf_invariant(conf, highest_supported_version=version)
+
+
+class TestDTLSConfiguration:
+    @pytest.fixture()
+    def conf(self) -> DTLSConfiguration:
+        return DTLSConfiguration()
+
+    def test_default_supported_versions(self, conf: DTLSConfiguration) -> None:
+        assert conf.lowest_supported_version is DTLSVersion.DTLSv1_0
+        assert conf.highest_supported_version is DTLSVersion.MAXIMUM_SUPPORTED
+
+    @pytest.mark.parametrize("version", _SUPPORTED_DTLS_VERSION)
+    def test_lowest_supported_version(
+        self, conf: DTLSConfiguration, version: DTLSVersion
+    ) -> None:
+        assert_conf_invariant(conf, lowest_supported_version=version)
+
+    @pytest.mark.parametrize("version", _SUPPORTED_DTLS_VERSION)
+    def test_highest_supported_version(
+        self, conf: DTLSConfiguration, version: DTLSVersion
+    ) -> None:
+        assert_conf_invariant(conf, highest_supported_version=version)
+
+    @pytest.mark.parametrize("anti_replay", [True, False])
+    def test_set_anti_replay(
+        self, conf: DTLSConfiguration, anti_replay: bool
+    ) -> None:
+        assert conf.anti_replay is True
+        assert_conf_invariant(conf, anti_replay=anti_replay)
+
+    @pytest.mark.parametrize(
+        "hs_min_max", [(1, 60), (42, 69), (4.2, 6.9), (42.0, 69.0)]
+    )
+    def test_handshake_timeout_minmax(
+        self,
+        conf: DTLSConfiguration,
+        hs_min_max: Tuple[float, float],
+    ) -> None:
+        hs_min, hs_max = hs_min_max
+        assert conf.handshake_timeout_min == 1.0
+        assert conf.handshake_timeout_max == 60.0
+        conf_ = conf.update(
+            handshake_timeout_min=hs_min,
+            handshake_timeout_max=hs_max,
+        )
+        assert conf_.handshake_timeout_min == hs_min
+        assert conf_.handshake_timeout_max == hs_max
+
+        assert_conf_invariant(conf, handshake_timeout_min=hs_min)
+        assert_conf_invariant(conf, handshake_timeout_max=hs_max)
+
+    @pytest.mark.parametrize("hs_min_max", [(1, 60), (42, 69), (4.2, 6.9)])
+    def test_handshake_timeout_default(
+        self,
+        conf: DTLSConfiguration,
+        hs_min_max: Tuple[float, float],
+    ) -> None:
+        assert conf.handshake_timeout_min == 1.0
+        assert conf.handshake_timeout_max == 60.0
+
+        hs_min, hs_max = hs_min_max
+        conf_ = conf.update(
+            handshake_timeout_min=hs_min,
+            handshake_timeout_max=hs_max,
+        )
+        assert conf_.handshake_timeout_min == hs_min
+        assert conf_.handshake_timeout_max == hs_max
+
+        assert_conf_invariant(conf, handshake_timeout_min=hs_min)
+        assert_conf_invariant(conf, handshake_timeout_max=hs_max)
+
+
+class TestContext:
+    @pytest.fixture(params=[Purpose.SERVER_AUTH, Purpose.CLIENT_AUTH])
+    def purpose(self, request: Any) -> Purpose:
+        assert isinstance(request.param, Purpose)
+        return request.param
+
+    @pytest.fixture(params=[TLSConfiguration, DTLSConfiguration])
+    def conf(self, request: Any) -> Union[TLSConfiguration, DTLSConfiguration]:
+        conf = request.param()
+        assert isinstance(conf, (TLSConfiguration, DTLSConfiguration))
+        return conf
+
+    @pytest.fixture(params=[ServerContext, ClientContext])
+    def context(
+        self, conf: Union[TLSConfiguration, DTLSConfiguration], request: Any
+    ) -> Union[ServerContext, ClientContext]:
+        ctx = request.param(conf)
+        assert isinstance(ctx, (ServerContext, ClientContext))
+        return ctx
+
+    def test_repr(self, context: Union[ServerContext, ClientContext]) -> None:
+        assert isinstance(repr(context), str)
+
+    def test_get_configuration(
+        self,
+        context: Union[ServerContext, ClientContext],
+        conf: Union[TLSConfiguration, DTLSConfiguration],
+    ) -> None:
+        assert context.configuration == conf
+
+
+CLIENT_HELLO = (HandshakeStep.CLIENT_HELLO,)
+SERVER_HELLO = (
+    HandshakeStep.SERVER_HELLO,
+    HandshakeStep.SERVER_CERTIFICATE,
+    HandshakeStep.SERVER_KEY_EXCHANGE,
+    HandshakeStep.CERTIFICATE_REQUEST,
+    HandshakeStep.SERVER_HELLO_DONE,
+)
+CLIENT_KEY_EXCHANGE = (
+    HandshakeStep.CLIENT_CERTIFICATE,
+    HandshakeStep.CLIENT_KEY_EXCHANGE,
+    HandshakeStep.CERTIFICATE_VERIFY,
+    HandshakeStep.CLIENT_CHANGE_CIPHER_SPEC,
+    HandshakeStep.CLIENT_FINISHED,
+)
+SERVER_CHANGE_CIPHER_SPEC = (
+    HandshakeStep.SERVER_CHANGE_CIPHER_SPEC,
+    HandshakeStep.SERVER_FINISHED,
+)
+HANDSHAKE_OVER = (
+    HandshakeStep.FLUSH_BUFFERS,
+    HandshakeStep.HANDSHAKE_WRAPUP,
+    HandshakeStep.HANDSHAKE_OVER,
+)
+
+
+def do_io(
+    *, src: TLSWrappedBuffer, dst: TLSWrappedBuffer, amt: int = 1024
+) -> None:
+    # pylint: disable=protected-access
+    __tracebackhide__ = True  # pylint: disable=unused-variable
+    assert src._output_buffer, "nothing to do"
+    while src._output_buffer:
+        in_transit = src.peek_outgoing(amt)
+        src.consume_outgoing(len(in_transit))
+        dst.receive_from_network(in_transit)
+
+
+def do_send(
+    data: bytes, *, src: TLSWrappedBuffer, dst: TLSWrappedBuffer
+) -> bytes:
+    amt = src.write(data)
+    do_io(src=src, dst=dst)
+    return dst.read(amt)
+
+
+def do_handshake(
+    end: TLSWrappedBuffer, states: Sequence[HandshakeStep]
+) -> None:
+    # pylint: disable=protected-access
+    __tracebackhide__ = True  # pylint: disable=unused-variable
+    while end._handshake_state is not states[0]:
+        # The backend goes through every state for both
+        # ends.  This is not relevant.
+        try:
+            end.do_handshake()
+        except (WantReadError, WantWriteError) as exc:
+            raise AssertionError(
+                f"{type(end.context).__name__} wants {end._handshake_state}"
+            ) from exc
+
+    for state in states:
+        assert end._handshake_state is state
+        if state is HandshakeStep.HANDSHAKE_OVER:
+            break
+        with suppress(WantWriteError):
+            end.do_handshake()
+
+
+def make_full_handshake(
+    *, client: TLSWrappedBuffer, server: TLSWrappedBuffer
+) -> None:
+    do_handshake(client, CLIENT_HELLO)
+    do_io(src=client, dst=server)
+
+    do_handshake(server, SERVER_HELLO)
+    do_io(src=server, dst=client)
+    assert client.negotiated_protocol() == server.negotiated_protocol()
+
+    do_handshake(client, CLIENT_KEY_EXCHANGE)
+    do_io(src=client, dst=server)
+    assert client.negotiated_tls_version() == server.negotiated_tls_version()
+
+    do_handshake(server, SERVER_CHANGE_CIPHER_SPEC)
+    do_io(src=server, dst=client)
+
+    do_handshake(server, HANDSHAKE_OVER)
+    do_handshake(client, HANDSHAKE_OVER)
+    assert client.cipher() == server.cipher()
+
+
+def make_hello_verify_request(
+    *, client: TLSWrappedBuffer, server: TLSWrappedBuffer, cookie: bytes
+) -> None:
+    do_handshake(client, CLIENT_HELLO)
+    do_io(src=client, dst=server)
+    server.setcookieparam(cookie)
+    with pytest.raises(HelloVerifyRequest):
+        do_handshake(
+            server,
+            (
+                HandshakeStep.SERVER_HELLO,
+                HandshakeStep.SERVER_HELLO_VERIFY_REQUEST_SENT,
+            ),
+        )
+
+    do_handshake(server, (HandshakeStep.HELLO_REQUEST,))
+    server.setcookieparam(cookie)
+    do_io(src=server, dst=client)
+
+
+def do_communicate(args: Any) -> str:
+    while True:
+        with subprocess.Popen(
+            args,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+            text=True,
+            encoding="utf8",
+        ) as proc:
+            out, err = proc.communicate()
+            if "ConnectionRefusedError" in err:
+                time.sleep(0.01)  # Avoid tight CPU loop.
+                continue
+            return out
+
+
+class TestTLSHandshake:
+    @pytest.fixture(scope="class")
+    def hostname(self) -> _HostName:
+        return "www.example.com"
+
+    @pytest.fixture(scope="class")
+    def certificate_chain(
+        self, hostname: _HostName
+    ) -> Tuple[Tuple[CRT, ...], _Key]:
+        root_crt, root_key = make_root_ca()
+        ee_crt, ee_key = make_crt(
+            root_crt, root_key, subject=f"OU=test, CN={hostname}"
+        )
+        return (ee_crt, root_crt), ee_key
+
+    def test_cert_without_validation(
+        self, certificate_chain: Tuple[Tuple[CRT, ...], _Key]
+    ) -> None:
+        server = ServerContext(
+            TLSConfiguration(
+                certificate_chain=certificate_chain,
+                validate_certificates=False,
+            )
+        ).wrap_buffers()
+        client = ClientContext(
+            TLSConfiguration(validate_certificates=False)
+        ).wrap_buffers("hostname")
+        make_full_handshake(client=client, server=server)
+
+        secret = b"a very secret message"
+        assert do_send(secret, src=client, dst=server) == secret
+        assert do_send(secret, src=server, dst=client) == secret
+
+    def test_cert_with_validation(
+        self,
+        hostname: _HostName,
+        certificate_chain: Tuple[Tuple[CRT, ...], _Key],
+    ) -> None:
+        trust_store = TrustStore()
+        crt: CRT
+        for crt in certificate_chain[0][1:]:
+            trust_store.add(crt)
+        server = ServerContext(
+            TLSConfiguration(
+                certificate_chain=certificate_chain,
+                validate_certificates=False,
+            )
+        ).wrap_buffers()
+        # Host name must now be the common name (CN) of the leaf certificate.
+        client = ClientContext(
+            TLSConfiguration(trust_store=trust_store)
+        ).wrap_buffers(hostname)
+        make_full_handshake(client=client, server=server)
+
+        secret = b"a very secret message"
+        assert do_send(secret, src=client, dst=server) == secret
+        assert do_send(secret, src=server, dst=client) == secret
+
+    def test_psk(self) -> None:
+        psk = ("cli", b"secret")
+        server = ServerContext(
+            TLSConfiguration(
+                pre_shared_key_store=dict((psk,)),
+                validate_certificates=False,
+            )
+        ).wrap_buffers()
+        client = ClientContext(
+            TLSConfiguration(
+                pre_shared_key=psk,
+                validate_certificates=False,
+            ),
+        ).wrap_buffers("hostname")
+        make_full_handshake(client=client, server=server)
+
+        secret = b"a very secret message"
+        assert do_send(secret, src=client, dst=server) == secret
+        assert do_send(secret, src=server, dst=client) == secret
+
+
+class TestDTLSHandshake:
+    def test_psk(self) -> None:
+        psk = ("cli", b"secret")
+        server = ServerContext(
+            DTLSConfiguration(
+                pre_shared_key_store=dict((psk,)),
+                validate_certificates=False,
+            )
+        ).wrap_buffers()
+        client = ClientContext(
+            DTLSConfiguration(
+                pre_shared_key=psk,
+                validate_certificates=False,
+            ),
+        ).wrap_buffers("hostname")
+        make_hello_verify_request(
+            client=client, server=server, cookie="🍪🍪🍪".encode()
+        )
+        make_full_handshake(client=client, server=server)
+
+        secret = b"a very secret message"
+        assert do_send(secret, src=client, dst=server) == secret
+        assert do_send(secret, src=server, dst=client) == secret
+
+    @pytest.mark.parametrize("mtu_cli", [0, 128, 380, 500, (1 << 16) - 1])
+    @pytest.mark.parametrize("mtu_srv", [0, 128, 380, 500, (1 << 16) - 1])
+    def test_psk_set_mtu(self, mtu_cli: int, mtu_srv: int) -> None:
+        psk = ("cli", b"secret")
+        server = ServerContext(
+            DTLSConfiguration(
+                pre_shared_key_store=dict((psk,)),
+                validate_certificates=False,
+            )
+        ).wrap_buffers()
+        server.setmtu(mtu_srv)
+        client = ClientContext(
+            DTLSConfiguration(
+                pre_shared_key=psk,
+                validate_certificates=False,
+            ),
+        ).wrap_buffers("hostname")
+        client.setmtu(mtu_cli)
+        make_hello_verify_request(
+            client=client, server=server, cookie="🍪🍪🍪".encode()
+        )
+        make_full_handshake(client=client, server=server)
+
+        secret = b"a very secret message"
+        assert do_send(secret, src=client, dst=server) == secret
+        assert do_send(secret, src=server, dst=client) == secret
+
+    def test_resume_from_pickle(self) -> None:
+        psk = ("cli", b"secret")
+        server = ServerContext(
+            DTLSConfiguration(
+                pre_shared_key_store=dict((psk,)),
+                validate_certificates=False,
+            )
+        ).wrap_buffers()
+        client = ClientContext(
+            DTLSConfiguration(
+                pre_shared_key=psk,
+                ciphers=("TLS-ECDHE-PSK-WITH-CHACHA20-POLY1305-SHA256",),
+                lowest_supported_version=DTLSVersion.DTLSv1_2,
+                validate_certificates=False,
+            ),
+        ).wrap_buffers("hostname")
+        make_hello_verify_request(
+            client=client, server=server, cookie="🍪🍪🍪".encode()
+        )
+        make_full_handshake(client=client, server=server)
+
+        secret = b"a very secret message"
+        do_send(secret, src=client, dst=server)
+        do_send(secret, src=server, dst=client)
+
+        client = pickle.loads(pickle.dumps(client))
+        do_send(secret, src=client, dst=server)
+        do_send(secret, src=server, dst=client)
+
+
+class TestWrappedSocket_SmokeTests:
+    @pytest.mark.parametrize("conf", [TLSConfiguration(), DTLSConfiguration()])
+    def test_wrap_unwrap_client(
+        self, conf: Union[TLSConfiguration, DTLSConfiguration]
+    ) -> None:
+        with ClientContext(conf).wrap_socket(socket.socket(), None):
+            pass
+
+    @pytest.mark.parametrize("conf", [TLSConfiguration(), DTLSConfiguration()])
+    def test_wrap_unwrap_server(
+        self, conf: Union[TLSConfiguration, DTLSConfiguration]
+    ) -> None:
+        with ServerContext(conf).wrap_socket(socket.socket()):
+            pass
+
+
+@pytest.mark.e2e()
+@pytest.mark.skipif(sys.platform == "win32", reason="Flaky under Windows")
+class TestProgramsTLS:
+    @pytest.fixture(scope="class")
+    def port(self) -> int:
+        """Return a free port
+
+        Note:
+            Not 100% race condition free.
+
+        """
+        port = 0
+        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
+            sock.bind(("localhost", port))
+            port = sock.getsockname()[1]
+        return port
+
+    @pytest.fixture(scope="class")
+    def server(
+        self, rootpath: Path, port: int
+    ) -> Iterator[subprocess.Popen[str]]:
+        args = [
+            sys.executable,
+            str(rootpath / "programs" / "server.py"),
+            "--port",
+            f"{port}",
+            "--tls",
+            "--psk-store",
+            "cli=secret",
+        ]
+        with subprocess.Popen(args, text=True, encoding="utf8") as proc:
+            yield proc
+            proc.kill()
+            proc.wait(1.0)
+
+    @pytest.mark.repeat(3)
+    @pytest.mark.usefixtures("server")
+    @pytest.mark.timeout(30)
+    def test_client(self, rootpath: Path, port: int) -> None:
+        secret = "a very secret message"
+        args = [
+            sys.executable,
+            str(rootpath / "programs" / "client.py"),
+            "--port",
+            f"{port}",
+            "--tls",
+            "--psk",
+            "cli=secret",
+            secret,
+        ]
+        for _ in range(3):
+            assert do_communicate(args) == secret + "\n"
+
+    @pytest.mark.usefixtures("server")
+    @pytest.mark.timeout(30)
+    def test_raw_socket_send_recv(self, port: int) -> None:
+        secret = b"a very secret message"
+        with ClientContext(
+            TLSConfiguration(
+                pre_shared_key=("cli", b"secret"),
+                validate_certificates=False,
+            ),
+        ).wrap_socket(
+            socket.socket(socket.AF_INET, socket.SOCK_STREAM), "localhost"
+        ) as client:
+            client.connect(("127.0.0.1", port))
+            client.do_handshake()
+            sent = client.send(secret)
+            assert sent == len(secret)
+
+            data = client.recv(1024)
+        assert data == secret
+
+    @pytest.mark.usefixtures("server")
+    @pytest.mark.timeout(30)
+    def test_raw_socket_send_recv_into(self, port: int) -> None:
+        secret = b"a very secret message"
+        buffer = bytearray(b"\0" * 256)
+        with ClientContext(
+            TLSConfiguration(
+                pre_shared_key=("cli", b"secret"),
+                validate_certificates=False,
+            ),
+        ).wrap_socket(
+            socket.socket(socket.AF_INET, socket.SOCK_STREAM), "localhost"
+        ) as client:
+            client.connect(("127.0.0.1", port))
+            client.do_handshake()
+            sent = client.send(secret)
+            assert sent == len(secret)
+
+            received = client.recv_into(buffer, 1024)
+        assert buffer[:received] == secret
+
+    @pytest.mark.usefixtures("server")
+    @pytest.mark.timeout(30)
+    def test_raw_socket_sendall_recv(self, port: int) -> None:
+        secret = b"a very secret message"
+        with ClientContext(
+            TLSConfiguration(
+                pre_shared_key=("cli", b"secret"),
+                validate_certificates=False,
+            ),
+        ).wrap_socket(
+            socket.socket(socket.AF_INET, socket.SOCK_STREAM), "localhost"
+        ) as client:
+            client.connect(("127.0.0.1", port))
+            client.do_handshake()
+            client.sendall(secret)
+            data = client.recv(1024)
+        assert data == secret
+
+    @pytest.mark.usefixtures("server")
+    @pytest.mark.timeout(30)
+    def test_raw_socket_connectionless_unavailable(self, port: int) -> None:
+        address = ("127.0.0.1", port)
+        with ClientContext(
+            TLSConfiguration(
+                pre_shared_key=("cli", b"secret"),
+                validate_certificates=False,
+            ),
+        ).wrap_socket(
+            socket.socket(socket.AF_INET, socket.SOCK_STREAM), "localhost"
+        ) as client:
+            with pytest.raises(OSError) as excinfo:
+                client.do_handshake(address)
+
+        assert excinfo.value.errno is errno.ENOTCONN
+
+
+@pytest.mark.e2e()
+@pytest.mark.skipif(sys.platform == "win32", reason="Flaky under Windows")
+class TestProgramsDTLS:
+    @pytest.fixture(scope="class")
+    def port(self) -> int:
+        """Return a free port
+
+        Note:
+            Not 100% race condition free.
+
+        """
+        port = 0
+        with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as sock:
+            sock.bind(("localhost", port))
+            port = sock.getsockname()[1]
+        return port
+
+    @pytest.fixture(scope="class")
+    def server(
+        self, rootpath: Path, port: int
+    ) -> Iterator[subprocess.Popen[str]]:
+        args = [
+            sys.executable,
+            str(rootpath / "programs" / "server.py"),
+            "--port",
+            f"{port}",
+            "--dtls",
+            "--psk-store",
+            "cli=secret",
+        ]
+        with subprocess.Popen(args, text=True, encoding="utf8") as proc:
+            yield proc
+            proc.kill()
+            proc.wait(1.0)
+
+    @pytest.mark.repeat(3)
+    @pytest.mark.usefixtures("server")
+    @pytest.mark.timeout(30)
+    def test_client(self, rootpath: Path, port: int) -> None:
+        secret = "a very secret message"
+        args = [
+            sys.executable,
+            str(rootpath / "programs" / "client.py"),
+            "--port",
+            f"{port}",
+            "--dtls",
+            "--psk",
+            "cli=secret",
+            secret,
+        ]
+        for _ in range(3):
+            assert do_communicate(args) == secret + "\n"
+
+    @pytest.mark.usefixtures("server")
+    @pytest.mark.timeout(30)
+    def test_raw_socket_send_recv(self, port: int) -> None:
+        address = ("127.0.0.1", port)
+        secret = b"a very secret message"
+        with ClientContext(
+            DTLSConfiguration(
+                pre_shared_key=("cli", b"secret"),
+                validate_certificates=False,
+            ),
+        ).wrap_socket(
+            socket.socket(socket.AF_INET, socket.SOCK_DGRAM), "localhost"
+        ) as client:
+            client.connect(address)
+            client.do_handshake()
+            sent = client.send(secret)
+            assert sent == len(secret)
+
+            data = client.recv(1024)
+        assert data == secret
+
+    @pytest.mark.usefixtures("server")
+    @pytest.mark.timeout(30)
+    def test_raw_socket_sendto_recvfrom(self, port: int) -> None:
+        address = ("127.0.0.1", port)
+        secret = b"a very secret message"
+        with ClientContext(
+            DTLSConfiguration(
+                pre_shared_key=("cli", b"secret"),
+                validate_certificates=False,
+            ),
+        ).wrap_socket(
+            socket.socket(socket.AF_INET, socket.SOCK_DGRAM), "localhost"
+        ) as client:
+            client.do_handshake(address)
+            sent = client.sendto(secret, address)
+            assert sent == len(secret)
+
+            data, addr = client.recvfrom(1024)
+            assert addr == address
+        assert data == secret
+
+    @pytest.mark.usefixtures("server")
+    @pytest.mark.timeout(30)
+    def test_raw_socket_sendto_recvfrom_with_flags(self, port: int) -> None:
+        # Note that flags is always 0 (noop) here because we are only
+        # interested in testing the API.  See also issue #62.
+        address = ("127.0.0.1", port)
+        secret = b"a very secret message"
+        with ClientContext(
+            DTLSConfiguration(
+                pre_shared_key=("cli", b"secret"),
+                validate_certificates=False,
+            ),
+        ).wrap_socket(
+            socket.socket(socket.AF_INET, socket.SOCK_DGRAM), "localhost"
+        ) as client:
+            client.do_handshake(0, address)
+            sent = client.sendto(secret, 0, address)
+            assert sent == len(secret)
+
+            data, addr = client.recvfrom(1024, 0)
+            assert addr == address
+        assert data == secret
+
+    @pytest.mark.usefixtures("server")
+    @pytest.mark.timeout(30)
+    def test_raw_socket_sendto_recvfrom_into(self, port: int) -> None:
+        address = ("127.0.0.1", port)
+        secret = b"a very secret message"
+        buffer = bytearray(b"\0" * 256)
+        with ClientContext(
+            DTLSConfiguration(
+                pre_shared_key=("cli", b"secret"),
+                validate_certificates=False,
+            ),
+        ).wrap_socket(
+            socket.socket(socket.AF_INET, socket.SOCK_DGRAM), "localhost"
+        ) as client:
+            client.do_handshake(address)
+            sent = client.sendto(secret, address)
+            assert sent == len(secret)
+
+            received, addr = client.recvfrom_into(buffer, 1024)
+            assert addr == address
+        assert buffer[:received] == secret
```

### Comparing `python-mbedtls-2.7.0/tests/test_version.py` & `python-mbedtls-2.7.1/tests/test_version.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-# SPDX-License-Identifier: MIT
-
-from __future__ import annotations
-
-import pytest
-
-from mbedtls import version
-
-
-def test_version_info() -> None:
-    assert len(version.version_info) == 3
-    assert version.version_info >= (2, 7, 9)
-
-
-def test_version() -> None:
-    major, minor, micro = version.version_info
-    assert version.version == f"mbed TLS {major}.{minor}.{micro}"
-
-
-@pytest.mark.parametrize("feature", ["i do not exist"])
-def test_feature_false(feature: str) -> None:
-    assert version.has_feature(feature) is False
-
-
-@pytest.mark.parametrize(
-    "feature",
-    [
-        "md5",
-        "md5_c",
-        "mbedtls_md5",
-        "mbedtls_md5_c",
-        "MD5",
-        "MD5_C",
-        "MBEDTLS_MD5",
-        "MBEDTLS_MD5_C",
-    ],
-)
-def test_feature_true(feature: str) -> None:
-    assert version.has_feature(feature) is True
+# SPDX-License-Identifier: MIT
+
+from __future__ import annotations
+
+import pytest
+
+from mbedtls import version
+
+
+def test_version_info() -> None:
+    assert len(version.version_info) == 3
+    assert version.version_info >= (2, 7, 9)
+
+
+def test_version() -> None:
+    major, minor, micro = version.version_info
+    assert version.version == f"mbed TLS {major}.{minor}.{micro}"
+
+
+@pytest.mark.parametrize("feature", ["i do not exist"])
+def test_feature_false(feature: str) -> None:
+    assert version.has_feature(feature) is False
+
+
+@pytest.mark.parametrize(
+    "feature",
+    [
+        "md5",
+        "md5_c",
+        "mbedtls_md5",
+        "mbedtls_md5_c",
+        "MD5",
+        "MD5_C",
+        "MBEDTLS_MD5",
+        "MBEDTLS_MD5_C",
+    ],
+)
+def test_feature_true(feature: str) -> None:
+    assert version.has_feature(feature) is True
```

### Comparing `python-mbedtls-2.7.0/tests/test_x509.py` & `python-mbedtls-2.7.1/tests/test_x509.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,325 +1,315 @@
-# SPDX-License-Identifier: MIT
-
-from __future__ import annotations
-
-import datetime as dt
-import pickle
-import sys
-from pathlib import Path
-from typing import Any, Callable, Optional, Tuple, Union
-
-import certifi
-import pytest
-
-from mbedtls import hashlib
-from mbedtls.pk import ECC, RSA
-from mbedtls.x509 import CRL, CRT, CSR, BasicConstraints
-
-if sys.version_info < (3, 8):
-    from typing_extensions import Final
-else:
-    from typing import Final
-
-_PEM = str
-_DER = bytes
-_PKey = Union[ECC, RSA]
-
-CRL_PEM: Final[
-    _PEM
-] = """
------BEGIN X509 CRL-----
-MIIBqzCBlDANBgkqhkiG9w0BAQUFADA7MQswCQYDVQQGEwJOTDERMA8GA1UEChMI
-UG9sYXJTU0wxGTAXBgNVBAMTEFBvbGFyU1NMIFRlc3QgQ0EXDTExMDIyMDEwMjI1
-OVoXDTE5MTEyNTEwMjI1OVowKDASAgEBFw0xMTAyMTIxNDQ0MDdaMBICAQMXDTEx
-MDIxMjE0NDQwN1owDQYJKoZIhvcNAQEFBQADggEBAJYuWdKPdblMVWCnxpMnchuL
-dqWzK2BA0RelCaGjpxuwX3NmLDm+5hKja/DJxaRqTOf4RSC3kcX8CdIldsLO96dz
-//wAQdFPDhy6AFT5vKTO8ItPHDb7qFOqFqpeJi5XN1yoZGTB1ei0mgD3xBaKbp6U
-yCOZJSIFomt7piT4GcgWVHLUmpyHDDeodNhYPrN0jf2mr+ECd9fQJYdz1qm0Xx+Q
-NbKXDiPRmPX0qVleCZSeSp1JAmU4GoCO+96qQUpjgll+6xWya3UNj61f9sh0Zzr7
-5ug2LZo5uBM/LpNR1K3TLxNCcg7uUPTn9r143d7ivJhPl3tEJn4PXjv6mlLoOgU=
------END X509 CRL-----
-"""
-# This CRL is from mbed TLS: `tests/data_files/crl.pem`.
-
-
-@pytest.fixture(scope="module")
-def now() -> dt.datetime:
-    return dt.datetime.utcnow().replace(microsecond=0)
-
-
-def make_csr(
-    key: Optional[_PKey] = None,
-    subject: Optional[str] = None,
-    digestmod: Optional[hashlib.Algorithm] = None,
-) -> Tuple[CSR, _PKey]:
-    if key is None:
-        key = RSA()
-        key.generate()
-    if subject is None:
-        subject = "OU=test, CN=example.com"
-    if digestmod is None:
-        digestmod = hashlib.sha256
-    return CSR.new(key, subject, digestmod()), key
-
-
-def make_root_ca(
-    # pylint: disable=too-many-arguments
-    subject: Optional[str] = None,
-    not_before: Optional[dt.datetime] = None,
-    not_after: Optional[dt.datetime] = None,
-    serial_number: Optional[int] = None,
-    basic_constraints: Optional[BasicConstraints] = None,
-    digestmod: Optional[hashlib.Algorithm] = None,
-    csr_key_pair: Optional[Tuple[CSR, _PKey]] = None,
-) -> Tuple[CRT, _PKey]:
-    if subject is None:
-        subject = "OU=test, CN=Trusted CA"
-    if not_before is None:
-        not_before = dt.datetime.utcnow()
-    if not_after is None:
-        not_after = not_before + dt.timedelta(days=90)
-    if serial_number is None:
-        serial_number = 0x123456
-    if basic_constraints is None:
-        basic_constraints = BasicConstraints(True, -1)
-    if digestmod is None:
-        digestmod = hashlib.sha256
-    if csr_key_pair is None:
-        csr, key = make_csr(subject=subject, digestmod=digestmod)
-    else:
-        csr, key = csr_key_pair
-
-    return (
-        CRT.selfsign(
-            csr=csr,
-            issuer_key=key,
-            not_before=not_before,
-            not_after=not_after,
-            serial_number=serial_number,
-            basic_constraints=basic_constraints,
-        ),
-        key,
-    )
-
-
-def make_crt(
-    # pylint: disable=too-many-arguments
-    issuer_crt: CRT,
-    issuer_key: _PKey,
-    subject: Optional[str] = None,
-    not_before: Optional[dt.datetime] = None,
-    not_after: Optional[dt.datetime] = None,
-    serial_number: Optional[int] = None,
-    basic_constraints: Optional[BasicConstraints] = None,
-    digestmod: Optional[hashlib.Algorithm] = None,
-    csr_key_pair: Optional[Tuple[CSR, _PKey]] = None,
-) -> Tuple[CRT, _PKey]:
-    if subject is None:
-        subject = "OU=test, CN=Intermediate Cert"
-    if not_before is None:
-        not_before = dt.datetime.utcnow()
-    if not_after is None:
-        not_after = not_before + dt.timedelta(days=90)
-    if serial_number is None:
-        serial_number = 0x123456
-    if basic_constraints is None:
-        basic_constraints = BasicConstraints(True, -1)
-    if digestmod is None:
-        digestmod = hashlib.sha256
-    if csr_key_pair is None:
-        csr, key = make_csr(subject=subject, digestmod=digestmod)
-
-    return (
-        issuer_crt.sign(
-            csr,
-            issuer_key,
-            not_before,
-            not_after,
-            serial_number,
-            basic_constraints,
-        ),
-        key,
-    )
-
-
-def make_crl() -> CRL:
-    return CRL.from_PEM(CRL_PEM)
-
-
-class TestCertificate:
-    @pytest.fixture(
-        scope="class", params=(make_csr()[0], make_root_ca()[0], make_crl())
-    )
-    def cert(self, request: Any) -> Union[CSR, CRT, CRL]:
-        assert isinstance(request.param, (CSR, CRT, CRL))
-        return request.param
-
-    @pytest.mark.parametrize(
-        "repr_",
-        [repr, str],
-        ids=lambda f: f.__name__,  # type: ignore[no-any-return]
-    )
-    def test_repr(
-        self, repr_: Callable[[object], str], cert: Union[CSR, CRT, CRL]
-    ) -> None:
-        assert isinstance(repr_(cert), str)
-
-    def test_pickle(self, cert: Union[CSR, CRT, CRL]) -> None:
-        assert cert == pickle.loads(pickle.dumps(cert))
-
-    def test_hash(self, cert: Union[CSR, CRT, CRL]) -> None:
-        assert isinstance(hash(cert), int)
-
-    def test_from_buffer(self, cert: Union[CSR, CRT, CRL]) -> None:
-        assert type(cert).from_buffer(cert.to_DER()) == cert
-
-    def test_from_file(
-        self, cert: Union[CSR, CRT, CRL], tmp_path: Path
-    ) -> None:
-        path = tmp_path / "key.der"
-        path.write_bytes(cert.to_DER())
-        assert type(cert).from_file(path) == cert
-
-    def test_from_DER(self, cert: Union[CSR, CRT, CRL]) -> None:
-        assert type(cert).from_DER(cert.to_DER()) == cert
-
-    def test_eq_DER(self, cert: Union[CSR, CRT, CRL]) -> None:
-        assert cert == cert.to_DER()
-        assert cert.to_DER() == cert
-
-    def test_eq_PEM(self, cert: Union[CSR, CRT, CRL]) -> None:
-        assert cert == cert.to_PEM()
-        assert cert.to_PEM() == cert
-
-    def test_empty_PEM_raises_ValueError(
-        self, cert: Union[CSR, CRT, CRL]
-    ) -> None:
-        with pytest.raises(ValueError):
-            type(cert).from_PEM("")
-
-    def test_empty_DER_raises_ValueError(
-        self, cert: Union[CSR, CRT, CRL]
-    ) -> None:
-        with pytest.raises(ValueError):
-            type(cert).from_DER(b"")
-
-
-class TestCRT:
-    @pytest.mark.parametrize(
-        "basic_constraints", [(True, 0), (True, 2), (False, 0)]
-    )
-    def test_accessor(
-        self, now: dt.datetime, basic_constraints: BasicConstraints
-    ) -> None:
-        not_before = now
-        not_after = now + dt.timedelta(days=90)
-        issuer = "C=NL, O=PolarSSL, CN=PolarSSL Test CA"
-        issuer_key = RSA()
-        issuer_key.generate(key_size=1024)
-        subject = "C=NL"
-        subject_key = RSA()
-        subject_key.generate(key_size=1024)
-        serial_number = 0x1234567890
-        digestmod = hashlib.sha256()
-
-        crt = CRT.new(
-            not_before=not_before,
-            not_after=not_after,
-            issuer=issuer,
-            issuer_key=issuer_key,
-            subject=subject,
-            subject_key=subject_key,
-            serial_number=serial_number,
-            digestmod=digestmod,
-            basic_constraints=basic_constraints,
-        )
-
-        assert crt.not_before == not_before
-        assert crt.not_after == not_after
-        assert crt.issuer == issuer
-        assert crt.serial_number == serial_number
-        assert crt.subject == "C=NL"
-        assert crt.subject_public_key == subject_key.export_public_key(
-            format="DER"
-        )
-        assert crt.basic_constraints == basic_constraints
-
-    def test_public_key(self) -> None:
-        crt, key = make_root_ca()
-        pem = crt.subject_public_key.export_public_key(format="PEM")
-        assert pem.startswith("-----BEGIN PUBLIC KEY-----\n")
-        assert pem.endswith("-----END PUBLIC KEY-----\n")
-        assert pem == key.export_public_key(format="PEM")
-
-    def test_revocation_bad_cast(self) -> None:
-        crt, _key = make_root_ca()
-        copy = CRT.from_buffer(crt.to_DER())
-        with pytest.raises(TypeError):
-            copy.check_revocation(crt)  # type: ignore[arg-type]
-
-    def test_next(self) -> None:
-        crt = CRT.from_file(certifi.where())
-        with pytest.raises(StopIteration):
-            while True:
-                crt = next(crt)
-
-
-class TestCSR:
-    def test_accessors(self) -> None:
-        subject = "C=NL, O=PolarSSL, CN=PolarSSL Server 1"
-        subject_key = RSA()
-        subject_key.generate(key_size=1024)
-
-        csr, _k = make_csr(
-            key=subject_key,
-            subject=subject,
-        )
-
-        assert csr.version == 1
-        assert csr.subject == subject
-        assert csr.subject_public_key == subject_key.export_public_key()
-
-
-class TestCRL:
-    def test_accessors(self) -> None:
-        crl = make_crl()
-
-        assert crl.version == 1
-        assert crl.issuer_name == "C=NL, O=PolarSSL, CN=PolarSSL Test CA"
-        assert crl.this_update == dt.datetime(2011, 2, 20, 10, 22, 59)
-        assert crl.next_update == dt.datetime(2019, 11, 25, 10, 22, 59)
-
-        assert isinstance(crl.tbs_certificate, bytes)
-        assert crl.tbs_certificate
-        assert isinstance(crl.signature_value, bytes)
-        assert crl.signature_value
-
-    def test_revoked_certificates(self) -> None:
-        crl = make_crl()
-        assert len(crl.revoked_certificates) == 2
-
-        entry = crl.revoked_certificates[0]
-        assert entry.revocation_date == dt.datetime(2011, 2, 12, 14, 44, 7)
-        assert entry.serial == 1
-
-    @pytest.mark.skip("not implemented")
-    def test_revocation_false(self, der: _DER) -> None:
-        pass
-        # crt = CRT.from_buffer(der)
-        # crl = CRL.from_buffer(crl_der)
-        # assert crt.check_revocation(crl) is False
-
-    @pytest.mark.skip("not implemented")
-    def test_crt_revocation_true(self, der: _DER) -> None:
-        pass
-
-
-class TestVerifyCertificateChain:
-    def test_verify_chain(self) -> None:
-        crt0, key0 = make_root_ca()
-        crt1, key1 = make_crt(crt0, key0)
-        crt2, _key2 = make_crt(crt1, key1)
-
-        assert crt0.verify(crt0) is True
-        assert crt1.verify(crt2) is True
-        assert crt2.verify(crt0) is False
+# SPDX-License-Identifier: MIT
+
+from __future__ import annotations
+
+import datetime as dt
+import pickle
+from pathlib import Path
+from typing import Any, Callable, Final, Optional, Tuple, Union
+
+import certifi
+import pytest
+
+from mbedtls import hashlib
+from mbedtls.pk import ECC, RSA
+from mbedtls.x509 import CRL, CRT, CSR, BasicConstraints
+
+_PEM = str
+_DER = bytes
+_PKey = Union[ECC, RSA]
+
+CRL_PEM: Final[
+    _PEM
+] = """
+-----BEGIN X509 CRL-----
+MIIBqzCBlDANBgkqhkiG9w0BAQUFADA7MQswCQYDVQQGEwJOTDERMA8GA1UEChMI
+UG9sYXJTU0wxGTAXBgNVBAMTEFBvbGFyU1NMIFRlc3QgQ0EXDTExMDIyMDEwMjI1
+OVoXDTE5MTEyNTEwMjI1OVowKDASAgEBFw0xMTAyMTIxNDQ0MDdaMBICAQMXDTEx
+MDIxMjE0NDQwN1owDQYJKoZIhvcNAQEFBQADggEBAJYuWdKPdblMVWCnxpMnchuL
+dqWzK2BA0RelCaGjpxuwX3NmLDm+5hKja/DJxaRqTOf4RSC3kcX8CdIldsLO96dz
+//wAQdFPDhy6AFT5vKTO8ItPHDb7qFOqFqpeJi5XN1yoZGTB1ei0mgD3xBaKbp6U
+yCOZJSIFomt7piT4GcgWVHLUmpyHDDeodNhYPrN0jf2mr+ECd9fQJYdz1qm0Xx+Q
+NbKXDiPRmPX0qVleCZSeSp1JAmU4GoCO+96qQUpjgll+6xWya3UNj61f9sh0Zzr7
+5ug2LZo5uBM/LpNR1K3TLxNCcg7uUPTn9r143d7ivJhPl3tEJn4PXjv6mlLoOgU=
+-----END X509 CRL-----
+"""
+# This CRL is from mbed TLS: `tests/data_files/crl.pem`.
+
+
+@pytest.fixture(scope="module")
+def now() -> dt.datetime:
+    return dt.datetime.utcnow().replace(microsecond=0)
+
+
+def make_csr(
+    key: Optional[_PKey] = None,
+    subject: Optional[str] = None,
+    digestmod: Optional[hashlib.Algorithm] = None,
+) -> Tuple[CSR, _PKey]:
+    if key is None:
+        key = RSA()
+        key.generate()
+    if subject is None:
+        subject = "OU=test, CN=example.com"
+    if digestmod is None:
+        digestmod = hashlib.sha256
+    return CSR.new(key, subject, digestmod()), key
+
+
+def make_root_ca(
+    # pylint: disable=too-many-arguments
+    subject: Optional[str] = None,
+    not_before: Optional[dt.datetime] = None,
+    not_after: Optional[dt.datetime] = None,
+    serial_number: Optional[int] = None,
+    basic_constraints: Optional[BasicConstraints] = None,
+    digestmod: Optional[hashlib.Algorithm] = None,
+    csr_key_pair: Optional[Tuple[CSR, _PKey]] = None,
+) -> Tuple[CRT, _PKey]:
+    if subject is None:
+        subject = "OU=test, CN=Trusted CA"
+    if not_before is None:
+        not_before = dt.datetime.utcnow()
+    if not_after is None:
+        not_after = not_before + dt.timedelta(days=90)
+    if serial_number is None:
+        serial_number = 0x123456
+    if basic_constraints is None:
+        basic_constraints = BasicConstraints(True, -1)
+    if digestmod is None:
+        digestmod = hashlib.sha256
+    if csr_key_pair is None:
+        csr, key = make_csr(subject=subject, digestmod=digestmod)
+    else:
+        csr, key = csr_key_pair
+
+    return (
+        CRT.selfsign(
+            csr=csr,
+            issuer_key=key,
+            not_before=not_before,
+            not_after=not_after,
+            serial_number=serial_number,
+            basic_constraints=basic_constraints,
+        ),
+        key,
+    )
+
+
+def make_crt(
+    # pylint: disable=too-many-arguments
+    issuer_crt: CRT,
+    issuer_key: _PKey,
+    subject: Optional[str] = None,
+    not_before: Optional[dt.datetime] = None,
+    not_after: Optional[dt.datetime] = None,
+    serial_number: Optional[int] = None,
+    basic_constraints: Optional[BasicConstraints] = None,
+    digestmod: Optional[hashlib.Algorithm] = None,
+    csr_key_pair: Optional[Tuple[CSR, _PKey]] = None,
+) -> Tuple[CRT, _PKey]:
+    if subject is None:
+        subject = "OU=test, CN=Intermediate Cert"
+    if not_before is None:
+        not_before = dt.datetime.utcnow()
+    if not_after is None:
+        not_after = not_before + dt.timedelta(days=90)
+    if serial_number is None:
+        serial_number = 0x123456
+    if basic_constraints is None:
+        basic_constraints = BasicConstraints(True, -1)
+    if digestmod is None:
+        digestmod = hashlib.sha256
+    if csr_key_pair is None:
+        csr, key = make_csr(subject=subject, digestmod=digestmod)
+
+    return (
+        issuer_crt.sign(
+            csr,
+            issuer_key,
+            not_before,
+            not_after,
+            serial_number,
+            basic_constraints,
+        ),
+        key,
+    )
+
+
+def make_crl() -> CRL:
+    return CRL.from_PEM(CRL_PEM)
+
+
+class TestCertificate:
+    @pytest.fixture(
+        scope="class", params=(make_csr()[0], make_root_ca()[0], make_crl())
+    )
+    def cert(self, request: Any) -> Union[CSR, CRT, CRL]:
+        assert isinstance(request.param, (CSR, CRT, CRL))
+        return request.param
+
+    @pytest.mark.parametrize("repr_", [repr, str], ids=lambda f: f.__name__)
+    def test_repr(
+        self, repr_: Callable[[object], str], cert: Union[CSR, CRT, CRL]
+    ) -> None:
+        assert isinstance(repr_(cert), str)
+
+    def test_pickle(self, cert: Union[CSR, CRT, CRL]) -> None:
+        assert cert == pickle.loads(pickle.dumps(cert))
+
+    def test_hash(self, cert: Union[CSR, CRT, CRL]) -> None:
+        assert isinstance(hash(cert), int)
+
+    def test_from_buffer(self, cert: Union[CSR, CRT, CRL]) -> None:
+        assert type(cert).from_buffer(cert.to_DER()) == cert
+
+    def test_from_file(
+        self, cert: Union[CSR, CRT, CRL], tmp_path: Path
+    ) -> None:
+        path = tmp_path / "key.der"
+        path.write_bytes(cert.to_DER())
+        assert type(cert).from_file(path) == cert
+
+    def test_from_DER(self, cert: Union[CSR, CRT, CRL]) -> None:
+        assert type(cert).from_DER(cert.to_DER()) == cert
+
+    def test_eq_DER(self, cert: Union[CSR, CRT, CRL]) -> None:
+        assert cert == cert.to_DER()
+        assert cert.to_DER() == cert
+
+    def test_eq_PEM(self, cert: Union[CSR, CRT, CRL]) -> None:
+        assert cert == cert.to_PEM()
+        assert cert.to_PEM() == cert
+
+    def test_empty_PEM_raises_ValueError(
+        self, cert: Union[CSR, CRT, CRL]
+    ) -> None:
+        with pytest.raises(ValueError):
+            type(cert).from_PEM("")
+
+    def test_empty_DER_raises_ValueError(
+        self, cert: Union[CSR, CRT, CRL]
+    ) -> None:
+        with pytest.raises(ValueError):
+            type(cert).from_DER(b"")
+
+
+class TestCRT:
+    @pytest.mark.parametrize(
+        "basic_constraints", [(True, 0), (True, 2), (False, 0)]
+    )
+    def test_accessor(
+        self, now: dt.datetime, basic_constraints: BasicConstraints
+    ) -> None:
+        not_before = now
+        not_after = now + dt.timedelta(days=90)
+        issuer = "C=NL, O=PolarSSL, CN=PolarSSL Test CA"
+        issuer_key = RSA()
+        issuer_key.generate(key_size=1024)
+        subject = "C=NL"
+        subject_key = RSA()
+        subject_key.generate(key_size=1024)
+        serial_number = 0x1234567890
+        digestmod = hashlib.sha256()
+
+        crt = CRT.new(
+            not_before=not_before,
+            not_after=not_after,
+            issuer=issuer,
+            issuer_key=issuer_key,
+            subject=subject,
+            subject_key=subject_key,
+            serial_number=serial_number,
+            digestmod=digestmod,
+            basic_constraints=basic_constraints,
+        )
+
+        assert crt.not_before == not_before
+        assert crt.not_after == not_after
+        assert crt.issuer == issuer
+        assert crt.serial_number == serial_number
+        assert crt.subject == "C=NL"
+        assert crt.subject_public_key == subject_key.export_public_key(
+            format="DER"
+        )
+        assert crt.basic_constraints == basic_constraints
+
+    def test_public_key(self) -> None:
+        crt, key = make_root_ca()
+        pem = crt.subject_public_key.export_public_key(format="PEM")
+        assert pem.startswith("-----BEGIN PUBLIC KEY-----\n")
+        assert pem.endswith("-----END PUBLIC KEY-----\n")
+        assert pem == key.export_public_key(format="PEM")
+
+    def test_revocation_bad_cast(self) -> None:
+        crt, _key = make_root_ca()
+        copy = CRT.from_buffer(crt.to_DER())
+        with pytest.raises(TypeError):
+            copy.check_revocation(crt)  # type: ignore[arg-type]
+
+    def test_next(self) -> None:
+        crt = CRT.from_file(certifi.where())
+        with pytest.raises(StopIteration):
+            while True:
+                crt = next(crt)
+
+
+class TestCSR:
+    def test_accessors(self) -> None:
+        subject = "C=NL, O=PolarSSL, CN=PolarSSL Server 1"
+        subject_key = RSA()
+        subject_key.generate(key_size=1024)
+
+        csr, _k = make_csr(
+            key=subject_key,
+            subject=subject,
+        )
+
+        assert csr.version == 1
+        assert csr.subject == subject
+        assert csr.subject_public_key == subject_key.export_public_key()
+
+
+class TestCRL:
+    def test_accessors(self) -> None:
+        crl = make_crl()
+
+        assert crl.version == 1
+        assert crl.issuer_name == "C=NL, O=PolarSSL, CN=PolarSSL Test CA"
+        assert crl.this_update == dt.datetime(2011, 2, 20, 10, 22, 59)
+        assert crl.next_update == dt.datetime(2019, 11, 25, 10, 22, 59)
+
+        assert isinstance(crl.tbs_certificate, bytes)
+        assert crl.tbs_certificate
+        assert isinstance(crl.signature_value, bytes)
+        assert crl.signature_value
+
+    def test_revoked_certificates(self) -> None:
+        crl = make_crl()
+        assert len(crl.revoked_certificates) == 2
+
+        entry = crl.revoked_certificates[0]
+        assert entry.revocation_date == dt.datetime(2011, 2, 12, 14, 44, 7)
+        assert entry.serial == 1
+
+    @pytest.mark.skip("not implemented")
+    def test_revocation_false(self, der: _DER) -> None:
+        pass
+        # crt = CRT.from_buffer(der)
+        # crl = CRL.from_buffer(crl_der)
+        # assert crt.check_revocation(crl) is False
+
+    @pytest.mark.skip("not implemented")
+    def test_crt_revocation_true(self, der: _DER) -> None:
+        pass
+
+
+class TestVerifyCertificateChain:
+    def test_verify_chain(self) -> None:
+        crt0, key0 = make_root_ca()
+        crt1, key1 = make_crt(crt0, key0)
+        crt2, _key2 = make_crt(crt1, key1)
+
+        assert crt0.verify(crt0) is True
+        assert crt1.verify(crt2) is True
+        assert crt2.verify(crt0) is False
```

