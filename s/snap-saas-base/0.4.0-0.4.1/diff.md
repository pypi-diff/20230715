# Comparing `tmp/snap_saas_base-0.4.0.tar.gz` & `tmp/snap_saas_base-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snap_saas_base-0.4.0.tar", max compression
+gzip compressed data, was "snap_saas_base-0.4.1.tar", max compression
```

## Comparing `snap_saas_base-0.4.0.tar` & `snap_saas_base-0.4.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4822 2023-07-15 17:02:42.007284 snap_saas_base-0.4.0/README.md
--rw-r--r--   0        0        0     4202 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       30 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/src/snap_saas_base/__init__.py
--rw-r--r--   0        0        0       30 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/src/snap_saas_base/models/__init__.py
--rw-r--r--   0        0        0     2153 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/src/snap_saas_base/models/base_model.py
--rw-r--r--   0        0        0     5268 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/src/snap_saas_base/models/organization.py
--rw-r--r--   0        0        0     3300 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/src/snap_saas_base/models/user.py
--rw-r--r--   0        0        0     6632 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/src/snap_saas_base/models/workspace.py
--rw-r--r--   0        0        0        0 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/src/snap_saas_base/py.typed
--rw-r--r--   0        0        0       38 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/src/snap_saas_base/schemas/__init__.py
--rw-r--r--   0        0        0     5426 1970-01-01 00:00:00.000000 snap_saas_base-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4822 2023-07-15 17:52:18.542059 snap_saas_base-0.4.1/README.md
+-rw-r--r--   0        0        0     4202 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/src/snap_saas_base/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/src/snap_saas_base/models/__init__.py
+-rw-r--r--   0        0        0     2153 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/src/snap_saas_base/models/base_model.py
+-rw-r--r--   0        0        0     5740 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/src/snap_saas_base/models/organization.py
+-rw-r--r--   0        0        0     3300 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/src/snap_saas_base/models/user.py
+-rw-r--r--   0        0        0     6632 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/src/snap_saas_base/models/workspace.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/src/snap_saas_base/py.typed
+-rw-r--r--   0        0        0       38 2023-07-15 17:52:18.546059 snap_saas_base-0.4.1/src/snap_saas_base/schemas/__init__.py
+-rw-r--r--   0        0        0     5426 1970-01-01 00:00:00.000000 snap_saas_base-0.4.1/PKG-INFO
```

### Comparing `snap_saas_base-0.4.0/README.md` & `snap_saas_base-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `snap_saas_base-0.4.0/pyproject.toml` & `snap_saas_base-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "snap-saas-base"
-version = "0.4.0"
+version = "0.4.1"
 description = "Snap Env (https://snapenv.com) Python base module."
 authors = ["Abner G Jacobsen <abner@apoana.com.br>"]
 readme = "README.md"
 repository = "https://github.com/orgs/snapenv/snap-saas-base"
 
 [tool.commitizen]  # https://commitizen-tools.github.io/commitizen/config/
 bump_message = "bump(release): v$current_version → v$new_version"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "0.4.0"
+version = "0.4.1"
 version_files = ["pyproject.toml:version"]
 
 [tool.poetry.dependencies]  # https://python-poetry.org/docs/dependency-specification/
 python = ">=3.11,<4.0"
 sqlalchemy = {extras = ["asyncio"], version = "^2.0.18"}
 cuid = "^0.4"
 pydantic = ">=1.0.0,<2.0.0"
```

### Comparing `snap_saas_base-0.4.0/src/snap_saas_base/models/base_model.py` & `snap_saas_base-0.4.1/src/snap_saas_base/models/base_model.py`

 * *Files identical despite different names*

### Comparing `snap_saas_base-0.4.0/src/snap_saas_base/models/organization.py` & `snap_saas_base-0.4.1/src/snap_saas_base/models/organization.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,19 +42,25 @@
     name: so.Mapped[str] = so.mapped_column(nullable=False)
     slug: so.Mapped[str] = so.mapped_column(nullable=False, unique=True)
     bucket: so.Mapped[str] = so.mapped_column(nullable=False)
     created_by: so.Mapped[str] = so.mapped_column(
         sa.ForeignKey("users.id", ondelete="RESTRICT"), nullable=False
     )
     revoke_link: so.Mapped[bool] = so.mapped_column(default=False, server_default=sa.text("false"))
-    org_member: so.WriteOnlyMapped["OrgMember"] = so.relationship(
-        back_populates="org", cascade="all, delete-orphan"
+    # org_memberxx: so.WriteOnlyMapped["OrgMember"] = so.relationship(
+    #     back_populates="org", cascade="all, delete-orphan"
+    # )
+    # org_member: so.WriteOnlyMapped["OrgMember"] = so.relationship(
+    org_member = so.relationship(
+        "OrgMember", back_populates="org", lazy="raise", passive_deletes=True
     )
     # org_workspaces: so.WriteOnlyMapped["Workspace"] = so.relationship(back_populates="org", cascade="all, delete-orphan")
 
+    __mapper_args__ = {"eager_defaults": True}
+
     @property
     def as_dict(self):
         """Returns a dictionary representation of the Organization instance.
 
         This method iterates over the columns of the 'organizations' table and gets the corresponding attribute value from the Organization instance.
 
         Returns
@@ -106,15 +112,19 @@
         sa.ForeignKey("organizations.id", ondelete="CASCADE"), nullable=False
     )
     member_id: so.Mapped[str] = so.mapped_column(
         sa.ForeignKey("users.id", ondelete="CASCADE"), nullable=False
     )
     role: so.Mapped[str] = so.mapped_column(nullable=False)
     # member: so.Mapped["User"] = so.relationship(back_populates="org_member")
-    org: so.Mapped["Organization"] = so.relationship(back_populates="org_member")
+    # org: so.Mapped["Organization"] = so.relationship(back_populates="org_member")
+    org = so.relationship("Organization", back_populates="org_member", uselist=False, lazy="raise")
+    # member: so.Mapped["User"] = so.relationship(back_populates="org_member")
+
+    __mapper_args__ = {"eager_defaults": True}
 
     __table_args__ = (
         sa.Index("ix_organizations_members_org_id_member_id_role", "org_id", "member_id", "role"),
     )
 
     @property
     def as_dict(self):
```

### Comparing `snap_saas_base-0.4.0/src/snap_saas_base/models/user.py` & `snap_saas_base-0.4.1/src/snap_saas_base/models/user.py`

 * *Files identical despite different names*

### Comparing `snap_saas_base-0.4.0/src/snap_saas_base/models/workspace.py` & `snap_saas_base-0.4.1/src/snap_saas_base/models/workspace.py`

 * *Files identical despite different names*

### Comparing `snap_saas_base-0.4.0/PKG-INFO` & `snap_saas_base-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snap-saas-base
-Version: 0.4.0
+Version: 0.4.1
 Summary: Snap Env (https://snapenv.com) Python base module.
 Home-page: https://github.com/orgs/snapenv/snap-saas-base
 Author: Abner G Jacobsen
 Author-email: abner@apoana.com.br
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

