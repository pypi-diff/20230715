# Comparing `tmp/mypy-boto3-iam-1.28.3.post1.tar.gz` & `tmp/mypy-boto3-iam-1.28.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iam-1.28.3.post1.tar", last modified: Fri Jul 14 16:17:59 2023, max compression
+gzip compressed data, was "mypy-boto3-iam-1.28.3.post2.tar", last modified: Sat Jul 15 06:38:32 2023, max compression
```

## Comparing `mypy-boto3-iam-1.28.3.post1.tar` & `mypy-boto3-iam-1.28.3.post2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.907362 mypy-boto3-iam-1.28.3.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:16:42.000000 mypy-boto3-iam-1.28.3.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    42754 2023-07-14 16:17:59.903361 mypy-boto3-iam-1.28.3.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    41279 2023-07-14 16:16:42.000000 mypy-boto3-iam-1.28.3.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.891360 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/
--rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-07-14 16:16:42.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-14 16:16:42.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-14 16:16:42.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   114262 2023-07-14 16:16:43.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   114058 2023-07-14 16:16:42.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-07-14 16:16:45.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15540 2023-07-14 16:16:45.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    38904 2023-07-14 16:16:45.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    38868 2023-07-14 16:16:44.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:16:42.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   141783 2023-07-14 16:16:44.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)   141430 2023-07-14 16:16:44.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   144793 2023-07-14 16:16:49.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   144612 2023-07-14 16:16:47.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:16:42.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-14 16:16:45.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-14 16:16:45.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.903361 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    42754 2023-07-14 16:17:59.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-14 16:17:59.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:17:59.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 16:17:59.000000 mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:17:59.907362 mypy-boto3-iam-1.28.3.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-14 16:16:41.000000 mypy-boto3-iam-1.28.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.330244 mypy-boto3-iam-1.28.3.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 06:37:13.000000 mypy-boto3-iam-1.28.3.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41956 2023-07-15 06:38:32.330244 mypy-boto3-iam-1.28.3.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40481 2023-07-15 06:37:13.000000 mypy-boto3-iam-1.28.3.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.330244 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/
+-rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-07-15 06:37:13.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-15 06:37:13.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-15 06:37:13.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113198 2023-07-15 06:37:15.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112994 2023-07-15 06:37:14.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15542 2023-07-15 06:37:17.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15540 2023-07-15 06:37:17.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    38502 2023-07-15 06:37:17.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38466 2023-07-15 06:37:17.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:37:13.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   141759 2023-07-15 06:37:16.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)   141406 2023-07-15 06:37:15.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   141841 2023-07-15 06:37:21.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   141660 2023-07-15 06:37:19.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-15 06:37:13.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-15 06:37:17.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-15 06:37:17.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.330244 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41956 2023-07-15 06:38:32.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-15 06:38:32.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:32.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:32.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-15 06:38:32.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-15 06:38:32.000000 mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:38:32.330244 mypy-boto3-iam-1.28.3.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-15 06:37:13.000000 mypy-boto3-iam-1.28.3.post2/setup.py
```

### Comparing `mypy-boto3-iam-1.28.3.post1/LICENSE` & `mypy-boto3-iam-1.28.3.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.3.post1/PKG-INFO` & `mypy-boto3-iam-1.28.3.post2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iam
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.IAM 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.IAM 1.28.3 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.7](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -639,18 +639,18 @@
 ### Typed dictionaries
 
 `mypy_boto3_iam.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iam.type_defs import (
-    AccessDetailOutputTypeDef,
-    AccessKeyLastUsedOutputTypeDef,
-    AccessKeyMetadataOutputTypeDef,
-    AccessKeyOutputTypeDef,
+    AccessDetailTypeDef,
+    AccessKeyLastUsedTypeDef,
+    AccessKeyMetadataTypeDef,
+    AccessKeyTypeDef,
     AddClientIDToOpenIDConnectProviderRequestRequestTypeDef,
     AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef,
     AddRoleToInstanceProfileRequestRequestTypeDef,
     AddUserToGroupRequestGroupAddUserTypeDef,
     AddUserToGroupRequestRequestTypeDef,
     AddUserToGroupRequestUserAddGroupTypeDef,
     AttachGroupPolicyRequestGroupAttachPolicyTypeDef,
@@ -658,39 +658,39 @@
     AttachGroupPolicyRequestRequestTypeDef,
     AttachRolePolicyRequestPolicyAttachRoleTypeDef,
     AttachRolePolicyRequestRequestTypeDef,
     AttachRolePolicyRequestRoleAttachPolicyTypeDef,
     AttachUserPolicyRequestPolicyAttachUserTypeDef,
     AttachUserPolicyRequestRequestTypeDef,
     AttachUserPolicyRequestUserAttachPolicyTypeDef,
-    AttachedPermissionsBoundaryOutputTypeDef,
     AttachedPermissionsBoundaryResponseMetadataTypeDef,
-    AttachedPolicyOutputTypeDef,
+    AttachedPermissionsBoundaryTypeDef,
+    AttachedPolicyTypeDef,
     ChangePasswordRequestRequestTypeDef,
     ChangePasswordRequestServiceResourceChangePasswordTypeDef,
     ContextEntryTypeDef,
     CreateAccessKeyRequestRequestTypeDef,
     CreateAccountAliasRequestRequestTypeDef,
     CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef,
     CreateGroupRequestGroupCreateTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateGroupRequestServiceResourceCreateGroupTypeDef,
-    GroupOutputTypeDef,
+    GroupTypeDef,
     TagTypeDef,
     CreateLoginProfileRequestLoginProfileCreateTypeDef,
     CreateLoginProfileRequestRequestTypeDef,
     CreateLoginProfileRequestUserCreateLoginProfileTypeDef,
-    LoginProfileOutputTypeDef,
+    LoginProfileTypeDef,
     TagOutputTypeDef,
     CreatePolicyVersionRequestPolicyCreateVersionTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
-    PolicyVersionOutputTypeDef,
+    PolicyVersionTypeDef,
     CreateServiceLinkedRoleRequestRequestTypeDef,
     CreateServiceSpecificCredentialRequestRequestTypeDef,
-    ServiceSpecificCredentialOutputTypeDef,
+    ServiceSpecificCredentialTypeDef,
     DeactivateMFADeviceRequestRequestTypeDef,
     DeleteAccessKeyRequestRequestTypeDef,
     DeleteAccountAliasRequestRequestTypeDef,
     DeleteGroupPolicyRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteInstanceProfileRequestRequestTypeDef,
     DeleteLoginProfileRequestRequestTypeDef,
@@ -700,159 +700,159 @@
     DeleteRolePermissionsBoundaryRequestRequestTypeDef,
     DeleteRolePolicyRequestRequestTypeDef,
     DeleteRoleRequestRequestTypeDef,
     DeleteSAMLProviderRequestRequestTypeDef,
     DeleteSSHPublicKeyRequestRequestTypeDef,
     DeleteServerCertificateRequestRequestTypeDef,
     DeleteServiceLinkedRoleRequestRequestTypeDef,
-    DeleteServiceLinkedRoleResponseOutputTypeDef,
+    DeleteServiceLinkedRoleResponseTypeDef,
     DeleteServiceSpecificCredentialRequestRequestTypeDef,
     DeleteSigningCertificateRequestRequestTypeDef,
     DeleteUserPermissionsBoundaryRequestRequestTypeDef,
     DeleteUserPolicyRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteVirtualMFADeviceRequestRequestTypeDef,
-    RoleUsageTypeOutputTypeDef,
+    RoleUsageTypeTypeDef,
     DetachGroupPolicyRequestGroupDetachPolicyTypeDef,
     DetachGroupPolicyRequestPolicyDetachGroupTypeDef,
     DetachGroupPolicyRequestRequestTypeDef,
     DetachRolePolicyRequestPolicyDetachRoleTypeDef,
     DetachRolePolicyRequestRequestTypeDef,
     DetachRolePolicyRequestRoleDetachPolicyTypeDef,
     DetachUserPolicyRequestPolicyDetachUserTypeDef,
     DetachUserPolicyRequestRequestTypeDef,
     DetachUserPolicyRequestUserDetachPolicyTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableMFADeviceRequestMfaDeviceAssociateTypeDef,
     EnableMFADeviceRequestRequestTypeDef,
     EnableMFADeviceRequestUserEnableMfaTypeDef,
-    EntityInfoOutputTypeDef,
-    ErrorDetailsOutputTypeDef,
-    OrganizationsDecisionDetailOutputTypeDef,
-    PermissionsBoundaryDecisionDetailOutputTypeDef,
-    GenerateCredentialReportResponseOutputTypeDef,
+    EntityInfoTypeDef,
+    ErrorDetailsTypeDef,
+    OrganizationsDecisionDetailTypeDef,
+    PermissionsBoundaryDecisionDetailTypeDef,
+    GenerateCredentialReportResponseTypeDef,
     GenerateOrganizationsAccessReportRequestRequestTypeDef,
-    GenerateOrganizationsAccessReportResponseOutputTypeDef,
+    GenerateOrganizationsAccessReportResponseTypeDef,
     GenerateServiceLastAccessedDetailsRequestRequestTypeDef,
-    GenerateServiceLastAccessedDetailsResponseOutputTypeDef,
+    GenerateServiceLastAccessedDetailsResponseTypeDef,
     GetAccessKeyLastUsedRequestRequestTypeDef,
     GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef,
     GetAccountAuthorizationDetailsRequestRequestTypeDef,
-    PasswordPolicyOutputTypeDef,
-    GetAccountSummaryResponseOutputTypeDef,
+    PasswordPolicyTypeDef,
+    GetAccountSummaryResponseTypeDef,
     GetContextKeysForCustomPolicyRequestRequestTypeDef,
-    GetContextKeysForPolicyResponseOutputTypeDef,
+    GetContextKeysForPolicyResponseTypeDef,
     GetContextKeysForPrincipalPolicyRequestRequestTypeDef,
-    GetCredentialReportResponseOutputTypeDef,
+    GetCredentialReportResponseTypeDef,
     GetGroupPolicyRequestRequestTypeDef,
-    GetGroupPolicyResponseOutputTypeDef,
+    GetGroupPolicyResponseTypeDef,
     GetGroupRequestGetGroupPaginateTypeDef,
     GetGroupRequestRequestTypeDef,
     WaiterConfigTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
     GetLoginProfileRequestRequestTypeDef,
     GetMFADeviceRequestRequestTypeDef,
-    GetMFADeviceResponseOutputTypeDef,
+    GetMFADeviceResponseTypeDef,
     GetOpenIDConnectProviderRequestRequestTypeDef,
     GetOrganizationsAccessReportRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetPolicyVersionRequestRequestTypeDef,
     GetRolePolicyRequestRequestTypeDef,
-    GetRolePolicyResponseOutputTypeDef,
+    GetRolePolicyResponseTypeDef,
     GetRoleRequestRequestTypeDef,
     GetSAMLProviderRequestRequestTypeDef,
     GetSSHPublicKeyRequestRequestTypeDef,
-    SSHPublicKeyOutputTypeDef,
+    SSHPublicKeyTypeDef,
     GetServerCertificateRequestRequestTypeDef,
     GetServiceLastAccessedDetailsRequestRequestTypeDef,
     GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef,
     GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef,
     GetUserPolicyRequestRequestTypeDef,
-    GetUserPolicyResponseOutputTypeDef,
+    GetUserPolicyResponseTypeDef,
     GetUserRequestRequestTypeDef,
-    PolicyDetailOutputTypeDef,
+    PolicyDetailTypeDef,
     ListAccessKeysRequestListAccessKeysPaginateTypeDef,
     ListAccessKeysRequestRequestTypeDef,
     ListAccountAliasesRequestListAccountAliasesPaginateTypeDef,
     ListAccountAliasesRequestRequestTypeDef,
-    ListAccountAliasesResponseOutputTypeDef,
+    ListAccountAliasesResponseTypeDef,
     ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
     ListAttachedGroupPoliciesRequestRequestTypeDef,
     ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
     ListAttachedRolePoliciesRequestRequestTypeDef,
     ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
     ListAttachedUserPoliciesRequestRequestTypeDef,
     ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
     ListEntitiesForPolicyRequestRequestTypeDef,
-    PolicyGroupOutputTypeDef,
-    PolicyRoleOutputTypeDef,
-    PolicyUserOutputTypeDef,
+    PolicyGroupTypeDef,
+    PolicyRoleTypeDef,
+    PolicyUserTypeDef,
     ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
     ListGroupPoliciesRequestRequestTypeDef,
-    ListGroupPoliciesResponseOutputTypeDef,
+    ListGroupPoliciesResponseTypeDef,
     ListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
     ListGroupsForUserRequestRequestTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
     ListInstanceProfileTagsRequestRequestTypeDef,
     ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
     ListInstanceProfilesForRoleRequestRequestTypeDef,
     ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListInstanceProfilesRequestRequestTypeDef,
     ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
     ListMFADeviceTagsRequestRequestTypeDef,
     ListMFADevicesRequestListMFADevicesPaginateTypeDef,
     ListMFADevicesRequestRequestTypeDef,
-    MFADeviceOutputTypeDef,
+    MFADeviceTypeDef,
     ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
     ListOpenIDConnectProviderTagsRequestRequestTypeDef,
-    OpenIDConnectProviderListEntryOutputTypeDef,
-    PolicyGrantingServiceAccessOutputTypeDef,
+    OpenIDConnectProviderListEntryTypeDef,
+    PolicyGrantingServiceAccessTypeDef,
     ListPoliciesGrantingServiceAccessRequestRequestTypeDef,
     ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
     ListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
     ListPolicyTagsRequestRequestTypeDef,
     ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
     ListPolicyVersionsRequestRequestTypeDef,
     ListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
     ListRolePoliciesRequestRequestTypeDef,
-    ListRolePoliciesResponseOutputTypeDef,
+    ListRolePoliciesResponseTypeDef,
     ListRoleTagsRequestListRoleTagsPaginateTypeDef,
     ListRoleTagsRequestRequestTypeDef,
     ListRolesRequestListRolesPaginateTypeDef,
     ListRolesRequestRequestTypeDef,
     ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
     ListSAMLProviderTagsRequestRequestTypeDef,
-    SAMLProviderListEntryOutputTypeDef,
+    SAMLProviderListEntryTypeDef,
     ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef,
     ListSSHPublicKeysRequestRequestTypeDef,
-    SSHPublicKeyMetadataOutputTypeDef,
+    SSHPublicKeyMetadataTypeDef,
     ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
     ListServerCertificateTagsRequestRequestTypeDef,
     ListServerCertificatesRequestListServerCertificatesPaginateTypeDef,
     ListServerCertificatesRequestRequestTypeDef,
-    ServerCertificateMetadataOutputTypeDef,
+    ServerCertificateMetadataTypeDef,
     ListServiceSpecificCredentialsRequestRequestTypeDef,
-    ServiceSpecificCredentialMetadataOutputTypeDef,
+    ServiceSpecificCredentialMetadataTypeDef,
     ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef,
     ListSigningCertificatesRequestRequestTypeDef,
-    SigningCertificateOutputTypeDef,
+    SigningCertificateTypeDef,
     ListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
     ListUserPoliciesRequestRequestTypeDef,
-    ListUserPoliciesResponseOutputTypeDef,
+    ListUserPoliciesResponseTypeDef,
     ListUserTagsRequestListUserTagsPaginateTypeDef,
     ListUserTagsRequestRequestTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef,
     ListVirtualMFADevicesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    PositionOutputTypeDef,
+    PositionTypeDef,
     PutGroupPolicyRequestGroupCreatePolicyTypeDef,
     PutGroupPolicyRequestGroupPolicyPutTypeDef,
     PutGroupPolicyRequestRequestTypeDef,
     PutRolePermissionsBoundaryRequestRequestTypeDef,
     PutRolePolicyRequestRequestTypeDef,
     PutRolePolicyRequestRolePolicyPutTypeDef,
     PutUserPermissionsBoundaryRequestRequestTypeDef,
@@ -865,18 +865,18 @@
     RemoveUserFromGroupRequestGroupRemoveUserTypeDef,
     RemoveUserFromGroupRequestRequestTypeDef,
     RemoveUserFromGroupRequestUserRemoveGroupTypeDef,
     ResetServiceSpecificCredentialRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ResyncMFADeviceRequestMfaDeviceResyncTypeDef,
     ResyncMFADeviceRequestRequestTypeDef,
-    RoleLastUsedOutputTypeDef,
+    RoleLastUsedTypeDef,
     RoleLastUsedResponseMetadataTypeDef,
     ServerCertificateMetadataResponseMetadataTypeDef,
-    TrackedActionLastAccessedOutputTypeDef,
+    TrackedActionLastAccessedTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetSecurityTokenServicePreferencesRequestRequestTypeDef,
     UntagInstanceProfileRequestRequestTypeDef,
     UntagMFADeviceRequestRequestTypeDef,
     UntagOpenIDConnectProviderRequestRequestTypeDef,
     UntagPolicyRequestRequestTypeDef,
     UntagRoleRequestRequestTypeDef,
@@ -898,40 +898,40 @@
     UpdateLoginProfileRequestLoginProfileUpdateTypeDef,
     UpdateLoginProfileRequestRequestTypeDef,
     UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef,
     UpdateRoleDescriptionRequestRequestTypeDef,
     UpdateRoleRequestRequestTypeDef,
     UpdateSAMLProviderRequestRequestTypeDef,
     UpdateSAMLProviderRequestSamlProviderUpdateTypeDef,
-    UpdateSAMLProviderResponseOutputTypeDef,
+    UpdateSAMLProviderResponseTypeDef,
     UpdateSSHPublicKeyRequestRequestTypeDef,
     UpdateServerCertificateRequestRequestTypeDef,
     UpdateServerCertificateRequestServerCertificateUpdateTypeDef,
     UpdateServiceSpecificCredentialRequestRequestTypeDef,
     UpdateSigningCertificateRequestRequestTypeDef,
     UpdateSigningCertificateRequestSigningCertificateActivateTypeDef,
     UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef,
     UpdateUserRequestRequestTypeDef,
     UpdateUserRequestUserUpdateTypeDef,
     UploadSSHPublicKeyRequestRequestTypeDef,
     UploadSigningCertificateRequestRequestTypeDef,
     UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
-    GetAccessKeyLastUsedResponseOutputTypeDef,
-    ListAccessKeysResponseOutputTypeDef,
-    CreateAccessKeyResponseOutputTypeDef,
-    ListAttachedGroupPoliciesResponseOutputTypeDef,
-    ListAttachedRolePoliciesResponseOutputTypeDef,
-    ListAttachedUserPoliciesResponseOutputTypeDef,
+    GetAccessKeyLastUsedResponseTypeDef,
+    ListAccessKeysResponseTypeDef,
+    CreateAccessKeyResponseTypeDef,
+    ListAttachedGroupPoliciesResponseTypeDef,
+    ListAttachedRolePoliciesResponseTypeDef,
+    ListAttachedUserPoliciesResponseTypeDef,
     SimulateCustomPolicyRequestRequestTypeDef,
     SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
     SimulatePrincipalPolicyRequestRequestTypeDef,
     SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
-    CreateGroupResponseOutputTypeDef,
-    ListGroupsForUserResponseOutputTypeDef,
-    ListGroupsResponseOutputTypeDef,
+    CreateGroupResponseTypeDef,
+    ListGroupsForUserResponseTypeDef,
+    ListGroupsResponseTypeDef,
     CreateInstanceProfileRequestRequestTypeDef,
     CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef,
     CreateOpenIDConnectProviderRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreatePolicyRequestServiceResourceCreatePolicyTypeDef,
     CreateRoleRequestRequestTypeDef,
     CreateRoleRequestServiceResourceCreateRoleTypeDef,
@@ -948,98 +948,98 @@
     TagPolicyRequestRequestTypeDef,
     TagRoleRequestRequestTypeDef,
     TagSAMLProviderRequestRequestTypeDef,
     TagServerCertificateRequestRequestTypeDef,
     TagUserRequestRequestTypeDef,
     UploadServerCertificateRequestRequestTypeDef,
     UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
-    CreateLoginProfileResponseOutputTypeDef,
-    GetLoginProfileResponseOutputTypeDef,
-    CreateOpenIDConnectProviderResponseOutputTypeDef,
-    CreateSAMLProviderResponseOutputTypeDef,
-    GetOpenIDConnectProviderResponseOutputTypeDef,
-    GetSAMLProviderResponseOutputTypeDef,
-    ListInstanceProfileTagsResponseOutputTypeDef,
-    ListMFADeviceTagsResponseOutputTypeDef,
-    ListOpenIDConnectProviderTagsResponseOutputTypeDef,
-    ListPolicyTagsResponseOutputTypeDef,
-    ListRoleTagsResponseOutputTypeDef,
-    ListSAMLProviderTagsResponseOutputTypeDef,
-    ListServerCertificateTagsResponseOutputTypeDef,
-    ListUserTagsResponseOutputTypeDef,
-    PolicyOutputTypeDef,
-    UserOutputTypeDef,
+    CreateLoginProfileResponseTypeDef,
+    GetLoginProfileResponseTypeDef,
+    CreateOpenIDConnectProviderResponseTypeDef,
+    CreateSAMLProviderResponseTypeDef,
+    GetOpenIDConnectProviderResponseTypeDef,
+    GetSAMLProviderResponseTypeDef,
+    ListInstanceProfileTagsResponseTypeDef,
+    ListMFADeviceTagsResponseTypeDef,
+    ListOpenIDConnectProviderTagsResponseTypeDef,
+    ListPolicyTagsResponseTypeDef,
+    ListRoleTagsResponseTypeDef,
+    ListSAMLProviderTagsResponseTypeDef,
+    ListServerCertificateTagsResponseTypeDef,
+    ListUserTagsResponseTypeDef,
+    PolicyTypeDef,
     UserResponseMetadataTypeDef,
-    CreatePolicyVersionResponseOutputTypeDef,
-    GetPolicyVersionResponseOutputTypeDef,
-    ListPolicyVersionsResponseOutputTypeDef,
-    ManagedPolicyDetailOutputTypeDef,
-    CreateServiceSpecificCredentialResponseOutputTypeDef,
-    ResetServiceSpecificCredentialResponseOutputTypeDef,
-    DeletionTaskFailureReasonTypeOutputTypeDef,
-    EntityDetailsOutputTypeDef,
-    GetOrganizationsAccessReportResponseOutputTypeDef,
-    GetAccountPasswordPolicyResponseOutputTypeDef,
+    UserTypeDef,
+    CreatePolicyVersionResponseTypeDef,
+    GetPolicyVersionResponseTypeDef,
+    ListPolicyVersionsResponseTypeDef,
+    ManagedPolicyDetailTypeDef,
+    CreateServiceSpecificCredentialResponseTypeDef,
+    ResetServiceSpecificCredentialResponseTypeDef,
+    DeletionTaskFailureReasonTypeTypeDef,
+    EntityDetailsTypeDef,
+    GetOrganizationsAccessReportResponseTypeDef,
+    GetAccountPasswordPolicyResponseTypeDef,
     GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef,
     GetPolicyRequestPolicyExistsWaitTypeDef,
     GetRoleRequestRoleExistsWaitTypeDef,
     GetUserRequestUserExistsWaitTypeDef,
-    GetSSHPublicKeyResponseOutputTypeDef,
-    UploadSSHPublicKeyResponseOutputTypeDef,
-    GroupDetailOutputTypeDef,
-    UserDetailOutputTypeDef,
-    ListEntitiesForPolicyResponseOutputTypeDef,
-    ListMFADevicesResponseOutputTypeDef,
-    ListOpenIDConnectProvidersResponseOutputTypeDef,
-    ListPoliciesGrantingServiceAccessEntryOutputTypeDef,
-    ListSAMLProvidersResponseOutputTypeDef,
-    ListSSHPublicKeysResponseOutputTypeDef,
-    ListServerCertificatesResponseOutputTypeDef,
-    ServerCertificateOutputTypeDef,
-    UploadServerCertificateResponseOutputTypeDef,
-    ListServiceSpecificCredentialsResponseOutputTypeDef,
-    ListSigningCertificatesResponseOutputTypeDef,
-    UploadSigningCertificateResponseOutputTypeDef,
-    StatementOutputTypeDef,
-    RoleOutputTypeDef,
-    ServiceLastAccessedOutputTypeDef,
-    CreatePolicyResponseOutputTypeDef,
-    GetPolicyResponseOutputTypeDef,
-    ListPoliciesResponseOutputTypeDef,
-    CreateUserResponseOutputTypeDef,
-    GetGroupResponseOutputTypeDef,
-    GetUserResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
-    VirtualMFADeviceOutputTypeDef,
-    GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef,
-    GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef,
-    ListPoliciesGrantingServiceAccessResponseOutputTypeDef,
-    GetServerCertificateResponseOutputTypeDef,
-    ResourceSpecificResultOutputTypeDef,
-    CreateRoleResponseOutputTypeDef,
-    CreateServiceLinkedRoleResponseOutputTypeDef,
-    GetRoleResponseOutputTypeDef,
-    InstanceProfileOutputTypeDef,
-    ListRolesResponseOutputTypeDef,
-    UpdateRoleDescriptionResponseOutputTypeDef,
-    GetServiceLastAccessedDetailsResponseOutputTypeDef,
-    CreateVirtualMFADeviceResponseOutputTypeDef,
-    ListVirtualMFADevicesResponseOutputTypeDef,
-    EvaluationResultOutputTypeDef,
-    CreateInstanceProfileResponseOutputTypeDef,
-    GetInstanceProfileResponseOutputTypeDef,
-    ListInstanceProfilesForRoleResponseOutputTypeDef,
-    ListInstanceProfilesResponseOutputTypeDef,
-    RoleDetailOutputTypeDef,
-    SimulatePolicyResponseOutputTypeDef,
-    GetAccountAuthorizationDetailsResponseOutputTypeDef,
+    GetSSHPublicKeyResponseTypeDef,
+    UploadSSHPublicKeyResponseTypeDef,
+    GroupDetailTypeDef,
+    UserDetailTypeDef,
+    ListEntitiesForPolicyResponseTypeDef,
+    ListMFADevicesResponseTypeDef,
+    ListOpenIDConnectProvidersResponseTypeDef,
+    ListPoliciesGrantingServiceAccessEntryTypeDef,
+    ListSAMLProvidersResponseTypeDef,
+    ListSSHPublicKeysResponseTypeDef,
+    ListServerCertificatesResponseTypeDef,
+    ServerCertificateTypeDef,
+    UploadServerCertificateResponseTypeDef,
+    ListServiceSpecificCredentialsResponseTypeDef,
+    ListSigningCertificatesResponseTypeDef,
+    UploadSigningCertificateResponseTypeDef,
+    StatementTypeDef,
+    RoleTypeDef,
+    ServiceLastAccessedTypeDef,
+    CreatePolicyResponseTypeDef,
+    GetPolicyResponseTypeDef,
+    ListPoliciesResponseTypeDef,
+    CreateUserResponseTypeDef,
+    GetGroupResponseTypeDef,
+    GetUserResponseTypeDef,
+    ListUsersResponseTypeDef,
+    VirtualMFADeviceTypeDef,
+    GetServiceLinkedRoleDeletionStatusResponseTypeDef,
+    GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef,
+    ListPoliciesGrantingServiceAccessResponseTypeDef,
+    GetServerCertificateResponseTypeDef,
+    ResourceSpecificResultTypeDef,
+    CreateRoleResponseTypeDef,
+    CreateServiceLinkedRoleResponseTypeDef,
+    GetRoleResponseTypeDef,
+    InstanceProfileTypeDef,
+    ListRolesResponseTypeDef,
+    UpdateRoleDescriptionResponseTypeDef,
+    GetServiceLastAccessedDetailsResponseTypeDef,
+    CreateVirtualMFADeviceResponseTypeDef,
+    ListVirtualMFADevicesResponseTypeDef,
+    EvaluationResultTypeDef,
+    CreateInstanceProfileResponseTypeDef,
+    GetInstanceProfileResponseTypeDef,
+    ListInstanceProfilesForRoleResponseTypeDef,
+    ListInstanceProfilesResponseTypeDef,
+    RoleDetailTypeDef,
+    SimulatePolicyResponseTypeDef,
+    GetAccountAuthorizationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> AccessDetailOutputTypeDef:
+def get_structure() -> AccessDetailTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iam-1.28.3.post1/README.md` & `mypy-boto3-iam-1.28.3.post2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.7](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -607,18 +607,18 @@
 ### Typed dictionaries
 
 `mypy_boto3_iam.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iam.type_defs import (
-    AccessDetailOutputTypeDef,
-    AccessKeyLastUsedOutputTypeDef,
-    AccessKeyMetadataOutputTypeDef,
-    AccessKeyOutputTypeDef,
+    AccessDetailTypeDef,
+    AccessKeyLastUsedTypeDef,
+    AccessKeyMetadataTypeDef,
+    AccessKeyTypeDef,
     AddClientIDToOpenIDConnectProviderRequestRequestTypeDef,
     AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef,
     AddRoleToInstanceProfileRequestRequestTypeDef,
     AddUserToGroupRequestGroupAddUserTypeDef,
     AddUserToGroupRequestRequestTypeDef,
     AddUserToGroupRequestUserAddGroupTypeDef,
     AttachGroupPolicyRequestGroupAttachPolicyTypeDef,
@@ -626,39 +626,39 @@
     AttachGroupPolicyRequestRequestTypeDef,
     AttachRolePolicyRequestPolicyAttachRoleTypeDef,
     AttachRolePolicyRequestRequestTypeDef,
     AttachRolePolicyRequestRoleAttachPolicyTypeDef,
     AttachUserPolicyRequestPolicyAttachUserTypeDef,
     AttachUserPolicyRequestRequestTypeDef,
     AttachUserPolicyRequestUserAttachPolicyTypeDef,
-    AttachedPermissionsBoundaryOutputTypeDef,
     AttachedPermissionsBoundaryResponseMetadataTypeDef,
-    AttachedPolicyOutputTypeDef,
+    AttachedPermissionsBoundaryTypeDef,
+    AttachedPolicyTypeDef,
     ChangePasswordRequestRequestTypeDef,
     ChangePasswordRequestServiceResourceChangePasswordTypeDef,
     ContextEntryTypeDef,
     CreateAccessKeyRequestRequestTypeDef,
     CreateAccountAliasRequestRequestTypeDef,
     CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef,
     CreateGroupRequestGroupCreateTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateGroupRequestServiceResourceCreateGroupTypeDef,
-    GroupOutputTypeDef,
+    GroupTypeDef,
     TagTypeDef,
     CreateLoginProfileRequestLoginProfileCreateTypeDef,
     CreateLoginProfileRequestRequestTypeDef,
     CreateLoginProfileRequestUserCreateLoginProfileTypeDef,
-    LoginProfileOutputTypeDef,
+    LoginProfileTypeDef,
     TagOutputTypeDef,
     CreatePolicyVersionRequestPolicyCreateVersionTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
-    PolicyVersionOutputTypeDef,
+    PolicyVersionTypeDef,
     CreateServiceLinkedRoleRequestRequestTypeDef,
     CreateServiceSpecificCredentialRequestRequestTypeDef,
-    ServiceSpecificCredentialOutputTypeDef,
+    ServiceSpecificCredentialTypeDef,
     DeactivateMFADeviceRequestRequestTypeDef,
     DeleteAccessKeyRequestRequestTypeDef,
     DeleteAccountAliasRequestRequestTypeDef,
     DeleteGroupPolicyRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteInstanceProfileRequestRequestTypeDef,
     DeleteLoginProfileRequestRequestTypeDef,
@@ -668,159 +668,159 @@
     DeleteRolePermissionsBoundaryRequestRequestTypeDef,
     DeleteRolePolicyRequestRequestTypeDef,
     DeleteRoleRequestRequestTypeDef,
     DeleteSAMLProviderRequestRequestTypeDef,
     DeleteSSHPublicKeyRequestRequestTypeDef,
     DeleteServerCertificateRequestRequestTypeDef,
     DeleteServiceLinkedRoleRequestRequestTypeDef,
-    DeleteServiceLinkedRoleResponseOutputTypeDef,
+    DeleteServiceLinkedRoleResponseTypeDef,
     DeleteServiceSpecificCredentialRequestRequestTypeDef,
     DeleteSigningCertificateRequestRequestTypeDef,
     DeleteUserPermissionsBoundaryRequestRequestTypeDef,
     DeleteUserPolicyRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteVirtualMFADeviceRequestRequestTypeDef,
-    RoleUsageTypeOutputTypeDef,
+    RoleUsageTypeTypeDef,
     DetachGroupPolicyRequestGroupDetachPolicyTypeDef,
     DetachGroupPolicyRequestPolicyDetachGroupTypeDef,
     DetachGroupPolicyRequestRequestTypeDef,
     DetachRolePolicyRequestPolicyDetachRoleTypeDef,
     DetachRolePolicyRequestRequestTypeDef,
     DetachRolePolicyRequestRoleDetachPolicyTypeDef,
     DetachUserPolicyRequestPolicyDetachUserTypeDef,
     DetachUserPolicyRequestRequestTypeDef,
     DetachUserPolicyRequestUserDetachPolicyTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableMFADeviceRequestMfaDeviceAssociateTypeDef,
     EnableMFADeviceRequestRequestTypeDef,
     EnableMFADeviceRequestUserEnableMfaTypeDef,
-    EntityInfoOutputTypeDef,
-    ErrorDetailsOutputTypeDef,
-    OrganizationsDecisionDetailOutputTypeDef,
-    PermissionsBoundaryDecisionDetailOutputTypeDef,
-    GenerateCredentialReportResponseOutputTypeDef,
+    EntityInfoTypeDef,
+    ErrorDetailsTypeDef,
+    OrganizationsDecisionDetailTypeDef,
+    PermissionsBoundaryDecisionDetailTypeDef,
+    GenerateCredentialReportResponseTypeDef,
     GenerateOrganizationsAccessReportRequestRequestTypeDef,
-    GenerateOrganizationsAccessReportResponseOutputTypeDef,
+    GenerateOrganizationsAccessReportResponseTypeDef,
     GenerateServiceLastAccessedDetailsRequestRequestTypeDef,
-    GenerateServiceLastAccessedDetailsResponseOutputTypeDef,
+    GenerateServiceLastAccessedDetailsResponseTypeDef,
     GetAccessKeyLastUsedRequestRequestTypeDef,
     GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef,
     GetAccountAuthorizationDetailsRequestRequestTypeDef,
-    PasswordPolicyOutputTypeDef,
-    GetAccountSummaryResponseOutputTypeDef,
+    PasswordPolicyTypeDef,
+    GetAccountSummaryResponseTypeDef,
     GetContextKeysForCustomPolicyRequestRequestTypeDef,
-    GetContextKeysForPolicyResponseOutputTypeDef,
+    GetContextKeysForPolicyResponseTypeDef,
     GetContextKeysForPrincipalPolicyRequestRequestTypeDef,
-    GetCredentialReportResponseOutputTypeDef,
+    GetCredentialReportResponseTypeDef,
     GetGroupPolicyRequestRequestTypeDef,
-    GetGroupPolicyResponseOutputTypeDef,
+    GetGroupPolicyResponseTypeDef,
     GetGroupRequestGetGroupPaginateTypeDef,
     GetGroupRequestRequestTypeDef,
     WaiterConfigTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
     GetLoginProfileRequestRequestTypeDef,
     GetMFADeviceRequestRequestTypeDef,
-    GetMFADeviceResponseOutputTypeDef,
+    GetMFADeviceResponseTypeDef,
     GetOpenIDConnectProviderRequestRequestTypeDef,
     GetOrganizationsAccessReportRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetPolicyVersionRequestRequestTypeDef,
     GetRolePolicyRequestRequestTypeDef,
-    GetRolePolicyResponseOutputTypeDef,
+    GetRolePolicyResponseTypeDef,
     GetRoleRequestRequestTypeDef,
     GetSAMLProviderRequestRequestTypeDef,
     GetSSHPublicKeyRequestRequestTypeDef,
-    SSHPublicKeyOutputTypeDef,
+    SSHPublicKeyTypeDef,
     GetServerCertificateRequestRequestTypeDef,
     GetServiceLastAccessedDetailsRequestRequestTypeDef,
     GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef,
     GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef,
     GetUserPolicyRequestRequestTypeDef,
-    GetUserPolicyResponseOutputTypeDef,
+    GetUserPolicyResponseTypeDef,
     GetUserRequestRequestTypeDef,
-    PolicyDetailOutputTypeDef,
+    PolicyDetailTypeDef,
     ListAccessKeysRequestListAccessKeysPaginateTypeDef,
     ListAccessKeysRequestRequestTypeDef,
     ListAccountAliasesRequestListAccountAliasesPaginateTypeDef,
     ListAccountAliasesRequestRequestTypeDef,
-    ListAccountAliasesResponseOutputTypeDef,
+    ListAccountAliasesResponseTypeDef,
     ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
     ListAttachedGroupPoliciesRequestRequestTypeDef,
     ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
     ListAttachedRolePoliciesRequestRequestTypeDef,
     ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
     ListAttachedUserPoliciesRequestRequestTypeDef,
     ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
     ListEntitiesForPolicyRequestRequestTypeDef,
-    PolicyGroupOutputTypeDef,
-    PolicyRoleOutputTypeDef,
-    PolicyUserOutputTypeDef,
+    PolicyGroupTypeDef,
+    PolicyRoleTypeDef,
+    PolicyUserTypeDef,
     ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
     ListGroupPoliciesRequestRequestTypeDef,
-    ListGroupPoliciesResponseOutputTypeDef,
+    ListGroupPoliciesResponseTypeDef,
     ListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
     ListGroupsForUserRequestRequestTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
     ListInstanceProfileTagsRequestRequestTypeDef,
     ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
     ListInstanceProfilesForRoleRequestRequestTypeDef,
     ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListInstanceProfilesRequestRequestTypeDef,
     ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
     ListMFADeviceTagsRequestRequestTypeDef,
     ListMFADevicesRequestListMFADevicesPaginateTypeDef,
     ListMFADevicesRequestRequestTypeDef,
-    MFADeviceOutputTypeDef,
+    MFADeviceTypeDef,
     ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
     ListOpenIDConnectProviderTagsRequestRequestTypeDef,
-    OpenIDConnectProviderListEntryOutputTypeDef,
-    PolicyGrantingServiceAccessOutputTypeDef,
+    OpenIDConnectProviderListEntryTypeDef,
+    PolicyGrantingServiceAccessTypeDef,
     ListPoliciesGrantingServiceAccessRequestRequestTypeDef,
     ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
     ListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
     ListPolicyTagsRequestRequestTypeDef,
     ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
     ListPolicyVersionsRequestRequestTypeDef,
     ListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
     ListRolePoliciesRequestRequestTypeDef,
-    ListRolePoliciesResponseOutputTypeDef,
+    ListRolePoliciesResponseTypeDef,
     ListRoleTagsRequestListRoleTagsPaginateTypeDef,
     ListRoleTagsRequestRequestTypeDef,
     ListRolesRequestListRolesPaginateTypeDef,
     ListRolesRequestRequestTypeDef,
     ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
     ListSAMLProviderTagsRequestRequestTypeDef,
-    SAMLProviderListEntryOutputTypeDef,
+    SAMLProviderListEntryTypeDef,
     ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef,
     ListSSHPublicKeysRequestRequestTypeDef,
-    SSHPublicKeyMetadataOutputTypeDef,
+    SSHPublicKeyMetadataTypeDef,
     ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
     ListServerCertificateTagsRequestRequestTypeDef,
     ListServerCertificatesRequestListServerCertificatesPaginateTypeDef,
     ListServerCertificatesRequestRequestTypeDef,
-    ServerCertificateMetadataOutputTypeDef,
+    ServerCertificateMetadataTypeDef,
     ListServiceSpecificCredentialsRequestRequestTypeDef,
-    ServiceSpecificCredentialMetadataOutputTypeDef,
+    ServiceSpecificCredentialMetadataTypeDef,
     ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef,
     ListSigningCertificatesRequestRequestTypeDef,
-    SigningCertificateOutputTypeDef,
+    SigningCertificateTypeDef,
     ListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
     ListUserPoliciesRequestRequestTypeDef,
-    ListUserPoliciesResponseOutputTypeDef,
+    ListUserPoliciesResponseTypeDef,
     ListUserTagsRequestListUserTagsPaginateTypeDef,
     ListUserTagsRequestRequestTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef,
     ListVirtualMFADevicesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    PositionOutputTypeDef,
+    PositionTypeDef,
     PutGroupPolicyRequestGroupCreatePolicyTypeDef,
     PutGroupPolicyRequestGroupPolicyPutTypeDef,
     PutGroupPolicyRequestRequestTypeDef,
     PutRolePermissionsBoundaryRequestRequestTypeDef,
     PutRolePolicyRequestRequestTypeDef,
     PutRolePolicyRequestRolePolicyPutTypeDef,
     PutUserPermissionsBoundaryRequestRequestTypeDef,
@@ -833,18 +833,18 @@
     RemoveUserFromGroupRequestGroupRemoveUserTypeDef,
     RemoveUserFromGroupRequestRequestTypeDef,
     RemoveUserFromGroupRequestUserRemoveGroupTypeDef,
     ResetServiceSpecificCredentialRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ResyncMFADeviceRequestMfaDeviceResyncTypeDef,
     ResyncMFADeviceRequestRequestTypeDef,
-    RoleLastUsedOutputTypeDef,
+    RoleLastUsedTypeDef,
     RoleLastUsedResponseMetadataTypeDef,
     ServerCertificateMetadataResponseMetadataTypeDef,
-    TrackedActionLastAccessedOutputTypeDef,
+    TrackedActionLastAccessedTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetSecurityTokenServicePreferencesRequestRequestTypeDef,
     UntagInstanceProfileRequestRequestTypeDef,
     UntagMFADeviceRequestRequestTypeDef,
     UntagOpenIDConnectProviderRequestRequestTypeDef,
     UntagPolicyRequestRequestTypeDef,
     UntagRoleRequestRequestTypeDef,
@@ -866,40 +866,40 @@
     UpdateLoginProfileRequestLoginProfileUpdateTypeDef,
     UpdateLoginProfileRequestRequestTypeDef,
     UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef,
     UpdateRoleDescriptionRequestRequestTypeDef,
     UpdateRoleRequestRequestTypeDef,
     UpdateSAMLProviderRequestRequestTypeDef,
     UpdateSAMLProviderRequestSamlProviderUpdateTypeDef,
-    UpdateSAMLProviderResponseOutputTypeDef,
+    UpdateSAMLProviderResponseTypeDef,
     UpdateSSHPublicKeyRequestRequestTypeDef,
     UpdateServerCertificateRequestRequestTypeDef,
     UpdateServerCertificateRequestServerCertificateUpdateTypeDef,
     UpdateServiceSpecificCredentialRequestRequestTypeDef,
     UpdateSigningCertificateRequestRequestTypeDef,
     UpdateSigningCertificateRequestSigningCertificateActivateTypeDef,
     UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef,
     UpdateUserRequestRequestTypeDef,
     UpdateUserRequestUserUpdateTypeDef,
     UploadSSHPublicKeyRequestRequestTypeDef,
     UploadSigningCertificateRequestRequestTypeDef,
     UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
-    GetAccessKeyLastUsedResponseOutputTypeDef,
-    ListAccessKeysResponseOutputTypeDef,
-    CreateAccessKeyResponseOutputTypeDef,
-    ListAttachedGroupPoliciesResponseOutputTypeDef,
-    ListAttachedRolePoliciesResponseOutputTypeDef,
-    ListAttachedUserPoliciesResponseOutputTypeDef,
+    GetAccessKeyLastUsedResponseTypeDef,
+    ListAccessKeysResponseTypeDef,
+    CreateAccessKeyResponseTypeDef,
+    ListAttachedGroupPoliciesResponseTypeDef,
+    ListAttachedRolePoliciesResponseTypeDef,
+    ListAttachedUserPoliciesResponseTypeDef,
     SimulateCustomPolicyRequestRequestTypeDef,
     SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
     SimulatePrincipalPolicyRequestRequestTypeDef,
     SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
-    CreateGroupResponseOutputTypeDef,
-    ListGroupsForUserResponseOutputTypeDef,
-    ListGroupsResponseOutputTypeDef,
+    CreateGroupResponseTypeDef,
+    ListGroupsForUserResponseTypeDef,
+    ListGroupsResponseTypeDef,
     CreateInstanceProfileRequestRequestTypeDef,
     CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef,
     CreateOpenIDConnectProviderRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreatePolicyRequestServiceResourceCreatePolicyTypeDef,
     CreateRoleRequestRequestTypeDef,
     CreateRoleRequestServiceResourceCreateRoleTypeDef,
@@ -916,98 +916,98 @@
     TagPolicyRequestRequestTypeDef,
     TagRoleRequestRequestTypeDef,
     TagSAMLProviderRequestRequestTypeDef,
     TagServerCertificateRequestRequestTypeDef,
     TagUserRequestRequestTypeDef,
     UploadServerCertificateRequestRequestTypeDef,
     UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
-    CreateLoginProfileResponseOutputTypeDef,
-    GetLoginProfileResponseOutputTypeDef,
-    CreateOpenIDConnectProviderResponseOutputTypeDef,
-    CreateSAMLProviderResponseOutputTypeDef,
-    GetOpenIDConnectProviderResponseOutputTypeDef,
-    GetSAMLProviderResponseOutputTypeDef,
-    ListInstanceProfileTagsResponseOutputTypeDef,
-    ListMFADeviceTagsResponseOutputTypeDef,
-    ListOpenIDConnectProviderTagsResponseOutputTypeDef,
-    ListPolicyTagsResponseOutputTypeDef,
-    ListRoleTagsResponseOutputTypeDef,
-    ListSAMLProviderTagsResponseOutputTypeDef,
-    ListServerCertificateTagsResponseOutputTypeDef,
-    ListUserTagsResponseOutputTypeDef,
-    PolicyOutputTypeDef,
-    UserOutputTypeDef,
+    CreateLoginProfileResponseTypeDef,
+    GetLoginProfileResponseTypeDef,
+    CreateOpenIDConnectProviderResponseTypeDef,
+    CreateSAMLProviderResponseTypeDef,
+    GetOpenIDConnectProviderResponseTypeDef,
+    GetSAMLProviderResponseTypeDef,
+    ListInstanceProfileTagsResponseTypeDef,
+    ListMFADeviceTagsResponseTypeDef,
+    ListOpenIDConnectProviderTagsResponseTypeDef,
+    ListPolicyTagsResponseTypeDef,
+    ListRoleTagsResponseTypeDef,
+    ListSAMLProviderTagsResponseTypeDef,
+    ListServerCertificateTagsResponseTypeDef,
+    ListUserTagsResponseTypeDef,
+    PolicyTypeDef,
     UserResponseMetadataTypeDef,
-    CreatePolicyVersionResponseOutputTypeDef,
-    GetPolicyVersionResponseOutputTypeDef,
-    ListPolicyVersionsResponseOutputTypeDef,
-    ManagedPolicyDetailOutputTypeDef,
-    CreateServiceSpecificCredentialResponseOutputTypeDef,
-    ResetServiceSpecificCredentialResponseOutputTypeDef,
-    DeletionTaskFailureReasonTypeOutputTypeDef,
-    EntityDetailsOutputTypeDef,
-    GetOrganizationsAccessReportResponseOutputTypeDef,
-    GetAccountPasswordPolicyResponseOutputTypeDef,
+    UserTypeDef,
+    CreatePolicyVersionResponseTypeDef,
+    GetPolicyVersionResponseTypeDef,
+    ListPolicyVersionsResponseTypeDef,
+    ManagedPolicyDetailTypeDef,
+    CreateServiceSpecificCredentialResponseTypeDef,
+    ResetServiceSpecificCredentialResponseTypeDef,
+    DeletionTaskFailureReasonTypeTypeDef,
+    EntityDetailsTypeDef,
+    GetOrganizationsAccessReportResponseTypeDef,
+    GetAccountPasswordPolicyResponseTypeDef,
     GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef,
     GetPolicyRequestPolicyExistsWaitTypeDef,
     GetRoleRequestRoleExistsWaitTypeDef,
     GetUserRequestUserExistsWaitTypeDef,
-    GetSSHPublicKeyResponseOutputTypeDef,
-    UploadSSHPublicKeyResponseOutputTypeDef,
-    GroupDetailOutputTypeDef,
-    UserDetailOutputTypeDef,
-    ListEntitiesForPolicyResponseOutputTypeDef,
-    ListMFADevicesResponseOutputTypeDef,
-    ListOpenIDConnectProvidersResponseOutputTypeDef,
-    ListPoliciesGrantingServiceAccessEntryOutputTypeDef,
-    ListSAMLProvidersResponseOutputTypeDef,
-    ListSSHPublicKeysResponseOutputTypeDef,
-    ListServerCertificatesResponseOutputTypeDef,
-    ServerCertificateOutputTypeDef,
-    UploadServerCertificateResponseOutputTypeDef,
-    ListServiceSpecificCredentialsResponseOutputTypeDef,
-    ListSigningCertificatesResponseOutputTypeDef,
-    UploadSigningCertificateResponseOutputTypeDef,
-    StatementOutputTypeDef,
-    RoleOutputTypeDef,
-    ServiceLastAccessedOutputTypeDef,
-    CreatePolicyResponseOutputTypeDef,
-    GetPolicyResponseOutputTypeDef,
-    ListPoliciesResponseOutputTypeDef,
-    CreateUserResponseOutputTypeDef,
-    GetGroupResponseOutputTypeDef,
-    GetUserResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
-    VirtualMFADeviceOutputTypeDef,
-    GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef,
-    GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef,
-    ListPoliciesGrantingServiceAccessResponseOutputTypeDef,
-    GetServerCertificateResponseOutputTypeDef,
-    ResourceSpecificResultOutputTypeDef,
-    CreateRoleResponseOutputTypeDef,
-    CreateServiceLinkedRoleResponseOutputTypeDef,
-    GetRoleResponseOutputTypeDef,
-    InstanceProfileOutputTypeDef,
-    ListRolesResponseOutputTypeDef,
-    UpdateRoleDescriptionResponseOutputTypeDef,
-    GetServiceLastAccessedDetailsResponseOutputTypeDef,
-    CreateVirtualMFADeviceResponseOutputTypeDef,
-    ListVirtualMFADevicesResponseOutputTypeDef,
-    EvaluationResultOutputTypeDef,
-    CreateInstanceProfileResponseOutputTypeDef,
-    GetInstanceProfileResponseOutputTypeDef,
-    ListInstanceProfilesForRoleResponseOutputTypeDef,
-    ListInstanceProfilesResponseOutputTypeDef,
-    RoleDetailOutputTypeDef,
-    SimulatePolicyResponseOutputTypeDef,
-    GetAccountAuthorizationDetailsResponseOutputTypeDef,
+    GetSSHPublicKeyResponseTypeDef,
+    UploadSSHPublicKeyResponseTypeDef,
+    GroupDetailTypeDef,
+    UserDetailTypeDef,
+    ListEntitiesForPolicyResponseTypeDef,
+    ListMFADevicesResponseTypeDef,
+    ListOpenIDConnectProvidersResponseTypeDef,
+    ListPoliciesGrantingServiceAccessEntryTypeDef,
+    ListSAMLProvidersResponseTypeDef,
+    ListSSHPublicKeysResponseTypeDef,
+    ListServerCertificatesResponseTypeDef,
+    ServerCertificateTypeDef,
+    UploadServerCertificateResponseTypeDef,
+    ListServiceSpecificCredentialsResponseTypeDef,
+    ListSigningCertificatesResponseTypeDef,
+    UploadSigningCertificateResponseTypeDef,
+    StatementTypeDef,
+    RoleTypeDef,
+    ServiceLastAccessedTypeDef,
+    CreatePolicyResponseTypeDef,
+    GetPolicyResponseTypeDef,
+    ListPoliciesResponseTypeDef,
+    CreateUserResponseTypeDef,
+    GetGroupResponseTypeDef,
+    GetUserResponseTypeDef,
+    ListUsersResponseTypeDef,
+    VirtualMFADeviceTypeDef,
+    GetServiceLinkedRoleDeletionStatusResponseTypeDef,
+    GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef,
+    ListPoliciesGrantingServiceAccessResponseTypeDef,
+    GetServerCertificateResponseTypeDef,
+    ResourceSpecificResultTypeDef,
+    CreateRoleResponseTypeDef,
+    CreateServiceLinkedRoleResponseTypeDef,
+    GetRoleResponseTypeDef,
+    InstanceProfileTypeDef,
+    ListRolesResponseTypeDef,
+    UpdateRoleDescriptionResponseTypeDef,
+    GetServiceLastAccessedDetailsResponseTypeDef,
+    CreateVirtualMFADeviceResponseTypeDef,
+    ListVirtualMFADevicesResponseTypeDef,
+    EvaluationResultTypeDef,
+    CreateInstanceProfileResponseTypeDef,
+    GetInstanceProfileResponseTypeDef,
+    ListInstanceProfilesForRoleResponseTypeDef,
+    ListInstanceProfilesResponseTypeDef,
+    RoleDetailTypeDef,
+    SimulatePolicyResponseTypeDef,
+    GetAccountAuthorizationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> AccessDetailOutputTypeDef:
+def get_structure() -> AccessDetailTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/__init__.py` & `mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/__init__.pyi` & `mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/__main__.py` & `mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IAM 1.28.3\nVersion:         1.28.3.post1\nBuilder version:"
-        " 7.14.7\nDocs:           "
+        "Type annotations for boto3.IAM 1.28.3\nVersion:         1.28.3.post2\nBuilder version:"
+        " 7.15.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.3.post1")
+    print("1.28.3.post2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/client.py` & `mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,99 +63,99 @@
     ListUserTagsPaginator,
     ListVirtualMFADevicesPaginator,
     SimulateCustomPolicyPaginator,
     SimulatePrincipalPolicyPaginator,
 )
 from .type_defs import (
     ContextEntryTypeDef,
-    CreateAccessKeyResponseOutputTypeDef,
-    CreateGroupResponseOutputTypeDef,
-    CreateInstanceProfileResponseOutputTypeDef,
-    CreateLoginProfileResponseOutputTypeDef,
-    CreateOpenIDConnectProviderResponseOutputTypeDef,
-    CreatePolicyResponseOutputTypeDef,
-    CreatePolicyVersionResponseOutputTypeDef,
-    CreateRoleResponseOutputTypeDef,
-    CreateSAMLProviderResponseOutputTypeDef,
-    CreateServiceLinkedRoleResponseOutputTypeDef,
-    CreateServiceSpecificCredentialResponseOutputTypeDef,
-    CreateUserResponseOutputTypeDef,
-    CreateVirtualMFADeviceResponseOutputTypeDef,
-    DeleteServiceLinkedRoleResponseOutputTypeDef,
+    CreateAccessKeyResponseTypeDef,
+    CreateGroupResponseTypeDef,
+    CreateInstanceProfileResponseTypeDef,
+    CreateLoginProfileResponseTypeDef,
+    CreateOpenIDConnectProviderResponseTypeDef,
+    CreatePolicyResponseTypeDef,
+    CreatePolicyVersionResponseTypeDef,
+    CreateRoleResponseTypeDef,
+    CreateSAMLProviderResponseTypeDef,
+    CreateServiceLinkedRoleResponseTypeDef,
+    CreateServiceSpecificCredentialResponseTypeDef,
+    CreateUserResponseTypeDef,
+    CreateVirtualMFADeviceResponseTypeDef,
+    DeleteServiceLinkedRoleResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    GenerateCredentialReportResponseOutputTypeDef,
-    GenerateOrganizationsAccessReportResponseOutputTypeDef,
-    GenerateServiceLastAccessedDetailsResponseOutputTypeDef,
-    GetAccessKeyLastUsedResponseOutputTypeDef,
-    GetAccountAuthorizationDetailsResponseOutputTypeDef,
-    GetAccountPasswordPolicyResponseOutputTypeDef,
-    GetAccountSummaryResponseOutputTypeDef,
-    GetContextKeysForPolicyResponseOutputTypeDef,
-    GetCredentialReportResponseOutputTypeDef,
-    GetGroupPolicyResponseOutputTypeDef,
-    GetGroupResponseOutputTypeDef,
-    GetInstanceProfileResponseOutputTypeDef,
-    GetLoginProfileResponseOutputTypeDef,
-    GetMFADeviceResponseOutputTypeDef,
-    GetOpenIDConnectProviderResponseOutputTypeDef,
-    GetOrganizationsAccessReportResponseOutputTypeDef,
-    GetPolicyResponseOutputTypeDef,
-    GetPolicyVersionResponseOutputTypeDef,
-    GetRolePolicyResponseOutputTypeDef,
-    GetRoleResponseOutputTypeDef,
-    GetSAMLProviderResponseOutputTypeDef,
-    GetServerCertificateResponseOutputTypeDef,
-    GetServiceLastAccessedDetailsResponseOutputTypeDef,
-    GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef,
-    GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef,
-    GetSSHPublicKeyResponseOutputTypeDef,
-    GetUserPolicyResponseOutputTypeDef,
-    GetUserResponseOutputTypeDef,
-    ListAccessKeysResponseOutputTypeDef,
-    ListAccountAliasesResponseOutputTypeDef,
-    ListAttachedGroupPoliciesResponseOutputTypeDef,
-    ListAttachedRolePoliciesResponseOutputTypeDef,
-    ListAttachedUserPoliciesResponseOutputTypeDef,
-    ListEntitiesForPolicyResponseOutputTypeDef,
-    ListGroupPoliciesResponseOutputTypeDef,
-    ListGroupsForUserResponseOutputTypeDef,
-    ListGroupsResponseOutputTypeDef,
-    ListInstanceProfilesForRoleResponseOutputTypeDef,
-    ListInstanceProfilesResponseOutputTypeDef,
-    ListInstanceProfileTagsResponseOutputTypeDef,
-    ListMFADevicesResponseOutputTypeDef,
-    ListMFADeviceTagsResponseOutputTypeDef,
-    ListOpenIDConnectProvidersResponseOutputTypeDef,
-    ListOpenIDConnectProviderTagsResponseOutputTypeDef,
-    ListPoliciesGrantingServiceAccessResponseOutputTypeDef,
-    ListPoliciesResponseOutputTypeDef,
-    ListPolicyTagsResponseOutputTypeDef,
-    ListPolicyVersionsResponseOutputTypeDef,
-    ListRolePoliciesResponseOutputTypeDef,
-    ListRolesResponseOutputTypeDef,
-    ListRoleTagsResponseOutputTypeDef,
-    ListSAMLProvidersResponseOutputTypeDef,
-    ListSAMLProviderTagsResponseOutputTypeDef,
-    ListServerCertificatesResponseOutputTypeDef,
-    ListServerCertificateTagsResponseOutputTypeDef,
-    ListServiceSpecificCredentialsResponseOutputTypeDef,
-    ListSigningCertificatesResponseOutputTypeDef,
-    ListSSHPublicKeysResponseOutputTypeDef,
-    ListUserPoliciesResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
-    ListUserTagsResponseOutputTypeDef,
-    ListVirtualMFADevicesResponseOutputTypeDef,
-    ResetServiceSpecificCredentialResponseOutputTypeDef,
-    SimulatePolicyResponseOutputTypeDef,
+    GenerateCredentialReportResponseTypeDef,
+    GenerateOrganizationsAccessReportResponseTypeDef,
+    GenerateServiceLastAccessedDetailsResponseTypeDef,
+    GetAccessKeyLastUsedResponseTypeDef,
+    GetAccountAuthorizationDetailsResponseTypeDef,
+    GetAccountPasswordPolicyResponseTypeDef,
+    GetAccountSummaryResponseTypeDef,
+    GetContextKeysForPolicyResponseTypeDef,
+    GetCredentialReportResponseTypeDef,
+    GetGroupPolicyResponseTypeDef,
+    GetGroupResponseTypeDef,
+    GetInstanceProfileResponseTypeDef,
+    GetLoginProfileResponseTypeDef,
+    GetMFADeviceResponseTypeDef,
+    GetOpenIDConnectProviderResponseTypeDef,
+    GetOrganizationsAccessReportResponseTypeDef,
+    GetPolicyResponseTypeDef,
+    GetPolicyVersionResponseTypeDef,
+    GetRolePolicyResponseTypeDef,
+    GetRoleResponseTypeDef,
+    GetSAMLProviderResponseTypeDef,
+    GetServerCertificateResponseTypeDef,
+    GetServiceLastAccessedDetailsResponseTypeDef,
+    GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef,
+    GetServiceLinkedRoleDeletionStatusResponseTypeDef,
+    GetSSHPublicKeyResponseTypeDef,
+    GetUserPolicyResponseTypeDef,
+    GetUserResponseTypeDef,
+    ListAccessKeysResponseTypeDef,
+    ListAccountAliasesResponseTypeDef,
+    ListAttachedGroupPoliciesResponseTypeDef,
+    ListAttachedRolePoliciesResponseTypeDef,
+    ListAttachedUserPoliciesResponseTypeDef,
+    ListEntitiesForPolicyResponseTypeDef,
+    ListGroupPoliciesResponseTypeDef,
+    ListGroupsForUserResponseTypeDef,
+    ListGroupsResponseTypeDef,
+    ListInstanceProfilesForRoleResponseTypeDef,
+    ListInstanceProfilesResponseTypeDef,
+    ListInstanceProfileTagsResponseTypeDef,
+    ListMFADevicesResponseTypeDef,
+    ListMFADeviceTagsResponseTypeDef,
+    ListOpenIDConnectProvidersResponseTypeDef,
+    ListOpenIDConnectProviderTagsResponseTypeDef,
+    ListPoliciesGrantingServiceAccessResponseTypeDef,
+    ListPoliciesResponseTypeDef,
+    ListPolicyTagsResponseTypeDef,
+    ListPolicyVersionsResponseTypeDef,
+    ListRolePoliciesResponseTypeDef,
+    ListRolesResponseTypeDef,
+    ListRoleTagsResponseTypeDef,
+    ListSAMLProvidersResponseTypeDef,
+    ListSAMLProviderTagsResponseTypeDef,
+    ListServerCertificatesResponseTypeDef,
+    ListServerCertificateTagsResponseTypeDef,
+    ListServiceSpecificCredentialsResponseTypeDef,
+    ListSigningCertificatesResponseTypeDef,
+    ListSSHPublicKeysResponseTypeDef,
+    ListUserPoliciesResponseTypeDef,
+    ListUsersResponseTypeDef,
+    ListUserTagsResponseTypeDef,
+    ListVirtualMFADevicesResponseTypeDef,
+    ResetServiceSpecificCredentialResponseTypeDef,
+    SimulatePolicyResponseTypeDef,
     TagTypeDef,
-    UpdateRoleDescriptionResponseOutputTypeDef,
-    UpdateSAMLProviderResponseOutputTypeDef,
-    UploadServerCertificateResponseOutputTypeDef,
-    UploadSigningCertificateResponseOutputTypeDef,
-    UploadSSHPublicKeyResponseOutputTypeDef,
+    UpdateRoleDescriptionResponseTypeDef,
+    UpdateSAMLProviderResponseTypeDef,
+    UploadServerCertificateResponseTypeDef,
+    UploadSigningCertificateResponseTypeDef,
+    UploadSSHPublicKeyResponseTypeDef,
 )
 from .waiter import (
     InstanceProfileExistsWaiter,
     PolicyExistsWaiter,
     RoleExistsWaiter,
     UserExistsWaiter,
 )
@@ -302,15 +302,15 @@
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#close)
         """
 
-    def create_access_key(self, *, UserName: str = ...) -> CreateAccessKeyResponseOutputTypeDef:
+    def create_access_key(self, *, UserName: str = ...) -> CreateAccessKeyResponseTypeDef:
         """
         Creates a new Amazon Web Services secret access key and corresponding Amazon Web
         Services access key ID for the specified user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_access_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_access_key)
         """
@@ -319,50 +319,50 @@
         """
         Creates an alias for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_account_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_account_alias)
         """
 
-    def create_group(self, *, GroupName: str, Path: str = ...) -> CreateGroupResponseOutputTypeDef:
+    def create_group(self, *, GroupName: str, Path: str = ...) -> CreateGroupResponseTypeDef:
         """
         Creates a new group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_group)
         """
 
     def create_instance_profile(
         self, *, InstanceProfileName: str, Path: str = ..., Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateInstanceProfileResponseOutputTypeDef:
+    ) -> CreateInstanceProfileResponseTypeDef:
         """
         Creates a new instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_instance_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_instance_profile)
         """
 
     def create_login_profile(
         self, *, UserName: str, Password: str, PasswordResetRequired: bool = ...
-    ) -> CreateLoginProfileResponseOutputTypeDef:
+    ) -> CreateLoginProfileResponseTypeDef:
         """
         Creates a password for the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_login_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_login_profile)
         """
 
     def create_open_id_connect_provider(
         self,
         *,
         Url: str,
         ThumbprintList: Sequence[str],
         ClientIDList: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateOpenIDConnectProviderResponseOutputTypeDef:
+    ) -> CreateOpenIDConnectProviderResponseTypeDef:
         """
         Creates an IAM entity to describe an identity provider (IdP) that supports
         `OpenID Connect (OIDC) <http://openid.net/connect/>`__.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_open_id_connect_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_open_id_connect_provider)
         """
@@ -371,25 +371,25 @@
         self,
         *,
         PolicyName: str,
         PolicyDocument: str,
         Path: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreatePolicyResponseOutputTypeDef:
+    ) -> CreatePolicyResponseTypeDef:
         """
         Creates a new managed policy for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_policy)
         """
 
     def create_policy_version(
         self, *, PolicyArn: str, PolicyDocument: str, SetAsDefault: bool = ...
-    ) -> CreatePolicyVersionResponseOutputTypeDef:
+    ) -> CreatePolicyVersionResponseTypeDef:
         """
         Creates a new version of the specified managed policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_policy_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_policy_version)
         """
 
@@ -399,46 +399,46 @@
         RoleName: str,
         AssumeRolePolicyDocument: str,
         Path: str = ...,
         Description: str = ...,
         MaxSessionDuration: int = ...,
         PermissionsBoundary: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateRoleResponseOutputTypeDef:
+    ) -> CreateRoleResponseTypeDef:
         """
         Creates a new role for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_role)
         """
 
     def create_saml_provider(
         self, *, SAMLMetadataDocument: str, Name: str, Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateSAMLProviderResponseOutputTypeDef:
+    ) -> CreateSAMLProviderResponseTypeDef:
         """
         Creates an IAM resource that describes an identity provider (IdP) that supports
         SAML 2.0.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_saml_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_saml_provider)
         """
 
     def create_service_linked_role(
         self, *, AWSServiceName: str, Description: str = ..., CustomSuffix: str = ...
-    ) -> CreateServiceLinkedRoleResponseOutputTypeDef:
+    ) -> CreateServiceLinkedRoleResponseTypeDef:
         """
         Creates an IAM role that is linked to a specific Amazon Web Services service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_service_linked_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_service_linked_role)
         """
 
     def create_service_specific_credential(
         self, *, UserName: str, ServiceName: str
-    ) -> CreateServiceSpecificCredentialResponseOutputTypeDef:
+    ) -> CreateServiceSpecificCredentialResponseTypeDef:
         """
         Generates a set of credentials consisting of a user name and password that can
         be used to access the service specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_service_specific_credential)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_service_specific_credential)
         """
@@ -446,25 +446,25 @@
     def create_user(
         self,
         *,
         UserName: str,
         Path: str = ...,
         PermissionsBoundary: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateUserResponseOutputTypeDef:
+    ) -> CreateUserResponseTypeDef:
         """
         Creates a new IAM user for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_user)
         """
 
     def create_virtual_mfa_device(
         self, *, VirtualMFADeviceName: str, Path: str = ..., Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateVirtualMFADeviceResponseOutputTypeDef:
+    ) -> CreateVirtualMFADeviceResponseTypeDef:
         """
         Creates a new virtual MFA device for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_virtual_mfa_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_virtual_mfa_device)
         """
 
@@ -610,15 +610,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.delete_server_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#delete_server_certificate)
         """
 
     def delete_service_linked_role(
         self, *, RoleName: str
-    ) -> DeleteServiceLinkedRoleResponseOutputTypeDef:
+    ) -> DeleteServiceLinkedRoleResponseTypeDef:
         """
         Submits a service-linked role deletion request and returns a `DeletionTaskId`,
         which you can use to check the status of the deletion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.delete_service_linked_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#delete_service_linked_role)
         """
@@ -722,25 +722,25 @@
         """
         Enables the specified MFA device and associates it with the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.enable_mfa_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#enable_mfa_device)
         """
 
-    def generate_credential_report(self) -> GenerateCredentialReportResponseOutputTypeDef:
+    def generate_credential_report(self) -> GenerateCredentialReportResponseTypeDef:
         """
         Generates a credential report for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.generate_credential_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#generate_credential_report)
         """
 
     def generate_organizations_access_report(
         self, *, EntityPath: str, OrganizationsPolicyId: str = ...
-    ) -> GenerateOrganizationsAccessReportResponseOutputTypeDef:
+    ) -> GenerateOrganizationsAccessReportResponseTypeDef:
         """
         Generates a report for service last accessed data for Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.generate_organizations_access_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#generate_organizations_access_report)
         """
 
@@ -756,331 +756,323 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#generate_presigned_url)
         """
 
     def generate_service_last_accessed_details(
         self, *, Arn: str, Granularity: AccessAdvisorUsageGranularityTypeType = ...
-    ) -> GenerateServiceLastAccessedDetailsResponseOutputTypeDef:
+    ) -> GenerateServiceLastAccessedDetailsResponseTypeDef:
         """
         Generates a report that includes details about when an IAM resource (user,
         group, role, or policy) was last used in an attempt to access Amazon Web
         Services services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.generate_service_last_accessed_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#generate_service_last_accessed_details)
         """
 
-    def get_access_key_last_used(
-        self, *, AccessKeyId: str
-    ) -> GetAccessKeyLastUsedResponseOutputTypeDef:
+    def get_access_key_last_used(self, *, AccessKeyId: str) -> GetAccessKeyLastUsedResponseTypeDef:
         """
         Retrieves information about when the specified access key was last used.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_access_key_last_used)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_access_key_last_used)
         """
 
     def get_account_authorization_details(
         self, *, Filter: Sequence[EntityTypeType] = ..., MaxItems: int = ..., Marker: str = ...
-    ) -> GetAccountAuthorizationDetailsResponseOutputTypeDef:
+    ) -> GetAccountAuthorizationDetailsResponseTypeDef:
         """
         Retrieves information about all IAM users, groups, roles, and policies in your
         Amazon Web Services account, including their relationships to one another.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_account_authorization_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_account_authorization_details)
         """
 
-    def get_account_password_policy(self) -> GetAccountPasswordPolicyResponseOutputTypeDef:
+    def get_account_password_policy(self) -> GetAccountPasswordPolicyResponseTypeDef:
         """
         Retrieves the password policy for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_account_password_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_account_password_policy)
         """
 
-    def get_account_summary(self) -> GetAccountSummaryResponseOutputTypeDef:
+    def get_account_summary(self) -> GetAccountSummaryResponseTypeDef:
         """
         Retrieves information about IAM entity usage and IAM quotas in the Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_account_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_account_summary)
         """
 
     def get_context_keys_for_custom_policy(
         self, *, PolicyInputList: Sequence[str]
-    ) -> GetContextKeysForPolicyResponseOutputTypeDef:
+    ) -> GetContextKeysForPolicyResponseTypeDef:
         """
         Gets a list of all of the context keys referenced in the input policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_context_keys_for_custom_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_context_keys_for_custom_policy)
         """
 
     def get_context_keys_for_principal_policy(
         self, *, PolicySourceArn: str, PolicyInputList: Sequence[str] = ...
-    ) -> GetContextKeysForPolicyResponseOutputTypeDef:
+    ) -> GetContextKeysForPolicyResponseTypeDef:
         """
         Gets a list of all of the context keys referenced in all the IAM policies that
         are attached to the specified IAM entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_context_keys_for_principal_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_context_keys_for_principal_policy)
         """
 
-    def get_credential_report(self) -> GetCredentialReportResponseOutputTypeDef:
+    def get_credential_report(self) -> GetCredentialReportResponseTypeDef:
         """
         Retrieves a credential report for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_credential_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_credential_report)
         """
 
     def get_group(
         self, *, GroupName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> GetGroupResponseOutputTypeDef:
+    ) -> GetGroupResponseTypeDef:
         """
         Returns a list of IAM users that are in the specified IAM group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_group)
         """
 
-    def get_group_policy(
-        self, *, GroupName: str, PolicyName: str
-    ) -> GetGroupPolicyResponseOutputTypeDef:
+    def get_group_policy(self, *, GroupName: str, PolicyName: str) -> GetGroupPolicyResponseTypeDef:
         """
         Retrieves the specified inline policy document that is embedded in the specified
         IAM group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_group_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_group_policy)
         """
 
     def get_instance_profile(
         self, *, InstanceProfileName: str
-    ) -> GetInstanceProfileResponseOutputTypeDef:
+    ) -> GetInstanceProfileResponseTypeDef:
         """
         Retrieves information about the specified instance profile, including the
         instance profile's path, GUID, ARN, and role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_instance_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_instance_profile)
         """
 
-    def get_login_profile(self, *, UserName: str) -> GetLoginProfileResponseOutputTypeDef:
+    def get_login_profile(self, *, UserName: str) -> GetLoginProfileResponseTypeDef:
         """
         Retrieves the user name for the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_login_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_login_profile)
         """
 
     def get_mfa_device(
         self, *, SerialNumber: str, UserName: str = ...
-    ) -> GetMFADeviceResponseOutputTypeDef:
+    ) -> GetMFADeviceResponseTypeDef:
         """
         Retrieves information about an MFA device for a specified user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_mfa_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_mfa_device)
         """
 
     def get_open_id_connect_provider(
         self, *, OpenIDConnectProviderArn: str
-    ) -> GetOpenIDConnectProviderResponseOutputTypeDef:
+    ) -> GetOpenIDConnectProviderResponseTypeDef:
         """
         Returns information about the specified OpenID Connect (OIDC) provider resource
         object in IAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_open_id_connect_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_open_id_connect_provider)
         """
 
     def get_organizations_access_report(
         self, *, JobId: str, MaxItems: int = ..., Marker: str = ..., SortKey: sortKeyTypeType = ...
-    ) -> GetOrganizationsAccessReportResponseOutputTypeDef:
+    ) -> GetOrganizationsAccessReportResponseTypeDef:
         """
         Retrieves the service last accessed data report for Organizations that was
         previously generated using the `GenerateOrganizationsAccessReport` operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_organizations_access_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_organizations_access_report)
         """
 
-    def get_policy(self, *, PolicyArn: str) -> GetPolicyResponseOutputTypeDef:
+    def get_policy(self, *, PolicyArn: str) -> GetPolicyResponseTypeDef:
         """
         Retrieves information about the specified managed policy, including the policy's
         default version and the total number of IAM users, groups, and roles to which
         the policy is attached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_policy)
         """
 
     def get_policy_version(
         self, *, PolicyArn: str, VersionId: str
-    ) -> GetPolicyVersionResponseOutputTypeDef:
+    ) -> GetPolicyVersionResponseTypeDef:
         """
         Retrieves information about the specified version of the specified managed
         policy, including the policy document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_policy_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_policy_version)
         """
 
-    def get_role(self, *, RoleName: str) -> GetRoleResponseOutputTypeDef:
+    def get_role(self, *, RoleName: str) -> GetRoleResponseTypeDef:
         """
         Retrieves information about the specified role, including the role's path, GUID,
         ARN, and the role's trust policy that grants permission to assume the role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_role)
         """
 
-    def get_role_policy(
-        self, *, RoleName: str, PolicyName: str
-    ) -> GetRolePolicyResponseOutputTypeDef:
+    def get_role_policy(self, *, RoleName: str, PolicyName: str) -> GetRolePolicyResponseTypeDef:
         """
         Retrieves the specified inline policy document that is embedded with the
         specified IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_role_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_role_policy)
         """
 
-    def get_saml_provider(self, *, SAMLProviderArn: str) -> GetSAMLProviderResponseOutputTypeDef:
+    def get_saml_provider(self, *, SAMLProviderArn: str) -> GetSAMLProviderResponseTypeDef:
         """
         Returns the SAML provider metadocument that was uploaded when the IAM SAML
         provider resource object was created or updated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_saml_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_saml_provider)
         """
 
     def get_server_certificate(
         self, *, ServerCertificateName: str
-    ) -> GetServerCertificateResponseOutputTypeDef:
+    ) -> GetServerCertificateResponseTypeDef:
         """
         Retrieves information about the specified server certificate stored in IAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_server_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_server_certificate)
         """
 
     def get_service_last_accessed_details(
         self, *, JobId: str, MaxItems: int = ..., Marker: str = ...
-    ) -> GetServiceLastAccessedDetailsResponseOutputTypeDef:
+    ) -> GetServiceLastAccessedDetailsResponseTypeDef:
         """
         Retrieves a service last accessed report that was created using the
         `GenerateServiceLastAccessedDetails` operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_service_last_accessed_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_service_last_accessed_details)
         """
 
     def get_service_last_accessed_details_with_entities(
         self, *, JobId: str, ServiceNamespace: str, MaxItems: int = ..., Marker: str = ...
-    ) -> GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef:
+    ) -> GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef:
         """
         After you generate a group or policy report using the
         `GenerateServiceLastAccessedDetails` operation, you can use the `JobId`
         parameter in `GetServiceLastAccessedDetailsWithEntities`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_service_last_accessed_details_with_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_service_last_accessed_details_with_entities)
         """
 
     def get_service_linked_role_deletion_status(
         self, *, DeletionTaskId: str
-    ) -> GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef:
+    ) -> GetServiceLinkedRoleDeletionStatusResponseTypeDef:
         """
         Retrieves the status of your service-linked role deletion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_service_linked_role_deletion_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_service_linked_role_deletion_status)
         """
 
     def get_ssh_public_key(
         self, *, UserName: str, SSHPublicKeyId: str, Encoding: encodingTypeType
-    ) -> GetSSHPublicKeyResponseOutputTypeDef:
+    ) -> GetSSHPublicKeyResponseTypeDef:
         """
         Retrieves the specified SSH public key, including metadata about the key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_ssh_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_ssh_public_key)
         """
 
-    def get_user(self, *, UserName: str = ...) -> GetUserResponseOutputTypeDef:
+    def get_user(self, *, UserName: str = ...) -> GetUserResponseTypeDef:
         """
         Retrieves information about the specified IAM user, including the user's
         creation date, path, unique ID, and ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_user)
         """
 
-    def get_user_policy(
-        self, *, UserName: str, PolicyName: str
-    ) -> GetUserPolicyResponseOutputTypeDef:
+    def get_user_policy(self, *, UserName: str, PolicyName: str) -> GetUserPolicyResponseTypeDef:
         """
         Retrieves the specified inline policy document that is embedded in the specified
         IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_user_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_user_policy)
         """
 
     def list_access_keys(
         self, *, UserName: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListAccessKeysResponseOutputTypeDef:
+    ) -> ListAccessKeysResponseTypeDef:
         """
         Returns information about the access key IDs associated with the specified IAM
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_access_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_access_keys)
         """
 
     def list_account_aliases(
         self, *, Marker: str = ..., MaxItems: int = ...
-    ) -> ListAccountAliasesResponseOutputTypeDef:
+    ) -> ListAccountAliasesResponseTypeDef:
         """
         Lists the account alias associated with the Amazon Web Services account (Note:
         you can have only one).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_account_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_account_aliases)
         """
 
     def list_attached_group_policies(
         self, *, GroupName: str, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListAttachedGroupPoliciesResponseOutputTypeDef:
+    ) -> ListAttachedGroupPoliciesResponseTypeDef:
         """
         Lists all managed policies that are attached to the specified IAM group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_attached_group_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_attached_group_policies)
         """
 
     def list_attached_role_policies(
         self, *, RoleName: str, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListAttachedRolePoliciesResponseOutputTypeDef:
+    ) -> ListAttachedRolePoliciesResponseTypeDef:
         """
         Lists all managed policies that are attached to the specified IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_attached_role_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_attached_role_policies)
         """
 
     def list_attached_user_policies(
         self, *, UserName: str, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListAttachedUserPoliciesResponseOutputTypeDef:
+    ) -> ListAttachedUserPoliciesResponseTypeDef:
         """
         Lists all managed policies that are attached to the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_attached_user_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_attached_user_policies)
         """
 
@@ -1089,117 +1081,117 @@
         *,
         PolicyArn: str,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
         MaxItems: int = ...
-    ) -> ListEntitiesForPolicyResponseOutputTypeDef:
+    ) -> ListEntitiesForPolicyResponseTypeDef:
         """
         Lists all IAM users, groups, and roles that the specified managed policy is
         attached to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_entities_for_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_entities_for_policy)
         """
 
     def list_group_policies(
         self, *, GroupName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListGroupPoliciesResponseOutputTypeDef:
+    ) -> ListGroupPoliciesResponseTypeDef:
         """
         Lists the names of the inline policies that are embedded in the specified IAM
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_group_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_group_policies)
         """
 
     def list_groups(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListGroupsResponseOutputTypeDef:
+    ) -> ListGroupsResponseTypeDef:
         """
         Lists the IAM groups that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_groups)
         """
 
     def list_groups_for_user(
         self, *, UserName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListGroupsForUserResponseOutputTypeDef:
+    ) -> ListGroupsForUserResponseTypeDef:
         """
         Lists the IAM groups that the specified IAM user belongs to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_groups_for_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_groups_for_user)
         """
 
     def list_instance_profile_tags(
         self, *, InstanceProfileName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListInstanceProfileTagsResponseOutputTypeDef:
+    ) -> ListInstanceProfileTagsResponseTypeDef:
         """
         Lists the tags that are attached to the specified IAM instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_instance_profile_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_instance_profile_tags)
         """
 
     def list_instance_profiles(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListInstanceProfilesResponseOutputTypeDef:
+    ) -> ListInstanceProfilesResponseTypeDef:
         """
         Lists the instance profiles that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_instance_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_instance_profiles)
         """
 
     def list_instance_profiles_for_role(
         self, *, RoleName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListInstanceProfilesForRoleResponseOutputTypeDef:
+    ) -> ListInstanceProfilesForRoleResponseTypeDef:
         """
         Lists the instance profiles that have the specified associated IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_instance_profiles_for_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_instance_profiles_for_role)
         """
 
     def list_mfa_device_tags(
         self, *, SerialNumber: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListMFADeviceTagsResponseOutputTypeDef:
+    ) -> ListMFADeviceTagsResponseTypeDef:
         """
         Lists the tags that are attached to the specified IAM virtual multi-factor
         authentication (MFA) device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_mfa_device_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_mfa_device_tags)
         """
 
     def list_mfa_devices(
         self, *, UserName: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListMFADevicesResponseOutputTypeDef:
+    ) -> ListMFADevicesResponseTypeDef:
         """
         Lists the MFA devices for an IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_mfa_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_mfa_devices)
         """
 
     def list_open_id_connect_provider_tags(
         self, *, OpenIDConnectProviderArn: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListOpenIDConnectProviderTagsResponseOutputTypeDef:
+    ) -> ListOpenIDConnectProviderTagsResponseTypeDef:
         """
         Lists the tags that are attached to the specified OpenID Connect
         (OIDC)-compatible identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_open_id_connect_provider_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_open_id_connect_provider_tags)
         """
 
-    def list_open_id_connect_providers(self) -> ListOpenIDConnectProvidersResponseOutputTypeDef:
+    def list_open_id_connect_providers(self) -> ListOpenIDConnectProvidersResponseTypeDef:
         """
         Lists information about the IAM OpenID Connect (OIDC) provider resource objects
         defined in the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_open_id_connect_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_open_id_connect_providers)
         """
@@ -1209,196 +1201,196 @@
         *,
         Scope: policyScopeTypeType = ...,
         OnlyAttached: bool = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
         MaxItems: int = ...
-    ) -> ListPoliciesResponseOutputTypeDef:
+    ) -> ListPoliciesResponseTypeDef:
         """
         Lists all the managed policies that are available in your Amazon Web Services
         account, including your own customer-defined managed policies and all Amazon Web
         Services managed policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_policies)
         """
 
     def list_policies_granting_service_access(
         self, *, Arn: str, ServiceNamespaces: Sequence[str], Marker: str = ...
-    ) -> ListPoliciesGrantingServiceAccessResponseOutputTypeDef:
+    ) -> ListPoliciesGrantingServiceAccessResponseTypeDef:
         """
         Retrieves a list of policies that the IAM identity (user, group, or role) can
         use to access each specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_policies_granting_service_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_policies_granting_service_access)
         """
 
     def list_policy_tags(
         self, *, PolicyArn: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListPolicyTagsResponseOutputTypeDef:
+    ) -> ListPolicyTagsResponseTypeDef:
         """
         Lists the tags that are attached to the specified IAM customer managed policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_policy_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_policy_tags)
         """
 
     def list_policy_versions(
         self, *, PolicyArn: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListPolicyVersionsResponseOutputTypeDef:
+    ) -> ListPolicyVersionsResponseTypeDef:
         """
         Lists information about the versions of the specified managed policy, including
         the version that is currently set as the policy's default version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_policy_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_policy_versions)
         """
 
     def list_role_policies(
         self, *, RoleName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListRolePoliciesResponseOutputTypeDef:
+    ) -> ListRolePoliciesResponseTypeDef:
         """
         Lists the names of the inline policies that are embedded in the specified IAM
         role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_role_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_role_policies)
         """
 
     def list_role_tags(
         self, *, RoleName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListRoleTagsResponseOutputTypeDef:
+    ) -> ListRoleTagsResponseTypeDef:
         """
         Lists the tags that are attached to the specified role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_role_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_role_tags)
         """
 
     def list_roles(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListRolesResponseOutputTypeDef:
+    ) -> ListRolesResponseTypeDef:
         """
         Lists the IAM roles that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_roles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_roles)
         """
 
     def list_saml_provider_tags(
         self, *, SAMLProviderArn: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListSAMLProviderTagsResponseOutputTypeDef:
+    ) -> ListSAMLProviderTagsResponseTypeDef:
         """
         Lists the tags that are attached to the specified Security Assertion Markup
         Language (SAML) identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_saml_provider_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_saml_provider_tags)
         """
 
-    def list_saml_providers(self) -> ListSAMLProvidersResponseOutputTypeDef:
+    def list_saml_providers(self) -> ListSAMLProvidersResponseTypeDef:
         """
         Lists the SAML provider resource objects defined in IAM in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_saml_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_saml_providers)
         """
 
     def list_server_certificate_tags(
         self, *, ServerCertificateName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListServerCertificateTagsResponseOutputTypeDef:
+    ) -> ListServerCertificateTagsResponseTypeDef:
         """
         Lists the tags that are attached to the specified IAM server certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_server_certificate_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_server_certificate_tags)
         """
 
     def list_server_certificates(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListServerCertificatesResponseOutputTypeDef:
+    ) -> ListServerCertificatesResponseTypeDef:
         """
         Lists the server certificates stored in IAM that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_server_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_server_certificates)
         """
 
     def list_service_specific_credentials(
         self, *, UserName: str = ..., ServiceName: str = ...
-    ) -> ListServiceSpecificCredentialsResponseOutputTypeDef:
+    ) -> ListServiceSpecificCredentialsResponseTypeDef:
         """
         Returns information about the service-specific credentials associated with the
         specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_service_specific_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_service_specific_credentials)
         """
 
     def list_signing_certificates(
         self, *, UserName: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListSigningCertificatesResponseOutputTypeDef:
+    ) -> ListSigningCertificatesResponseTypeDef:
         """
         Returns information about the signing certificates associated with the specified
         IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_signing_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_signing_certificates)
         """
 
     def list_ssh_public_keys(
         self, *, UserName: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListSSHPublicKeysResponseOutputTypeDef:
+    ) -> ListSSHPublicKeysResponseTypeDef:
         """
         Returns information about the SSH public keys associated with the specified IAM
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_ssh_public_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_ssh_public_keys)
         """
 
     def list_user_policies(
         self, *, UserName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListUserPoliciesResponseOutputTypeDef:
+    ) -> ListUserPoliciesResponseTypeDef:
         """
         Lists the names of the inline policies embedded in the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_user_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_user_policies)
         """
 
     def list_user_tags(
         self, *, UserName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListUserTagsResponseOutputTypeDef:
+    ) -> ListUserTagsResponseTypeDef:
         """
         Lists the tags that are attached to the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_user_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_user_tags)
         """
 
     def list_users(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListUsersResponseOutputTypeDef:
+    ) -> ListUsersResponseTypeDef:
         """
         Lists the IAM users that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_users)
         """
 
     def list_virtual_mfa_devices(
         self,
         *,
         AssignmentStatus: assignmentStatusTypeType = ...,
         Marker: str = ...,
         MaxItems: int = ...
-    ) -> ListVirtualMFADevicesResponseOutputTypeDef:
+    ) -> ListVirtualMFADevicesResponseTypeDef:
         """
         Lists the virtual MFA devices defined in the Amazon Web Services account by
         assignment status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_virtual_mfa_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_virtual_mfa_devices)
         """
@@ -1488,15 +1480,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.remove_user_from_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#remove_user_from_group)
         """
 
     def reset_service_specific_credential(
         self, *, ServiceSpecificCredentialId: str, UserName: str = ...
-    ) -> ResetServiceSpecificCredentialResponseOutputTypeDef:
+    ) -> ResetServiceSpecificCredentialResponseTypeDef:
         """
         Resets the password for a service-specific credential.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.reset_service_specific_credential)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#reset_service_specific_credential)
         """
 
@@ -1548,15 +1540,15 @@
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         MaxItems: int = ...,
         Marker: str = ...
-    ) -> SimulatePolicyResponseOutputTypeDef:
+    ) -> SimulatePolicyResponseTypeDef:
         """
         Simulate how a set of IAM policies and optionally a resource-based policy works
         with a list of API operations and Amazon Web Services resources to determine the
         policies' effective permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.simulate_custom_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#simulate_custom_policy)
@@ -1573,15 +1565,15 @@
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         MaxItems: int = ...,
         Marker: str = ...
-    ) -> SimulatePolicyResponseOutputTypeDef:
+    ) -> SimulatePolicyResponseTypeDef:
         """
         Simulate how a set of IAM policies attached to an IAM entity works with a list
         of API operations and Amazon Web Services resources to determine the policies'
         effective permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.simulate_principal_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#simulate_principal_policy)
@@ -1828,25 +1820,25 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.update_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#update_role)
         """
 
     def update_role_description(
         self, *, RoleName: str, Description: str
-    ) -> UpdateRoleDescriptionResponseOutputTypeDef:
+    ) -> UpdateRoleDescriptionResponseTypeDef:
         """
         Use  UpdateRole instead.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.update_role_description)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#update_role_description)
         """
 
     def update_saml_provider(
         self, *, SAMLMetadataDocument: str, SAMLProviderArn: str
-    ) -> UpdateSAMLProviderResponseOutputTypeDef:
+    ) -> UpdateSAMLProviderResponseTypeDef:
         """
         Updates the metadata document for an existing SAML provider resource object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.update_saml_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#update_saml_provider)
         """
 
@@ -1907,36 +1899,36 @@
         *,
         ServerCertificateName: str,
         CertificateBody: str,
         PrivateKey: str,
         Path: str = ...,
         CertificateChain: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> UploadServerCertificateResponseOutputTypeDef:
+    ) -> UploadServerCertificateResponseTypeDef:
         """
         Uploads a server certificate entity for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.upload_server_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#upload_server_certificate)
         """
 
     def upload_signing_certificate(
         self, *, CertificateBody: str, UserName: str = ...
-    ) -> UploadSigningCertificateResponseOutputTypeDef:
+    ) -> UploadSigningCertificateResponseTypeDef:
         """
         Uploads an X.509 signing certificate and associates it with the specified IAM
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.upload_signing_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#upload_signing_certificate)
         """
 
     def upload_ssh_public_key(
         self, *, UserName: str, SSHPublicKeyBody: str
-    ) -> UploadSSHPublicKeyResponseOutputTypeDef:
+    ) -> UploadSSHPublicKeyResponseTypeDef:
         """
         Uploads an SSH public key and associates it with the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.upload_ssh_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#upload_ssh_public_key)
         """
```

### Comparing `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/client.pyi` & `mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -63,99 +63,99 @@
     ListUserTagsPaginator,
     ListVirtualMFADevicesPaginator,
     SimulateCustomPolicyPaginator,
     SimulatePrincipalPolicyPaginator,
 )
 from .type_defs import (
     ContextEntryTypeDef,
-    CreateAccessKeyResponseOutputTypeDef,
-    CreateGroupResponseOutputTypeDef,
-    CreateInstanceProfileResponseOutputTypeDef,
-    CreateLoginProfileResponseOutputTypeDef,
-    CreateOpenIDConnectProviderResponseOutputTypeDef,
-    CreatePolicyResponseOutputTypeDef,
-    CreatePolicyVersionResponseOutputTypeDef,
-    CreateRoleResponseOutputTypeDef,
-    CreateSAMLProviderResponseOutputTypeDef,
-    CreateServiceLinkedRoleResponseOutputTypeDef,
-    CreateServiceSpecificCredentialResponseOutputTypeDef,
-    CreateUserResponseOutputTypeDef,
-    CreateVirtualMFADeviceResponseOutputTypeDef,
-    DeleteServiceLinkedRoleResponseOutputTypeDef,
+    CreateAccessKeyResponseTypeDef,
+    CreateGroupResponseTypeDef,
+    CreateInstanceProfileResponseTypeDef,
+    CreateLoginProfileResponseTypeDef,
+    CreateOpenIDConnectProviderResponseTypeDef,
+    CreatePolicyResponseTypeDef,
+    CreatePolicyVersionResponseTypeDef,
+    CreateRoleResponseTypeDef,
+    CreateSAMLProviderResponseTypeDef,
+    CreateServiceLinkedRoleResponseTypeDef,
+    CreateServiceSpecificCredentialResponseTypeDef,
+    CreateUserResponseTypeDef,
+    CreateVirtualMFADeviceResponseTypeDef,
+    DeleteServiceLinkedRoleResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    GenerateCredentialReportResponseOutputTypeDef,
-    GenerateOrganizationsAccessReportResponseOutputTypeDef,
-    GenerateServiceLastAccessedDetailsResponseOutputTypeDef,
-    GetAccessKeyLastUsedResponseOutputTypeDef,
-    GetAccountAuthorizationDetailsResponseOutputTypeDef,
-    GetAccountPasswordPolicyResponseOutputTypeDef,
-    GetAccountSummaryResponseOutputTypeDef,
-    GetContextKeysForPolicyResponseOutputTypeDef,
-    GetCredentialReportResponseOutputTypeDef,
-    GetGroupPolicyResponseOutputTypeDef,
-    GetGroupResponseOutputTypeDef,
-    GetInstanceProfileResponseOutputTypeDef,
-    GetLoginProfileResponseOutputTypeDef,
-    GetMFADeviceResponseOutputTypeDef,
-    GetOpenIDConnectProviderResponseOutputTypeDef,
-    GetOrganizationsAccessReportResponseOutputTypeDef,
-    GetPolicyResponseOutputTypeDef,
-    GetPolicyVersionResponseOutputTypeDef,
-    GetRolePolicyResponseOutputTypeDef,
-    GetRoleResponseOutputTypeDef,
-    GetSAMLProviderResponseOutputTypeDef,
-    GetServerCertificateResponseOutputTypeDef,
-    GetServiceLastAccessedDetailsResponseOutputTypeDef,
-    GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef,
-    GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef,
-    GetSSHPublicKeyResponseOutputTypeDef,
-    GetUserPolicyResponseOutputTypeDef,
-    GetUserResponseOutputTypeDef,
-    ListAccessKeysResponseOutputTypeDef,
-    ListAccountAliasesResponseOutputTypeDef,
-    ListAttachedGroupPoliciesResponseOutputTypeDef,
-    ListAttachedRolePoliciesResponseOutputTypeDef,
-    ListAttachedUserPoliciesResponseOutputTypeDef,
-    ListEntitiesForPolicyResponseOutputTypeDef,
-    ListGroupPoliciesResponseOutputTypeDef,
-    ListGroupsForUserResponseOutputTypeDef,
-    ListGroupsResponseOutputTypeDef,
-    ListInstanceProfilesForRoleResponseOutputTypeDef,
-    ListInstanceProfilesResponseOutputTypeDef,
-    ListInstanceProfileTagsResponseOutputTypeDef,
-    ListMFADevicesResponseOutputTypeDef,
-    ListMFADeviceTagsResponseOutputTypeDef,
-    ListOpenIDConnectProvidersResponseOutputTypeDef,
-    ListOpenIDConnectProviderTagsResponseOutputTypeDef,
-    ListPoliciesGrantingServiceAccessResponseOutputTypeDef,
-    ListPoliciesResponseOutputTypeDef,
-    ListPolicyTagsResponseOutputTypeDef,
-    ListPolicyVersionsResponseOutputTypeDef,
-    ListRolePoliciesResponseOutputTypeDef,
-    ListRolesResponseOutputTypeDef,
-    ListRoleTagsResponseOutputTypeDef,
-    ListSAMLProvidersResponseOutputTypeDef,
-    ListSAMLProviderTagsResponseOutputTypeDef,
-    ListServerCertificatesResponseOutputTypeDef,
-    ListServerCertificateTagsResponseOutputTypeDef,
-    ListServiceSpecificCredentialsResponseOutputTypeDef,
-    ListSigningCertificatesResponseOutputTypeDef,
-    ListSSHPublicKeysResponseOutputTypeDef,
-    ListUserPoliciesResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
-    ListUserTagsResponseOutputTypeDef,
-    ListVirtualMFADevicesResponseOutputTypeDef,
-    ResetServiceSpecificCredentialResponseOutputTypeDef,
-    SimulatePolicyResponseOutputTypeDef,
+    GenerateCredentialReportResponseTypeDef,
+    GenerateOrganizationsAccessReportResponseTypeDef,
+    GenerateServiceLastAccessedDetailsResponseTypeDef,
+    GetAccessKeyLastUsedResponseTypeDef,
+    GetAccountAuthorizationDetailsResponseTypeDef,
+    GetAccountPasswordPolicyResponseTypeDef,
+    GetAccountSummaryResponseTypeDef,
+    GetContextKeysForPolicyResponseTypeDef,
+    GetCredentialReportResponseTypeDef,
+    GetGroupPolicyResponseTypeDef,
+    GetGroupResponseTypeDef,
+    GetInstanceProfileResponseTypeDef,
+    GetLoginProfileResponseTypeDef,
+    GetMFADeviceResponseTypeDef,
+    GetOpenIDConnectProviderResponseTypeDef,
+    GetOrganizationsAccessReportResponseTypeDef,
+    GetPolicyResponseTypeDef,
+    GetPolicyVersionResponseTypeDef,
+    GetRolePolicyResponseTypeDef,
+    GetRoleResponseTypeDef,
+    GetSAMLProviderResponseTypeDef,
+    GetServerCertificateResponseTypeDef,
+    GetServiceLastAccessedDetailsResponseTypeDef,
+    GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef,
+    GetServiceLinkedRoleDeletionStatusResponseTypeDef,
+    GetSSHPublicKeyResponseTypeDef,
+    GetUserPolicyResponseTypeDef,
+    GetUserResponseTypeDef,
+    ListAccessKeysResponseTypeDef,
+    ListAccountAliasesResponseTypeDef,
+    ListAttachedGroupPoliciesResponseTypeDef,
+    ListAttachedRolePoliciesResponseTypeDef,
+    ListAttachedUserPoliciesResponseTypeDef,
+    ListEntitiesForPolicyResponseTypeDef,
+    ListGroupPoliciesResponseTypeDef,
+    ListGroupsForUserResponseTypeDef,
+    ListGroupsResponseTypeDef,
+    ListInstanceProfilesForRoleResponseTypeDef,
+    ListInstanceProfilesResponseTypeDef,
+    ListInstanceProfileTagsResponseTypeDef,
+    ListMFADevicesResponseTypeDef,
+    ListMFADeviceTagsResponseTypeDef,
+    ListOpenIDConnectProvidersResponseTypeDef,
+    ListOpenIDConnectProviderTagsResponseTypeDef,
+    ListPoliciesGrantingServiceAccessResponseTypeDef,
+    ListPoliciesResponseTypeDef,
+    ListPolicyTagsResponseTypeDef,
+    ListPolicyVersionsResponseTypeDef,
+    ListRolePoliciesResponseTypeDef,
+    ListRolesResponseTypeDef,
+    ListRoleTagsResponseTypeDef,
+    ListSAMLProvidersResponseTypeDef,
+    ListSAMLProviderTagsResponseTypeDef,
+    ListServerCertificatesResponseTypeDef,
+    ListServerCertificateTagsResponseTypeDef,
+    ListServiceSpecificCredentialsResponseTypeDef,
+    ListSigningCertificatesResponseTypeDef,
+    ListSSHPublicKeysResponseTypeDef,
+    ListUserPoliciesResponseTypeDef,
+    ListUsersResponseTypeDef,
+    ListUserTagsResponseTypeDef,
+    ListVirtualMFADevicesResponseTypeDef,
+    ResetServiceSpecificCredentialResponseTypeDef,
+    SimulatePolicyResponseTypeDef,
     TagTypeDef,
-    UpdateRoleDescriptionResponseOutputTypeDef,
-    UpdateSAMLProviderResponseOutputTypeDef,
-    UploadServerCertificateResponseOutputTypeDef,
-    UploadSigningCertificateResponseOutputTypeDef,
-    UploadSSHPublicKeyResponseOutputTypeDef,
+    UpdateRoleDescriptionResponseTypeDef,
+    UpdateSAMLProviderResponseTypeDef,
+    UploadServerCertificateResponseTypeDef,
+    UploadSigningCertificateResponseTypeDef,
+    UploadSSHPublicKeyResponseTypeDef,
 )
 from .waiter import (
     InstanceProfileExistsWaiter,
     PolicyExistsWaiter,
     RoleExistsWaiter,
     UserExistsWaiter,
 )
@@ -288,62 +288,62 @@
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#close)
         """
-    def create_access_key(self, *, UserName: str = ...) -> CreateAccessKeyResponseOutputTypeDef:
+    def create_access_key(self, *, UserName: str = ...) -> CreateAccessKeyResponseTypeDef:
         """
         Creates a new Amazon Web Services secret access key and corresponding Amazon Web
         Services access key ID for the specified user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_access_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_access_key)
         """
     def create_account_alias(self, *, AccountAlias: str) -> EmptyResponseMetadataTypeDef:
         """
         Creates an alias for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_account_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_account_alias)
         """
-    def create_group(self, *, GroupName: str, Path: str = ...) -> CreateGroupResponseOutputTypeDef:
+    def create_group(self, *, GroupName: str, Path: str = ...) -> CreateGroupResponseTypeDef:
         """
         Creates a new group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_group)
         """
     def create_instance_profile(
         self, *, InstanceProfileName: str, Path: str = ..., Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateInstanceProfileResponseOutputTypeDef:
+    ) -> CreateInstanceProfileResponseTypeDef:
         """
         Creates a new instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_instance_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_instance_profile)
         """
     def create_login_profile(
         self, *, UserName: str, Password: str, PasswordResetRequired: bool = ...
-    ) -> CreateLoginProfileResponseOutputTypeDef:
+    ) -> CreateLoginProfileResponseTypeDef:
         """
         Creates a password for the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_login_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_login_profile)
         """
     def create_open_id_connect_provider(
         self,
         *,
         Url: str,
         ThumbprintList: Sequence[str],
         ClientIDList: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateOpenIDConnectProviderResponseOutputTypeDef:
+    ) -> CreateOpenIDConnectProviderResponseTypeDef:
         """
         Creates an IAM entity to describe an identity provider (IdP) that supports
         `OpenID Connect (OIDC) <http://openid.net/connect/>`__.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_open_id_connect_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_open_id_connect_provider)
         """
@@ -351,24 +351,24 @@
         self,
         *,
         PolicyName: str,
         PolicyDocument: str,
         Path: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreatePolicyResponseOutputTypeDef:
+    ) -> CreatePolicyResponseTypeDef:
         """
         Creates a new managed policy for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_policy)
         """
     def create_policy_version(
         self, *, PolicyArn: str, PolicyDocument: str, SetAsDefault: bool = ...
-    ) -> CreatePolicyVersionResponseOutputTypeDef:
+    ) -> CreatePolicyVersionResponseTypeDef:
         """
         Creates a new version of the specified managed policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_policy_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_policy_version)
         """
     def create_role(
@@ -377,67 +377,67 @@
         RoleName: str,
         AssumeRolePolicyDocument: str,
         Path: str = ...,
         Description: str = ...,
         MaxSessionDuration: int = ...,
         PermissionsBoundary: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateRoleResponseOutputTypeDef:
+    ) -> CreateRoleResponseTypeDef:
         """
         Creates a new role for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_role)
         """
     def create_saml_provider(
         self, *, SAMLMetadataDocument: str, Name: str, Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateSAMLProviderResponseOutputTypeDef:
+    ) -> CreateSAMLProviderResponseTypeDef:
         """
         Creates an IAM resource that describes an identity provider (IdP) that supports
         SAML 2.0.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_saml_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_saml_provider)
         """
     def create_service_linked_role(
         self, *, AWSServiceName: str, Description: str = ..., CustomSuffix: str = ...
-    ) -> CreateServiceLinkedRoleResponseOutputTypeDef:
+    ) -> CreateServiceLinkedRoleResponseTypeDef:
         """
         Creates an IAM role that is linked to a specific Amazon Web Services service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_service_linked_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_service_linked_role)
         """
     def create_service_specific_credential(
         self, *, UserName: str, ServiceName: str
-    ) -> CreateServiceSpecificCredentialResponseOutputTypeDef:
+    ) -> CreateServiceSpecificCredentialResponseTypeDef:
         """
         Generates a set of credentials consisting of a user name and password that can
         be used to access the service specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_service_specific_credential)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_service_specific_credential)
         """
     def create_user(
         self,
         *,
         UserName: str,
         Path: str = ...,
         PermissionsBoundary: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateUserResponseOutputTypeDef:
+    ) -> CreateUserResponseTypeDef:
         """
         Creates a new IAM user for your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_user)
         """
     def create_virtual_mfa_device(
         self, *, VirtualMFADeviceName: str, Path: str = ..., Tags: Sequence[TagTypeDef] = ...
-    ) -> CreateVirtualMFADeviceResponseOutputTypeDef:
+    ) -> CreateVirtualMFADeviceResponseTypeDef:
         """
         Creates a new virtual MFA device for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.create_virtual_mfa_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#create_virtual_mfa_device)
         """
     def deactivate_mfa_device(
@@ -566,15 +566,15 @@
         Deletes the specified server certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.delete_server_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#delete_server_certificate)
         """
     def delete_service_linked_role(
         self, *, RoleName: str
-    ) -> DeleteServiceLinkedRoleResponseOutputTypeDef:
+    ) -> DeleteServiceLinkedRoleResponseTypeDef:
         """
         Submits a service-linked role deletion request and returns a `DeletionTaskId`,
         which you can use to check the status of the deletion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.delete_service_linked_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#delete_service_linked_role)
         """
@@ -666,24 +666,24 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Enables the specified MFA device and associates it with the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.enable_mfa_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#enable_mfa_device)
         """
-    def generate_credential_report(self) -> GenerateCredentialReportResponseOutputTypeDef:
+    def generate_credential_report(self) -> GenerateCredentialReportResponseTypeDef:
         """
         Generates a credential report for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.generate_credential_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#generate_credential_report)
         """
     def generate_organizations_access_report(
         self, *, EntityPath: str, OrganizationsPolicyId: str = ...
-    ) -> GenerateOrganizationsAccessReportResponseOutputTypeDef:
+    ) -> GenerateOrganizationsAccessReportResponseTypeDef:
         """
         Generates a report for service last accessed data for Organizations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.generate_organizations_access_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#generate_organizations_access_report)
         """
     def generate_presigned_url(
@@ -697,300 +697,292 @@
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#generate_presigned_url)
         """
     def generate_service_last_accessed_details(
         self, *, Arn: str, Granularity: AccessAdvisorUsageGranularityTypeType = ...
-    ) -> GenerateServiceLastAccessedDetailsResponseOutputTypeDef:
+    ) -> GenerateServiceLastAccessedDetailsResponseTypeDef:
         """
         Generates a report that includes details about when an IAM resource (user,
         group, role, or policy) was last used in an attempt to access Amazon Web
         Services services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.generate_service_last_accessed_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#generate_service_last_accessed_details)
         """
-    def get_access_key_last_used(
-        self, *, AccessKeyId: str
-    ) -> GetAccessKeyLastUsedResponseOutputTypeDef:
+    def get_access_key_last_used(self, *, AccessKeyId: str) -> GetAccessKeyLastUsedResponseTypeDef:
         """
         Retrieves information about when the specified access key was last used.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_access_key_last_used)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_access_key_last_used)
         """
     def get_account_authorization_details(
         self, *, Filter: Sequence[EntityTypeType] = ..., MaxItems: int = ..., Marker: str = ...
-    ) -> GetAccountAuthorizationDetailsResponseOutputTypeDef:
+    ) -> GetAccountAuthorizationDetailsResponseTypeDef:
         """
         Retrieves information about all IAM users, groups, roles, and policies in your
         Amazon Web Services account, including their relationships to one another.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_account_authorization_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_account_authorization_details)
         """
-    def get_account_password_policy(self) -> GetAccountPasswordPolicyResponseOutputTypeDef:
+    def get_account_password_policy(self) -> GetAccountPasswordPolicyResponseTypeDef:
         """
         Retrieves the password policy for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_account_password_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_account_password_policy)
         """
-    def get_account_summary(self) -> GetAccountSummaryResponseOutputTypeDef:
+    def get_account_summary(self) -> GetAccountSummaryResponseTypeDef:
         """
         Retrieves information about IAM entity usage and IAM quotas in the Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_account_summary)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_account_summary)
         """
     def get_context_keys_for_custom_policy(
         self, *, PolicyInputList: Sequence[str]
-    ) -> GetContextKeysForPolicyResponseOutputTypeDef:
+    ) -> GetContextKeysForPolicyResponseTypeDef:
         """
         Gets a list of all of the context keys referenced in the input policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_context_keys_for_custom_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_context_keys_for_custom_policy)
         """
     def get_context_keys_for_principal_policy(
         self, *, PolicySourceArn: str, PolicyInputList: Sequence[str] = ...
-    ) -> GetContextKeysForPolicyResponseOutputTypeDef:
+    ) -> GetContextKeysForPolicyResponseTypeDef:
         """
         Gets a list of all of the context keys referenced in all the IAM policies that
         are attached to the specified IAM entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_context_keys_for_principal_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_context_keys_for_principal_policy)
         """
-    def get_credential_report(self) -> GetCredentialReportResponseOutputTypeDef:
+    def get_credential_report(self) -> GetCredentialReportResponseTypeDef:
         """
         Retrieves a credential report for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_credential_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_credential_report)
         """
     def get_group(
         self, *, GroupName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> GetGroupResponseOutputTypeDef:
+    ) -> GetGroupResponseTypeDef:
         """
         Returns a list of IAM users that are in the specified IAM group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_group)
         """
-    def get_group_policy(
-        self, *, GroupName: str, PolicyName: str
-    ) -> GetGroupPolicyResponseOutputTypeDef:
+    def get_group_policy(self, *, GroupName: str, PolicyName: str) -> GetGroupPolicyResponseTypeDef:
         """
         Retrieves the specified inline policy document that is embedded in the specified
         IAM group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_group_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_group_policy)
         """
     def get_instance_profile(
         self, *, InstanceProfileName: str
-    ) -> GetInstanceProfileResponseOutputTypeDef:
+    ) -> GetInstanceProfileResponseTypeDef:
         """
         Retrieves information about the specified instance profile, including the
         instance profile's path, GUID, ARN, and role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_instance_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_instance_profile)
         """
-    def get_login_profile(self, *, UserName: str) -> GetLoginProfileResponseOutputTypeDef:
+    def get_login_profile(self, *, UserName: str) -> GetLoginProfileResponseTypeDef:
         """
         Retrieves the user name for the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_login_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_login_profile)
         """
     def get_mfa_device(
         self, *, SerialNumber: str, UserName: str = ...
-    ) -> GetMFADeviceResponseOutputTypeDef:
+    ) -> GetMFADeviceResponseTypeDef:
         """
         Retrieves information about an MFA device for a specified user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_mfa_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_mfa_device)
         """
     def get_open_id_connect_provider(
         self, *, OpenIDConnectProviderArn: str
-    ) -> GetOpenIDConnectProviderResponseOutputTypeDef:
+    ) -> GetOpenIDConnectProviderResponseTypeDef:
         """
         Returns information about the specified OpenID Connect (OIDC) provider resource
         object in IAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_open_id_connect_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_open_id_connect_provider)
         """
     def get_organizations_access_report(
         self, *, JobId: str, MaxItems: int = ..., Marker: str = ..., SortKey: sortKeyTypeType = ...
-    ) -> GetOrganizationsAccessReportResponseOutputTypeDef:
+    ) -> GetOrganizationsAccessReportResponseTypeDef:
         """
         Retrieves the service last accessed data report for Organizations that was
         previously generated using the `GenerateOrganizationsAccessReport` operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_organizations_access_report)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_organizations_access_report)
         """
-    def get_policy(self, *, PolicyArn: str) -> GetPolicyResponseOutputTypeDef:
+    def get_policy(self, *, PolicyArn: str) -> GetPolicyResponseTypeDef:
         """
         Retrieves information about the specified managed policy, including the policy's
         default version and the total number of IAM users, groups, and roles to which
         the policy is attached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_policy)
         """
     def get_policy_version(
         self, *, PolicyArn: str, VersionId: str
-    ) -> GetPolicyVersionResponseOutputTypeDef:
+    ) -> GetPolicyVersionResponseTypeDef:
         """
         Retrieves information about the specified version of the specified managed
         policy, including the policy document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_policy_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_policy_version)
         """
-    def get_role(self, *, RoleName: str) -> GetRoleResponseOutputTypeDef:
+    def get_role(self, *, RoleName: str) -> GetRoleResponseTypeDef:
         """
         Retrieves information about the specified role, including the role's path, GUID,
         ARN, and the role's trust policy that grants permission to assume the role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_role)
         """
-    def get_role_policy(
-        self, *, RoleName: str, PolicyName: str
-    ) -> GetRolePolicyResponseOutputTypeDef:
+    def get_role_policy(self, *, RoleName: str, PolicyName: str) -> GetRolePolicyResponseTypeDef:
         """
         Retrieves the specified inline policy document that is embedded with the
         specified IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_role_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_role_policy)
         """
-    def get_saml_provider(self, *, SAMLProviderArn: str) -> GetSAMLProviderResponseOutputTypeDef:
+    def get_saml_provider(self, *, SAMLProviderArn: str) -> GetSAMLProviderResponseTypeDef:
         """
         Returns the SAML provider metadocument that was uploaded when the IAM SAML
         provider resource object was created or updated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_saml_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_saml_provider)
         """
     def get_server_certificate(
         self, *, ServerCertificateName: str
-    ) -> GetServerCertificateResponseOutputTypeDef:
+    ) -> GetServerCertificateResponseTypeDef:
         """
         Retrieves information about the specified server certificate stored in IAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_server_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_server_certificate)
         """
     def get_service_last_accessed_details(
         self, *, JobId: str, MaxItems: int = ..., Marker: str = ...
-    ) -> GetServiceLastAccessedDetailsResponseOutputTypeDef:
+    ) -> GetServiceLastAccessedDetailsResponseTypeDef:
         """
         Retrieves a service last accessed report that was created using the
         `GenerateServiceLastAccessedDetails` operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_service_last_accessed_details)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_service_last_accessed_details)
         """
     def get_service_last_accessed_details_with_entities(
         self, *, JobId: str, ServiceNamespace: str, MaxItems: int = ..., Marker: str = ...
-    ) -> GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef:
+    ) -> GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef:
         """
         After you generate a group or policy report using the
         `GenerateServiceLastAccessedDetails` operation, you can use the `JobId`
         parameter in `GetServiceLastAccessedDetailsWithEntities`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_service_last_accessed_details_with_entities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_service_last_accessed_details_with_entities)
         """
     def get_service_linked_role_deletion_status(
         self, *, DeletionTaskId: str
-    ) -> GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef:
+    ) -> GetServiceLinkedRoleDeletionStatusResponseTypeDef:
         """
         Retrieves the status of your service-linked role deletion.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_service_linked_role_deletion_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_service_linked_role_deletion_status)
         """
     def get_ssh_public_key(
         self, *, UserName: str, SSHPublicKeyId: str, Encoding: encodingTypeType
-    ) -> GetSSHPublicKeyResponseOutputTypeDef:
+    ) -> GetSSHPublicKeyResponseTypeDef:
         """
         Retrieves the specified SSH public key, including metadata about the key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_ssh_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_ssh_public_key)
         """
-    def get_user(self, *, UserName: str = ...) -> GetUserResponseOutputTypeDef:
+    def get_user(self, *, UserName: str = ...) -> GetUserResponseTypeDef:
         """
         Retrieves information about the specified IAM user, including the user's
         creation date, path, unique ID, and ARN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_user)
         """
-    def get_user_policy(
-        self, *, UserName: str, PolicyName: str
-    ) -> GetUserPolicyResponseOutputTypeDef:
+    def get_user_policy(self, *, UserName: str, PolicyName: str) -> GetUserPolicyResponseTypeDef:
         """
         Retrieves the specified inline policy document that is embedded in the specified
         IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.get_user_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#get_user_policy)
         """
     def list_access_keys(
         self, *, UserName: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListAccessKeysResponseOutputTypeDef:
+    ) -> ListAccessKeysResponseTypeDef:
         """
         Returns information about the access key IDs associated with the specified IAM
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_access_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_access_keys)
         """
     def list_account_aliases(
         self, *, Marker: str = ..., MaxItems: int = ...
-    ) -> ListAccountAliasesResponseOutputTypeDef:
+    ) -> ListAccountAliasesResponseTypeDef:
         """
         Lists the account alias associated with the Amazon Web Services account (Note:
         you can have only one).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_account_aliases)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_account_aliases)
         """
     def list_attached_group_policies(
         self, *, GroupName: str, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListAttachedGroupPoliciesResponseOutputTypeDef:
+    ) -> ListAttachedGroupPoliciesResponseTypeDef:
         """
         Lists all managed policies that are attached to the specified IAM group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_attached_group_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_attached_group_policies)
         """
     def list_attached_role_policies(
         self, *, RoleName: str, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListAttachedRolePoliciesResponseOutputTypeDef:
+    ) -> ListAttachedRolePoliciesResponseTypeDef:
         """
         Lists all managed policies that are attached to the specified IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_attached_role_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_attached_role_policies)
         """
     def list_attached_user_policies(
         self, *, UserName: str, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListAttachedUserPoliciesResponseOutputTypeDef:
+    ) -> ListAttachedUserPoliciesResponseTypeDef:
         """
         Lists all managed policies that are attached to the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_attached_user_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_attached_user_policies)
         """
     def list_entities_for_policy(
@@ -998,107 +990,107 @@
         *,
         PolicyArn: str,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
         MaxItems: int = ...
-    ) -> ListEntitiesForPolicyResponseOutputTypeDef:
+    ) -> ListEntitiesForPolicyResponseTypeDef:
         """
         Lists all IAM users, groups, and roles that the specified managed policy is
         attached to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_entities_for_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_entities_for_policy)
         """
     def list_group_policies(
         self, *, GroupName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListGroupPoliciesResponseOutputTypeDef:
+    ) -> ListGroupPoliciesResponseTypeDef:
         """
         Lists the names of the inline policies that are embedded in the specified IAM
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_group_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_group_policies)
         """
     def list_groups(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListGroupsResponseOutputTypeDef:
+    ) -> ListGroupsResponseTypeDef:
         """
         Lists the IAM groups that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_groups)
         """
     def list_groups_for_user(
         self, *, UserName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListGroupsForUserResponseOutputTypeDef:
+    ) -> ListGroupsForUserResponseTypeDef:
         """
         Lists the IAM groups that the specified IAM user belongs to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_groups_for_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_groups_for_user)
         """
     def list_instance_profile_tags(
         self, *, InstanceProfileName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListInstanceProfileTagsResponseOutputTypeDef:
+    ) -> ListInstanceProfileTagsResponseTypeDef:
         """
         Lists the tags that are attached to the specified IAM instance profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_instance_profile_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_instance_profile_tags)
         """
     def list_instance_profiles(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListInstanceProfilesResponseOutputTypeDef:
+    ) -> ListInstanceProfilesResponseTypeDef:
         """
         Lists the instance profiles that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_instance_profiles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_instance_profiles)
         """
     def list_instance_profiles_for_role(
         self, *, RoleName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListInstanceProfilesForRoleResponseOutputTypeDef:
+    ) -> ListInstanceProfilesForRoleResponseTypeDef:
         """
         Lists the instance profiles that have the specified associated IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_instance_profiles_for_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_instance_profiles_for_role)
         """
     def list_mfa_device_tags(
         self, *, SerialNumber: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListMFADeviceTagsResponseOutputTypeDef:
+    ) -> ListMFADeviceTagsResponseTypeDef:
         """
         Lists the tags that are attached to the specified IAM virtual multi-factor
         authentication (MFA) device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_mfa_device_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_mfa_device_tags)
         """
     def list_mfa_devices(
         self, *, UserName: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListMFADevicesResponseOutputTypeDef:
+    ) -> ListMFADevicesResponseTypeDef:
         """
         Lists the MFA devices for an IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_mfa_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_mfa_devices)
         """
     def list_open_id_connect_provider_tags(
         self, *, OpenIDConnectProviderArn: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListOpenIDConnectProviderTagsResponseOutputTypeDef:
+    ) -> ListOpenIDConnectProviderTagsResponseTypeDef:
         """
         Lists the tags that are attached to the specified OpenID Connect
         (OIDC)-compatible identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_open_id_connect_provider_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_open_id_connect_provider_tags)
         """
-    def list_open_id_connect_providers(self) -> ListOpenIDConnectProvidersResponseOutputTypeDef:
+    def list_open_id_connect_providers(self) -> ListOpenIDConnectProvidersResponseTypeDef:
         """
         Lists information about the IAM OpenID Connect (OIDC) provider resource objects
         defined in the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_open_id_connect_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_open_id_connect_providers)
         """
@@ -1107,179 +1099,179 @@
         *,
         Scope: policyScopeTypeType = ...,
         OnlyAttached: bool = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         Marker: str = ...,
         MaxItems: int = ...
-    ) -> ListPoliciesResponseOutputTypeDef:
+    ) -> ListPoliciesResponseTypeDef:
         """
         Lists all the managed policies that are available in your Amazon Web Services
         account, including your own customer-defined managed policies and all Amazon Web
         Services managed policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_policies)
         """
     def list_policies_granting_service_access(
         self, *, Arn: str, ServiceNamespaces: Sequence[str], Marker: str = ...
-    ) -> ListPoliciesGrantingServiceAccessResponseOutputTypeDef:
+    ) -> ListPoliciesGrantingServiceAccessResponseTypeDef:
         """
         Retrieves a list of policies that the IAM identity (user, group, or role) can
         use to access each specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_policies_granting_service_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_policies_granting_service_access)
         """
     def list_policy_tags(
         self, *, PolicyArn: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListPolicyTagsResponseOutputTypeDef:
+    ) -> ListPolicyTagsResponseTypeDef:
         """
         Lists the tags that are attached to the specified IAM customer managed policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_policy_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_policy_tags)
         """
     def list_policy_versions(
         self, *, PolicyArn: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListPolicyVersionsResponseOutputTypeDef:
+    ) -> ListPolicyVersionsResponseTypeDef:
         """
         Lists information about the versions of the specified managed policy, including
         the version that is currently set as the policy's default version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_policy_versions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_policy_versions)
         """
     def list_role_policies(
         self, *, RoleName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListRolePoliciesResponseOutputTypeDef:
+    ) -> ListRolePoliciesResponseTypeDef:
         """
         Lists the names of the inline policies that are embedded in the specified IAM
         role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_role_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_role_policies)
         """
     def list_role_tags(
         self, *, RoleName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListRoleTagsResponseOutputTypeDef:
+    ) -> ListRoleTagsResponseTypeDef:
         """
         Lists the tags that are attached to the specified role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_role_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_role_tags)
         """
     def list_roles(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListRolesResponseOutputTypeDef:
+    ) -> ListRolesResponseTypeDef:
         """
         Lists the IAM roles that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_roles)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_roles)
         """
     def list_saml_provider_tags(
         self, *, SAMLProviderArn: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListSAMLProviderTagsResponseOutputTypeDef:
+    ) -> ListSAMLProviderTagsResponseTypeDef:
         """
         Lists the tags that are attached to the specified Security Assertion Markup
         Language (SAML) identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_saml_provider_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_saml_provider_tags)
         """
-    def list_saml_providers(self) -> ListSAMLProvidersResponseOutputTypeDef:
+    def list_saml_providers(self) -> ListSAMLProvidersResponseTypeDef:
         """
         Lists the SAML provider resource objects defined in IAM in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_saml_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_saml_providers)
         """
     def list_server_certificate_tags(
         self, *, ServerCertificateName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListServerCertificateTagsResponseOutputTypeDef:
+    ) -> ListServerCertificateTagsResponseTypeDef:
         """
         Lists the tags that are attached to the specified IAM server certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_server_certificate_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_server_certificate_tags)
         """
     def list_server_certificates(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListServerCertificatesResponseOutputTypeDef:
+    ) -> ListServerCertificatesResponseTypeDef:
         """
         Lists the server certificates stored in IAM that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_server_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_server_certificates)
         """
     def list_service_specific_credentials(
         self, *, UserName: str = ..., ServiceName: str = ...
-    ) -> ListServiceSpecificCredentialsResponseOutputTypeDef:
+    ) -> ListServiceSpecificCredentialsResponseTypeDef:
         """
         Returns information about the service-specific credentials associated with the
         specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_service_specific_credentials)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_service_specific_credentials)
         """
     def list_signing_certificates(
         self, *, UserName: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListSigningCertificatesResponseOutputTypeDef:
+    ) -> ListSigningCertificatesResponseTypeDef:
         """
         Returns information about the signing certificates associated with the specified
         IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_signing_certificates)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_signing_certificates)
         """
     def list_ssh_public_keys(
         self, *, UserName: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListSSHPublicKeysResponseOutputTypeDef:
+    ) -> ListSSHPublicKeysResponseTypeDef:
         """
         Returns information about the SSH public keys associated with the specified IAM
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_ssh_public_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_ssh_public_keys)
         """
     def list_user_policies(
         self, *, UserName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListUserPoliciesResponseOutputTypeDef:
+    ) -> ListUserPoliciesResponseTypeDef:
         """
         Lists the names of the inline policies embedded in the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_user_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_user_policies)
         """
     def list_user_tags(
         self, *, UserName: str, Marker: str = ..., MaxItems: int = ...
-    ) -> ListUserTagsResponseOutputTypeDef:
+    ) -> ListUserTagsResponseTypeDef:
         """
         Lists the tags that are attached to the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_user_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_user_tags)
         """
     def list_users(
         self, *, PathPrefix: str = ..., Marker: str = ..., MaxItems: int = ...
-    ) -> ListUsersResponseOutputTypeDef:
+    ) -> ListUsersResponseTypeDef:
         """
         Lists the IAM users that have the specified path prefix.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_users)
         """
     def list_virtual_mfa_devices(
         self,
         *,
         AssignmentStatus: assignmentStatusTypeType = ...,
         Marker: str = ...,
         MaxItems: int = ...
-    ) -> ListVirtualMFADevicesResponseOutputTypeDef:
+    ) -> ListVirtualMFADevicesResponseTypeDef:
         """
         Lists the virtual MFA devices defined in the Amazon Web Services account by
         assignment status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.list_virtual_mfa_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#list_virtual_mfa_devices)
         """
@@ -1360,15 +1352,15 @@
         Removes the specified user from the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.remove_user_from_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#remove_user_from_group)
         """
     def reset_service_specific_credential(
         self, *, ServiceSpecificCredentialId: str, UserName: str = ...
-    ) -> ResetServiceSpecificCredentialResponseOutputTypeDef:
+    ) -> ResetServiceSpecificCredentialResponseTypeDef:
         """
         Resets the password for a service-specific credential.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.reset_service_specific_credential)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#reset_service_specific_credential)
         """
     def resync_mfa_device(
@@ -1416,15 +1408,15 @@
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         MaxItems: int = ...,
         Marker: str = ...
-    ) -> SimulatePolicyResponseOutputTypeDef:
+    ) -> SimulatePolicyResponseTypeDef:
         """
         Simulate how a set of IAM policies and optionally a resource-based policy works
         with a list of API operations and Amazon Web Services resources to determine the
         policies' effective permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.simulate_custom_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#simulate_custom_policy)
@@ -1440,15 +1432,15 @@
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         MaxItems: int = ...,
         Marker: str = ...
-    ) -> SimulatePolicyResponseOutputTypeDef:
+    ) -> SimulatePolicyResponseTypeDef:
         """
         Simulate how a set of IAM policies attached to an IAM entity works with a list
         of API operations and Amazon Web Services resources to determine the policies'
         effective permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.simulate_principal_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#simulate_principal_policy)
@@ -1671,24 +1663,24 @@
         Updates the description or maximum session duration setting of a role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.update_role)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#update_role)
         """
     def update_role_description(
         self, *, RoleName: str, Description: str
-    ) -> UpdateRoleDescriptionResponseOutputTypeDef:
+    ) -> UpdateRoleDescriptionResponseTypeDef:
         """
         Use  UpdateRole instead.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.update_role_description)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#update_role_description)
         """
     def update_saml_provider(
         self, *, SAMLMetadataDocument: str, SAMLProviderArn: str
-    ) -> UpdateSAMLProviderResponseOutputTypeDef:
+    ) -> UpdateSAMLProviderResponseTypeDef:
         """
         Updates the metadata document for an existing SAML provider resource object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.update_saml_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#update_saml_provider)
         """
     def update_server_certificate(
@@ -1743,34 +1735,34 @@
         *,
         ServerCertificateName: str,
         CertificateBody: str,
         PrivateKey: str,
         Path: str = ...,
         CertificateChain: str = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> UploadServerCertificateResponseOutputTypeDef:
+    ) -> UploadServerCertificateResponseTypeDef:
         """
         Uploads a server certificate entity for the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.upload_server_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#upload_server_certificate)
         """
     def upload_signing_certificate(
         self, *, CertificateBody: str, UserName: str = ...
-    ) -> UploadSigningCertificateResponseOutputTypeDef:
+    ) -> UploadSigningCertificateResponseTypeDef:
         """
         Uploads an X.509 signing certificate and associates it with the specified IAM
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.upload_signing_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#upload_signing_certificate)
         """
     def upload_ssh_public_key(
         self, *, UserName: str, SSHPublicKeyBody: str
-    ) -> UploadSSHPublicKeyResponseOutputTypeDef:
+    ) -> UploadSSHPublicKeyResponseTypeDef:
         """
         Uploads an SSH public key and associates it with the specified IAM user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Client.upload_ssh_public_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/client/#upload_ssh_public_key)
         """
     @overload
```

### Comparing `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/literals.py` & `mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/literals.pyi` & `mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/paginator.py` & `mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,48 +93,48 @@
     EntityTypeType,
     PolicyUsageTypeType,
     assignmentStatusTypeType,
     policyScopeTypeType,
 )
 from .type_defs import (
     ContextEntryTypeDef,
-    GetAccountAuthorizationDetailsResponseOutputTypeDef,
-    GetGroupResponseOutputTypeDef,
-    ListAccessKeysResponseOutputTypeDef,
-    ListAccountAliasesResponseOutputTypeDef,
-    ListAttachedGroupPoliciesResponseOutputTypeDef,
-    ListAttachedRolePoliciesResponseOutputTypeDef,
-    ListAttachedUserPoliciesResponseOutputTypeDef,
-    ListEntitiesForPolicyResponseOutputTypeDef,
-    ListGroupPoliciesResponseOutputTypeDef,
-    ListGroupsForUserResponseOutputTypeDef,
-    ListGroupsResponseOutputTypeDef,
-    ListInstanceProfilesForRoleResponseOutputTypeDef,
-    ListInstanceProfilesResponseOutputTypeDef,
-    ListInstanceProfileTagsResponseOutputTypeDef,
-    ListMFADevicesResponseOutputTypeDef,
-    ListMFADeviceTagsResponseOutputTypeDef,
-    ListOpenIDConnectProviderTagsResponseOutputTypeDef,
-    ListPoliciesResponseOutputTypeDef,
-    ListPolicyTagsResponseOutputTypeDef,
-    ListPolicyVersionsResponseOutputTypeDef,
-    ListRolePoliciesResponseOutputTypeDef,
-    ListRolesResponseOutputTypeDef,
-    ListRoleTagsResponseOutputTypeDef,
-    ListSAMLProviderTagsResponseOutputTypeDef,
-    ListServerCertificatesResponseOutputTypeDef,
-    ListServerCertificateTagsResponseOutputTypeDef,
-    ListSigningCertificatesResponseOutputTypeDef,
-    ListSSHPublicKeysResponseOutputTypeDef,
-    ListUserPoliciesResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
-    ListUserTagsResponseOutputTypeDef,
-    ListVirtualMFADevicesResponseOutputTypeDef,
+    GetAccountAuthorizationDetailsResponseTypeDef,
+    GetGroupResponseTypeDef,
+    ListAccessKeysResponseTypeDef,
+    ListAccountAliasesResponseTypeDef,
+    ListAttachedGroupPoliciesResponseTypeDef,
+    ListAttachedRolePoliciesResponseTypeDef,
+    ListAttachedUserPoliciesResponseTypeDef,
+    ListEntitiesForPolicyResponseTypeDef,
+    ListGroupPoliciesResponseTypeDef,
+    ListGroupsForUserResponseTypeDef,
+    ListGroupsResponseTypeDef,
+    ListInstanceProfilesForRoleResponseTypeDef,
+    ListInstanceProfilesResponseTypeDef,
+    ListInstanceProfileTagsResponseTypeDef,
+    ListMFADevicesResponseTypeDef,
+    ListMFADeviceTagsResponseTypeDef,
+    ListOpenIDConnectProviderTagsResponseTypeDef,
+    ListPoliciesResponseTypeDef,
+    ListPolicyTagsResponseTypeDef,
+    ListPolicyVersionsResponseTypeDef,
+    ListRolePoliciesResponseTypeDef,
+    ListRolesResponseTypeDef,
+    ListRoleTagsResponseTypeDef,
+    ListSAMLProviderTagsResponseTypeDef,
+    ListServerCertificatesResponseTypeDef,
+    ListServerCertificateTagsResponseTypeDef,
+    ListSigningCertificatesResponseTypeDef,
+    ListSSHPublicKeysResponseTypeDef,
+    ListUserPoliciesResponseTypeDef,
+    ListUsersResponseTypeDef,
+    ListUserTagsResponseTypeDef,
+    ListVirtualMFADevicesResponseTypeDef,
     PaginatorConfigTypeDef,
-    SimulatePolicyResponseOutputTypeDef,
+    SimulatePolicyResponseTypeDef,
 )
 
 __all__ = (
     "GetAccountAuthorizationDetailsPaginator",
     "GetGroupPaginator",
     "ListAccessKeysPaginator",
     "ListAccountAliasesPaginator",
@@ -188,60 +188,60 @@
     """
 
     def paginate(
         self,
         *,
         Filter: Sequence[EntityTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[GetAccountAuthorizationDetailsResponseOutputTypeDef]:
+    ) -> _PageIterator[GetAccountAuthorizationDetailsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetAccountAuthorizationDetails.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#getaccountauthorizationdetailspaginator)
         """
 
 
 class GetGroupPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#getgrouppaginator)
     """
 
     def paginate(
         self, *, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[GetGroupResponseOutputTypeDef]:
+    ) -> _PageIterator[GetGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#getgrouppaginator)
         """
 
 
 class ListAccessKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccessKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listaccesskeyspaginator)
     """
 
     def paginate(
         self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAccessKeysResponseOutputTypeDef]:
+    ) -> _PageIterator[ListAccessKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccessKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listaccesskeyspaginator)
         """
 
 
 class ListAccountAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccountAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listaccountaliasespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAccountAliasesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListAccountAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccountAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listaccountaliasespaginator)
         """
 
 
 class ListAttachedGroupPoliciesPaginator(Paginator):
@@ -252,15 +252,15 @@
 
     def paginate(
         self,
         *,
         GroupName: str,
         PathPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAttachedGroupPoliciesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListAttachedGroupPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedGroupPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listattachedgrouppoliciespaginator)
         """
 
 
 class ListAttachedRolePoliciesPaginator(Paginator):
@@ -271,15 +271,15 @@
 
     def paginate(
         self,
         *,
         RoleName: str,
         PathPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAttachedRolePoliciesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListAttachedRolePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedRolePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listattachedrolepoliciespaginator)
         """
 
 
 class ListAttachedUserPoliciesPaginator(Paginator):
@@ -290,15 +290,15 @@
 
     def paginate(
         self,
         *,
         UserName: str,
         PathPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAttachedUserPoliciesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListAttachedUserPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedUserPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listattacheduserpoliciespaginator)
         """
 
 
 class ListEntitiesForPolicyPaginator(Paginator):
@@ -311,150 +311,150 @@
         self,
         *,
         PolicyArn: str,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEntitiesForPolicyResponseOutputTypeDef]:
+    ) -> _PageIterator[ListEntitiesForPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListEntitiesForPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listentitiesforpolicypaginator)
         """
 
 
 class ListGroupPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgrouppoliciespaginator)
     """
 
     def paginate(
         self, *, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListGroupPoliciesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListGroupPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgrouppoliciespaginator)
         """
 
 
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListGroupsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgroupspaginator)
         """
 
 
 class ListGroupsForUserPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupsForUser)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgroupsforuserpaginator)
     """
 
     def paginate(
         self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListGroupsForUserResponseOutputTypeDef]:
+    ) -> _PageIterator[ListGroupsForUserResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupsForUser.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgroupsforuserpaginator)
         """
 
 
 class ListInstanceProfileTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfileTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofiletagspaginator)
     """
 
     def paginate(
         self, *, InstanceProfileName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceProfileTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListInstanceProfileTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfileTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofiletagspaginator)
         """
 
 
 class ListInstanceProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofilespaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceProfilesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListInstanceProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofilespaginator)
         """
 
 
 class ListInstanceProfilesForRolePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfilesForRole)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofilesforrolepaginator)
     """
 
     def paginate(
         self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceProfilesForRoleResponseOutputTypeDef]:
+    ) -> _PageIterator[ListInstanceProfilesForRoleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfilesForRole.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofilesforrolepaginator)
         """
 
 
 class ListMFADeviceTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADeviceTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listmfadevicetagspaginator)
     """
 
     def paginate(
         self, *, SerialNumber: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMFADeviceTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListMFADeviceTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADeviceTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listmfadevicetagspaginator)
         """
 
 
 class ListMFADevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listmfadevicespaginator)
     """
 
     def paginate(
         self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMFADevicesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListMFADevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listmfadevicespaginator)
         """
 
 
 class ListOpenIDConnectProviderTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListOpenIDConnectProviderTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listopenidconnectprovidertagspaginator)
     """
 
     def paginate(
         self, *, OpenIDConnectProviderArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListOpenIDConnectProviderTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListOpenIDConnectProviderTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListOpenIDConnectProviderTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listopenidconnectprovidertagspaginator)
         """
 
 
 class ListPoliciesPaginator(Paginator):
@@ -467,210 +467,210 @@
         self,
         *,
         Scope: policyScopeTypeType = ...,
         OnlyAttached: bool = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPoliciesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpoliciespaginator)
         """
 
 
 class ListPolicyTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpolicytagspaginator)
     """
 
     def paginate(
         self, *, PolicyArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPolicyTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListPolicyTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpolicytagspaginator)
         """
 
 
 class ListPolicyVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpolicyversionspaginator)
     """
 
     def paginate(
         self, *, PolicyArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPolicyVersionsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListPolicyVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpolicyversionspaginator)
         """
 
 
 class ListRolePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRolePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listrolepoliciespaginator)
     """
 
     def paginate(
         self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRolePoliciesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListRolePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRolePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listrolepoliciespaginator)
         """
 
 
 class ListRoleTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoleTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listroletagspaginator)
     """
 
     def paginate(
         self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRoleTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListRoleTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoleTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listroletagspaginator)
         """
 
 
 class ListRolesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listrolespaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRolesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListRolesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listrolespaginator)
         """
 
 
 class ListSAMLProviderTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSAMLProviderTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsamlprovidertagspaginator)
     """
 
     def paginate(
         self, *, SAMLProviderArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSAMLProviderTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSAMLProviderTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSAMLProviderTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsamlprovidertagspaginator)
         """
 
 
 class ListSSHPublicKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSSHPublicKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsshpublickeyspaginator)
     """
 
     def paginate(
         self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSSHPublicKeysResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSSHPublicKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSSHPublicKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsshpublickeyspaginator)
         """
 
 
 class ListServerCertificateTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificateTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listservercertificatetagspaginator)
     """
 
     def paginate(
         self, *, ServerCertificateName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServerCertificateTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListServerCertificateTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificateTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listservercertificatetagspaginator)
         """
 
 
 class ListServerCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listservercertificatespaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServerCertificatesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListServerCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listservercertificatespaginator)
         """
 
 
 class ListSigningCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSigningCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsigningcertificatespaginator)
     """
 
     def paginate(
         self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSigningCertificatesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSigningCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSigningCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsigningcertificatespaginator)
         """
 
 
 class ListUserPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listuserpoliciespaginator)
     """
 
     def paginate(
         self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUserPoliciesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUserPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listuserpoliciespaginator)
         """
 
 
 class ListUserTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listusertagspaginator)
     """
 
     def paginate(
         self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUserTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUserTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listusertagspaginator)
         """
 
 
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listuserspaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUsersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listuserspaginator)
         """
 
 
 class ListVirtualMFADevicesPaginator(Paginator):
@@ -680,15 +680,15 @@
     """
 
     def paginate(
         self,
         *,
         AssignmentStatus: assignmentStatusTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListVirtualMFADevicesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListVirtualMFADevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListVirtualMFADevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listvirtualmfadevicespaginator)
         """
 
 
 class SimulateCustomPolicyPaginator(Paginator):
@@ -706,15 +706,15 @@
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SimulatePolicyResponseOutputTypeDef]:
+    ) -> _PageIterator[SimulatePolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulateCustomPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#simulatecustompolicypaginator)
         """
 
 
 class SimulatePrincipalPolicyPaginator(Paginator):
@@ -733,12 +733,12 @@
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SimulatePolicyResponseOutputTypeDef]:
+    ) -> _PageIterator[SimulatePolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulatePrincipalPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#simulateprincipalpolicypaginator)
         """
```

### Comparing `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/paginator.pyi` & `mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -93,48 +93,48 @@
     EntityTypeType,
     PolicyUsageTypeType,
     assignmentStatusTypeType,
     policyScopeTypeType,
 )
 from .type_defs import (
     ContextEntryTypeDef,
-    GetAccountAuthorizationDetailsResponseOutputTypeDef,
-    GetGroupResponseOutputTypeDef,
-    ListAccessKeysResponseOutputTypeDef,
-    ListAccountAliasesResponseOutputTypeDef,
-    ListAttachedGroupPoliciesResponseOutputTypeDef,
-    ListAttachedRolePoliciesResponseOutputTypeDef,
-    ListAttachedUserPoliciesResponseOutputTypeDef,
-    ListEntitiesForPolicyResponseOutputTypeDef,
-    ListGroupPoliciesResponseOutputTypeDef,
-    ListGroupsForUserResponseOutputTypeDef,
-    ListGroupsResponseOutputTypeDef,
-    ListInstanceProfilesForRoleResponseOutputTypeDef,
-    ListInstanceProfilesResponseOutputTypeDef,
-    ListInstanceProfileTagsResponseOutputTypeDef,
-    ListMFADevicesResponseOutputTypeDef,
-    ListMFADeviceTagsResponseOutputTypeDef,
-    ListOpenIDConnectProviderTagsResponseOutputTypeDef,
-    ListPoliciesResponseOutputTypeDef,
-    ListPolicyTagsResponseOutputTypeDef,
-    ListPolicyVersionsResponseOutputTypeDef,
-    ListRolePoliciesResponseOutputTypeDef,
-    ListRolesResponseOutputTypeDef,
-    ListRoleTagsResponseOutputTypeDef,
-    ListSAMLProviderTagsResponseOutputTypeDef,
-    ListServerCertificatesResponseOutputTypeDef,
-    ListServerCertificateTagsResponseOutputTypeDef,
-    ListSigningCertificatesResponseOutputTypeDef,
-    ListSSHPublicKeysResponseOutputTypeDef,
-    ListUserPoliciesResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
-    ListUserTagsResponseOutputTypeDef,
-    ListVirtualMFADevicesResponseOutputTypeDef,
+    GetAccountAuthorizationDetailsResponseTypeDef,
+    GetGroupResponseTypeDef,
+    ListAccessKeysResponseTypeDef,
+    ListAccountAliasesResponseTypeDef,
+    ListAttachedGroupPoliciesResponseTypeDef,
+    ListAttachedRolePoliciesResponseTypeDef,
+    ListAttachedUserPoliciesResponseTypeDef,
+    ListEntitiesForPolicyResponseTypeDef,
+    ListGroupPoliciesResponseTypeDef,
+    ListGroupsForUserResponseTypeDef,
+    ListGroupsResponseTypeDef,
+    ListInstanceProfilesForRoleResponseTypeDef,
+    ListInstanceProfilesResponseTypeDef,
+    ListInstanceProfileTagsResponseTypeDef,
+    ListMFADevicesResponseTypeDef,
+    ListMFADeviceTagsResponseTypeDef,
+    ListOpenIDConnectProviderTagsResponseTypeDef,
+    ListPoliciesResponseTypeDef,
+    ListPolicyTagsResponseTypeDef,
+    ListPolicyVersionsResponseTypeDef,
+    ListRolePoliciesResponseTypeDef,
+    ListRolesResponseTypeDef,
+    ListRoleTagsResponseTypeDef,
+    ListSAMLProviderTagsResponseTypeDef,
+    ListServerCertificatesResponseTypeDef,
+    ListServerCertificateTagsResponseTypeDef,
+    ListSigningCertificatesResponseTypeDef,
+    ListSSHPublicKeysResponseTypeDef,
+    ListUserPoliciesResponseTypeDef,
+    ListUsersResponseTypeDef,
+    ListUserTagsResponseTypeDef,
+    ListVirtualMFADevicesResponseTypeDef,
     PaginatorConfigTypeDef,
-    SimulatePolicyResponseOutputTypeDef,
+    SimulatePolicyResponseTypeDef,
 )
 
 __all__ = (
     "GetAccountAuthorizationDetailsPaginator",
     "GetGroupPaginator",
     "ListAccessKeysPaginator",
     "ListAccountAliasesPaginator",
@@ -185,57 +185,57 @@
     """
 
     def paginate(
         self,
         *,
         Filter: Sequence[EntityTypeType] = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[GetAccountAuthorizationDetailsResponseOutputTypeDef]:
+    ) -> _PageIterator[GetAccountAuthorizationDetailsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetAccountAuthorizationDetails.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#getaccountauthorizationdetailspaginator)
         """
 
 class GetGroupPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#getgrouppaginator)
     """
 
     def paginate(
         self, *, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[GetGroupResponseOutputTypeDef]:
+    ) -> _PageIterator[GetGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.GetGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#getgrouppaginator)
         """
 
 class ListAccessKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccessKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listaccesskeyspaginator)
     """
 
     def paginate(
         self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAccessKeysResponseOutputTypeDef]:
+    ) -> _PageIterator[ListAccessKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccessKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listaccesskeyspaginator)
         """
 
 class ListAccountAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccountAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listaccountaliasespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAccountAliasesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListAccountAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAccountAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listaccountaliasespaginator)
         """
 
 class ListAttachedGroupPoliciesPaginator(Paginator):
     """
@@ -245,15 +245,15 @@
 
     def paginate(
         self,
         *,
         GroupName: str,
         PathPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAttachedGroupPoliciesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListAttachedGroupPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedGroupPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listattachedgrouppoliciespaginator)
         """
 
 class ListAttachedRolePoliciesPaginator(Paginator):
     """
@@ -263,15 +263,15 @@
 
     def paginate(
         self,
         *,
         RoleName: str,
         PathPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAttachedRolePoliciesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListAttachedRolePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedRolePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listattachedrolepoliciespaginator)
         """
 
 class ListAttachedUserPoliciesPaginator(Paginator):
     """
@@ -281,15 +281,15 @@
 
     def paginate(
         self,
         *,
         UserName: str,
         PathPrefix: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListAttachedUserPoliciesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListAttachedUserPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListAttachedUserPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listattacheduserpoliciespaginator)
         """
 
 class ListEntitiesForPolicyPaginator(Paginator):
     """
@@ -301,141 +301,141 @@
         self,
         *,
         PolicyArn: str,
         EntityFilter: EntityTypeType = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListEntitiesForPolicyResponseOutputTypeDef]:
+    ) -> _PageIterator[ListEntitiesForPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListEntitiesForPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listentitiesforpolicypaginator)
         """
 
 class ListGroupPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgrouppoliciespaginator)
     """
 
     def paginate(
         self, *, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListGroupPoliciesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListGroupPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgrouppoliciespaginator)
         """
 
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListGroupsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgroupspaginator)
         """
 
 class ListGroupsForUserPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupsForUser)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgroupsforuserpaginator)
     """
 
     def paginate(
         self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListGroupsForUserResponseOutputTypeDef]:
+    ) -> _PageIterator[ListGroupsForUserResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListGroupsForUser.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listgroupsforuserpaginator)
         """
 
 class ListInstanceProfileTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfileTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofiletagspaginator)
     """
 
     def paginate(
         self, *, InstanceProfileName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceProfileTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListInstanceProfileTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfileTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofiletagspaginator)
         """
 
 class ListInstanceProfilesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfiles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofilespaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceProfilesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListInstanceProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofilespaginator)
         """
 
 class ListInstanceProfilesForRolePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfilesForRole)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofilesforrolepaginator)
     """
 
     def paginate(
         self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListInstanceProfilesForRoleResponseOutputTypeDef]:
+    ) -> _PageIterator[ListInstanceProfilesForRoleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListInstanceProfilesForRole.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listinstanceprofilesforrolepaginator)
         """
 
 class ListMFADeviceTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADeviceTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listmfadevicetagspaginator)
     """
 
     def paginate(
         self, *, SerialNumber: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMFADeviceTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListMFADeviceTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADeviceTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listmfadevicetagspaginator)
         """
 
 class ListMFADevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listmfadevicespaginator)
     """
 
     def paginate(
         self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListMFADevicesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListMFADevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListMFADevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listmfadevicespaginator)
         """
 
 class ListOpenIDConnectProviderTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListOpenIDConnectProviderTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listopenidconnectprovidertagspaginator)
     """
 
     def paginate(
         self, *, OpenIDConnectProviderArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListOpenIDConnectProviderTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListOpenIDConnectProviderTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListOpenIDConnectProviderTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listopenidconnectprovidertagspaginator)
         """
 
 class ListPoliciesPaginator(Paginator):
     """
@@ -447,197 +447,197 @@
         self,
         *,
         Scope: policyScopeTypeType = ...,
         OnlyAttached: bool = ...,
         PathPrefix: str = ...,
         PolicyUsageFilter: PolicyUsageTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPoliciesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpoliciespaginator)
         """
 
 class ListPolicyTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpolicytagspaginator)
     """
 
     def paginate(
         self, *, PolicyArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPolicyTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListPolicyTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpolicytagspaginator)
         """
 
 class ListPolicyVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpolicyversionspaginator)
     """
 
     def paginate(
         self, *, PolicyArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListPolicyVersionsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListPolicyVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListPolicyVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listpolicyversionspaginator)
         """
 
 class ListRolePoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRolePolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listrolepoliciespaginator)
     """
 
     def paginate(
         self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRolePoliciesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListRolePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRolePolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listrolepoliciespaginator)
         """
 
 class ListRoleTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoleTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listroletagspaginator)
     """
 
     def paginate(
         self, *, RoleName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRoleTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListRoleTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoleTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listroletagspaginator)
         """
 
 class ListRolesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listrolespaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListRolesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListRolesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListRoles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listrolespaginator)
         """
 
 class ListSAMLProviderTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSAMLProviderTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsamlprovidertagspaginator)
     """
 
     def paginate(
         self, *, SAMLProviderArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSAMLProviderTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSAMLProviderTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSAMLProviderTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsamlprovidertagspaginator)
         """
 
 class ListSSHPublicKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSSHPublicKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsshpublickeyspaginator)
     """
 
     def paginate(
         self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSSHPublicKeysResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSSHPublicKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSSHPublicKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsshpublickeyspaginator)
         """
 
 class ListServerCertificateTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificateTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listservercertificatetagspaginator)
     """
 
     def paginate(
         self, *, ServerCertificateName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServerCertificateTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListServerCertificateTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificateTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listservercertificatetagspaginator)
         """
 
 class ListServerCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listservercertificatespaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListServerCertificatesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListServerCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListServerCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listservercertificatespaginator)
         """
 
 class ListSigningCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSigningCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsigningcertificatespaginator)
     """
 
     def paginate(
         self, *, UserName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListSigningCertificatesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListSigningCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListSigningCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listsigningcertificatespaginator)
         """
 
 class ListUserPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listuserpoliciespaginator)
     """
 
     def paginate(
         self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUserPoliciesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUserPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listuserpoliciespaginator)
         """
 
 class ListUserTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listusertagspaginator)
     """
 
     def paginate(
         self, *, UserName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUserTagsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUserTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUserTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listusertagspaginator)
         """
 
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listuserspaginator)
     """
 
     def paginate(
         self, *, PathPrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListUsersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listuserspaginator)
         """
 
 class ListVirtualMFADevicesPaginator(Paginator):
     """
@@ -646,15 +646,15 @@
     """
 
     def paginate(
         self,
         *,
         AssignmentStatus: assignmentStatusTypeType = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[ListVirtualMFADevicesResponseOutputTypeDef]:
+    ) -> _PageIterator[ListVirtualMFADevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.ListVirtualMFADevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#listvirtualmfadevicespaginator)
         """
 
 class SimulateCustomPolicyPaginator(Paginator):
     """
@@ -671,15 +671,15 @@
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SimulatePolicyResponseOutputTypeDef]:
+    ) -> _PageIterator[SimulatePolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulateCustomPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#simulatecustompolicypaginator)
         """
 
 class SimulatePrincipalPolicyPaginator(Paginator):
     """
@@ -697,12 +697,12 @@
         ResourceArns: Sequence[str] = ...,
         ResourcePolicy: str = ...,
         ResourceOwner: str = ...,
         CallerArn: str = ...,
         ContextEntries: Sequence[ContextEntryTypeDef] = ...,
         ResourceHandlingOption: str = ...,
         PaginationConfig: "PaginatorConfigTypeDef" = ...
-    ) -> _PageIterator[SimulatePolicyResponseOutputTypeDef]:
+    ) -> _PageIterator[SimulatePolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Paginator.SimulatePrincipalPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/paginators/#simulateprincipalpolicypaginator)
         """
```

### Comparing `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/service_resource.py` & `mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,19 +51,19 @@
     policyScopeTypeType,
     statusTypeType,
     summaryKeyTypeType,
 )
 from .type_defs import (
     AttachedPermissionsBoundaryResponseMetadataTypeDef,
     RoleLastUsedResponseMetadataTypeDef,
-    RoleOutputTypeDef,
+    RoleTypeDef,
     ServerCertificateMetadataResponseMetadataTypeDef,
     TagOutputTypeDef,
     TagTypeDef,
-    UpdateSAMLProviderResponseOutputTypeDef,
+    UpdateSAMLProviderResponseTypeDef,
     UserResponseMetadataTypeDef,
 )
 
 __all__ = (
     "IAMServiceResource",
     "AccessKey",
     "AccessKeyPair",
@@ -1466,15 +1466,15 @@
     """
 
     path: str
     instance_profile_name: str
     instance_profile_id: str
     arn: str
     create_date: datetime
-    roles_attribute: List[RoleOutputTypeDef]
+    roles_attribute: List[RoleTypeDef]
     tags: List[TagOutputTypeDef]
     name: str
     roles: List["Role"]
 
     def add_role(self, *, RoleName: str) -> None:
         """
         Adds the specified IAM role to the specified instance profile.
@@ -1630,15 +1630,15 @@
         Calls :py:meth:`IAM.Client.get_saml_provider` to update the attributes of the
         SamlProvider resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.reload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#samlproviderreload-method)
         """
 
-    def update(self, *, SAMLMetadataDocument: str) -> UpdateSAMLProviderResponseOutputTypeDef:
+    def update(self, *, SAMLMetadataDocument: str) -> UpdateSAMLProviderResponseTypeDef:
         """
         Updates the metadata document for an existing SAML provider resource object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#samlproviderupdate-method)
         """
```

### Comparing `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/service_resource.pyi` & `mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -51,19 +51,19 @@
     policyScopeTypeType,
     statusTypeType,
     summaryKeyTypeType,
 )
 from .type_defs import (
     AttachedPermissionsBoundaryResponseMetadataTypeDef,
     RoleLastUsedResponseMetadataTypeDef,
-    RoleOutputTypeDef,
+    RoleTypeDef,
     ServerCertificateMetadataResponseMetadataTypeDef,
     TagOutputTypeDef,
     TagTypeDef,
-    UpdateSAMLProviderResponseOutputTypeDef,
+    UpdateSAMLProviderResponseTypeDef,
     UserResponseMetadataTypeDef,
 )
 
 __all__ = (
     "IAMServiceResource",
     "AccessKey",
     "AccessKeyPair",
@@ -1284,15 +1284,15 @@
     """
 
     path: str
     instance_profile_name: str
     instance_profile_id: str
     arn: str
     create_date: datetime
-    roles_attribute: List[RoleOutputTypeDef]
+    roles_attribute: List[RoleTypeDef]
     tags: List[TagOutputTypeDef]
     name: str
     roles: List["Role"]
 
     def add_role(self, *, RoleName: str) -> None:
         """
         Adds the specified IAM role to the specified instance profile.
@@ -1431,15 +1431,15 @@
         """
         Calls :py:meth:`IAM.Client.get_saml_provider` to update the attributes of the
         SamlProvider resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.reload)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#samlproviderreload-method)
         """
-    def update(self, *, SAMLMetadataDocument: str) -> UpdateSAMLProviderResponseOutputTypeDef:
+    def update(self, *, SAMLMetadataDocument: str) -> UpdateSAMLProviderResponseTypeDef:
         """
         Updates the metadata document for an existing SAML provider resource object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.SamlProvider.update)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/service_resource/#samlproviderupdate-method)
         """
```

### Comparing `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/type_defs.py` & `mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iam service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iam.type_defs import AccessDetailOutputTypeDef
+    from mypy_boto3_iam.type_defs import AccessDetailTypeDef
 
-    data: AccessDetailOutputTypeDef = {...}
+    data: AccessDetailTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -43,18 +43,18 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AccessDetailOutputTypeDef",
-    "AccessKeyLastUsedOutputTypeDef",
-    "AccessKeyMetadataOutputTypeDef",
-    "AccessKeyOutputTypeDef",
+    "AccessDetailTypeDef",
+    "AccessKeyLastUsedTypeDef",
+    "AccessKeyMetadataTypeDef",
+    "AccessKeyTypeDef",
     "AddClientIDToOpenIDConnectProviderRequestRequestTypeDef",
     "AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef",
     "AddRoleToInstanceProfileRequestRequestTypeDef",
     "AddUserToGroupRequestGroupAddUserTypeDef",
     "AddUserToGroupRequestRequestTypeDef",
     "AddUserToGroupRequestUserAddGroupTypeDef",
     "AttachGroupPolicyRequestGroupAttachPolicyTypeDef",
@@ -62,39 +62,39 @@
     "AttachGroupPolicyRequestRequestTypeDef",
     "AttachRolePolicyRequestPolicyAttachRoleTypeDef",
     "AttachRolePolicyRequestRequestTypeDef",
     "AttachRolePolicyRequestRoleAttachPolicyTypeDef",
     "AttachUserPolicyRequestPolicyAttachUserTypeDef",
     "AttachUserPolicyRequestRequestTypeDef",
     "AttachUserPolicyRequestUserAttachPolicyTypeDef",
-    "AttachedPermissionsBoundaryOutputTypeDef",
     "AttachedPermissionsBoundaryResponseMetadataTypeDef",
-    "AttachedPolicyOutputTypeDef",
+    "AttachedPermissionsBoundaryTypeDef",
+    "AttachedPolicyTypeDef",
     "ChangePasswordRequestRequestTypeDef",
     "ChangePasswordRequestServiceResourceChangePasswordTypeDef",
     "ContextEntryTypeDef",
     "CreateAccessKeyRequestRequestTypeDef",
     "CreateAccountAliasRequestRequestTypeDef",
     "CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef",
     "CreateGroupRequestGroupCreateTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "CreateGroupRequestServiceResourceCreateGroupTypeDef",
-    "GroupOutputTypeDef",
+    "GroupTypeDef",
     "TagTypeDef",
     "CreateLoginProfileRequestLoginProfileCreateTypeDef",
     "CreateLoginProfileRequestRequestTypeDef",
     "CreateLoginProfileRequestUserCreateLoginProfileTypeDef",
-    "LoginProfileOutputTypeDef",
+    "LoginProfileTypeDef",
     "TagOutputTypeDef",
     "CreatePolicyVersionRequestPolicyCreateVersionTypeDef",
     "CreatePolicyVersionRequestRequestTypeDef",
-    "PolicyVersionOutputTypeDef",
+    "PolicyVersionTypeDef",
     "CreateServiceLinkedRoleRequestRequestTypeDef",
     "CreateServiceSpecificCredentialRequestRequestTypeDef",
-    "ServiceSpecificCredentialOutputTypeDef",
+    "ServiceSpecificCredentialTypeDef",
     "DeactivateMFADeviceRequestRequestTypeDef",
     "DeleteAccessKeyRequestRequestTypeDef",
     "DeleteAccountAliasRequestRequestTypeDef",
     "DeleteGroupPolicyRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteInstanceProfileRequestRequestTypeDef",
     "DeleteLoginProfileRequestRequestTypeDef",
@@ -104,159 +104,159 @@
     "DeleteRolePermissionsBoundaryRequestRequestTypeDef",
     "DeleteRolePolicyRequestRequestTypeDef",
     "DeleteRoleRequestRequestTypeDef",
     "DeleteSAMLProviderRequestRequestTypeDef",
     "DeleteSSHPublicKeyRequestRequestTypeDef",
     "DeleteServerCertificateRequestRequestTypeDef",
     "DeleteServiceLinkedRoleRequestRequestTypeDef",
-    "DeleteServiceLinkedRoleResponseOutputTypeDef",
+    "DeleteServiceLinkedRoleResponseTypeDef",
     "DeleteServiceSpecificCredentialRequestRequestTypeDef",
     "DeleteSigningCertificateRequestRequestTypeDef",
     "DeleteUserPermissionsBoundaryRequestRequestTypeDef",
     "DeleteUserPolicyRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeleteVirtualMFADeviceRequestRequestTypeDef",
-    "RoleUsageTypeOutputTypeDef",
+    "RoleUsageTypeTypeDef",
     "DetachGroupPolicyRequestGroupDetachPolicyTypeDef",
     "DetachGroupPolicyRequestPolicyDetachGroupTypeDef",
     "DetachGroupPolicyRequestRequestTypeDef",
     "DetachRolePolicyRequestPolicyDetachRoleTypeDef",
     "DetachRolePolicyRequestRequestTypeDef",
     "DetachRolePolicyRequestRoleDetachPolicyTypeDef",
     "DetachUserPolicyRequestPolicyDetachUserTypeDef",
     "DetachUserPolicyRequestRequestTypeDef",
     "DetachUserPolicyRequestUserDetachPolicyTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnableMFADeviceRequestMfaDeviceAssociateTypeDef",
     "EnableMFADeviceRequestRequestTypeDef",
     "EnableMFADeviceRequestUserEnableMfaTypeDef",
-    "EntityInfoOutputTypeDef",
-    "ErrorDetailsOutputTypeDef",
-    "OrganizationsDecisionDetailOutputTypeDef",
-    "PermissionsBoundaryDecisionDetailOutputTypeDef",
-    "GenerateCredentialReportResponseOutputTypeDef",
+    "EntityInfoTypeDef",
+    "ErrorDetailsTypeDef",
+    "OrganizationsDecisionDetailTypeDef",
+    "PermissionsBoundaryDecisionDetailTypeDef",
+    "GenerateCredentialReportResponseTypeDef",
     "GenerateOrganizationsAccessReportRequestRequestTypeDef",
-    "GenerateOrganizationsAccessReportResponseOutputTypeDef",
+    "GenerateOrganizationsAccessReportResponseTypeDef",
     "GenerateServiceLastAccessedDetailsRequestRequestTypeDef",
-    "GenerateServiceLastAccessedDetailsResponseOutputTypeDef",
+    "GenerateServiceLastAccessedDetailsResponseTypeDef",
     "GetAccessKeyLastUsedRequestRequestTypeDef",
     "GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef",
     "GetAccountAuthorizationDetailsRequestRequestTypeDef",
-    "PasswordPolicyOutputTypeDef",
-    "GetAccountSummaryResponseOutputTypeDef",
+    "PasswordPolicyTypeDef",
+    "GetAccountSummaryResponseTypeDef",
     "GetContextKeysForCustomPolicyRequestRequestTypeDef",
-    "GetContextKeysForPolicyResponseOutputTypeDef",
+    "GetContextKeysForPolicyResponseTypeDef",
     "GetContextKeysForPrincipalPolicyRequestRequestTypeDef",
-    "GetCredentialReportResponseOutputTypeDef",
+    "GetCredentialReportResponseTypeDef",
     "GetGroupPolicyRequestRequestTypeDef",
-    "GetGroupPolicyResponseOutputTypeDef",
+    "GetGroupPolicyResponseTypeDef",
     "GetGroupRequestGetGroupPaginateTypeDef",
     "GetGroupRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetInstanceProfileRequestRequestTypeDef",
     "GetLoginProfileRequestRequestTypeDef",
     "GetMFADeviceRequestRequestTypeDef",
-    "GetMFADeviceResponseOutputTypeDef",
+    "GetMFADeviceResponseTypeDef",
     "GetOpenIDConnectProviderRequestRequestTypeDef",
     "GetOrganizationsAccessReportRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetPolicyVersionRequestRequestTypeDef",
     "GetRolePolicyRequestRequestTypeDef",
-    "GetRolePolicyResponseOutputTypeDef",
+    "GetRolePolicyResponseTypeDef",
     "GetRoleRequestRequestTypeDef",
     "GetSAMLProviderRequestRequestTypeDef",
     "GetSSHPublicKeyRequestRequestTypeDef",
-    "SSHPublicKeyOutputTypeDef",
+    "SSHPublicKeyTypeDef",
     "GetServerCertificateRequestRequestTypeDef",
     "GetServiceLastAccessedDetailsRequestRequestTypeDef",
     "GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef",
     "GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef",
     "GetUserPolicyRequestRequestTypeDef",
-    "GetUserPolicyResponseOutputTypeDef",
+    "GetUserPolicyResponseTypeDef",
     "GetUserRequestRequestTypeDef",
-    "PolicyDetailOutputTypeDef",
+    "PolicyDetailTypeDef",
     "ListAccessKeysRequestListAccessKeysPaginateTypeDef",
     "ListAccessKeysRequestRequestTypeDef",
     "ListAccountAliasesRequestListAccountAliasesPaginateTypeDef",
     "ListAccountAliasesRequestRequestTypeDef",
-    "ListAccountAliasesResponseOutputTypeDef",
+    "ListAccountAliasesResponseTypeDef",
     "ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef",
     "ListAttachedGroupPoliciesRequestRequestTypeDef",
     "ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef",
     "ListAttachedRolePoliciesRequestRequestTypeDef",
     "ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef",
     "ListAttachedUserPoliciesRequestRequestTypeDef",
     "ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef",
     "ListEntitiesForPolicyRequestRequestTypeDef",
-    "PolicyGroupOutputTypeDef",
-    "PolicyRoleOutputTypeDef",
-    "PolicyUserOutputTypeDef",
+    "PolicyGroupTypeDef",
+    "PolicyRoleTypeDef",
+    "PolicyUserTypeDef",
     "ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
     "ListGroupPoliciesRequestRequestTypeDef",
-    "ListGroupPoliciesResponseOutputTypeDef",
+    "ListGroupPoliciesResponseTypeDef",
     "ListGroupsForUserRequestListGroupsForUserPaginateTypeDef",
     "ListGroupsForUserRequestRequestTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef",
     "ListInstanceProfileTagsRequestRequestTypeDef",
     "ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef",
     "ListInstanceProfilesForRoleRequestRequestTypeDef",
     "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     "ListInstanceProfilesRequestRequestTypeDef",
     "ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef",
     "ListMFADeviceTagsRequestRequestTypeDef",
     "ListMFADevicesRequestListMFADevicesPaginateTypeDef",
     "ListMFADevicesRequestRequestTypeDef",
-    "MFADeviceOutputTypeDef",
+    "MFADeviceTypeDef",
     "ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef",
     "ListOpenIDConnectProviderTagsRequestRequestTypeDef",
-    "OpenIDConnectProviderListEntryOutputTypeDef",
-    "PolicyGrantingServiceAccessOutputTypeDef",
+    "OpenIDConnectProviderListEntryTypeDef",
+    "PolicyGrantingServiceAccessTypeDef",
     "ListPoliciesGrantingServiceAccessRequestRequestTypeDef",
     "ListPoliciesRequestListPoliciesPaginateTypeDef",
     "ListPoliciesRequestRequestTypeDef",
     "ListPolicyTagsRequestListPolicyTagsPaginateTypeDef",
     "ListPolicyTagsRequestRequestTypeDef",
     "ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef",
     "ListPolicyVersionsRequestRequestTypeDef",
     "ListRolePoliciesRequestListRolePoliciesPaginateTypeDef",
     "ListRolePoliciesRequestRequestTypeDef",
-    "ListRolePoliciesResponseOutputTypeDef",
+    "ListRolePoliciesResponseTypeDef",
     "ListRoleTagsRequestListRoleTagsPaginateTypeDef",
     "ListRoleTagsRequestRequestTypeDef",
     "ListRolesRequestListRolesPaginateTypeDef",
     "ListRolesRequestRequestTypeDef",
     "ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef",
     "ListSAMLProviderTagsRequestRequestTypeDef",
-    "SAMLProviderListEntryOutputTypeDef",
+    "SAMLProviderListEntryTypeDef",
     "ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef",
     "ListSSHPublicKeysRequestRequestTypeDef",
-    "SSHPublicKeyMetadataOutputTypeDef",
+    "SSHPublicKeyMetadataTypeDef",
     "ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef",
     "ListServerCertificateTagsRequestRequestTypeDef",
     "ListServerCertificatesRequestListServerCertificatesPaginateTypeDef",
     "ListServerCertificatesRequestRequestTypeDef",
-    "ServerCertificateMetadataOutputTypeDef",
+    "ServerCertificateMetadataTypeDef",
     "ListServiceSpecificCredentialsRequestRequestTypeDef",
-    "ServiceSpecificCredentialMetadataOutputTypeDef",
+    "ServiceSpecificCredentialMetadataTypeDef",
     "ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef",
     "ListSigningCertificatesRequestRequestTypeDef",
-    "SigningCertificateOutputTypeDef",
+    "SigningCertificateTypeDef",
     "ListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
     "ListUserPoliciesRequestRequestTypeDef",
-    "ListUserPoliciesResponseOutputTypeDef",
+    "ListUserPoliciesResponseTypeDef",
     "ListUserTagsRequestListUserTagsPaginateTypeDef",
     "ListUserTagsRequestRequestTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef",
     "ListVirtualMFADevicesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "PositionOutputTypeDef",
+    "PositionTypeDef",
     "PutGroupPolicyRequestGroupCreatePolicyTypeDef",
     "PutGroupPolicyRequestGroupPolicyPutTypeDef",
     "PutGroupPolicyRequestRequestTypeDef",
     "PutRolePermissionsBoundaryRequestRequestTypeDef",
     "PutRolePolicyRequestRequestTypeDef",
     "PutRolePolicyRequestRolePolicyPutTypeDef",
     "PutUserPermissionsBoundaryRequestRequestTypeDef",
@@ -269,18 +269,18 @@
     "RemoveUserFromGroupRequestGroupRemoveUserTypeDef",
     "RemoveUserFromGroupRequestRequestTypeDef",
     "RemoveUserFromGroupRequestUserRemoveGroupTypeDef",
     "ResetServiceSpecificCredentialRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ResyncMFADeviceRequestMfaDeviceResyncTypeDef",
     "ResyncMFADeviceRequestRequestTypeDef",
-    "RoleLastUsedOutputTypeDef",
+    "RoleLastUsedTypeDef",
     "RoleLastUsedResponseMetadataTypeDef",
     "ServerCertificateMetadataResponseMetadataTypeDef",
-    "TrackedActionLastAccessedOutputTypeDef",
+    "TrackedActionLastAccessedTypeDef",
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     "SetSecurityTokenServicePreferencesRequestRequestTypeDef",
     "UntagInstanceProfileRequestRequestTypeDef",
     "UntagMFADeviceRequestRequestTypeDef",
     "UntagOpenIDConnectProviderRequestRequestTypeDef",
     "UntagPolicyRequestRequestTypeDef",
     "UntagRoleRequestRequestTypeDef",
@@ -302,40 +302,40 @@
     "UpdateLoginProfileRequestLoginProfileUpdateTypeDef",
     "UpdateLoginProfileRequestRequestTypeDef",
     "UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef",
     "UpdateRoleDescriptionRequestRequestTypeDef",
     "UpdateRoleRequestRequestTypeDef",
     "UpdateSAMLProviderRequestRequestTypeDef",
     "UpdateSAMLProviderRequestSamlProviderUpdateTypeDef",
-    "UpdateSAMLProviderResponseOutputTypeDef",
+    "UpdateSAMLProviderResponseTypeDef",
     "UpdateSSHPublicKeyRequestRequestTypeDef",
     "UpdateServerCertificateRequestRequestTypeDef",
     "UpdateServerCertificateRequestServerCertificateUpdateTypeDef",
     "UpdateServiceSpecificCredentialRequestRequestTypeDef",
     "UpdateSigningCertificateRequestRequestTypeDef",
     "UpdateSigningCertificateRequestSigningCertificateActivateTypeDef",
     "UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateUserRequestUserUpdateTypeDef",
     "UploadSSHPublicKeyRequestRequestTypeDef",
     "UploadSigningCertificateRequestRequestTypeDef",
     "UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef",
-    "GetAccessKeyLastUsedResponseOutputTypeDef",
-    "ListAccessKeysResponseOutputTypeDef",
-    "CreateAccessKeyResponseOutputTypeDef",
-    "ListAttachedGroupPoliciesResponseOutputTypeDef",
-    "ListAttachedRolePoliciesResponseOutputTypeDef",
-    "ListAttachedUserPoliciesResponseOutputTypeDef",
+    "GetAccessKeyLastUsedResponseTypeDef",
+    "ListAccessKeysResponseTypeDef",
+    "CreateAccessKeyResponseTypeDef",
+    "ListAttachedGroupPoliciesResponseTypeDef",
+    "ListAttachedRolePoliciesResponseTypeDef",
+    "ListAttachedUserPoliciesResponseTypeDef",
     "SimulateCustomPolicyRequestRequestTypeDef",
     "SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef",
     "SimulatePrincipalPolicyRequestRequestTypeDef",
     "SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef",
-    "CreateGroupResponseOutputTypeDef",
-    "ListGroupsForUserResponseOutputTypeDef",
-    "ListGroupsResponseOutputTypeDef",
+    "CreateGroupResponseTypeDef",
+    "ListGroupsForUserResponseTypeDef",
+    "ListGroupsResponseTypeDef",
     "CreateInstanceProfileRequestRequestTypeDef",
     "CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef",
     "CreateOpenIDConnectProviderRequestRequestTypeDef",
     "CreatePolicyRequestRequestTypeDef",
     "CreatePolicyRequestServiceResourceCreatePolicyTypeDef",
     "CreateRoleRequestRequestTypeDef",
     "CreateRoleRequestServiceResourceCreateRoleTypeDef",
@@ -352,129 +352,129 @@
     "TagPolicyRequestRequestTypeDef",
     "TagRoleRequestRequestTypeDef",
     "TagSAMLProviderRequestRequestTypeDef",
     "TagServerCertificateRequestRequestTypeDef",
     "TagUserRequestRequestTypeDef",
     "UploadServerCertificateRequestRequestTypeDef",
     "UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef",
-    "CreateLoginProfileResponseOutputTypeDef",
-    "GetLoginProfileResponseOutputTypeDef",
-    "CreateOpenIDConnectProviderResponseOutputTypeDef",
-    "CreateSAMLProviderResponseOutputTypeDef",
-    "GetOpenIDConnectProviderResponseOutputTypeDef",
-    "GetSAMLProviderResponseOutputTypeDef",
-    "ListInstanceProfileTagsResponseOutputTypeDef",
-    "ListMFADeviceTagsResponseOutputTypeDef",
-    "ListOpenIDConnectProviderTagsResponseOutputTypeDef",
-    "ListPolicyTagsResponseOutputTypeDef",
-    "ListRoleTagsResponseOutputTypeDef",
-    "ListSAMLProviderTagsResponseOutputTypeDef",
-    "ListServerCertificateTagsResponseOutputTypeDef",
-    "ListUserTagsResponseOutputTypeDef",
-    "PolicyOutputTypeDef",
-    "UserOutputTypeDef",
+    "CreateLoginProfileResponseTypeDef",
+    "GetLoginProfileResponseTypeDef",
+    "CreateOpenIDConnectProviderResponseTypeDef",
+    "CreateSAMLProviderResponseTypeDef",
+    "GetOpenIDConnectProviderResponseTypeDef",
+    "GetSAMLProviderResponseTypeDef",
+    "ListInstanceProfileTagsResponseTypeDef",
+    "ListMFADeviceTagsResponseTypeDef",
+    "ListOpenIDConnectProviderTagsResponseTypeDef",
+    "ListPolicyTagsResponseTypeDef",
+    "ListRoleTagsResponseTypeDef",
+    "ListSAMLProviderTagsResponseTypeDef",
+    "ListServerCertificateTagsResponseTypeDef",
+    "ListUserTagsResponseTypeDef",
+    "PolicyTypeDef",
     "UserResponseMetadataTypeDef",
-    "CreatePolicyVersionResponseOutputTypeDef",
-    "GetPolicyVersionResponseOutputTypeDef",
-    "ListPolicyVersionsResponseOutputTypeDef",
-    "ManagedPolicyDetailOutputTypeDef",
-    "CreateServiceSpecificCredentialResponseOutputTypeDef",
-    "ResetServiceSpecificCredentialResponseOutputTypeDef",
-    "DeletionTaskFailureReasonTypeOutputTypeDef",
-    "EntityDetailsOutputTypeDef",
-    "GetOrganizationsAccessReportResponseOutputTypeDef",
-    "GetAccountPasswordPolicyResponseOutputTypeDef",
+    "UserTypeDef",
+    "CreatePolicyVersionResponseTypeDef",
+    "GetPolicyVersionResponseTypeDef",
+    "ListPolicyVersionsResponseTypeDef",
+    "ManagedPolicyDetailTypeDef",
+    "CreateServiceSpecificCredentialResponseTypeDef",
+    "ResetServiceSpecificCredentialResponseTypeDef",
+    "DeletionTaskFailureReasonTypeTypeDef",
+    "EntityDetailsTypeDef",
+    "GetOrganizationsAccessReportResponseTypeDef",
+    "GetAccountPasswordPolicyResponseTypeDef",
     "GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef",
     "GetPolicyRequestPolicyExistsWaitTypeDef",
     "GetRoleRequestRoleExistsWaitTypeDef",
     "GetUserRequestUserExistsWaitTypeDef",
-    "GetSSHPublicKeyResponseOutputTypeDef",
-    "UploadSSHPublicKeyResponseOutputTypeDef",
-    "GroupDetailOutputTypeDef",
-    "UserDetailOutputTypeDef",
-    "ListEntitiesForPolicyResponseOutputTypeDef",
-    "ListMFADevicesResponseOutputTypeDef",
-    "ListOpenIDConnectProvidersResponseOutputTypeDef",
-    "ListPoliciesGrantingServiceAccessEntryOutputTypeDef",
-    "ListSAMLProvidersResponseOutputTypeDef",
-    "ListSSHPublicKeysResponseOutputTypeDef",
-    "ListServerCertificatesResponseOutputTypeDef",
-    "ServerCertificateOutputTypeDef",
-    "UploadServerCertificateResponseOutputTypeDef",
-    "ListServiceSpecificCredentialsResponseOutputTypeDef",
-    "ListSigningCertificatesResponseOutputTypeDef",
-    "UploadSigningCertificateResponseOutputTypeDef",
-    "StatementOutputTypeDef",
-    "RoleOutputTypeDef",
-    "ServiceLastAccessedOutputTypeDef",
-    "CreatePolicyResponseOutputTypeDef",
-    "GetPolicyResponseOutputTypeDef",
-    "ListPoliciesResponseOutputTypeDef",
-    "CreateUserResponseOutputTypeDef",
-    "GetGroupResponseOutputTypeDef",
-    "GetUserResponseOutputTypeDef",
-    "ListUsersResponseOutputTypeDef",
-    "VirtualMFADeviceOutputTypeDef",
-    "GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef",
-    "GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef",
-    "ListPoliciesGrantingServiceAccessResponseOutputTypeDef",
-    "GetServerCertificateResponseOutputTypeDef",
-    "ResourceSpecificResultOutputTypeDef",
-    "CreateRoleResponseOutputTypeDef",
-    "CreateServiceLinkedRoleResponseOutputTypeDef",
-    "GetRoleResponseOutputTypeDef",
-    "InstanceProfileOutputTypeDef",
-    "ListRolesResponseOutputTypeDef",
-    "UpdateRoleDescriptionResponseOutputTypeDef",
-    "GetServiceLastAccessedDetailsResponseOutputTypeDef",
-    "CreateVirtualMFADeviceResponseOutputTypeDef",
-    "ListVirtualMFADevicesResponseOutputTypeDef",
-    "EvaluationResultOutputTypeDef",
-    "CreateInstanceProfileResponseOutputTypeDef",
-    "GetInstanceProfileResponseOutputTypeDef",
-    "ListInstanceProfilesForRoleResponseOutputTypeDef",
-    "ListInstanceProfilesResponseOutputTypeDef",
-    "RoleDetailOutputTypeDef",
-    "SimulatePolicyResponseOutputTypeDef",
-    "GetAccountAuthorizationDetailsResponseOutputTypeDef",
+    "GetSSHPublicKeyResponseTypeDef",
+    "UploadSSHPublicKeyResponseTypeDef",
+    "GroupDetailTypeDef",
+    "UserDetailTypeDef",
+    "ListEntitiesForPolicyResponseTypeDef",
+    "ListMFADevicesResponseTypeDef",
+    "ListOpenIDConnectProvidersResponseTypeDef",
+    "ListPoliciesGrantingServiceAccessEntryTypeDef",
+    "ListSAMLProvidersResponseTypeDef",
+    "ListSSHPublicKeysResponseTypeDef",
+    "ListServerCertificatesResponseTypeDef",
+    "ServerCertificateTypeDef",
+    "UploadServerCertificateResponseTypeDef",
+    "ListServiceSpecificCredentialsResponseTypeDef",
+    "ListSigningCertificatesResponseTypeDef",
+    "UploadSigningCertificateResponseTypeDef",
+    "StatementTypeDef",
+    "RoleTypeDef",
+    "ServiceLastAccessedTypeDef",
+    "CreatePolicyResponseTypeDef",
+    "GetPolicyResponseTypeDef",
+    "ListPoliciesResponseTypeDef",
+    "CreateUserResponseTypeDef",
+    "GetGroupResponseTypeDef",
+    "GetUserResponseTypeDef",
+    "ListUsersResponseTypeDef",
+    "VirtualMFADeviceTypeDef",
+    "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
+    "GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef",
+    "ListPoliciesGrantingServiceAccessResponseTypeDef",
+    "GetServerCertificateResponseTypeDef",
+    "ResourceSpecificResultTypeDef",
+    "CreateRoleResponseTypeDef",
+    "CreateServiceLinkedRoleResponseTypeDef",
+    "GetRoleResponseTypeDef",
+    "InstanceProfileTypeDef",
+    "ListRolesResponseTypeDef",
+    "UpdateRoleDescriptionResponseTypeDef",
+    "GetServiceLastAccessedDetailsResponseTypeDef",
+    "CreateVirtualMFADeviceResponseTypeDef",
+    "ListVirtualMFADevicesResponseTypeDef",
+    "EvaluationResultTypeDef",
+    "CreateInstanceProfileResponseTypeDef",
+    "GetInstanceProfileResponseTypeDef",
+    "ListInstanceProfilesForRoleResponseTypeDef",
+    "ListInstanceProfilesResponseTypeDef",
+    "RoleDetailTypeDef",
+    "SimulatePolicyResponseTypeDef",
+    "GetAccountAuthorizationDetailsResponseTypeDef",
 )
 
-AccessDetailOutputTypeDef = TypedDict(
-    "AccessDetailOutputTypeDef",
+AccessDetailTypeDef = TypedDict(
+    "AccessDetailTypeDef",
     {
         "ServiceName": str,
         "ServiceNamespace": str,
         "Region": str,
         "EntityPath": str,
         "LastAuthenticatedTime": datetime,
         "TotalAuthenticatedEntities": int,
     },
 )
 
-AccessKeyLastUsedOutputTypeDef = TypedDict(
-    "AccessKeyLastUsedOutputTypeDef",
+AccessKeyLastUsedTypeDef = TypedDict(
+    "AccessKeyLastUsedTypeDef",
     {
         "LastUsedDate": datetime,
         "ServiceName": str,
         "Region": str,
     },
 )
 
-AccessKeyMetadataOutputTypeDef = TypedDict(
-    "AccessKeyMetadataOutputTypeDef",
+AccessKeyMetadataTypeDef = TypedDict(
+    "AccessKeyMetadataTypeDef",
     {
         "UserName": str,
         "AccessKeyId": str,
         "Status": statusTypeType,
         "CreateDate": datetime,
     },
 )
 
-AccessKeyOutputTypeDef = TypedDict(
-    "AccessKeyOutputTypeDef",
+AccessKeyTypeDef = TypedDict(
+    "AccessKeyTypeDef",
     {
         "UserName": str,
         "AccessKeyId": str,
         "Status": statusTypeType,
         "SecretAccessKey": str,
         "CreateDate": datetime,
     },
@@ -587,33 +587,33 @@
 AttachUserPolicyRequestUserAttachPolicyTypeDef = TypedDict(
     "AttachUserPolicyRequestUserAttachPolicyTypeDef",
     {
         "PolicyArn": str,
     },
 )
 
-AttachedPermissionsBoundaryOutputTypeDef = TypedDict(
-    "AttachedPermissionsBoundaryOutputTypeDef",
+AttachedPermissionsBoundaryResponseMetadataTypeDef = TypedDict(
+    "AttachedPermissionsBoundaryResponseMetadataTypeDef",
     {
         "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
         "PermissionsBoundaryArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AttachedPermissionsBoundaryResponseMetadataTypeDef = TypedDict(
-    "AttachedPermissionsBoundaryResponseMetadataTypeDef",
+AttachedPermissionsBoundaryTypeDef = TypedDict(
+    "AttachedPermissionsBoundaryTypeDef",
     {
         "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
         "PermissionsBoundaryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AttachedPolicyOutputTypeDef = TypedDict(
-    "AttachedPolicyOutputTypeDef",
+AttachedPolicyTypeDef = TypedDict(
+    "AttachedPolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyArn": str,
     },
 )
 
 ChangePasswordRequestRequestTypeDef = TypedDict(
@@ -711,16 +711,16 @@
 class CreateGroupRequestServiceResourceCreateGroupTypeDef(
     _RequiredCreateGroupRequestServiceResourceCreateGroupTypeDef,
     _OptionalCreateGroupRequestServiceResourceCreateGroupTypeDef,
 ):
     pass
 
 
-GroupOutputTypeDef = TypedDict(
-    "GroupOutputTypeDef",
+GroupTypeDef = TypedDict(
+    "GroupTypeDef",
     {
         "Path": str,
         "GroupName": str,
         "GroupId": str,
         "Arn": str,
         "CreateDate": datetime,
     },
@@ -797,16 +797,16 @@
 class CreateLoginProfileRequestUserCreateLoginProfileTypeDef(
     _RequiredCreateLoginProfileRequestUserCreateLoginProfileTypeDef,
     _OptionalCreateLoginProfileRequestUserCreateLoginProfileTypeDef,
 ):
     pass
 
 
-LoginProfileOutputTypeDef = TypedDict(
-    "LoginProfileOutputTypeDef",
+LoginProfileTypeDef = TypedDict(
+    "LoginProfileTypeDef",
     {
         "UserName": str,
         "CreateDate": datetime,
         "PasswordResetRequired": bool,
     },
 )
 
@@ -859,16 +859,16 @@
 class CreatePolicyVersionRequestRequestTypeDef(
     _RequiredCreatePolicyVersionRequestRequestTypeDef,
     _OptionalCreatePolicyVersionRequestRequestTypeDef,
 ):
     pass
 
 
-PolicyVersionOutputTypeDef = TypedDict(
-    "PolicyVersionOutputTypeDef",
+PolicyVersionTypeDef = TypedDict(
+    "PolicyVersionTypeDef",
     {
         "Document": str,
         "VersionId": str,
         "IsDefaultVersion": bool,
         "CreateDate": datetime,
     },
 )
@@ -900,16 +900,16 @@
     "CreateServiceSpecificCredentialRequestRequestTypeDef",
     {
         "UserName": str,
         "ServiceName": str,
     },
 )
 
-ServiceSpecificCredentialOutputTypeDef = TypedDict(
-    "ServiceSpecificCredentialOutputTypeDef",
+ServiceSpecificCredentialTypeDef = TypedDict(
+    "ServiceSpecificCredentialTypeDef",
     {
         "CreateDate": datetime,
         "ServiceName": str,
         "ServiceUserName": str,
         "ServicePassword": str,
         "ServiceSpecificCredentialId": str,
         "UserName": str,
@@ -1051,16 +1051,16 @@
 DeleteServiceLinkedRoleRequestRequestTypeDef = TypedDict(
     "DeleteServiceLinkedRoleRequestRequestTypeDef",
     {
         "RoleName": str,
     },
 )
 
-DeleteServiceLinkedRoleResponseOutputTypeDef = TypedDict(
-    "DeleteServiceLinkedRoleResponseOutputTypeDef",
+DeleteServiceLinkedRoleResponseTypeDef = TypedDict(
+    "DeleteServiceLinkedRoleResponseTypeDef",
     {
         "DeletionTaskId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeleteServiceSpecificCredentialRequestRequestTypeDef = TypedDict(
@@ -1132,16 +1132,16 @@
 DeleteVirtualMFADeviceRequestRequestTypeDef = TypedDict(
     "DeleteVirtualMFADeviceRequestRequestTypeDef",
     {
         "SerialNumber": str,
     },
 )
 
-RoleUsageTypeOutputTypeDef = TypedDict(
-    "RoleUsageTypeOutputTypeDef",
+RoleUsageTypeTypeDef = TypedDict(
+    "RoleUsageTypeTypeDef",
     {
         "Region": str,
         "Resources": List[str],
     },
 )
 
 DetachGroupPolicyRequestGroupDetachPolicyTypeDef = TypedDict(
@@ -1240,49 +1240,49 @@
     {
         "SerialNumber": str,
         "AuthenticationCode1": str,
         "AuthenticationCode2": str,
     },
 )
 
-EntityInfoOutputTypeDef = TypedDict(
-    "EntityInfoOutputTypeDef",
+EntityInfoTypeDef = TypedDict(
+    "EntityInfoTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Type": policyOwnerEntityTypeType,
         "Id": str,
         "Path": str,
     },
 )
 
-ErrorDetailsOutputTypeDef = TypedDict(
-    "ErrorDetailsOutputTypeDef",
+ErrorDetailsTypeDef = TypedDict(
+    "ErrorDetailsTypeDef",
     {
         "Message": str,
         "Code": str,
     },
 )
 
-OrganizationsDecisionDetailOutputTypeDef = TypedDict(
-    "OrganizationsDecisionDetailOutputTypeDef",
+OrganizationsDecisionDetailTypeDef = TypedDict(
+    "OrganizationsDecisionDetailTypeDef",
     {
         "AllowedByOrganizations": bool,
     },
 )
 
-PermissionsBoundaryDecisionDetailOutputTypeDef = TypedDict(
-    "PermissionsBoundaryDecisionDetailOutputTypeDef",
+PermissionsBoundaryDecisionDetailTypeDef = TypedDict(
+    "PermissionsBoundaryDecisionDetailTypeDef",
     {
         "AllowedByPermissionsBoundary": bool,
     },
 )
 
-GenerateCredentialReportResponseOutputTypeDef = TypedDict(
-    "GenerateCredentialReportResponseOutputTypeDef",
+GenerateCredentialReportResponseTypeDef = TypedDict(
+    "GenerateCredentialReportResponseTypeDef",
     {
         "State": ReportStateTypeType,
         "Description": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1304,16 +1304,16 @@
 class GenerateOrganizationsAccessReportRequestRequestTypeDef(
     _RequiredGenerateOrganizationsAccessReportRequestRequestTypeDef,
     _OptionalGenerateOrganizationsAccessReportRequestRequestTypeDef,
 ):
     pass
 
 
-GenerateOrganizationsAccessReportResponseOutputTypeDef = TypedDict(
-    "GenerateOrganizationsAccessReportResponseOutputTypeDef",
+GenerateOrganizationsAccessReportResponseTypeDef = TypedDict(
+    "GenerateOrganizationsAccessReportResponseTypeDef",
     {
         "JobId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGenerateServiceLastAccessedDetailsRequestRequestTypeDef = TypedDict(
@@ -1334,16 +1334,16 @@
 class GenerateServiceLastAccessedDetailsRequestRequestTypeDef(
     _RequiredGenerateServiceLastAccessedDetailsRequestRequestTypeDef,
     _OptionalGenerateServiceLastAccessedDetailsRequestRequestTypeDef,
 ):
     pass
 
 
-GenerateServiceLastAccessedDetailsResponseOutputTypeDef = TypedDict(
-    "GenerateServiceLastAccessedDetailsResponseOutputTypeDef",
+GenerateServiceLastAccessedDetailsResponseTypeDef = TypedDict(
+    "GenerateServiceLastAccessedDetailsResponseTypeDef",
     {
         "JobId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccessKeyLastUsedRequestRequestTypeDef = TypedDict(
@@ -1368,47 +1368,47 @@
         "Filter": Sequence[EntityTypeType],
         "MaxItems": int,
         "Marker": str,
     },
     total=False,
 )
 
-PasswordPolicyOutputTypeDef = TypedDict(
-    "PasswordPolicyOutputTypeDef",
+PasswordPolicyTypeDef = TypedDict(
+    "PasswordPolicyTypeDef",
     {
         "MinimumPasswordLength": int,
         "RequireSymbols": bool,
         "RequireNumbers": bool,
         "RequireUppercaseCharacters": bool,
         "RequireLowercaseCharacters": bool,
         "AllowUsersToChangePassword": bool,
         "ExpirePasswords": bool,
         "MaxPasswordAge": int,
         "PasswordReusePrevention": int,
         "HardExpiry": bool,
     },
 )
 
-GetAccountSummaryResponseOutputTypeDef = TypedDict(
-    "GetAccountSummaryResponseOutputTypeDef",
+GetAccountSummaryResponseTypeDef = TypedDict(
+    "GetAccountSummaryResponseTypeDef",
     {
         "SummaryMap": Dict[summaryKeyTypeType, int],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetContextKeysForCustomPolicyRequestRequestTypeDef = TypedDict(
     "GetContextKeysForCustomPolicyRequestRequestTypeDef",
     {
         "PolicyInputList": Sequence[str],
     },
 )
 
-GetContextKeysForPolicyResponseOutputTypeDef = TypedDict(
-    "GetContextKeysForPolicyResponseOutputTypeDef",
+GetContextKeysForPolicyResponseTypeDef = TypedDict(
+    "GetContextKeysForPolicyResponseTypeDef",
     {
         "ContextKeyNames": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetContextKeysForPrincipalPolicyRequestRequestTypeDef = TypedDict(
@@ -1429,16 +1429,16 @@
 class GetContextKeysForPrincipalPolicyRequestRequestTypeDef(
     _RequiredGetContextKeysForPrincipalPolicyRequestRequestTypeDef,
     _OptionalGetContextKeysForPrincipalPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-GetCredentialReportResponseOutputTypeDef = TypedDict(
-    "GetCredentialReportResponseOutputTypeDef",
+GetCredentialReportResponseTypeDef = TypedDict(
+    "GetCredentialReportResponseTypeDef",
     {
         "Content": bytes,
         "ReportFormat": Literal["text/csv"],
         "GeneratedTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1447,16 +1447,16 @@
     "GetGroupPolicyRequestRequestTypeDef",
     {
         "GroupName": str,
         "PolicyName": str,
     },
 )
 
-GetGroupPolicyResponseOutputTypeDef = TypedDict(
-    "GetGroupPolicyResponseOutputTypeDef",
+GetGroupPolicyResponseTypeDef = TypedDict(
+    "GetGroupPolicyResponseTypeDef",
     {
         "GroupName": str,
         "PolicyName": str,
         "PolicyDocument": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1544,16 +1544,16 @@
 
 class GetMFADeviceRequestRequestTypeDef(
     _RequiredGetMFADeviceRequestRequestTypeDef, _OptionalGetMFADeviceRequestRequestTypeDef
 ):
     pass
 
 
-GetMFADeviceResponseOutputTypeDef = TypedDict(
-    "GetMFADeviceResponseOutputTypeDef",
+GetMFADeviceResponseTypeDef = TypedDict(
+    "GetMFADeviceResponseTypeDef",
     {
         "UserName": str,
         "SerialNumber": str,
         "EnableDate": datetime,
         "Certifications": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1609,16 +1609,16 @@
     "GetRolePolicyRequestRequestTypeDef",
     {
         "RoleName": str,
         "PolicyName": str,
     },
 )
 
-GetRolePolicyResponseOutputTypeDef = TypedDict(
-    "GetRolePolicyResponseOutputTypeDef",
+GetRolePolicyResponseTypeDef = TypedDict(
+    "GetRolePolicyResponseTypeDef",
     {
         "RoleName": str,
         "PolicyName": str,
         "PolicyDocument": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1642,16 +1642,16 @@
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Encoding": encodingTypeType,
     },
 )
 
-SSHPublicKeyOutputTypeDef = TypedDict(
-    "SSHPublicKeyOutputTypeDef",
+SSHPublicKeyTypeDef = TypedDict(
+    "SSHPublicKeyTypeDef",
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Fingerprint": str,
         "SSHPublicKeyBody": str,
         "Status": statusTypeType,
         "UploadDate": datetime,
@@ -1723,16 +1723,16 @@
     "GetUserPolicyRequestRequestTypeDef",
     {
         "UserName": str,
         "PolicyName": str,
     },
 )
 
-GetUserPolicyResponseOutputTypeDef = TypedDict(
-    "GetUserPolicyResponseOutputTypeDef",
+GetUserPolicyResponseTypeDef = TypedDict(
+    "GetUserPolicyResponseTypeDef",
     {
         "UserName": str,
         "PolicyName": str,
         "PolicyDocument": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1741,16 +1741,16 @@
     "GetUserRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
-PolicyDetailOutputTypeDef = TypedDict(
-    "PolicyDetailOutputTypeDef",
+PolicyDetailTypeDef = TypedDict(
+    "PolicyDetailTypeDef",
     {
         "PolicyName": str,
         "PolicyDocument": str,
     },
 )
 
 ListAccessKeysRequestListAccessKeysPaginateTypeDef = TypedDict(
@@ -1785,16 +1785,16 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListAccountAliasesResponseOutputTypeDef = TypedDict(
-    "ListAccountAliasesResponseOutputTypeDef",
+ListAccountAliasesResponseTypeDef = TypedDict(
+    "ListAccountAliasesResponseTypeDef",
     {
         "AccountAliases": List[str],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1987,32 +1987,32 @@
 class ListEntitiesForPolicyRequestRequestTypeDef(
     _RequiredListEntitiesForPolicyRequestRequestTypeDef,
     _OptionalListEntitiesForPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-PolicyGroupOutputTypeDef = TypedDict(
-    "PolicyGroupOutputTypeDef",
+PolicyGroupTypeDef = TypedDict(
+    "PolicyGroupTypeDef",
     {
         "GroupName": str,
         "GroupId": str,
     },
 )
 
-PolicyRoleOutputTypeDef = TypedDict(
-    "PolicyRoleOutputTypeDef",
+PolicyRoleTypeDef = TypedDict(
+    "PolicyRoleTypeDef",
     {
         "RoleName": str,
         "RoleId": str,
     },
 )
 
-PolicyUserOutputTypeDef = TypedDict(
-    "PolicyUserOutputTypeDef",
+PolicyUserTypeDef = TypedDict(
+    "PolicyUserTypeDef",
     {
         "UserName": str,
         "UserId": str,
     },
 )
 
 _RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef = TypedDict(
@@ -2055,16 +2055,16 @@
 
 class ListGroupPoliciesRequestRequestTypeDef(
     _RequiredListGroupPoliciesRequestRequestTypeDef, _OptionalListGroupPoliciesRequestRequestTypeDef
 ):
     pass
 
 
-ListGroupPoliciesResponseOutputTypeDef = TypedDict(
-    "ListGroupPoliciesResponseOutputTypeDef",
+ListGroupPoliciesResponseTypeDef = TypedDict(
+    "ListGroupPoliciesResponseTypeDef",
     {
         "PolicyNames": List[str],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2300,16 +2300,16 @@
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-MFADeviceOutputTypeDef = TypedDict(
-    "MFADeviceOutputTypeDef",
+MFADeviceTypeDef = TypedDict(
+    "MFADeviceTypeDef",
     {
         "UserName": str,
         "SerialNumber": str,
         "EnableDate": datetime,
     },
 )
 
@@ -2358,23 +2358,23 @@
 class ListOpenIDConnectProviderTagsRequestRequestTypeDef(
     _RequiredListOpenIDConnectProviderTagsRequestRequestTypeDef,
     _OptionalListOpenIDConnectProviderTagsRequestRequestTypeDef,
 ):
     pass
 
 
-OpenIDConnectProviderListEntryOutputTypeDef = TypedDict(
-    "OpenIDConnectProviderListEntryOutputTypeDef",
+OpenIDConnectProviderListEntryTypeDef = TypedDict(
+    "OpenIDConnectProviderListEntryTypeDef",
     {
         "Arn": str,
     },
 )
 
-PolicyGrantingServiceAccessOutputTypeDef = TypedDict(
-    "PolicyGrantingServiceAccessOutputTypeDef",
+PolicyGrantingServiceAccessTypeDef = TypedDict(
+    "PolicyGrantingServiceAccessTypeDef",
     {
         "PolicyName": str,
         "PolicyType": policyTypeType,
         "PolicyArn": str,
         "EntityType": policyOwnerEntityTypeType,
         "EntityName": str,
     },
@@ -2557,16 +2557,16 @@
 
 class ListRolePoliciesRequestRequestTypeDef(
     _RequiredListRolePoliciesRequestRequestTypeDef, _OptionalListRolePoliciesRequestRequestTypeDef
 ):
     pass
 
 
-ListRolePoliciesResponseOutputTypeDef = TypedDict(
-    "ListRolePoliciesResponseOutputTypeDef",
+ListRolePoliciesResponseTypeDef = TypedDict(
+    "ListRolePoliciesResponseTypeDef",
     {
         "PolicyNames": List[str],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2675,16 +2675,16 @@
 class ListSAMLProviderTagsRequestRequestTypeDef(
     _RequiredListSAMLProviderTagsRequestRequestTypeDef,
     _OptionalListSAMLProviderTagsRequestRequestTypeDef,
 ):
     pass
 
 
-SAMLProviderListEntryOutputTypeDef = TypedDict(
-    "SAMLProviderListEntryOutputTypeDef",
+SAMLProviderListEntryTypeDef = TypedDict(
+    "SAMLProviderListEntryTypeDef",
     {
         "Arn": str,
         "ValidUntil": datetime,
         "CreateDate": datetime,
     },
 )
 
@@ -2703,16 +2703,16 @@
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-SSHPublicKeyMetadataOutputTypeDef = TypedDict(
-    "SSHPublicKeyMetadataOutputTypeDef",
+SSHPublicKeyMetadataTypeDef = TypedDict(
+    "SSHPublicKeyMetadataTypeDef",
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Status": statusTypeType,
         "UploadDate": datetime,
     },
 )
@@ -2777,16 +2777,16 @@
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ServerCertificateMetadataOutputTypeDef = TypedDict(
-    "ServerCertificateMetadataOutputTypeDef",
+ServerCertificateMetadataTypeDef = TypedDict(
+    "ServerCertificateMetadataTypeDef",
     {
         "Path": str,
         "ServerCertificateName": str,
         "ServerCertificateId": str,
         "Arn": str,
         "UploadDate": datetime,
         "Expiration": datetime,
@@ -2798,16 +2798,16 @@
     {
         "UserName": str,
         "ServiceName": str,
     },
     total=False,
 )
 
-ServiceSpecificCredentialMetadataOutputTypeDef = TypedDict(
-    "ServiceSpecificCredentialMetadataOutputTypeDef",
+ServiceSpecificCredentialMetadataTypeDef = TypedDict(
+    "ServiceSpecificCredentialMetadataTypeDef",
     {
         "UserName": str,
         "Status": statusTypeType,
         "ServiceUserName": str,
         "CreateDate": datetime,
         "ServiceSpecificCredentialId": str,
         "ServiceName": str,
@@ -2829,16 +2829,16 @@
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-SigningCertificateOutputTypeDef = TypedDict(
-    "SigningCertificateOutputTypeDef",
+SigningCertificateTypeDef = TypedDict(
+    "SigningCertificateTypeDef",
     {
         "UserName": str,
         "CertificateId": str,
         "CertificateBody": str,
         "Status": statusTypeType,
         "UploadDate": datetime,
     },
@@ -2884,16 +2884,16 @@
 
 class ListUserPoliciesRequestRequestTypeDef(
     _RequiredListUserPoliciesRequestRequestTypeDef, _OptionalListUserPoliciesRequestRequestTypeDef
 ):
     pass
 
 
-ListUserPoliciesResponseOutputTypeDef = TypedDict(
-    "ListUserPoliciesResponseOutputTypeDef",
+ListUserPoliciesResponseTypeDef = TypedDict(
+    "ListUserPoliciesResponseTypeDef",
     {
         "PolicyNames": List[str],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2986,16 +2986,16 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-PositionOutputTypeDef = TypedDict(
-    "PositionOutputTypeDef",
+PositionTypeDef = TypedDict(
+    "PositionTypeDef",
     {
         "Line": int,
         "Column": int,
     },
 )
 
 PutGroupPolicyRequestGroupCreatePolicyTypeDef = TypedDict(
@@ -3170,16 +3170,16 @@
         "UserName": str,
         "SerialNumber": str,
         "AuthenticationCode1": str,
         "AuthenticationCode2": str,
     },
 )
 
-RoleLastUsedOutputTypeDef = TypedDict(
-    "RoleLastUsedOutputTypeDef",
+RoleLastUsedTypeDef = TypedDict(
+    "RoleLastUsedTypeDef",
     {
         "LastUsedDate": datetime,
         "Region": str,
     },
 )
 
 RoleLastUsedResponseMetadataTypeDef = TypedDict(
@@ -3200,16 +3200,16 @@
         "Arn": str,
         "UploadDate": datetime,
         "Expiration": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TrackedActionLastAccessedOutputTypeDef = TypedDict(
-    "TrackedActionLastAccessedOutputTypeDef",
+TrackedActionLastAccessedTypeDef = TypedDict(
+    "TrackedActionLastAccessedTypeDef",
     {
         "ActionName": str,
         "LastAccessedEntity": str,
         "LastAccessedTime": datetime,
         "LastAccessedRegion": str,
     },
 )
@@ -3522,16 +3522,16 @@
 UpdateSAMLProviderRequestSamlProviderUpdateTypeDef = TypedDict(
     "UpdateSAMLProviderRequestSamlProviderUpdateTypeDef",
     {
         "SAMLMetadataDocument": str,
     },
 )
 
-UpdateSAMLProviderResponseOutputTypeDef = TypedDict(
-    "UpdateSAMLProviderResponseOutputTypeDef",
+UpdateSAMLProviderResponseTypeDef = TypedDict(
+    "UpdateSAMLProviderResponseTypeDef",
     {
         "SAMLProviderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSSHPublicKeyRequestRequestTypeDef = TypedDict(
@@ -3716,65 +3716,65 @@
 class UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef(
     _RequiredUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
     _OptionalUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
 ):
     pass
 
 
-GetAccessKeyLastUsedResponseOutputTypeDef = TypedDict(
-    "GetAccessKeyLastUsedResponseOutputTypeDef",
+GetAccessKeyLastUsedResponseTypeDef = TypedDict(
+    "GetAccessKeyLastUsedResponseTypeDef",
     {
         "UserName": str,
-        "AccessKeyLastUsed": AccessKeyLastUsedOutputTypeDef,
+        "AccessKeyLastUsed": AccessKeyLastUsedTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAccessKeysResponseOutputTypeDef = TypedDict(
-    "ListAccessKeysResponseOutputTypeDef",
+ListAccessKeysResponseTypeDef = TypedDict(
+    "ListAccessKeysResponseTypeDef",
     {
-        "AccessKeyMetadata": List[AccessKeyMetadataOutputTypeDef],
+        "AccessKeyMetadata": List[AccessKeyMetadataTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateAccessKeyResponseOutputTypeDef = TypedDict(
-    "CreateAccessKeyResponseOutputTypeDef",
+CreateAccessKeyResponseTypeDef = TypedDict(
+    "CreateAccessKeyResponseTypeDef",
     {
-        "AccessKey": AccessKeyOutputTypeDef,
+        "AccessKey": AccessKeyTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAttachedGroupPoliciesResponseOutputTypeDef = TypedDict(
-    "ListAttachedGroupPoliciesResponseOutputTypeDef",
+ListAttachedGroupPoliciesResponseTypeDef = TypedDict(
+    "ListAttachedGroupPoliciesResponseTypeDef",
     {
-        "AttachedPolicies": List[AttachedPolicyOutputTypeDef],
+        "AttachedPolicies": List[AttachedPolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAttachedRolePoliciesResponseOutputTypeDef = TypedDict(
-    "ListAttachedRolePoliciesResponseOutputTypeDef",
+ListAttachedRolePoliciesResponseTypeDef = TypedDict(
+    "ListAttachedRolePoliciesResponseTypeDef",
     {
-        "AttachedPolicies": List[AttachedPolicyOutputTypeDef],
+        "AttachedPolicies": List[AttachedPolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAttachedUserPoliciesResponseOutputTypeDef = TypedDict(
-    "ListAttachedUserPoliciesResponseOutputTypeDef",
+ListAttachedUserPoliciesResponseTypeDef = TypedDict(
+    "ListAttachedUserPoliciesResponseTypeDef",
     {
-        "AttachedPolicies": List[AttachedPolicyOutputTypeDef],
+        "AttachedPolicies": List[AttachedPolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSimulateCustomPolicyRequestRequestTypeDef = TypedDict(
@@ -3897,36 +3897,36 @@
 class SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef(
     _RequiredSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
     _OptionalSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
 ):
     pass
 
 
-CreateGroupResponseOutputTypeDef = TypedDict(
-    "CreateGroupResponseOutputTypeDef",
+CreateGroupResponseTypeDef = TypedDict(
+    "CreateGroupResponseTypeDef",
     {
-        "Group": GroupOutputTypeDef,
+        "Group": GroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListGroupsForUserResponseOutputTypeDef = TypedDict(
-    "ListGroupsForUserResponseOutputTypeDef",
+ListGroupsForUserResponseTypeDef = TypedDict(
+    "ListGroupsForUserResponseTypeDef",
     {
-        "Groups": List[GroupOutputTypeDef],
+        "Groups": List[GroupTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListGroupsResponseOutputTypeDef = TypedDict(
-    "ListGroupsResponseOutputTypeDef",
+ListGroupsResponseTypeDef = TypedDict(
+    "ListGroupsResponseTypeDef",
     {
-        "Groups": List[GroupOutputTypeDef],
+        "Groups": List[GroupTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateInstanceProfileRequestRequestTypeDef = TypedDict(
@@ -4362,153 +4362,153 @@
 class UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef(
     _RequiredUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
     _OptionalUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
 ):
     pass
 
 
-CreateLoginProfileResponseOutputTypeDef = TypedDict(
-    "CreateLoginProfileResponseOutputTypeDef",
+CreateLoginProfileResponseTypeDef = TypedDict(
+    "CreateLoginProfileResponseTypeDef",
     {
-        "LoginProfile": LoginProfileOutputTypeDef,
+        "LoginProfile": LoginProfileTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetLoginProfileResponseOutputTypeDef = TypedDict(
-    "GetLoginProfileResponseOutputTypeDef",
+GetLoginProfileResponseTypeDef = TypedDict(
+    "GetLoginProfileResponseTypeDef",
     {
-        "LoginProfile": LoginProfileOutputTypeDef,
+        "LoginProfile": LoginProfileTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateOpenIDConnectProviderResponseOutputTypeDef = TypedDict(
-    "CreateOpenIDConnectProviderResponseOutputTypeDef",
+CreateOpenIDConnectProviderResponseTypeDef = TypedDict(
+    "CreateOpenIDConnectProviderResponseTypeDef",
     {
         "OpenIDConnectProviderArn": str,
         "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateSAMLProviderResponseOutputTypeDef = TypedDict(
-    "CreateSAMLProviderResponseOutputTypeDef",
+CreateSAMLProviderResponseTypeDef = TypedDict(
+    "CreateSAMLProviderResponseTypeDef",
     {
         "SAMLProviderArn": str,
         "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetOpenIDConnectProviderResponseOutputTypeDef = TypedDict(
-    "GetOpenIDConnectProviderResponseOutputTypeDef",
+GetOpenIDConnectProviderResponseTypeDef = TypedDict(
+    "GetOpenIDConnectProviderResponseTypeDef",
     {
         "Url": str,
         "ClientIDList": List[str],
         "ThumbprintList": List[str],
         "CreateDate": datetime,
         "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetSAMLProviderResponseOutputTypeDef = TypedDict(
-    "GetSAMLProviderResponseOutputTypeDef",
+GetSAMLProviderResponseTypeDef = TypedDict(
+    "GetSAMLProviderResponseTypeDef",
     {
         "SAMLMetadataDocument": str,
         "CreateDate": datetime,
         "ValidUntil": datetime,
         "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListInstanceProfileTagsResponseOutputTypeDef = TypedDict(
-    "ListInstanceProfileTagsResponseOutputTypeDef",
+ListInstanceProfileTagsResponseTypeDef = TypedDict(
+    "ListInstanceProfileTagsResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListMFADeviceTagsResponseOutputTypeDef = TypedDict(
-    "ListMFADeviceTagsResponseOutputTypeDef",
+ListMFADeviceTagsResponseTypeDef = TypedDict(
+    "ListMFADeviceTagsResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListOpenIDConnectProviderTagsResponseOutputTypeDef = TypedDict(
-    "ListOpenIDConnectProviderTagsResponseOutputTypeDef",
+ListOpenIDConnectProviderTagsResponseTypeDef = TypedDict(
+    "ListOpenIDConnectProviderTagsResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPolicyTagsResponseOutputTypeDef = TypedDict(
-    "ListPolicyTagsResponseOutputTypeDef",
+ListPolicyTagsResponseTypeDef = TypedDict(
+    "ListPolicyTagsResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListRoleTagsResponseOutputTypeDef = TypedDict(
-    "ListRoleTagsResponseOutputTypeDef",
+ListRoleTagsResponseTypeDef = TypedDict(
+    "ListRoleTagsResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSAMLProviderTagsResponseOutputTypeDef = TypedDict(
-    "ListSAMLProviderTagsResponseOutputTypeDef",
+ListSAMLProviderTagsResponseTypeDef = TypedDict(
+    "ListSAMLProviderTagsResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServerCertificateTagsResponseOutputTypeDef = TypedDict(
-    "ListServerCertificateTagsResponseOutputTypeDef",
+ListServerCertificateTagsResponseTypeDef = TypedDict(
+    "ListServerCertificateTagsResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListUserTagsResponseOutputTypeDef = TypedDict(
-    "ListUserTagsResponseOutputTypeDef",
+ListUserTagsResponseTypeDef = TypedDict(
+    "ListUserTagsResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PolicyOutputTypeDef = TypedDict(
-    "PolicyOutputTypeDef",
+PolicyTypeDef = TypedDict(
+    "PolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyId": str,
         "Arn": str,
         "Path": str,
         "DefaultVersionId": str,
         "AttachmentCount": int,
@@ -4517,139 +4517,139 @@
         "Description": str,
         "CreateDate": datetime,
         "UpdateDate": datetime,
         "Tags": List[TagOutputTypeDef],
     },
 )
 
-UserOutputTypeDef = TypedDict(
-    "UserOutputTypeDef",
+UserResponseMetadataTypeDef = TypedDict(
+    "UserResponseMetadataTypeDef",
     {
         "Path": str,
         "UserName": str,
         "UserId": str,
         "Arn": str,
         "CreateDate": datetime,
         "PasswordLastUsed": datetime,
-        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UserResponseMetadataTypeDef = TypedDict(
-    "UserResponseMetadataTypeDef",
+UserTypeDef = TypedDict(
+    "UserTypeDef",
     {
         "Path": str,
         "UserName": str,
         "UserId": str,
         "Arn": str,
         "CreateDate": datetime,
         "PasswordLastUsed": datetime,
-        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreatePolicyVersionResponseOutputTypeDef = TypedDict(
-    "CreatePolicyVersionResponseOutputTypeDef",
+CreatePolicyVersionResponseTypeDef = TypedDict(
+    "CreatePolicyVersionResponseTypeDef",
     {
-        "PolicyVersion": PolicyVersionOutputTypeDef,
+        "PolicyVersion": PolicyVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPolicyVersionResponseOutputTypeDef = TypedDict(
-    "GetPolicyVersionResponseOutputTypeDef",
+GetPolicyVersionResponseTypeDef = TypedDict(
+    "GetPolicyVersionResponseTypeDef",
     {
-        "PolicyVersion": PolicyVersionOutputTypeDef,
+        "PolicyVersion": PolicyVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPolicyVersionsResponseOutputTypeDef = TypedDict(
-    "ListPolicyVersionsResponseOutputTypeDef",
+ListPolicyVersionsResponseTypeDef = TypedDict(
+    "ListPolicyVersionsResponseTypeDef",
     {
-        "Versions": List[PolicyVersionOutputTypeDef],
+        "Versions": List[PolicyVersionTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ManagedPolicyDetailOutputTypeDef = TypedDict(
-    "ManagedPolicyDetailOutputTypeDef",
+ManagedPolicyDetailTypeDef = TypedDict(
+    "ManagedPolicyDetailTypeDef",
     {
         "PolicyName": str,
         "PolicyId": str,
         "Arn": str,
         "Path": str,
         "DefaultVersionId": str,
         "AttachmentCount": int,
         "PermissionsBoundaryUsageCount": int,
         "IsAttachable": bool,
         "Description": str,
         "CreateDate": datetime,
         "UpdateDate": datetime,
-        "PolicyVersionList": List[PolicyVersionOutputTypeDef],
+        "PolicyVersionList": List[PolicyVersionTypeDef],
     },
 )
 
-CreateServiceSpecificCredentialResponseOutputTypeDef = TypedDict(
-    "CreateServiceSpecificCredentialResponseOutputTypeDef",
+CreateServiceSpecificCredentialResponseTypeDef = TypedDict(
+    "CreateServiceSpecificCredentialResponseTypeDef",
     {
-        "ServiceSpecificCredential": ServiceSpecificCredentialOutputTypeDef,
+        "ServiceSpecificCredential": ServiceSpecificCredentialTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResetServiceSpecificCredentialResponseOutputTypeDef = TypedDict(
-    "ResetServiceSpecificCredentialResponseOutputTypeDef",
+ResetServiceSpecificCredentialResponseTypeDef = TypedDict(
+    "ResetServiceSpecificCredentialResponseTypeDef",
     {
-        "ServiceSpecificCredential": ServiceSpecificCredentialOutputTypeDef,
+        "ServiceSpecificCredential": ServiceSpecificCredentialTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeletionTaskFailureReasonTypeOutputTypeDef = TypedDict(
-    "DeletionTaskFailureReasonTypeOutputTypeDef",
+DeletionTaskFailureReasonTypeTypeDef = TypedDict(
+    "DeletionTaskFailureReasonTypeTypeDef",
     {
         "Reason": str,
-        "RoleUsageList": List[RoleUsageTypeOutputTypeDef],
+        "RoleUsageList": List[RoleUsageTypeTypeDef],
     },
 )
 
-EntityDetailsOutputTypeDef = TypedDict(
-    "EntityDetailsOutputTypeDef",
+EntityDetailsTypeDef = TypedDict(
+    "EntityDetailsTypeDef",
     {
-        "EntityInfo": EntityInfoOutputTypeDef,
+        "EntityInfo": EntityInfoTypeDef,
         "LastAuthenticated": datetime,
     },
 )
 
-GetOrganizationsAccessReportResponseOutputTypeDef = TypedDict(
-    "GetOrganizationsAccessReportResponseOutputTypeDef",
+GetOrganizationsAccessReportResponseTypeDef = TypedDict(
+    "GetOrganizationsAccessReportResponseTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobCreationDate": datetime,
         "JobCompletionDate": datetime,
         "NumberOfServicesAccessible": int,
         "NumberOfServicesNotAccessed": int,
-        "AccessDetails": List[AccessDetailOutputTypeDef],
+        "AccessDetails": List[AccessDetailTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ErrorDetails": ErrorDetailsOutputTypeDef,
+        "ErrorDetails": ErrorDetailsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAccountPasswordPolicyResponseOutputTypeDef = TypedDict(
-    "GetAccountPasswordPolicyResponseOutputTypeDef",
+GetAccountPasswordPolicyResponseTypeDef = TypedDict(
+    "GetAccountPasswordPolicyResponseTypeDef",
     {
-        "PasswordPolicy": PasswordPolicyOutputTypeDef,
+        "PasswordPolicy": PasswordPolicyTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef = TypedDict(
     "_RequiredGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef",
     {
@@ -4720,510 +4720,510 @@
     {
         "UserName": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-GetSSHPublicKeyResponseOutputTypeDef = TypedDict(
-    "GetSSHPublicKeyResponseOutputTypeDef",
+GetSSHPublicKeyResponseTypeDef = TypedDict(
+    "GetSSHPublicKeyResponseTypeDef",
     {
-        "SSHPublicKey": SSHPublicKeyOutputTypeDef,
+        "SSHPublicKey": SSHPublicKeyTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UploadSSHPublicKeyResponseOutputTypeDef = TypedDict(
-    "UploadSSHPublicKeyResponseOutputTypeDef",
+UploadSSHPublicKeyResponseTypeDef = TypedDict(
+    "UploadSSHPublicKeyResponseTypeDef",
     {
-        "SSHPublicKey": SSHPublicKeyOutputTypeDef,
+        "SSHPublicKey": SSHPublicKeyTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GroupDetailOutputTypeDef = TypedDict(
-    "GroupDetailOutputTypeDef",
+GroupDetailTypeDef = TypedDict(
+    "GroupDetailTypeDef",
     {
         "Path": str,
         "GroupName": str,
         "GroupId": str,
         "Arn": str,
         "CreateDate": datetime,
-        "GroupPolicyList": List[PolicyDetailOutputTypeDef],
-        "AttachedManagedPolicies": List[AttachedPolicyOutputTypeDef],
+        "GroupPolicyList": List[PolicyDetailTypeDef],
+        "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
     },
 )
 
-UserDetailOutputTypeDef = TypedDict(
-    "UserDetailOutputTypeDef",
+UserDetailTypeDef = TypedDict(
+    "UserDetailTypeDef",
     {
         "Path": str,
         "UserName": str,
         "UserId": str,
         "Arn": str,
         "CreateDate": datetime,
-        "UserPolicyList": List[PolicyDetailOutputTypeDef],
+        "UserPolicyList": List[PolicyDetailTypeDef],
         "GroupList": List[str],
-        "AttachedManagedPolicies": List[AttachedPolicyOutputTypeDef],
-        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagOutputTypeDef],
     },
 )
 
-ListEntitiesForPolicyResponseOutputTypeDef = TypedDict(
-    "ListEntitiesForPolicyResponseOutputTypeDef",
+ListEntitiesForPolicyResponseTypeDef = TypedDict(
+    "ListEntitiesForPolicyResponseTypeDef",
     {
-        "PolicyGroups": List[PolicyGroupOutputTypeDef],
-        "PolicyUsers": List[PolicyUserOutputTypeDef],
-        "PolicyRoles": List[PolicyRoleOutputTypeDef],
+        "PolicyGroups": List[PolicyGroupTypeDef],
+        "PolicyUsers": List[PolicyUserTypeDef],
+        "PolicyRoles": List[PolicyRoleTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListMFADevicesResponseOutputTypeDef = TypedDict(
-    "ListMFADevicesResponseOutputTypeDef",
+ListMFADevicesResponseTypeDef = TypedDict(
+    "ListMFADevicesResponseTypeDef",
     {
-        "MFADevices": List[MFADeviceOutputTypeDef],
+        "MFADevices": List[MFADeviceTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListOpenIDConnectProvidersResponseOutputTypeDef = TypedDict(
-    "ListOpenIDConnectProvidersResponseOutputTypeDef",
+ListOpenIDConnectProvidersResponseTypeDef = TypedDict(
+    "ListOpenIDConnectProvidersResponseTypeDef",
     {
-        "OpenIDConnectProviderList": List[OpenIDConnectProviderListEntryOutputTypeDef],
+        "OpenIDConnectProviderList": List[OpenIDConnectProviderListEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPoliciesGrantingServiceAccessEntryOutputTypeDef = TypedDict(
-    "ListPoliciesGrantingServiceAccessEntryOutputTypeDef",
+ListPoliciesGrantingServiceAccessEntryTypeDef = TypedDict(
+    "ListPoliciesGrantingServiceAccessEntryTypeDef",
     {
         "ServiceNamespace": str,
-        "Policies": List[PolicyGrantingServiceAccessOutputTypeDef],
+        "Policies": List[PolicyGrantingServiceAccessTypeDef],
     },
 )
 
-ListSAMLProvidersResponseOutputTypeDef = TypedDict(
-    "ListSAMLProvidersResponseOutputTypeDef",
+ListSAMLProvidersResponseTypeDef = TypedDict(
+    "ListSAMLProvidersResponseTypeDef",
     {
-        "SAMLProviderList": List[SAMLProviderListEntryOutputTypeDef],
+        "SAMLProviderList": List[SAMLProviderListEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSSHPublicKeysResponseOutputTypeDef = TypedDict(
-    "ListSSHPublicKeysResponseOutputTypeDef",
+ListSSHPublicKeysResponseTypeDef = TypedDict(
+    "ListSSHPublicKeysResponseTypeDef",
     {
-        "SSHPublicKeys": List[SSHPublicKeyMetadataOutputTypeDef],
+        "SSHPublicKeys": List[SSHPublicKeyMetadataTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServerCertificatesResponseOutputTypeDef = TypedDict(
-    "ListServerCertificatesResponseOutputTypeDef",
+ListServerCertificatesResponseTypeDef = TypedDict(
+    "ListServerCertificatesResponseTypeDef",
     {
-        "ServerCertificateMetadataList": List[ServerCertificateMetadataOutputTypeDef],
+        "ServerCertificateMetadataList": List[ServerCertificateMetadataTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ServerCertificateOutputTypeDef = TypedDict(
-    "ServerCertificateOutputTypeDef",
+ServerCertificateTypeDef = TypedDict(
+    "ServerCertificateTypeDef",
     {
-        "ServerCertificateMetadata": ServerCertificateMetadataOutputTypeDef,
+        "ServerCertificateMetadata": ServerCertificateMetadataTypeDef,
         "CertificateBody": str,
         "CertificateChain": str,
         "Tags": List[TagOutputTypeDef],
     },
 )
 
-UploadServerCertificateResponseOutputTypeDef = TypedDict(
-    "UploadServerCertificateResponseOutputTypeDef",
+UploadServerCertificateResponseTypeDef = TypedDict(
+    "UploadServerCertificateResponseTypeDef",
     {
-        "ServerCertificateMetadata": ServerCertificateMetadataOutputTypeDef,
+        "ServerCertificateMetadata": ServerCertificateMetadataTypeDef,
         "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceSpecificCredentialsResponseOutputTypeDef = TypedDict(
-    "ListServiceSpecificCredentialsResponseOutputTypeDef",
+ListServiceSpecificCredentialsResponseTypeDef = TypedDict(
+    "ListServiceSpecificCredentialsResponseTypeDef",
     {
-        "ServiceSpecificCredentials": List[ServiceSpecificCredentialMetadataOutputTypeDef],
+        "ServiceSpecificCredentials": List[ServiceSpecificCredentialMetadataTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSigningCertificatesResponseOutputTypeDef = TypedDict(
-    "ListSigningCertificatesResponseOutputTypeDef",
+ListSigningCertificatesResponseTypeDef = TypedDict(
+    "ListSigningCertificatesResponseTypeDef",
     {
-        "Certificates": List[SigningCertificateOutputTypeDef],
+        "Certificates": List[SigningCertificateTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UploadSigningCertificateResponseOutputTypeDef = TypedDict(
-    "UploadSigningCertificateResponseOutputTypeDef",
+UploadSigningCertificateResponseTypeDef = TypedDict(
+    "UploadSigningCertificateResponseTypeDef",
     {
-        "Certificate": SigningCertificateOutputTypeDef,
+        "Certificate": SigningCertificateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StatementOutputTypeDef = TypedDict(
-    "StatementOutputTypeDef",
+StatementTypeDef = TypedDict(
+    "StatementTypeDef",
     {
         "SourcePolicyId": str,
         "SourcePolicyType": PolicySourceTypeType,
-        "StartPosition": PositionOutputTypeDef,
-        "EndPosition": PositionOutputTypeDef,
+        "StartPosition": PositionTypeDef,
+        "EndPosition": PositionTypeDef,
     },
 )
 
-RoleOutputTypeDef = TypedDict(
-    "RoleOutputTypeDef",
+RoleTypeDef = TypedDict(
+    "RoleTypeDef",
     {
         "Path": str,
         "RoleName": str,
         "RoleId": str,
         "Arn": str,
         "CreateDate": datetime,
         "AssumeRolePolicyDocument": str,
         "Description": str,
         "MaxSessionDuration": int,
-        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagOutputTypeDef],
-        "RoleLastUsed": RoleLastUsedOutputTypeDef,
+        "RoleLastUsed": RoleLastUsedTypeDef,
     },
 )
 
-ServiceLastAccessedOutputTypeDef = TypedDict(
-    "ServiceLastAccessedOutputTypeDef",
+ServiceLastAccessedTypeDef = TypedDict(
+    "ServiceLastAccessedTypeDef",
     {
         "ServiceName": str,
         "LastAuthenticated": datetime,
         "ServiceNamespace": str,
         "LastAuthenticatedEntity": str,
         "LastAuthenticatedRegion": str,
         "TotalAuthenticatedEntities": int,
-        "TrackedActionsLastAccessed": List[TrackedActionLastAccessedOutputTypeDef],
+        "TrackedActionsLastAccessed": List[TrackedActionLastAccessedTypeDef],
     },
 )
 
-CreatePolicyResponseOutputTypeDef = TypedDict(
-    "CreatePolicyResponseOutputTypeDef",
+CreatePolicyResponseTypeDef = TypedDict(
+    "CreatePolicyResponseTypeDef",
     {
-        "Policy": PolicyOutputTypeDef,
+        "Policy": PolicyTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPolicyResponseOutputTypeDef = TypedDict(
-    "GetPolicyResponseOutputTypeDef",
+GetPolicyResponseTypeDef = TypedDict(
+    "GetPolicyResponseTypeDef",
     {
-        "Policy": PolicyOutputTypeDef,
+        "Policy": PolicyTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPoliciesResponseOutputTypeDef = TypedDict(
-    "ListPoliciesResponseOutputTypeDef",
+ListPoliciesResponseTypeDef = TypedDict(
+    "ListPoliciesResponseTypeDef",
     {
-        "Policies": List[PolicyOutputTypeDef],
+        "Policies": List[PolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateUserResponseOutputTypeDef = TypedDict(
-    "CreateUserResponseOutputTypeDef",
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
     {
-        "User": UserOutputTypeDef,
+        "User": UserTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetGroupResponseOutputTypeDef = TypedDict(
-    "GetGroupResponseOutputTypeDef",
+GetGroupResponseTypeDef = TypedDict(
+    "GetGroupResponseTypeDef",
     {
-        "Group": GroupOutputTypeDef,
-        "Users": List[UserOutputTypeDef],
+        "Group": GroupTypeDef,
+        "Users": List[UserTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetUserResponseOutputTypeDef = TypedDict(
-    "GetUserResponseOutputTypeDef",
+GetUserResponseTypeDef = TypedDict(
+    "GetUserResponseTypeDef",
     {
-        "User": UserOutputTypeDef,
+        "User": UserTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListUsersResponseOutputTypeDef = TypedDict(
-    "ListUsersResponseOutputTypeDef",
+ListUsersResponseTypeDef = TypedDict(
+    "ListUsersResponseTypeDef",
     {
-        "Users": List[UserOutputTypeDef],
+        "Users": List[UserTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-VirtualMFADeviceOutputTypeDef = TypedDict(
-    "VirtualMFADeviceOutputTypeDef",
+VirtualMFADeviceTypeDef = TypedDict(
+    "VirtualMFADeviceTypeDef",
     {
         "SerialNumber": str,
         "Base32StringSeed": bytes,
         "QRCodePNG": bytes,
-        "User": UserOutputTypeDef,
+        "User": UserTypeDef,
         "EnableDate": datetime,
         "Tags": List[TagOutputTypeDef],
     },
 )
 
-GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef = TypedDict(
-    "GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef",
+GetServiceLinkedRoleDeletionStatusResponseTypeDef = TypedDict(
+    "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
     {
         "Status": DeletionTaskStatusTypeType,
-        "Reason": DeletionTaskFailureReasonTypeOutputTypeDef,
+        "Reason": DeletionTaskFailureReasonTypeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef = TypedDict(
-    "GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef",
+GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef = TypedDict(
+    "GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobCreationDate": datetime,
         "JobCompletionDate": datetime,
-        "EntityDetailsList": List[EntityDetailsOutputTypeDef],
+        "EntityDetailsList": List[EntityDetailsTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "Error": ErrorDetailsOutputTypeDef,
+        "Error": ErrorDetailsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPoliciesGrantingServiceAccessResponseOutputTypeDef = TypedDict(
-    "ListPoliciesGrantingServiceAccessResponseOutputTypeDef",
+ListPoliciesGrantingServiceAccessResponseTypeDef = TypedDict(
+    "ListPoliciesGrantingServiceAccessResponseTypeDef",
     {
-        "PoliciesGrantingServiceAccess": List[ListPoliciesGrantingServiceAccessEntryOutputTypeDef],
+        "PoliciesGrantingServiceAccess": List[ListPoliciesGrantingServiceAccessEntryTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServerCertificateResponseOutputTypeDef = TypedDict(
-    "GetServerCertificateResponseOutputTypeDef",
+GetServerCertificateResponseTypeDef = TypedDict(
+    "GetServerCertificateResponseTypeDef",
     {
-        "ServerCertificate": ServerCertificateOutputTypeDef,
+        "ServerCertificate": ServerCertificateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResourceSpecificResultOutputTypeDef = TypedDict(
-    "ResourceSpecificResultOutputTypeDef",
+ResourceSpecificResultTypeDef = TypedDict(
+    "ResourceSpecificResultTypeDef",
     {
         "EvalResourceName": str,
         "EvalResourceDecision": PolicyEvaluationDecisionTypeType,
-        "MatchedStatements": List[StatementOutputTypeDef],
+        "MatchedStatements": List[StatementTypeDef],
         "MissingContextValues": List[str],
         "EvalDecisionDetails": Dict[str, PolicyEvaluationDecisionTypeType],
-        "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailOutputTypeDef,
+        "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailTypeDef,
     },
 )
 
-CreateRoleResponseOutputTypeDef = TypedDict(
-    "CreateRoleResponseOutputTypeDef",
+CreateRoleResponseTypeDef = TypedDict(
+    "CreateRoleResponseTypeDef",
     {
-        "Role": RoleOutputTypeDef,
+        "Role": RoleTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceLinkedRoleResponseOutputTypeDef = TypedDict(
-    "CreateServiceLinkedRoleResponseOutputTypeDef",
+CreateServiceLinkedRoleResponseTypeDef = TypedDict(
+    "CreateServiceLinkedRoleResponseTypeDef",
     {
-        "Role": RoleOutputTypeDef,
+        "Role": RoleTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetRoleResponseOutputTypeDef = TypedDict(
-    "GetRoleResponseOutputTypeDef",
+GetRoleResponseTypeDef = TypedDict(
+    "GetRoleResponseTypeDef",
     {
-        "Role": RoleOutputTypeDef,
+        "Role": RoleTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-InstanceProfileOutputTypeDef = TypedDict(
-    "InstanceProfileOutputTypeDef",
+InstanceProfileTypeDef = TypedDict(
+    "InstanceProfileTypeDef",
     {
         "Path": str,
         "InstanceProfileName": str,
         "InstanceProfileId": str,
         "Arn": str,
         "CreateDate": datetime,
-        "Roles": List[RoleOutputTypeDef],
+        "Roles": List[RoleTypeDef],
         "Tags": List[TagOutputTypeDef],
     },
 )
 
-ListRolesResponseOutputTypeDef = TypedDict(
-    "ListRolesResponseOutputTypeDef",
+ListRolesResponseTypeDef = TypedDict(
+    "ListRolesResponseTypeDef",
     {
-        "Roles": List[RoleOutputTypeDef],
+        "Roles": List[RoleTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateRoleDescriptionResponseOutputTypeDef = TypedDict(
-    "UpdateRoleDescriptionResponseOutputTypeDef",
+UpdateRoleDescriptionResponseTypeDef = TypedDict(
+    "UpdateRoleDescriptionResponseTypeDef",
     {
-        "Role": RoleOutputTypeDef,
+        "Role": RoleTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceLastAccessedDetailsResponseOutputTypeDef = TypedDict(
-    "GetServiceLastAccessedDetailsResponseOutputTypeDef",
+GetServiceLastAccessedDetailsResponseTypeDef = TypedDict(
+    "GetServiceLastAccessedDetailsResponseTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobType": AccessAdvisorUsageGranularityTypeType,
         "JobCreationDate": datetime,
-        "ServicesLastAccessed": List[ServiceLastAccessedOutputTypeDef],
+        "ServicesLastAccessed": List[ServiceLastAccessedTypeDef],
         "JobCompletionDate": datetime,
         "IsTruncated": bool,
         "Marker": str,
-        "Error": ErrorDetailsOutputTypeDef,
+        "Error": ErrorDetailsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateVirtualMFADeviceResponseOutputTypeDef = TypedDict(
-    "CreateVirtualMFADeviceResponseOutputTypeDef",
+CreateVirtualMFADeviceResponseTypeDef = TypedDict(
+    "CreateVirtualMFADeviceResponseTypeDef",
     {
-        "VirtualMFADevice": VirtualMFADeviceOutputTypeDef,
+        "VirtualMFADevice": VirtualMFADeviceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListVirtualMFADevicesResponseOutputTypeDef = TypedDict(
-    "ListVirtualMFADevicesResponseOutputTypeDef",
+ListVirtualMFADevicesResponseTypeDef = TypedDict(
+    "ListVirtualMFADevicesResponseTypeDef",
     {
-        "VirtualMFADevices": List[VirtualMFADeviceOutputTypeDef],
+        "VirtualMFADevices": List[VirtualMFADeviceTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EvaluationResultOutputTypeDef = TypedDict(
-    "EvaluationResultOutputTypeDef",
+EvaluationResultTypeDef = TypedDict(
+    "EvaluationResultTypeDef",
     {
         "EvalActionName": str,
         "EvalResourceName": str,
         "EvalDecision": PolicyEvaluationDecisionTypeType,
-        "MatchedStatements": List[StatementOutputTypeDef],
+        "MatchedStatements": List[StatementTypeDef],
         "MissingContextValues": List[str],
-        "OrganizationsDecisionDetail": OrganizationsDecisionDetailOutputTypeDef,
-        "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailOutputTypeDef,
+        "OrganizationsDecisionDetail": OrganizationsDecisionDetailTypeDef,
+        "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailTypeDef,
         "EvalDecisionDetails": Dict[str, PolicyEvaluationDecisionTypeType],
-        "ResourceSpecificResults": List[ResourceSpecificResultOutputTypeDef],
+        "ResourceSpecificResults": List[ResourceSpecificResultTypeDef],
     },
 )
 
-CreateInstanceProfileResponseOutputTypeDef = TypedDict(
-    "CreateInstanceProfileResponseOutputTypeDef",
+CreateInstanceProfileResponseTypeDef = TypedDict(
+    "CreateInstanceProfileResponseTypeDef",
     {
-        "InstanceProfile": InstanceProfileOutputTypeDef,
+        "InstanceProfile": InstanceProfileTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetInstanceProfileResponseOutputTypeDef = TypedDict(
-    "GetInstanceProfileResponseOutputTypeDef",
+GetInstanceProfileResponseTypeDef = TypedDict(
+    "GetInstanceProfileResponseTypeDef",
     {
-        "InstanceProfile": InstanceProfileOutputTypeDef,
+        "InstanceProfile": InstanceProfileTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListInstanceProfilesForRoleResponseOutputTypeDef = TypedDict(
-    "ListInstanceProfilesForRoleResponseOutputTypeDef",
+ListInstanceProfilesForRoleResponseTypeDef = TypedDict(
+    "ListInstanceProfilesForRoleResponseTypeDef",
     {
-        "InstanceProfiles": List[InstanceProfileOutputTypeDef],
+        "InstanceProfiles": List[InstanceProfileTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListInstanceProfilesResponseOutputTypeDef = TypedDict(
-    "ListInstanceProfilesResponseOutputTypeDef",
+ListInstanceProfilesResponseTypeDef = TypedDict(
+    "ListInstanceProfilesResponseTypeDef",
     {
-        "InstanceProfiles": List[InstanceProfileOutputTypeDef],
+        "InstanceProfiles": List[InstanceProfileTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RoleDetailOutputTypeDef = TypedDict(
-    "RoleDetailOutputTypeDef",
+RoleDetailTypeDef = TypedDict(
+    "RoleDetailTypeDef",
     {
         "Path": str,
         "RoleName": str,
         "RoleId": str,
         "Arn": str,
         "CreateDate": datetime,
         "AssumeRolePolicyDocument": str,
-        "InstanceProfileList": List[InstanceProfileOutputTypeDef],
-        "RolePolicyList": List[PolicyDetailOutputTypeDef],
-        "AttachedManagedPolicies": List[AttachedPolicyOutputTypeDef],
-        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "InstanceProfileList": List[InstanceProfileTypeDef],
+        "RolePolicyList": List[PolicyDetailTypeDef],
+        "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagOutputTypeDef],
-        "RoleLastUsed": RoleLastUsedOutputTypeDef,
+        "RoleLastUsed": RoleLastUsedTypeDef,
     },
 )
 
-SimulatePolicyResponseOutputTypeDef = TypedDict(
-    "SimulatePolicyResponseOutputTypeDef",
+SimulatePolicyResponseTypeDef = TypedDict(
+    "SimulatePolicyResponseTypeDef",
     {
-        "EvaluationResults": List[EvaluationResultOutputTypeDef],
+        "EvaluationResults": List[EvaluationResultTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAccountAuthorizationDetailsResponseOutputTypeDef = TypedDict(
-    "GetAccountAuthorizationDetailsResponseOutputTypeDef",
+GetAccountAuthorizationDetailsResponseTypeDef = TypedDict(
+    "GetAccountAuthorizationDetailsResponseTypeDef",
     {
-        "UserDetailList": List[UserDetailOutputTypeDef],
-        "GroupDetailList": List[GroupDetailOutputTypeDef],
-        "RoleDetailList": List[RoleDetailOutputTypeDef],
-        "Policies": List[ManagedPolicyDetailOutputTypeDef],
+        "UserDetailList": List[UserDetailTypeDef],
+        "GroupDetailList": List[GroupDetailTypeDef],
+        "RoleDetailList": List[RoleDetailTypeDef],
+        "Policies": List[ManagedPolicyDetailTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/type_defs.pyi` & `mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/type_defs.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iam service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iam.type_defs import AccessDetailOutputTypeDef
+    from mypy_boto3_iam.type_defs import AccessDetailTypeDef
 
-    data: AccessDetailOutputTypeDef = {...}
+    data: AccessDetailTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -42,18 +42,18 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AccessDetailOutputTypeDef",
-    "AccessKeyLastUsedOutputTypeDef",
-    "AccessKeyMetadataOutputTypeDef",
-    "AccessKeyOutputTypeDef",
+    "AccessDetailTypeDef",
+    "AccessKeyLastUsedTypeDef",
+    "AccessKeyMetadataTypeDef",
+    "AccessKeyTypeDef",
     "AddClientIDToOpenIDConnectProviderRequestRequestTypeDef",
     "AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef",
     "AddRoleToInstanceProfileRequestRequestTypeDef",
     "AddUserToGroupRequestGroupAddUserTypeDef",
     "AddUserToGroupRequestRequestTypeDef",
     "AddUserToGroupRequestUserAddGroupTypeDef",
     "AttachGroupPolicyRequestGroupAttachPolicyTypeDef",
@@ -61,39 +61,39 @@
     "AttachGroupPolicyRequestRequestTypeDef",
     "AttachRolePolicyRequestPolicyAttachRoleTypeDef",
     "AttachRolePolicyRequestRequestTypeDef",
     "AttachRolePolicyRequestRoleAttachPolicyTypeDef",
     "AttachUserPolicyRequestPolicyAttachUserTypeDef",
     "AttachUserPolicyRequestRequestTypeDef",
     "AttachUserPolicyRequestUserAttachPolicyTypeDef",
-    "AttachedPermissionsBoundaryOutputTypeDef",
     "AttachedPermissionsBoundaryResponseMetadataTypeDef",
-    "AttachedPolicyOutputTypeDef",
+    "AttachedPermissionsBoundaryTypeDef",
+    "AttachedPolicyTypeDef",
     "ChangePasswordRequestRequestTypeDef",
     "ChangePasswordRequestServiceResourceChangePasswordTypeDef",
     "ContextEntryTypeDef",
     "CreateAccessKeyRequestRequestTypeDef",
     "CreateAccountAliasRequestRequestTypeDef",
     "CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef",
     "CreateGroupRequestGroupCreateTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "CreateGroupRequestServiceResourceCreateGroupTypeDef",
-    "GroupOutputTypeDef",
+    "GroupTypeDef",
     "TagTypeDef",
     "CreateLoginProfileRequestLoginProfileCreateTypeDef",
     "CreateLoginProfileRequestRequestTypeDef",
     "CreateLoginProfileRequestUserCreateLoginProfileTypeDef",
-    "LoginProfileOutputTypeDef",
+    "LoginProfileTypeDef",
     "TagOutputTypeDef",
     "CreatePolicyVersionRequestPolicyCreateVersionTypeDef",
     "CreatePolicyVersionRequestRequestTypeDef",
-    "PolicyVersionOutputTypeDef",
+    "PolicyVersionTypeDef",
     "CreateServiceLinkedRoleRequestRequestTypeDef",
     "CreateServiceSpecificCredentialRequestRequestTypeDef",
-    "ServiceSpecificCredentialOutputTypeDef",
+    "ServiceSpecificCredentialTypeDef",
     "DeactivateMFADeviceRequestRequestTypeDef",
     "DeleteAccessKeyRequestRequestTypeDef",
     "DeleteAccountAliasRequestRequestTypeDef",
     "DeleteGroupPolicyRequestRequestTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteInstanceProfileRequestRequestTypeDef",
     "DeleteLoginProfileRequestRequestTypeDef",
@@ -103,159 +103,159 @@
     "DeleteRolePermissionsBoundaryRequestRequestTypeDef",
     "DeleteRolePolicyRequestRequestTypeDef",
     "DeleteRoleRequestRequestTypeDef",
     "DeleteSAMLProviderRequestRequestTypeDef",
     "DeleteSSHPublicKeyRequestRequestTypeDef",
     "DeleteServerCertificateRequestRequestTypeDef",
     "DeleteServiceLinkedRoleRequestRequestTypeDef",
-    "DeleteServiceLinkedRoleResponseOutputTypeDef",
+    "DeleteServiceLinkedRoleResponseTypeDef",
     "DeleteServiceSpecificCredentialRequestRequestTypeDef",
     "DeleteSigningCertificateRequestRequestTypeDef",
     "DeleteUserPermissionsBoundaryRequestRequestTypeDef",
     "DeleteUserPolicyRequestRequestTypeDef",
     "DeleteUserRequestRequestTypeDef",
     "DeleteVirtualMFADeviceRequestRequestTypeDef",
-    "RoleUsageTypeOutputTypeDef",
+    "RoleUsageTypeTypeDef",
     "DetachGroupPolicyRequestGroupDetachPolicyTypeDef",
     "DetachGroupPolicyRequestPolicyDetachGroupTypeDef",
     "DetachGroupPolicyRequestRequestTypeDef",
     "DetachRolePolicyRequestPolicyDetachRoleTypeDef",
     "DetachRolePolicyRequestRequestTypeDef",
     "DetachRolePolicyRequestRoleDetachPolicyTypeDef",
     "DetachUserPolicyRequestPolicyDetachUserTypeDef",
     "DetachUserPolicyRequestRequestTypeDef",
     "DetachUserPolicyRequestUserDetachPolicyTypeDef",
     "EmptyResponseMetadataTypeDef",
     "EnableMFADeviceRequestMfaDeviceAssociateTypeDef",
     "EnableMFADeviceRequestRequestTypeDef",
     "EnableMFADeviceRequestUserEnableMfaTypeDef",
-    "EntityInfoOutputTypeDef",
-    "ErrorDetailsOutputTypeDef",
-    "OrganizationsDecisionDetailOutputTypeDef",
-    "PermissionsBoundaryDecisionDetailOutputTypeDef",
-    "GenerateCredentialReportResponseOutputTypeDef",
+    "EntityInfoTypeDef",
+    "ErrorDetailsTypeDef",
+    "OrganizationsDecisionDetailTypeDef",
+    "PermissionsBoundaryDecisionDetailTypeDef",
+    "GenerateCredentialReportResponseTypeDef",
     "GenerateOrganizationsAccessReportRequestRequestTypeDef",
-    "GenerateOrganizationsAccessReportResponseOutputTypeDef",
+    "GenerateOrganizationsAccessReportResponseTypeDef",
     "GenerateServiceLastAccessedDetailsRequestRequestTypeDef",
-    "GenerateServiceLastAccessedDetailsResponseOutputTypeDef",
+    "GenerateServiceLastAccessedDetailsResponseTypeDef",
     "GetAccessKeyLastUsedRequestRequestTypeDef",
     "GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef",
     "GetAccountAuthorizationDetailsRequestRequestTypeDef",
-    "PasswordPolicyOutputTypeDef",
-    "GetAccountSummaryResponseOutputTypeDef",
+    "PasswordPolicyTypeDef",
+    "GetAccountSummaryResponseTypeDef",
     "GetContextKeysForCustomPolicyRequestRequestTypeDef",
-    "GetContextKeysForPolicyResponseOutputTypeDef",
+    "GetContextKeysForPolicyResponseTypeDef",
     "GetContextKeysForPrincipalPolicyRequestRequestTypeDef",
-    "GetCredentialReportResponseOutputTypeDef",
+    "GetCredentialReportResponseTypeDef",
     "GetGroupPolicyRequestRequestTypeDef",
-    "GetGroupPolicyResponseOutputTypeDef",
+    "GetGroupPolicyResponseTypeDef",
     "GetGroupRequestGetGroupPaginateTypeDef",
     "GetGroupRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetInstanceProfileRequestRequestTypeDef",
     "GetLoginProfileRequestRequestTypeDef",
     "GetMFADeviceRequestRequestTypeDef",
-    "GetMFADeviceResponseOutputTypeDef",
+    "GetMFADeviceResponseTypeDef",
     "GetOpenIDConnectProviderRequestRequestTypeDef",
     "GetOrganizationsAccessReportRequestRequestTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetPolicyVersionRequestRequestTypeDef",
     "GetRolePolicyRequestRequestTypeDef",
-    "GetRolePolicyResponseOutputTypeDef",
+    "GetRolePolicyResponseTypeDef",
     "GetRoleRequestRequestTypeDef",
     "GetSAMLProviderRequestRequestTypeDef",
     "GetSSHPublicKeyRequestRequestTypeDef",
-    "SSHPublicKeyOutputTypeDef",
+    "SSHPublicKeyTypeDef",
     "GetServerCertificateRequestRequestTypeDef",
     "GetServiceLastAccessedDetailsRequestRequestTypeDef",
     "GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef",
     "GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef",
     "GetUserPolicyRequestRequestTypeDef",
-    "GetUserPolicyResponseOutputTypeDef",
+    "GetUserPolicyResponseTypeDef",
     "GetUserRequestRequestTypeDef",
-    "PolicyDetailOutputTypeDef",
+    "PolicyDetailTypeDef",
     "ListAccessKeysRequestListAccessKeysPaginateTypeDef",
     "ListAccessKeysRequestRequestTypeDef",
     "ListAccountAliasesRequestListAccountAliasesPaginateTypeDef",
     "ListAccountAliasesRequestRequestTypeDef",
-    "ListAccountAliasesResponseOutputTypeDef",
+    "ListAccountAliasesResponseTypeDef",
     "ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef",
     "ListAttachedGroupPoliciesRequestRequestTypeDef",
     "ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef",
     "ListAttachedRolePoliciesRequestRequestTypeDef",
     "ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef",
     "ListAttachedUserPoliciesRequestRequestTypeDef",
     "ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef",
     "ListEntitiesForPolicyRequestRequestTypeDef",
-    "PolicyGroupOutputTypeDef",
-    "PolicyRoleOutputTypeDef",
-    "PolicyUserOutputTypeDef",
+    "PolicyGroupTypeDef",
+    "PolicyRoleTypeDef",
+    "PolicyUserTypeDef",
     "ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef",
     "ListGroupPoliciesRequestRequestTypeDef",
-    "ListGroupPoliciesResponseOutputTypeDef",
+    "ListGroupPoliciesResponseTypeDef",
     "ListGroupsForUserRequestListGroupsForUserPaginateTypeDef",
     "ListGroupsForUserRequestRequestTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef",
     "ListInstanceProfileTagsRequestRequestTypeDef",
     "ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef",
     "ListInstanceProfilesForRoleRequestRequestTypeDef",
     "ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef",
     "ListInstanceProfilesRequestRequestTypeDef",
     "ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef",
     "ListMFADeviceTagsRequestRequestTypeDef",
     "ListMFADevicesRequestListMFADevicesPaginateTypeDef",
     "ListMFADevicesRequestRequestTypeDef",
-    "MFADeviceOutputTypeDef",
+    "MFADeviceTypeDef",
     "ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef",
     "ListOpenIDConnectProviderTagsRequestRequestTypeDef",
-    "OpenIDConnectProviderListEntryOutputTypeDef",
-    "PolicyGrantingServiceAccessOutputTypeDef",
+    "OpenIDConnectProviderListEntryTypeDef",
+    "PolicyGrantingServiceAccessTypeDef",
     "ListPoliciesGrantingServiceAccessRequestRequestTypeDef",
     "ListPoliciesRequestListPoliciesPaginateTypeDef",
     "ListPoliciesRequestRequestTypeDef",
     "ListPolicyTagsRequestListPolicyTagsPaginateTypeDef",
     "ListPolicyTagsRequestRequestTypeDef",
     "ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef",
     "ListPolicyVersionsRequestRequestTypeDef",
     "ListRolePoliciesRequestListRolePoliciesPaginateTypeDef",
     "ListRolePoliciesRequestRequestTypeDef",
-    "ListRolePoliciesResponseOutputTypeDef",
+    "ListRolePoliciesResponseTypeDef",
     "ListRoleTagsRequestListRoleTagsPaginateTypeDef",
     "ListRoleTagsRequestRequestTypeDef",
     "ListRolesRequestListRolesPaginateTypeDef",
     "ListRolesRequestRequestTypeDef",
     "ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef",
     "ListSAMLProviderTagsRequestRequestTypeDef",
-    "SAMLProviderListEntryOutputTypeDef",
+    "SAMLProviderListEntryTypeDef",
     "ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef",
     "ListSSHPublicKeysRequestRequestTypeDef",
-    "SSHPublicKeyMetadataOutputTypeDef",
+    "SSHPublicKeyMetadataTypeDef",
     "ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef",
     "ListServerCertificateTagsRequestRequestTypeDef",
     "ListServerCertificatesRequestListServerCertificatesPaginateTypeDef",
     "ListServerCertificatesRequestRequestTypeDef",
-    "ServerCertificateMetadataOutputTypeDef",
+    "ServerCertificateMetadataTypeDef",
     "ListServiceSpecificCredentialsRequestRequestTypeDef",
-    "ServiceSpecificCredentialMetadataOutputTypeDef",
+    "ServiceSpecificCredentialMetadataTypeDef",
     "ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef",
     "ListSigningCertificatesRequestRequestTypeDef",
-    "SigningCertificateOutputTypeDef",
+    "SigningCertificateTypeDef",
     "ListUserPoliciesRequestListUserPoliciesPaginateTypeDef",
     "ListUserPoliciesRequestRequestTypeDef",
-    "ListUserPoliciesResponseOutputTypeDef",
+    "ListUserPoliciesResponseTypeDef",
     "ListUserTagsRequestListUserTagsPaginateTypeDef",
     "ListUserTagsRequestRequestTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef",
     "ListVirtualMFADevicesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "PositionOutputTypeDef",
+    "PositionTypeDef",
     "PutGroupPolicyRequestGroupCreatePolicyTypeDef",
     "PutGroupPolicyRequestGroupPolicyPutTypeDef",
     "PutGroupPolicyRequestRequestTypeDef",
     "PutRolePermissionsBoundaryRequestRequestTypeDef",
     "PutRolePolicyRequestRequestTypeDef",
     "PutRolePolicyRequestRolePolicyPutTypeDef",
     "PutUserPermissionsBoundaryRequestRequestTypeDef",
@@ -268,18 +268,18 @@
     "RemoveUserFromGroupRequestGroupRemoveUserTypeDef",
     "RemoveUserFromGroupRequestRequestTypeDef",
     "RemoveUserFromGroupRequestUserRemoveGroupTypeDef",
     "ResetServiceSpecificCredentialRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ResyncMFADeviceRequestMfaDeviceResyncTypeDef",
     "ResyncMFADeviceRequestRequestTypeDef",
-    "RoleLastUsedOutputTypeDef",
+    "RoleLastUsedTypeDef",
     "RoleLastUsedResponseMetadataTypeDef",
     "ServerCertificateMetadataResponseMetadataTypeDef",
-    "TrackedActionLastAccessedOutputTypeDef",
+    "TrackedActionLastAccessedTypeDef",
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     "SetSecurityTokenServicePreferencesRequestRequestTypeDef",
     "UntagInstanceProfileRequestRequestTypeDef",
     "UntagMFADeviceRequestRequestTypeDef",
     "UntagOpenIDConnectProviderRequestRequestTypeDef",
     "UntagPolicyRequestRequestTypeDef",
     "UntagRoleRequestRequestTypeDef",
@@ -301,40 +301,40 @@
     "UpdateLoginProfileRequestLoginProfileUpdateTypeDef",
     "UpdateLoginProfileRequestRequestTypeDef",
     "UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef",
     "UpdateRoleDescriptionRequestRequestTypeDef",
     "UpdateRoleRequestRequestTypeDef",
     "UpdateSAMLProviderRequestRequestTypeDef",
     "UpdateSAMLProviderRequestSamlProviderUpdateTypeDef",
-    "UpdateSAMLProviderResponseOutputTypeDef",
+    "UpdateSAMLProviderResponseTypeDef",
     "UpdateSSHPublicKeyRequestRequestTypeDef",
     "UpdateServerCertificateRequestRequestTypeDef",
     "UpdateServerCertificateRequestServerCertificateUpdateTypeDef",
     "UpdateServiceSpecificCredentialRequestRequestTypeDef",
     "UpdateSigningCertificateRequestRequestTypeDef",
     "UpdateSigningCertificateRequestSigningCertificateActivateTypeDef",
     "UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateUserRequestUserUpdateTypeDef",
     "UploadSSHPublicKeyRequestRequestTypeDef",
     "UploadSigningCertificateRequestRequestTypeDef",
     "UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef",
-    "GetAccessKeyLastUsedResponseOutputTypeDef",
-    "ListAccessKeysResponseOutputTypeDef",
-    "CreateAccessKeyResponseOutputTypeDef",
-    "ListAttachedGroupPoliciesResponseOutputTypeDef",
-    "ListAttachedRolePoliciesResponseOutputTypeDef",
-    "ListAttachedUserPoliciesResponseOutputTypeDef",
+    "GetAccessKeyLastUsedResponseTypeDef",
+    "ListAccessKeysResponseTypeDef",
+    "CreateAccessKeyResponseTypeDef",
+    "ListAttachedGroupPoliciesResponseTypeDef",
+    "ListAttachedRolePoliciesResponseTypeDef",
+    "ListAttachedUserPoliciesResponseTypeDef",
     "SimulateCustomPolicyRequestRequestTypeDef",
     "SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef",
     "SimulatePrincipalPolicyRequestRequestTypeDef",
     "SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef",
-    "CreateGroupResponseOutputTypeDef",
-    "ListGroupsForUserResponseOutputTypeDef",
-    "ListGroupsResponseOutputTypeDef",
+    "CreateGroupResponseTypeDef",
+    "ListGroupsForUserResponseTypeDef",
+    "ListGroupsResponseTypeDef",
     "CreateInstanceProfileRequestRequestTypeDef",
     "CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef",
     "CreateOpenIDConnectProviderRequestRequestTypeDef",
     "CreatePolicyRequestRequestTypeDef",
     "CreatePolicyRequestServiceResourceCreatePolicyTypeDef",
     "CreateRoleRequestRequestTypeDef",
     "CreateRoleRequestServiceResourceCreateRoleTypeDef",
@@ -351,129 +351,129 @@
     "TagPolicyRequestRequestTypeDef",
     "TagRoleRequestRequestTypeDef",
     "TagSAMLProviderRequestRequestTypeDef",
     "TagServerCertificateRequestRequestTypeDef",
     "TagUserRequestRequestTypeDef",
     "UploadServerCertificateRequestRequestTypeDef",
     "UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef",
-    "CreateLoginProfileResponseOutputTypeDef",
-    "GetLoginProfileResponseOutputTypeDef",
-    "CreateOpenIDConnectProviderResponseOutputTypeDef",
-    "CreateSAMLProviderResponseOutputTypeDef",
-    "GetOpenIDConnectProviderResponseOutputTypeDef",
-    "GetSAMLProviderResponseOutputTypeDef",
-    "ListInstanceProfileTagsResponseOutputTypeDef",
-    "ListMFADeviceTagsResponseOutputTypeDef",
-    "ListOpenIDConnectProviderTagsResponseOutputTypeDef",
-    "ListPolicyTagsResponseOutputTypeDef",
-    "ListRoleTagsResponseOutputTypeDef",
-    "ListSAMLProviderTagsResponseOutputTypeDef",
-    "ListServerCertificateTagsResponseOutputTypeDef",
-    "ListUserTagsResponseOutputTypeDef",
-    "PolicyOutputTypeDef",
-    "UserOutputTypeDef",
+    "CreateLoginProfileResponseTypeDef",
+    "GetLoginProfileResponseTypeDef",
+    "CreateOpenIDConnectProviderResponseTypeDef",
+    "CreateSAMLProviderResponseTypeDef",
+    "GetOpenIDConnectProviderResponseTypeDef",
+    "GetSAMLProviderResponseTypeDef",
+    "ListInstanceProfileTagsResponseTypeDef",
+    "ListMFADeviceTagsResponseTypeDef",
+    "ListOpenIDConnectProviderTagsResponseTypeDef",
+    "ListPolicyTagsResponseTypeDef",
+    "ListRoleTagsResponseTypeDef",
+    "ListSAMLProviderTagsResponseTypeDef",
+    "ListServerCertificateTagsResponseTypeDef",
+    "ListUserTagsResponseTypeDef",
+    "PolicyTypeDef",
     "UserResponseMetadataTypeDef",
-    "CreatePolicyVersionResponseOutputTypeDef",
-    "GetPolicyVersionResponseOutputTypeDef",
-    "ListPolicyVersionsResponseOutputTypeDef",
-    "ManagedPolicyDetailOutputTypeDef",
-    "CreateServiceSpecificCredentialResponseOutputTypeDef",
-    "ResetServiceSpecificCredentialResponseOutputTypeDef",
-    "DeletionTaskFailureReasonTypeOutputTypeDef",
-    "EntityDetailsOutputTypeDef",
-    "GetOrganizationsAccessReportResponseOutputTypeDef",
-    "GetAccountPasswordPolicyResponseOutputTypeDef",
+    "UserTypeDef",
+    "CreatePolicyVersionResponseTypeDef",
+    "GetPolicyVersionResponseTypeDef",
+    "ListPolicyVersionsResponseTypeDef",
+    "ManagedPolicyDetailTypeDef",
+    "CreateServiceSpecificCredentialResponseTypeDef",
+    "ResetServiceSpecificCredentialResponseTypeDef",
+    "DeletionTaskFailureReasonTypeTypeDef",
+    "EntityDetailsTypeDef",
+    "GetOrganizationsAccessReportResponseTypeDef",
+    "GetAccountPasswordPolicyResponseTypeDef",
     "GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef",
     "GetPolicyRequestPolicyExistsWaitTypeDef",
     "GetRoleRequestRoleExistsWaitTypeDef",
     "GetUserRequestUserExistsWaitTypeDef",
-    "GetSSHPublicKeyResponseOutputTypeDef",
-    "UploadSSHPublicKeyResponseOutputTypeDef",
-    "GroupDetailOutputTypeDef",
-    "UserDetailOutputTypeDef",
-    "ListEntitiesForPolicyResponseOutputTypeDef",
-    "ListMFADevicesResponseOutputTypeDef",
-    "ListOpenIDConnectProvidersResponseOutputTypeDef",
-    "ListPoliciesGrantingServiceAccessEntryOutputTypeDef",
-    "ListSAMLProvidersResponseOutputTypeDef",
-    "ListSSHPublicKeysResponseOutputTypeDef",
-    "ListServerCertificatesResponseOutputTypeDef",
-    "ServerCertificateOutputTypeDef",
-    "UploadServerCertificateResponseOutputTypeDef",
-    "ListServiceSpecificCredentialsResponseOutputTypeDef",
-    "ListSigningCertificatesResponseOutputTypeDef",
-    "UploadSigningCertificateResponseOutputTypeDef",
-    "StatementOutputTypeDef",
-    "RoleOutputTypeDef",
-    "ServiceLastAccessedOutputTypeDef",
-    "CreatePolicyResponseOutputTypeDef",
-    "GetPolicyResponseOutputTypeDef",
-    "ListPoliciesResponseOutputTypeDef",
-    "CreateUserResponseOutputTypeDef",
-    "GetGroupResponseOutputTypeDef",
-    "GetUserResponseOutputTypeDef",
-    "ListUsersResponseOutputTypeDef",
-    "VirtualMFADeviceOutputTypeDef",
-    "GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef",
-    "GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef",
-    "ListPoliciesGrantingServiceAccessResponseOutputTypeDef",
-    "GetServerCertificateResponseOutputTypeDef",
-    "ResourceSpecificResultOutputTypeDef",
-    "CreateRoleResponseOutputTypeDef",
-    "CreateServiceLinkedRoleResponseOutputTypeDef",
-    "GetRoleResponseOutputTypeDef",
-    "InstanceProfileOutputTypeDef",
-    "ListRolesResponseOutputTypeDef",
-    "UpdateRoleDescriptionResponseOutputTypeDef",
-    "GetServiceLastAccessedDetailsResponseOutputTypeDef",
-    "CreateVirtualMFADeviceResponseOutputTypeDef",
-    "ListVirtualMFADevicesResponseOutputTypeDef",
-    "EvaluationResultOutputTypeDef",
-    "CreateInstanceProfileResponseOutputTypeDef",
-    "GetInstanceProfileResponseOutputTypeDef",
-    "ListInstanceProfilesForRoleResponseOutputTypeDef",
-    "ListInstanceProfilesResponseOutputTypeDef",
-    "RoleDetailOutputTypeDef",
-    "SimulatePolicyResponseOutputTypeDef",
-    "GetAccountAuthorizationDetailsResponseOutputTypeDef",
+    "GetSSHPublicKeyResponseTypeDef",
+    "UploadSSHPublicKeyResponseTypeDef",
+    "GroupDetailTypeDef",
+    "UserDetailTypeDef",
+    "ListEntitiesForPolicyResponseTypeDef",
+    "ListMFADevicesResponseTypeDef",
+    "ListOpenIDConnectProvidersResponseTypeDef",
+    "ListPoliciesGrantingServiceAccessEntryTypeDef",
+    "ListSAMLProvidersResponseTypeDef",
+    "ListSSHPublicKeysResponseTypeDef",
+    "ListServerCertificatesResponseTypeDef",
+    "ServerCertificateTypeDef",
+    "UploadServerCertificateResponseTypeDef",
+    "ListServiceSpecificCredentialsResponseTypeDef",
+    "ListSigningCertificatesResponseTypeDef",
+    "UploadSigningCertificateResponseTypeDef",
+    "StatementTypeDef",
+    "RoleTypeDef",
+    "ServiceLastAccessedTypeDef",
+    "CreatePolicyResponseTypeDef",
+    "GetPolicyResponseTypeDef",
+    "ListPoliciesResponseTypeDef",
+    "CreateUserResponseTypeDef",
+    "GetGroupResponseTypeDef",
+    "GetUserResponseTypeDef",
+    "ListUsersResponseTypeDef",
+    "VirtualMFADeviceTypeDef",
+    "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
+    "GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef",
+    "ListPoliciesGrantingServiceAccessResponseTypeDef",
+    "GetServerCertificateResponseTypeDef",
+    "ResourceSpecificResultTypeDef",
+    "CreateRoleResponseTypeDef",
+    "CreateServiceLinkedRoleResponseTypeDef",
+    "GetRoleResponseTypeDef",
+    "InstanceProfileTypeDef",
+    "ListRolesResponseTypeDef",
+    "UpdateRoleDescriptionResponseTypeDef",
+    "GetServiceLastAccessedDetailsResponseTypeDef",
+    "CreateVirtualMFADeviceResponseTypeDef",
+    "ListVirtualMFADevicesResponseTypeDef",
+    "EvaluationResultTypeDef",
+    "CreateInstanceProfileResponseTypeDef",
+    "GetInstanceProfileResponseTypeDef",
+    "ListInstanceProfilesForRoleResponseTypeDef",
+    "ListInstanceProfilesResponseTypeDef",
+    "RoleDetailTypeDef",
+    "SimulatePolicyResponseTypeDef",
+    "GetAccountAuthorizationDetailsResponseTypeDef",
 )
 
-AccessDetailOutputTypeDef = TypedDict(
-    "AccessDetailOutputTypeDef",
+AccessDetailTypeDef = TypedDict(
+    "AccessDetailTypeDef",
     {
         "ServiceName": str,
         "ServiceNamespace": str,
         "Region": str,
         "EntityPath": str,
         "LastAuthenticatedTime": datetime,
         "TotalAuthenticatedEntities": int,
     },
 )
 
-AccessKeyLastUsedOutputTypeDef = TypedDict(
-    "AccessKeyLastUsedOutputTypeDef",
+AccessKeyLastUsedTypeDef = TypedDict(
+    "AccessKeyLastUsedTypeDef",
     {
         "LastUsedDate": datetime,
         "ServiceName": str,
         "Region": str,
     },
 )
 
-AccessKeyMetadataOutputTypeDef = TypedDict(
-    "AccessKeyMetadataOutputTypeDef",
+AccessKeyMetadataTypeDef = TypedDict(
+    "AccessKeyMetadataTypeDef",
     {
         "UserName": str,
         "AccessKeyId": str,
         "Status": statusTypeType,
         "CreateDate": datetime,
     },
 )
 
-AccessKeyOutputTypeDef = TypedDict(
-    "AccessKeyOutputTypeDef",
+AccessKeyTypeDef = TypedDict(
+    "AccessKeyTypeDef",
     {
         "UserName": str,
         "AccessKeyId": str,
         "Status": statusTypeType,
         "SecretAccessKey": str,
         "CreateDate": datetime,
     },
@@ -586,33 +586,33 @@
 AttachUserPolicyRequestUserAttachPolicyTypeDef = TypedDict(
     "AttachUserPolicyRequestUserAttachPolicyTypeDef",
     {
         "PolicyArn": str,
     },
 )
 
-AttachedPermissionsBoundaryOutputTypeDef = TypedDict(
-    "AttachedPermissionsBoundaryOutputTypeDef",
+AttachedPermissionsBoundaryResponseMetadataTypeDef = TypedDict(
+    "AttachedPermissionsBoundaryResponseMetadataTypeDef",
     {
         "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
         "PermissionsBoundaryArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AttachedPermissionsBoundaryResponseMetadataTypeDef = TypedDict(
-    "AttachedPermissionsBoundaryResponseMetadataTypeDef",
+AttachedPermissionsBoundaryTypeDef = TypedDict(
+    "AttachedPermissionsBoundaryTypeDef",
     {
         "PermissionsBoundaryType": Literal["PermissionsBoundaryPolicy"],
         "PermissionsBoundaryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-AttachedPolicyOutputTypeDef = TypedDict(
-    "AttachedPolicyOutputTypeDef",
+AttachedPolicyTypeDef = TypedDict(
+    "AttachedPolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyArn": str,
     },
 )
 
 ChangePasswordRequestRequestTypeDef = TypedDict(
@@ -706,16 +706,16 @@
 
 class CreateGroupRequestServiceResourceCreateGroupTypeDef(
     _RequiredCreateGroupRequestServiceResourceCreateGroupTypeDef,
     _OptionalCreateGroupRequestServiceResourceCreateGroupTypeDef,
 ):
     pass
 
-GroupOutputTypeDef = TypedDict(
-    "GroupOutputTypeDef",
+GroupTypeDef = TypedDict(
+    "GroupTypeDef",
     {
         "Path": str,
         "GroupName": str,
         "GroupId": str,
         "Arn": str,
         "CreateDate": datetime,
     },
@@ -786,16 +786,16 @@
 
 class CreateLoginProfileRequestUserCreateLoginProfileTypeDef(
     _RequiredCreateLoginProfileRequestUserCreateLoginProfileTypeDef,
     _OptionalCreateLoginProfileRequestUserCreateLoginProfileTypeDef,
 ):
     pass
 
-LoginProfileOutputTypeDef = TypedDict(
-    "LoginProfileOutputTypeDef",
+LoginProfileTypeDef = TypedDict(
+    "LoginProfileTypeDef",
     {
         "UserName": str,
         "CreateDate": datetime,
         "PasswordResetRequired": bool,
     },
 )
 
@@ -844,16 +844,16 @@
 
 class CreatePolicyVersionRequestRequestTypeDef(
     _RequiredCreatePolicyVersionRequestRequestTypeDef,
     _OptionalCreatePolicyVersionRequestRequestTypeDef,
 ):
     pass
 
-PolicyVersionOutputTypeDef = TypedDict(
-    "PolicyVersionOutputTypeDef",
+PolicyVersionTypeDef = TypedDict(
+    "PolicyVersionTypeDef",
     {
         "Document": str,
         "VersionId": str,
         "IsDefaultVersion": bool,
         "CreateDate": datetime,
     },
 )
@@ -883,16 +883,16 @@
     "CreateServiceSpecificCredentialRequestRequestTypeDef",
     {
         "UserName": str,
         "ServiceName": str,
     },
 )
 
-ServiceSpecificCredentialOutputTypeDef = TypedDict(
-    "ServiceSpecificCredentialOutputTypeDef",
+ServiceSpecificCredentialTypeDef = TypedDict(
+    "ServiceSpecificCredentialTypeDef",
     {
         "CreateDate": datetime,
         "ServiceName": str,
         "ServiceUserName": str,
         "ServicePassword": str,
         "ServiceSpecificCredentialId": str,
         "UserName": str,
@@ -1032,16 +1032,16 @@
 DeleteServiceLinkedRoleRequestRequestTypeDef = TypedDict(
     "DeleteServiceLinkedRoleRequestRequestTypeDef",
     {
         "RoleName": str,
     },
 )
 
-DeleteServiceLinkedRoleResponseOutputTypeDef = TypedDict(
-    "DeleteServiceLinkedRoleResponseOutputTypeDef",
+DeleteServiceLinkedRoleResponseTypeDef = TypedDict(
+    "DeleteServiceLinkedRoleResponseTypeDef",
     {
         "DeletionTaskId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredDeleteServiceSpecificCredentialRequestRequestTypeDef = TypedDict(
@@ -1109,16 +1109,16 @@
 DeleteVirtualMFADeviceRequestRequestTypeDef = TypedDict(
     "DeleteVirtualMFADeviceRequestRequestTypeDef",
     {
         "SerialNumber": str,
     },
 )
 
-RoleUsageTypeOutputTypeDef = TypedDict(
-    "RoleUsageTypeOutputTypeDef",
+RoleUsageTypeTypeDef = TypedDict(
+    "RoleUsageTypeTypeDef",
     {
         "Region": str,
         "Resources": List[str],
     },
 )
 
 DetachGroupPolicyRequestGroupDetachPolicyTypeDef = TypedDict(
@@ -1217,49 +1217,49 @@
     {
         "SerialNumber": str,
         "AuthenticationCode1": str,
         "AuthenticationCode2": str,
     },
 )
 
-EntityInfoOutputTypeDef = TypedDict(
-    "EntityInfoOutputTypeDef",
+EntityInfoTypeDef = TypedDict(
+    "EntityInfoTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Type": policyOwnerEntityTypeType,
         "Id": str,
         "Path": str,
     },
 )
 
-ErrorDetailsOutputTypeDef = TypedDict(
-    "ErrorDetailsOutputTypeDef",
+ErrorDetailsTypeDef = TypedDict(
+    "ErrorDetailsTypeDef",
     {
         "Message": str,
         "Code": str,
     },
 )
 
-OrganizationsDecisionDetailOutputTypeDef = TypedDict(
-    "OrganizationsDecisionDetailOutputTypeDef",
+OrganizationsDecisionDetailTypeDef = TypedDict(
+    "OrganizationsDecisionDetailTypeDef",
     {
         "AllowedByOrganizations": bool,
     },
 )
 
-PermissionsBoundaryDecisionDetailOutputTypeDef = TypedDict(
-    "PermissionsBoundaryDecisionDetailOutputTypeDef",
+PermissionsBoundaryDecisionDetailTypeDef = TypedDict(
+    "PermissionsBoundaryDecisionDetailTypeDef",
     {
         "AllowedByPermissionsBoundary": bool,
     },
 )
 
-GenerateCredentialReportResponseOutputTypeDef = TypedDict(
-    "GenerateCredentialReportResponseOutputTypeDef",
+GenerateCredentialReportResponseTypeDef = TypedDict(
+    "GenerateCredentialReportResponseTypeDef",
     {
         "State": ReportStateTypeType,
         "Description": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
@@ -1279,16 +1279,16 @@
 
 class GenerateOrganizationsAccessReportRequestRequestTypeDef(
     _RequiredGenerateOrganizationsAccessReportRequestRequestTypeDef,
     _OptionalGenerateOrganizationsAccessReportRequestRequestTypeDef,
 ):
     pass
 
-GenerateOrganizationsAccessReportResponseOutputTypeDef = TypedDict(
-    "GenerateOrganizationsAccessReportResponseOutputTypeDef",
+GenerateOrganizationsAccessReportResponseTypeDef = TypedDict(
+    "GenerateOrganizationsAccessReportResponseTypeDef",
     {
         "JobId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGenerateServiceLastAccessedDetailsRequestRequestTypeDef = TypedDict(
@@ -1307,16 +1307,16 @@
 
 class GenerateServiceLastAccessedDetailsRequestRequestTypeDef(
     _RequiredGenerateServiceLastAccessedDetailsRequestRequestTypeDef,
     _OptionalGenerateServiceLastAccessedDetailsRequestRequestTypeDef,
 ):
     pass
 
-GenerateServiceLastAccessedDetailsResponseOutputTypeDef = TypedDict(
-    "GenerateServiceLastAccessedDetailsResponseOutputTypeDef",
+GenerateServiceLastAccessedDetailsResponseTypeDef = TypedDict(
+    "GenerateServiceLastAccessedDetailsResponseTypeDef",
     {
         "JobId": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetAccessKeyLastUsedRequestRequestTypeDef = TypedDict(
@@ -1341,47 +1341,47 @@
         "Filter": Sequence[EntityTypeType],
         "MaxItems": int,
         "Marker": str,
     },
     total=False,
 )
 
-PasswordPolicyOutputTypeDef = TypedDict(
-    "PasswordPolicyOutputTypeDef",
+PasswordPolicyTypeDef = TypedDict(
+    "PasswordPolicyTypeDef",
     {
         "MinimumPasswordLength": int,
         "RequireSymbols": bool,
         "RequireNumbers": bool,
         "RequireUppercaseCharacters": bool,
         "RequireLowercaseCharacters": bool,
         "AllowUsersToChangePassword": bool,
         "ExpirePasswords": bool,
         "MaxPasswordAge": int,
         "PasswordReusePrevention": int,
         "HardExpiry": bool,
     },
 )
 
-GetAccountSummaryResponseOutputTypeDef = TypedDict(
-    "GetAccountSummaryResponseOutputTypeDef",
+GetAccountSummaryResponseTypeDef = TypedDict(
+    "GetAccountSummaryResponseTypeDef",
     {
         "SummaryMap": Dict[summaryKeyTypeType, int],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetContextKeysForCustomPolicyRequestRequestTypeDef = TypedDict(
     "GetContextKeysForCustomPolicyRequestRequestTypeDef",
     {
         "PolicyInputList": Sequence[str],
     },
 )
 
-GetContextKeysForPolicyResponseOutputTypeDef = TypedDict(
-    "GetContextKeysForPolicyResponseOutputTypeDef",
+GetContextKeysForPolicyResponseTypeDef = TypedDict(
+    "GetContextKeysForPolicyResponseTypeDef",
     {
         "ContextKeyNames": List[str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetContextKeysForPrincipalPolicyRequestRequestTypeDef = TypedDict(
@@ -1400,16 +1400,16 @@
 
 class GetContextKeysForPrincipalPolicyRequestRequestTypeDef(
     _RequiredGetContextKeysForPrincipalPolicyRequestRequestTypeDef,
     _OptionalGetContextKeysForPrincipalPolicyRequestRequestTypeDef,
 ):
     pass
 
-GetCredentialReportResponseOutputTypeDef = TypedDict(
-    "GetCredentialReportResponseOutputTypeDef",
+GetCredentialReportResponseTypeDef = TypedDict(
+    "GetCredentialReportResponseTypeDef",
     {
         "Content": bytes,
         "ReportFormat": Literal["text/csv"],
         "GeneratedTime": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1418,16 +1418,16 @@
     "GetGroupPolicyRequestRequestTypeDef",
     {
         "GroupName": str,
         "PolicyName": str,
     },
 )
 
-GetGroupPolicyResponseOutputTypeDef = TypedDict(
-    "GetGroupPolicyResponseOutputTypeDef",
+GetGroupPolicyResponseTypeDef = TypedDict(
+    "GetGroupPolicyResponseTypeDef",
     {
         "GroupName": str,
         "PolicyName": str,
         "PolicyDocument": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1509,16 +1509,16 @@
 )
 
 class GetMFADeviceRequestRequestTypeDef(
     _RequiredGetMFADeviceRequestRequestTypeDef, _OptionalGetMFADeviceRequestRequestTypeDef
 ):
     pass
 
-GetMFADeviceResponseOutputTypeDef = TypedDict(
-    "GetMFADeviceResponseOutputTypeDef",
+GetMFADeviceResponseTypeDef = TypedDict(
+    "GetMFADeviceResponseTypeDef",
     {
         "UserName": str,
         "SerialNumber": str,
         "EnableDate": datetime,
         "Certifications": Dict[str, str],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
@@ -1572,16 +1572,16 @@
     "GetRolePolicyRequestRequestTypeDef",
     {
         "RoleName": str,
         "PolicyName": str,
     },
 )
 
-GetRolePolicyResponseOutputTypeDef = TypedDict(
-    "GetRolePolicyResponseOutputTypeDef",
+GetRolePolicyResponseTypeDef = TypedDict(
+    "GetRolePolicyResponseTypeDef",
     {
         "RoleName": str,
         "PolicyName": str,
         "PolicyDocument": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1605,16 +1605,16 @@
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Encoding": encodingTypeType,
     },
 )
 
-SSHPublicKeyOutputTypeDef = TypedDict(
-    "SSHPublicKeyOutputTypeDef",
+SSHPublicKeyTypeDef = TypedDict(
+    "SSHPublicKeyTypeDef",
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Fingerprint": str,
         "SSHPublicKeyBody": str,
         "Status": statusTypeType,
         "UploadDate": datetime,
@@ -1682,16 +1682,16 @@
     "GetUserPolicyRequestRequestTypeDef",
     {
         "UserName": str,
         "PolicyName": str,
     },
 )
 
-GetUserPolicyResponseOutputTypeDef = TypedDict(
-    "GetUserPolicyResponseOutputTypeDef",
+GetUserPolicyResponseTypeDef = TypedDict(
+    "GetUserPolicyResponseTypeDef",
     {
         "UserName": str,
         "PolicyName": str,
         "PolicyDocument": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1700,16 +1700,16 @@
     "GetUserRequestRequestTypeDef",
     {
         "UserName": str,
     },
     total=False,
 )
 
-PolicyDetailOutputTypeDef = TypedDict(
-    "PolicyDetailOutputTypeDef",
+PolicyDetailTypeDef = TypedDict(
+    "PolicyDetailTypeDef",
     {
         "PolicyName": str,
         "PolicyDocument": str,
     },
 )
 
 ListAccessKeysRequestListAccessKeysPaginateTypeDef = TypedDict(
@@ -1744,16 +1744,16 @@
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListAccountAliasesResponseOutputTypeDef = TypedDict(
-    "ListAccountAliasesResponseOutputTypeDef",
+ListAccountAliasesResponseTypeDef = TypedDict(
+    "ListAccountAliasesResponseTypeDef",
     {
         "AccountAliases": List[str],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -1930,32 +1930,32 @@
 
 class ListEntitiesForPolicyRequestRequestTypeDef(
     _RequiredListEntitiesForPolicyRequestRequestTypeDef,
     _OptionalListEntitiesForPolicyRequestRequestTypeDef,
 ):
     pass
 
-PolicyGroupOutputTypeDef = TypedDict(
-    "PolicyGroupOutputTypeDef",
+PolicyGroupTypeDef = TypedDict(
+    "PolicyGroupTypeDef",
     {
         "GroupName": str,
         "GroupId": str,
     },
 )
 
-PolicyRoleOutputTypeDef = TypedDict(
-    "PolicyRoleOutputTypeDef",
+PolicyRoleTypeDef = TypedDict(
+    "PolicyRoleTypeDef",
     {
         "RoleName": str,
         "RoleId": str,
     },
 )
 
-PolicyUserOutputTypeDef = TypedDict(
-    "PolicyUserOutputTypeDef",
+PolicyUserTypeDef = TypedDict(
+    "PolicyUserTypeDef",
     {
         "UserName": str,
         "UserId": str,
     },
 )
 
 _RequiredListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef = TypedDict(
@@ -1994,16 +1994,16 @@
 )
 
 class ListGroupPoliciesRequestRequestTypeDef(
     _RequiredListGroupPoliciesRequestRequestTypeDef, _OptionalListGroupPoliciesRequestRequestTypeDef
 ):
     pass
 
-ListGroupPoliciesResponseOutputTypeDef = TypedDict(
-    "ListGroupPoliciesResponseOutputTypeDef",
+ListGroupPoliciesResponseTypeDef = TypedDict(
+    "ListGroupPoliciesResponseTypeDef",
     {
         "PolicyNames": List[str],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2223,16 +2223,16 @@
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-MFADeviceOutputTypeDef = TypedDict(
-    "MFADeviceOutputTypeDef",
+MFADeviceTypeDef = TypedDict(
+    "MFADeviceTypeDef",
     {
         "UserName": str,
         "SerialNumber": str,
         "EnableDate": datetime,
     },
 )
 
@@ -2277,23 +2277,23 @@
 
 class ListOpenIDConnectProviderTagsRequestRequestTypeDef(
     _RequiredListOpenIDConnectProviderTagsRequestRequestTypeDef,
     _OptionalListOpenIDConnectProviderTagsRequestRequestTypeDef,
 ):
     pass
 
-OpenIDConnectProviderListEntryOutputTypeDef = TypedDict(
-    "OpenIDConnectProviderListEntryOutputTypeDef",
+OpenIDConnectProviderListEntryTypeDef = TypedDict(
+    "OpenIDConnectProviderListEntryTypeDef",
     {
         "Arn": str,
     },
 )
 
-PolicyGrantingServiceAccessOutputTypeDef = TypedDict(
-    "PolicyGrantingServiceAccessOutputTypeDef",
+PolicyGrantingServiceAccessTypeDef = TypedDict(
+    "PolicyGrantingServiceAccessTypeDef",
     {
         "PolicyName": str,
         "PolicyType": policyTypeType,
         "PolicyArn": str,
         "EntityType": policyOwnerEntityTypeType,
         "EntityName": str,
     },
@@ -2462,16 +2462,16 @@
 )
 
 class ListRolePoliciesRequestRequestTypeDef(
     _RequiredListRolePoliciesRequestRequestTypeDef, _OptionalListRolePoliciesRequestRequestTypeDef
 ):
     pass
 
-ListRolePoliciesResponseOutputTypeDef = TypedDict(
-    "ListRolePoliciesResponseOutputTypeDef",
+ListRolePoliciesResponseTypeDef = TypedDict(
+    "ListRolePoliciesResponseTypeDef",
     {
         "PolicyNames": List[str],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2572,16 +2572,16 @@
 
 class ListSAMLProviderTagsRequestRequestTypeDef(
     _RequiredListSAMLProviderTagsRequestRequestTypeDef,
     _OptionalListSAMLProviderTagsRequestRequestTypeDef,
 ):
     pass
 
-SAMLProviderListEntryOutputTypeDef = TypedDict(
-    "SAMLProviderListEntryOutputTypeDef",
+SAMLProviderListEntryTypeDef = TypedDict(
+    "SAMLProviderListEntryTypeDef",
     {
         "Arn": str,
         "ValidUntil": datetime,
         "CreateDate": datetime,
     },
 )
 
@@ -2600,16 +2600,16 @@
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-SSHPublicKeyMetadataOutputTypeDef = TypedDict(
-    "SSHPublicKeyMetadataOutputTypeDef",
+SSHPublicKeyMetadataTypeDef = TypedDict(
+    "SSHPublicKeyMetadataTypeDef",
     {
         "UserName": str,
         "SSHPublicKeyId": str,
         "Status": statusTypeType,
         "UploadDate": datetime,
     },
 )
@@ -2670,16 +2670,16 @@
         "PathPrefix": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ServerCertificateMetadataOutputTypeDef = TypedDict(
-    "ServerCertificateMetadataOutputTypeDef",
+ServerCertificateMetadataTypeDef = TypedDict(
+    "ServerCertificateMetadataTypeDef",
     {
         "Path": str,
         "ServerCertificateName": str,
         "ServerCertificateId": str,
         "Arn": str,
         "UploadDate": datetime,
         "Expiration": datetime,
@@ -2691,16 +2691,16 @@
     {
         "UserName": str,
         "ServiceName": str,
     },
     total=False,
 )
 
-ServiceSpecificCredentialMetadataOutputTypeDef = TypedDict(
-    "ServiceSpecificCredentialMetadataOutputTypeDef",
+ServiceSpecificCredentialMetadataTypeDef = TypedDict(
+    "ServiceSpecificCredentialMetadataTypeDef",
     {
         "UserName": str,
         "Status": statusTypeType,
         "ServiceUserName": str,
         "CreateDate": datetime,
         "ServiceSpecificCredentialId": str,
         "ServiceName": str,
@@ -2722,16 +2722,16 @@
         "UserName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-SigningCertificateOutputTypeDef = TypedDict(
-    "SigningCertificateOutputTypeDef",
+SigningCertificateTypeDef = TypedDict(
+    "SigningCertificateTypeDef",
     {
         "UserName": str,
         "CertificateId": str,
         "CertificateBody": str,
         "Status": statusTypeType,
         "UploadDate": datetime,
     },
@@ -2773,16 +2773,16 @@
 )
 
 class ListUserPoliciesRequestRequestTypeDef(
     _RequiredListUserPoliciesRequestRequestTypeDef, _OptionalListUserPoliciesRequestRequestTypeDef
 ):
     pass
 
-ListUserPoliciesResponseOutputTypeDef = TypedDict(
-    "ListUserPoliciesResponseOutputTypeDef",
+ListUserPoliciesResponseTypeDef = TypedDict(
+    "ListUserPoliciesResponseTypeDef",
     {
         "PolicyNames": List[str],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
@@ -2871,16 +2871,16 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
     total=False,
 )
 
-PositionOutputTypeDef = TypedDict(
-    "PositionOutputTypeDef",
+PositionTypeDef = TypedDict(
+    "PositionTypeDef",
     {
         "Line": int,
         "Column": int,
     },
 )
 
 PutGroupPolicyRequestGroupCreatePolicyTypeDef = TypedDict(
@@ -3053,16 +3053,16 @@
         "UserName": str,
         "SerialNumber": str,
         "AuthenticationCode1": str,
         "AuthenticationCode2": str,
     },
 )
 
-RoleLastUsedOutputTypeDef = TypedDict(
-    "RoleLastUsedOutputTypeDef",
+RoleLastUsedTypeDef = TypedDict(
+    "RoleLastUsedTypeDef",
     {
         "LastUsedDate": datetime,
         "Region": str,
     },
 )
 
 RoleLastUsedResponseMetadataTypeDef = TypedDict(
@@ -3083,16 +3083,16 @@
         "Arn": str,
         "UploadDate": datetime,
         "Expiration": datetime,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-TrackedActionLastAccessedOutputTypeDef = TypedDict(
-    "TrackedActionLastAccessedOutputTypeDef",
+TrackedActionLastAccessedTypeDef = TypedDict(
+    "TrackedActionLastAccessedTypeDef",
     {
         "ActionName": str,
         "LastAccessedEntity": str,
         "LastAccessedTime": datetime,
         "LastAccessedRegion": str,
     },
 )
@@ -3397,16 +3397,16 @@
 UpdateSAMLProviderRequestSamlProviderUpdateTypeDef = TypedDict(
     "UpdateSAMLProviderRequestSamlProviderUpdateTypeDef",
     {
         "SAMLMetadataDocument": str,
     },
 )
 
-UpdateSAMLProviderResponseOutputTypeDef = TypedDict(
-    "UpdateSAMLProviderResponseOutputTypeDef",
+UpdateSAMLProviderResponseTypeDef = TypedDict(
+    "UpdateSAMLProviderResponseTypeDef",
     {
         "SAMLProviderArn": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 UpdateSSHPublicKeyRequestRequestTypeDef = TypedDict(
@@ -3579,65 +3579,65 @@
 
 class UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef(
     _RequiredUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
     _OptionalUploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
 ):
     pass
 
-GetAccessKeyLastUsedResponseOutputTypeDef = TypedDict(
-    "GetAccessKeyLastUsedResponseOutputTypeDef",
+GetAccessKeyLastUsedResponseTypeDef = TypedDict(
+    "GetAccessKeyLastUsedResponseTypeDef",
     {
         "UserName": str,
-        "AccessKeyLastUsed": AccessKeyLastUsedOutputTypeDef,
+        "AccessKeyLastUsed": AccessKeyLastUsedTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAccessKeysResponseOutputTypeDef = TypedDict(
-    "ListAccessKeysResponseOutputTypeDef",
+ListAccessKeysResponseTypeDef = TypedDict(
+    "ListAccessKeysResponseTypeDef",
     {
-        "AccessKeyMetadata": List[AccessKeyMetadataOutputTypeDef],
+        "AccessKeyMetadata": List[AccessKeyMetadataTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateAccessKeyResponseOutputTypeDef = TypedDict(
-    "CreateAccessKeyResponseOutputTypeDef",
+CreateAccessKeyResponseTypeDef = TypedDict(
+    "CreateAccessKeyResponseTypeDef",
     {
-        "AccessKey": AccessKeyOutputTypeDef,
+        "AccessKey": AccessKeyTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAttachedGroupPoliciesResponseOutputTypeDef = TypedDict(
-    "ListAttachedGroupPoliciesResponseOutputTypeDef",
+ListAttachedGroupPoliciesResponseTypeDef = TypedDict(
+    "ListAttachedGroupPoliciesResponseTypeDef",
     {
-        "AttachedPolicies": List[AttachedPolicyOutputTypeDef],
+        "AttachedPolicies": List[AttachedPolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAttachedRolePoliciesResponseOutputTypeDef = TypedDict(
-    "ListAttachedRolePoliciesResponseOutputTypeDef",
+ListAttachedRolePoliciesResponseTypeDef = TypedDict(
+    "ListAttachedRolePoliciesResponseTypeDef",
     {
-        "AttachedPolicies": List[AttachedPolicyOutputTypeDef],
+        "AttachedPolicies": List[AttachedPolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListAttachedUserPoliciesResponseOutputTypeDef = TypedDict(
-    "ListAttachedUserPoliciesResponseOutputTypeDef",
+ListAttachedUserPoliciesResponseTypeDef = TypedDict(
+    "ListAttachedUserPoliciesResponseTypeDef",
     {
-        "AttachedPolicies": List[AttachedPolicyOutputTypeDef],
+        "AttachedPolicies": List[AttachedPolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredSimulateCustomPolicyRequestRequestTypeDef = TypedDict(
@@ -3752,36 +3752,36 @@
 
 class SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef(
     _RequiredSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
     _OptionalSimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
 ):
     pass
 
-CreateGroupResponseOutputTypeDef = TypedDict(
-    "CreateGroupResponseOutputTypeDef",
+CreateGroupResponseTypeDef = TypedDict(
+    "CreateGroupResponseTypeDef",
     {
-        "Group": GroupOutputTypeDef,
+        "Group": GroupTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListGroupsForUserResponseOutputTypeDef = TypedDict(
-    "ListGroupsForUserResponseOutputTypeDef",
+ListGroupsForUserResponseTypeDef = TypedDict(
+    "ListGroupsForUserResponseTypeDef",
     {
-        "Groups": List[GroupOutputTypeDef],
+        "Groups": List[GroupTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListGroupsResponseOutputTypeDef = TypedDict(
-    "ListGroupsResponseOutputTypeDef",
+ListGroupsResponseTypeDef = TypedDict(
+    "ListGroupsResponseTypeDef",
     {
-        "Groups": List[GroupOutputTypeDef],
+        "Groups": List[GroupTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredCreateInstanceProfileRequestRequestTypeDef = TypedDict(
@@ -4187,153 +4187,153 @@
 
 class UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef(
     _RequiredUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
     _OptionalUploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
 ):
     pass
 
-CreateLoginProfileResponseOutputTypeDef = TypedDict(
-    "CreateLoginProfileResponseOutputTypeDef",
+CreateLoginProfileResponseTypeDef = TypedDict(
+    "CreateLoginProfileResponseTypeDef",
     {
-        "LoginProfile": LoginProfileOutputTypeDef,
+        "LoginProfile": LoginProfileTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetLoginProfileResponseOutputTypeDef = TypedDict(
-    "GetLoginProfileResponseOutputTypeDef",
+GetLoginProfileResponseTypeDef = TypedDict(
+    "GetLoginProfileResponseTypeDef",
     {
-        "LoginProfile": LoginProfileOutputTypeDef,
+        "LoginProfile": LoginProfileTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateOpenIDConnectProviderResponseOutputTypeDef = TypedDict(
-    "CreateOpenIDConnectProviderResponseOutputTypeDef",
+CreateOpenIDConnectProviderResponseTypeDef = TypedDict(
+    "CreateOpenIDConnectProviderResponseTypeDef",
     {
         "OpenIDConnectProviderArn": str,
         "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateSAMLProviderResponseOutputTypeDef = TypedDict(
-    "CreateSAMLProviderResponseOutputTypeDef",
+CreateSAMLProviderResponseTypeDef = TypedDict(
+    "CreateSAMLProviderResponseTypeDef",
     {
         "SAMLProviderArn": str,
         "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetOpenIDConnectProviderResponseOutputTypeDef = TypedDict(
-    "GetOpenIDConnectProviderResponseOutputTypeDef",
+GetOpenIDConnectProviderResponseTypeDef = TypedDict(
+    "GetOpenIDConnectProviderResponseTypeDef",
     {
         "Url": str,
         "ClientIDList": List[str],
         "ThumbprintList": List[str],
         "CreateDate": datetime,
         "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetSAMLProviderResponseOutputTypeDef = TypedDict(
-    "GetSAMLProviderResponseOutputTypeDef",
+GetSAMLProviderResponseTypeDef = TypedDict(
+    "GetSAMLProviderResponseTypeDef",
     {
         "SAMLMetadataDocument": str,
         "CreateDate": datetime,
         "ValidUntil": datetime,
         "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListInstanceProfileTagsResponseOutputTypeDef = TypedDict(
-    "ListInstanceProfileTagsResponseOutputTypeDef",
+ListInstanceProfileTagsResponseTypeDef = TypedDict(
+    "ListInstanceProfileTagsResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListMFADeviceTagsResponseOutputTypeDef = TypedDict(
-    "ListMFADeviceTagsResponseOutputTypeDef",
+ListMFADeviceTagsResponseTypeDef = TypedDict(
+    "ListMFADeviceTagsResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListOpenIDConnectProviderTagsResponseOutputTypeDef = TypedDict(
-    "ListOpenIDConnectProviderTagsResponseOutputTypeDef",
+ListOpenIDConnectProviderTagsResponseTypeDef = TypedDict(
+    "ListOpenIDConnectProviderTagsResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPolicyTagsResponseOutputTypeDef = TypedDict(
-    "ListPolicyTagsResponseOutputTypeDef",
+ListPolicyTagsResponseTypeDef = TypedDict(
+    "ListPolicyTagsResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListRoleTagsResponseOutputTypeDef = TypedDict(
-    "ListRoleTagsResponseOutputTypeDef",
+ListRoleTagsResponseTypeDef = TypedDict(
+    "ListRoleTagsResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSAMLProviderTagsResponseOutputTypeDef = TypedDict(
-    "ListSAMLProviderTagsResponseOutputTypeDef",
+ListSAMLProviderTagsResponseTypeDef = TypedDict(
+    "ListSAMLProviderTagsResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServerCertificateTagsResponseOutputTypeDef = TypedDict(
-    "ListServerCertificateTagsResponseOutputTypeDef",
+ListServerCertificateTagsResponseTypeDef = TypedDict(
+    "ListServerCertificateTagsResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListUserTagsResponseOutputTypeDef = TypedDict(
-    "ListUserTagsResponseOutputTypeDef",
+ListUserTagsResponseTypeDef = TypedDict(
+    "ListUserTagsResponseTypeDef",
     {
         "Tags": List[TagOutputTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-PolicyOutputTypeDef = TypedDict(
-    "PolicyOutputTypeDef",
+PolicyTypeDef = TypedDict(
+    "PolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyId": str,
         "Arn": str,
         "Path": str,
         "DefaultVersionId": str,
         "AttachmentCount": int,
@@ -4342,139 +4342,139 @@
         "Description": str,
         "CreateDate": datetime,
         "UpdateDate": datetime,
         "Tags": List[TagOutputTypeDef],
     },
 )
 
-UserOutputTypeDef = TypedDict(
-    "UserOutputTypeDef",
+UserResponseMetadataTypeDef = TypedDict(
+    "UserResponseMetadataTypeDef",
     {
         "Path": str,
         "UserName": str,
         "UserId": str,
         "Arn": str,
         "CreateDate": datetime,
         "PasswordLastUsed": datetime,
-        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagOutputTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UserResponseMetadataTypeDef = TypedDict(
-    "UserResponseMetadataTypeDef",
+UserTypeDef = TypedDict(
+    "UserTypeDef",
     {
         "Path": str,
         "UserName": str,
         "UserId": str,
         "Arn": str,
         "CreateDate": datetime,
         "PasswordLastUsed": datetime,
-        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreatePolicyVersionResponseOutputTypeDef = TypedDict(
-    "CreatePolicyVersionResponseOutputTypeDef",
+CreatePolicyVersionResponseTypeDef = TypedDict(
+    "CreatePolicyVersionResponseTypeDef",
     {
-        "PolicyVersion": PolicyVersionOutputTypeDef,
+        "PolicyVersion": PolicyVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPolicyVersionResponseOutputTypeDef = TypedDict(
-    "GetPolicyVersionResponseOutputTypeDef",
+GetPolicyVersionResponseTypeDef = TypedDict(
+    "GetPolicyVersionResponseTypeDef",
     {
-        "PolicyVersion": PolicyVersionOutputTypeDef,
+        "PolicyVersion": PolicyVersionTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPolicyVersionsResponseOutputTypeDef = TypedDict(
-    "ListPolicyVersionsResponseOutputTypeDef",
+ListPolicyVersionsResponseTypeDef = TypedDict(
+    "ListPolicyVersionsResponseTypeDef",
     {
-        "Versions": List[PolicyVersionOutputTypeDef],
+        "Versions": List[PolicyVersionTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ManagedPolicyDetailOutputTypeDef = TypedDict(
-    "ManagedPolicyDetailOutputTypeDef",
+ManagedPolicyDetailTypeDef = TypedDict(
+    "ManagedPolicyDetailTypeDef",
     {
         "PolicyName": str,
         "PolicyId": str,
         "Arn": str,
         "Path": str,
         "DefaultVersionId": str,
         "AttachmentCount": int,
         "PermissionsBoundaryUsageCount": int,
         "IsAttachable": bool,
         "Description": str,
         "CreateDate": datetime,
         "UpdateDate": datetime,
-        "PolicyVersionList": List[PolicyVersionOutputTypeDef],
+        "PolicyVersionList": List[PolicyVersionTypeDef],
     },
 )
 
-CreateServiceSpecificCredentialResponseOutputTypeDef = TypedDict(
-    "CreateServiceSpecificCredentialResponseOutputTypeDef",
+CreateServiceSpecificCredentialResponseTypeDef = TypedDict(
+    "CreateServiceSpecificCredentialResponseTypeDef",
     {
-        "ServiceSpecificCredential": ServiceSpecificCredentialOutputTypeDef,
+        "ServiceSpecificCredential": ServiceSpecificCredentialTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResetServiceSpecificCredentialResponseOutputTypeDef = TypedDict(
-    "ResetServiceSpecificCredentialResponseOutputTypeDef",
+ResetServiceSpecificCredentialResponseTypeDef = TypedDict(
+    "ResetServiceSpecificCredentialResponseTypeDef",
     {
-        "ServiceSpecificCredential": ServiceSpecificCredentialOutputTypeDef,
+        "ServiceSpecificCredential": ServiceSpecificCredentialTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-DeletionTaskFailureReasonTypeOutputTypeDef = TypedDict(
-    "DeletionTaskFailureReasonTypeOutputTypeDef",
+DeletionTaskFailureReasonTypeTypeDef = TypedDict(
+    "DeletionTaskFailureReasonTypeTypeDef",
     {
         "Reason": str,
-        "RoleUsageList": List[RoleUsageTypeOutputTypeDef],
+        "RoleUsageList": List[RoleUsageTypeTypeDef],
     },
 )
 
-EntityDetailsOutputTypeDef = TypedDict(
-    "EntityDetailsOutputTypeDef",
+EntityDetailsTypeDef = TypedDict(
+    "EntityDetailsTypeDef",
     {
-        "EntityInfo": EntityInfoOutputTypeDef,
+        "EntityInfo": EntityInfoTypeDef,
         "LastAuthenticated": datetime,
     },
 )
 
-GetOrganizationsAccessReportResponseOutputTypeDef = TypedDict(
-    "GetOrganizationsAccessReportResponseOutputTypeDef",
+GetOrganizationsAccessReportResponseTypeDef = TypedDict(
+    "GetOrganizationsAccessReportResponseTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobCreationDate": datetime,
         "JobCompletionDate": datetime,
         "NumberOfServicesAccessible": int,
         "NumberOfServicesNotAccessed": int,
-        "AccessDetails": List[AccessDetailOutputTypeDef],
+        "AccessDetails": List[AccessDetailTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "ErrorDetails": ErrorDetailsOutputTypeDef,
+        "ErrorDetails": ErrorDetailsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAccountPasswordPolicyResponseOutputTypeDef = TypedDict(
-    "GetAccountPasswordPolicyResponseOutputTypeDef",
+GetAccountPasswordPolicyResponseTypeDef = TypedDict(
+    "GetAccountPasswordPolicyResponseTypeDef",
     {
-        "PasswordPolicy": PasswordPolicyOutputTypeDef,
+        "PasswordPolicy": PasswordPolicyTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef = TypedDict(
     "_RequiredGetInstanceProfileRequestInstanceProfileExistsWaitTypeDef",
     {
@@ -4539,510 +4539,510 @@
     {
         "UserName": str,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-GetSSHPublicKeyResponseOutputTypeDef = TypedDict(
-    "GetSSHPublicKeyResponseOutputTypeDef",
+GetSSHPublicKeyResponseTypeDef = TypedDict(
+    "GetSSHPublicKeyResponseTypeDef",
     {
-        "SSHPublicKey": SSHPublicKeyOutputTypeDef,
+        "SSHPublicKey": SSHPublicKeyTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UploadSSHPublicKeyResponseOutputTypeDef = TypedDict(
-    "UploadSSHPublicKeyResponseOutputTypeDef",
+UploadSSHPublicKeyResponseTypeDef = TypedDict(
+    "UploadSSHPublicKeyResponseTypeDef",
     {
-        "SSHPublicKey": SSHPublicKeyOutputTypeDef,
+        "SSHPublicKey": SSHPublicKeyTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GroupDetailOutputTypeDef = TypedDict(
-    "GroupDetailOutputTypeDef",
+GroupDetailTypeDef = TypedDict(
+    "GroupDetailTypeDef",
     {
         "Path": str,
         "GroupName": str,
         "GroupId": str,
         "Arn": str,
         "CreateDate": datetime,
-        "GroupPolicyList": List[PolicyDetailOutputTypeDef],
-        "AttachedManagedPolicies": List[AttachedPolicyOutputTypeDef],
+        "GroupPolicyList": List[PolicyDetailTypeDef],
+        "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
     },
 )
 
-UserDetailOutputTypeDef = TypedDict(
-    "UserDetailOutputTypeDef",
+UserDetailTypeDef = TypedDict(
+    "UserDetailTypeDef",
     {
         "Path": str,
         "UserName": str,
         "UserId": str,
         "Arn": str,
         "CreateDate": datetime,
-        "UserPolicyList": List[PolicyDetailOutputTypeDef],
+        "UserPolicyList": List[PolicyDetailTypeDef],
         "GroupList": List[str],
-        "AttachedManagedPolicies": List[AttachedPolicyOutputTypeDef],
-        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagOutputTypeDef],
     },
 )
 
-ListEntitiesForPolicyResponseOutputTypeDef = TypedDict(
-    "ListEntitiesForPolicyResponseOutputTypeDef",
+ListEntitiesForPolicyResponseTypeDef = TypedDict(
+    "ListEntitiesForPolicyResponseTypeDef",
     {
-        "PolicyGroups": List[PolicyGroupOutputTypeDef],
-        "PolicyUsers": List[PolicyUserOutputTypeDef],
-        "PolicyRoles": List[PolicyRoleOutputTypeDef],
+        "PolicyGroups": List[PolicyGroupTypeDef],
+        "PolicyUsers": List[PolicyUserTypeDef],
+        "PolicyRoles": List[PolicyRoleTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListMFADevicesResponseOutputTypeDef = TypedDict(
-    "ListMFADevicesResponseOutputTypeDef",
+ListMFADevicesResponseTypeDef = TypedDict(
+    "ListMFADevicesResponseTypeDef",
     {
-        "MFADevices": List[MFADeviceOutputTypeDef],
+        "MFADevices": List[MFADeviceTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListOpenIDConnectProvidersResponseOutputTypeDef = TypedDict(
-    "ListOpenIDConnectProvidersResponseOutputTypeDef",
+ListOpenIDConnectProvidersResponseTypeDef = TypedDict(
+    "ListOpenIDConnectProvidersResponseTypeDef",
     {
-        "OpenIDConnectProviderList": List[OpenIDConnectProviderListEntryOutputTypeDef],
+        "OpenIDConnectProviderList": List[OpenIDConnectProviderListEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPoliciesGrantingServiceAccessEntryOutputTypeDef = TypedDict(
-    "ListPoliciesGrantingServiceAccessEntryOutputTypeDef",
+ListPoliciesGrantingServiceAccessEntryTypeDef = TypedDict(
+    "ListPoliciesGrantingServiceAccessEntryTypeDef",
     {
         "ServiceNamespace": str,
-        "Policies": List[PolicyGrantingServiceAccessOutputTypeDef],
+        "Policies": List[PolicyGrantingServiceAccessTypeDef],
     },
 )
 
-ListSAMLProvidersResponseOutputTypeDef = TypedDict(
-    "ListSAMLProvidersResponseOutputTypeDef",
+ListSAMLProvidersResponseTypeDef = TypedDict(
+    "ListSAMLProvidersResponseTypeDef",
     {
-        "SAMLProviderList": List[SAMLProviderListEntryOutputTypeDef],
+        "SAMLProviderList": List[SAMLProviderListEntryTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSSHPublicKeysResponseOutputTypeDef = TypedDict(
-    "ListSSHPublicKeysResponseOutputTypeDef",
+ListSSHPublicKeysResponseTypeDef = TypedDict(
+    "ListSSHPublicKeysResponseTypeDef",
     {
-        "SSHPublicKeys": List[SSHPublicKeyMetadataOutputTypeDef],
+        "SSHPublicKeys": List[SSHPublicKeyMetadataTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServerCertificatesResponseOutputTypeDef = TypedDict(
-    "ListServerCertificatesResponseOutputTypeDef",
+ListServerCertificatesResponseTypeDef = TypedDict(
+    "ListServerCertificatesResponseTypeDef",
     {
-        "ServerCertificateMetadataList": List[ServerCertificateMetadataOutputTypeDef],
+        "ServerCertificateMetadataList": List[ServerCertificateMetadataTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ServerCertificateOutputTypeDef = TypedDict(
-    "ServerCertificateOutputTypeDef",
+ServerCertificateTypeDef = TypedDict(
+    "ServerCertificateTypeDef",
     {
-        "ServerCertificateMetadata": ServerCertificateMetadataOutputTypeDef,
+        "ServerCertificateMetadata": ServerCertificateMetadataTypeDef,
         "CertificateBody": str,
         "CertificateChain": str,
         "Tags": List[TagOutputTypeDef],
     },
 )
 
-UploadServerCertificateResponseOutputTypeDef = TypedDict(
-    "UploadServerCertificateResponseOutputTypeDef",
+UploadServerCertificateResponseTypeDef = TypedDict(
+    "UploadServerCertificateResponseTypeDef",
     {
-        "ServerCertificateMetadata": ServerCertificateMetadataOutputTypeDef,
+        "ServerCertificateMetadata": ServerCertificateMetadataTypeDef,
         "Tags": List[TagOutputTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListServiceSpecificCredentialsResponseOutputTypeDef = TypedDict(
-    "ListServiceSpecificCredentialsResponseOutputTypeDef",
+ListServiceSpecificCredentialsResponseTypeDef = TypedDict(
+    "ListServiceSpecificCredentialsResponseTypeDef",
     {
-        "ServiceSpecificCredentials": List[ServiceSpecificCredentialMetadataOutputTypeDef],
+        "ServiceSpecificCredentials": List[ServiceSpecificCredentialMetadataTypeDef],
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListSigningCertificatesResponseOutputTypeDef = TypedDict(
-    "ListSigningCertificatesResponseOutputTypeDef",
+ListSigningCertificatesResponseTypeDef = TypedDict(
+    "ListSigningCertificatesResponseTypeDef",
     {
-        "Certificates": List[SigningCertificateOutputTypeDef],
+        "Certificates": List[SigningCertificateTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UploadSigningCertificateResponseOutputTypeDef = TypedDict(
-    "UploadSigningCertificateResponseOutputTypeDef",
+UploadSigningCertificateResponseTypeDef = TypedDict(
+    "UploadSigningCertificateResponseTypeDef",
     {
-        "Certificate": SigningCertificateOutputTypeDef,
+        "Certificate": SigningCertificateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-StatementOutputTypeDef = TypedDict(
-    "StatementOutputTypeDef",
+StatementTypeDef = TypedDict(
+    "StatementTypeDef",
     {
         "SourcePolicyId": str,
         "SourcePolicyType": PolicySourceTypeType,
-        "StartPosition": PositionOutputTypeDef,
-        "EndPosition": PositionOutputTypeDef,
+        "StartPosition": PositionTypeDef,
+        "EndPosition": PositionTypeDef,
     },
 )
 
-RoleOutputTypeDef = TypedDict(
-    "RoleOutputTypeDef",
+RoleTypeDef = TypedDict(
+    "RoleTypeDef",
     {
         "Path": str,
         "RoleName": str,
         "RoleId": str,
         "Arn": str,
         "CreateDate": datetime,
         "AssumeRolePolicyDocument": str,
         "Description": str,
         "MaxSessionDuration": int,
-        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagOutputTypeDef],
-        "RoleLastUsed": RoleLastUsedOutputTypeDef,
+        "RoleLastUsed": RoleLastUsedTypeDef,
     },
 )
 
-ServiceLastAccessedOutputTypeDef = TypedDict(
-    "ServiceLastAccessedOutputTypeDef",
+ServiceLastAccessedTypeDef = TypedDict(
+    "ServiceLastAccessedTypeDef",
     {
         "ServiceName": str,
         "LastAuthenticated": datetime,
         "ServiceNamespace": str,
         "LastAuthenticatedEntity": str,
         "LastAuthenticatedRegion": str,
         "TotalAuthenticatedEntities": int,
-        "TrackedActionsLastAccessed": List[TrackedActionLastAccessedOutputTypeDef],
+        "TrackedActionsLastAccessed": List[TrackedActionLastAccessedTypeDef],
     },
 )
 
-CreatePolicyResponseOutputTypeDef = TypedDict(
-    "CreatePolicyResponseOutputTypeDef",
+CreatePolicyResponseTypeDef = TypedDict(
+    "CreatePolicyResponseTypeDef",
     {
-        "Policy": PolicyOutputTypeDef,
+        "Policy": PolicyTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetPolicyResponseOutputTypeDef = TypedDict(
-    "GetPolicyResponseOutputTypeDef",
+GetPolicyResponseTypeDef = TypedDict(
+    "GetPolicyResponseTypeDef",
     {
-        "Policy": PolicyOutputTypeDef,
+        "Policy": PolicyTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPoliciesResponseOutputTypeDef = TypedDict(
-    "ListPoliciesResponseOutputTypeDef",
+ListPoliciesResponseTypeDef = TypedDict(
+    "ListPoliciesResponseTypeDef",
     {
-        "Policies": List[PolicyOutputTypeDef],
+        "Policies": List[PolicyTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateUserResponseOutputTypeDef = TypedDict(
-    "CreateUserResponseOutputTypeDef",
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
     {
-        "User": UserOutputTypeDef,
+        "User": UserTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetGroupResponseOutputTypeDef = TypedDict(
-    "GetGroupResponseOutputTypeDef",
+GetGroupResponseTypeDef = TypedDict(
+    "GetGroupResponseTypeDef",
     {
-        "Group": GroupOutputTypeDef,
-        "Users": List[UserOutputTypeDef],
+        "Group": GroupTypeDef,
+        "Users": List[UserTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetUserResponseOutputTypeDef = TypedDict(
-    "GetUserResponseOutputTypeDef",
+GetUserResponseTypeDef = TypedDict(
+    "GetUserResponseTypeDef",
     {
-        "User": UserOutputTypeDef,
+        "User": UserTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListUsersResponseOutputTypeDef = TypedDict(
-    "ListUsersResponseOutputTypeDef",
+ListUsersResponseTypeDef = TypedDict(
+    "ListUsersResponseTypeDef",
     {
-        "Users": List[UserOutputTypeDef],
+        "Users": List[UserTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-VirtualMFADeviceOutputTypeDef = TypedDict(
-    "VirtualMFADeviceOutputTypeDef",
+VirtualMFADeviceTypeDef = TypedDict(
+    "VirtualMFADeviceTypeDef",
     {
         "SerialNumber": str,
         "Base32StringSeed": bytes,
         "QRCodePNG": bytes,
-        "User": UserOutputTypeDef,
+        "User": UserTypeDef,
         "EnableDate": datetime,
         "Tags": List[TagOutputTypeDef],
     },
 )
 
-GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef = TypedDict(
-    "GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef",
+GetServiceLinkedRoleDeletionStatusResponseTypeDef = TypedDict(
+    "GetServiceLinkedRoleDeletionStatusResponseTypeDef",
     {
         "Status": DeletionTaskStatusTypeType,
-        "Reason": DeletionTaskFailureReasonTypeOutputTypeDef,
+        "Reason": DeletionTaskFailureReasonTypeTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef = TypedDict(
-    "GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef",
+GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef = TypedDict(
+    "GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobCreationDate": datetime,
         "JobCompletionDate": datetime,
-        "EntityDetailsList": List[EntityDetailsOutputTypeDef],
+        "EntityDetailsList": List[EntityDetailsTypeDef],
         "IsTruncated": bool,
         "Marker": str,
-        "Error": ErrorDetailsOutputTypeDef,
+        "Error": ErrorDetailsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListPoliciesGrantingServiceAccessResponseOutputTypeDef = TypedDict(
-    "ListPoliciesGrantingServiceAccessResponseOutputTypeDef",
+ListPoliciesGrantingServiceAccessResponseTypeDef = TypedDict(
+    "ListPoliciesGrantingServiceAccessResponseTypeDef",
     {
-        "PoliciesGrantingServiceAccess": List[ListPoliciesGrantingServiceAccessEntryOutputTypeDef],
+        "PoliciesGrantingServiceAccess": List[ListPoliciesGrantingServiceAccessEntryTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServerCertificateResponseOutputTypeDef = TypedDict(
-    "GetServerCertificateResponseOutputTypeDef",
+GetServerCertificateResponseTypeDef = TypedDict(
+    "GetServerCertificateResponseTypeDef",
     {
-        "ServerCertificate": ServerCertificateOutputTypeDef,
+        "ServerCertificate": ServerCertificateTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ResourceSpecificResultOutputTypeDef = TypedDict(
-    "ResourceSpecificResultOutputTypeDef",
+ResourceSpecificResultTypeDef = TypedDict(
+    "ResourceSpecificResultTypeDef",
     {
         "EvalResourceName": str,
         "EvalResourceDecision": PolicyEvaluationDecisionTypeType,
-        "MatchedStatements": List[StatementOutputTypeDef],
+        "MatchedStatements": List[StatementTypeDef],
         "MissingContextValues": List[str],
         "EvalDecisionDetails": Dict[str, PolicyEvaluationDecisionTypeType],
-        "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailOutputTypeDef,
+        "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailTypeDef,
     },
 )
 
-CreateRoleResponseOutputTypeDef = TypedDict(
-    "CreateRoleResponseOutputTypeDef",
+CreateRoleResponseTypeDef = TypedDict(
+    "CreateRoleResponseTypeDef",
     {
-        "Role": RoleOutputTypeDef,
+        "Role": RoleTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateServiceLinkedRoleResponseOutputTypeDef = TypedDict(
-    "CreateServiceLinkedRoleResponseOutputTypeDef",
+CreateServiceLinkedRoleResponseTypeDef = TypedDict(
+    "CreateServiceLinkedRoleResponseTypeDef",
     {
-        "Role": RoleOutputTypeDef,
+        "Role": RoleTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetRoleResponseOutputTypeDef = TypedDict(
-    "GetRoleResponseOutputTypeDef",
+GetRoleResponseTypeDef = TypedDict(
+    "GetRoleResponseTypeDef",
     {
-        "Role": RoleOutputTypeDef,
+        "Role": RoleTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-InstanceProfileOutputTypeDef = TypedDict(
-    "InstanceProfileOutputTypeDef",
+InstanceProfileTypeDef = TypedDict(
+    "InstanceProfileTypeDef",
     {
         "Path": str,
         "InstanceProfileName": str,
         "InstanceProfileId": str,
         "Arn": str,
         "CreateDate": datetime,
-        "Roles": List[RoleOutputTypeDef],
+        "Roles": List[RoleTypeDef],
         "Tags": List[TagOutputTypeDef],
     },
 )
 
-ListRolesResponseOutputTypeDef = TypedDict(
-    "ListRolesResponseOutputTypeDef",
+ListRolesResponseTypeDef = TypedDict(
+    "ListRolesResponseTypeDef",
     {
-        "Roles": List[RoleOutputTypeDef],
+        "Roles": List[RoleTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-UpdateRoleDescriptionResponseOutputTypeDef = TypedDict(
-    "UpdateRoleDescriptionResponseOutputTypeDef",
+UpdateRoleDescriptionResponseTypeDef = TypedDict(
+    "UpdateRoleDescriptionResponseTypeDef",
     {
-        "Role": RoleOutputTypeDef,
+        "Role": RoleTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetServiceLastAccessedDetailsResponseOutputTypeDef = TypedDict(
-    "GetServiceLastAccessedDetailsResponseOutputTypeDef",
+GetServiceLastAccessedDetailsResponseTypeDef = TypedDict(
+    "GetServiceLastAccessedDetailsResponseTypeDef",
     {
         "JobStatus": jobStatusTypeType,
         "JobType": AccessAdvisorUsageGranularityTypeType,
         "JobCreationDate": datetime,
-        "ServicesLastAccessed": List[ServiceLastAccessedOutputTypeDef],
+        "ServicesLastAccessed": List[ServiceLastAccessedTypeDef],
         "JobCompletionDate": datetime,
         "IsTruncated": bool,
         "Marker": str,
-        "Error": ErrorDetailsOutputTypeDef,
+        "Error": ErrorDetailsTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-CreateVirtualMFADeviceResponseOutputTypeDef = TypedDict(
-    "CreateVirtualMFADeviceResponseOutputTypeDef",
+CreateVirtualMFADeviceResponseTypeDef = TypedDict(
+    "CreateVirtualMFADeviceResponseTypeDef",
     {
-        "VirtualMFADevice": VirtualMFADeviceOutputTypeDef,
+        "VirtualMFADevice": VirtualMFADeviceTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListVirtualMFADevicesResponseOutputTypeDef = TypedDict(
-    "ListVirtualMFADevicesResponseOutputTypeDef",
+ListVirtualMFADevicesResponseTypeDef = TypedDict(
+    "ListVirtualMFADevicesResponseTypeDef",
     {
-        "VirtualMFADevices": List[VirtualMFADeviceOutputTypeDef],
+        "VirtualMFADevices": List[VirtualMFADeviceTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-EvaluationResultOutputTypeDef = TypedDict(
-    "EvaluationResultOutputTypeDef",
+EvaluationResultTypeDef = TypedDict(
+    "EvaluationResultTypeDef",
     {
         "EvalActionName": str,
         "EvalResourceName": str,
         "EvalDecision": PolicyEvaluationDecisionTypeType,
-        "MatchedStatements": List[StatementOutputTypeDef],
+        "MatchedStatements": List[StatementTypeDef],
         "MissingContextValues": List[str],
-        "OrganizationsDecisionDetail": OrganizationsDecisionDetailOutputTypeDef,
-        "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailOutputTypeDef,
+        "OrganizationsDecisionDetail": OrganizationsDecisionDetailTypeDef,
+        "PermissionsBoundaryDecisionDetail": PermissionsBoundaryDecisionDetailTypeDef,
         "EvalDecisionDetails": Dict[str, PolicyEvaluationDecisionTypeType],
-        "ResourceSpecificResults": List[ResourceSpecificResultOutputTypeDef],
+        "ResourceSpecificResults": List[ResourceSpecificResultTypeDef],
     },
 )
 
-CreateInstanceProfileResponseOutputTypeDef = TypedDict(
-    "CreateInstanceProfileResponseOutputTypeDef",
+CreateInstanceProfileResponseTypeDef = TypedDict(
+    "CreateInstanceProfileResponseTypeDef",
     {
-        "InstanceProfile": InstanceProfileOutputTypeDef,
+        "InstanceProfile": InstanceProfileTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetInstanceProfileResponseOutputTypeDef = TypedDict(
-    "GetInstanceProfileResponseOutputTypeDef",
+GetInstanceProfileResponseTypeDef = TypedDict(
+    "GetInstanceProfileResponseTypeDef",
     {
-        "InstanceProfile": InstanceProfileOutputTypeDef,
+        "InstanceProfile": InstanceProfileTypeDef,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListInstanceProfilesForRoleResponseOutputTypeDef = TypedDict(
-    "ListInstanceProfilesForRoleResponseOutputTypeDef",
+ListInstanceProfilesForRoleResponseTypeDef = TypedDict(
+    "ListInstanceProfilesForRoleResponseTypeDef",
     {
-        "InstanceProfiles": List[InstanceProfileOutputTypeDef],
+        "InstanceProfiles": List[InstanceProfileTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListInstanceProfilesResponseOutputTypeDef = TypedDict(
-    "ListInstanceProfilesResponseOutputTypeDef",
+ListInstanceProfilesResponseTypeDef = TypedDict(
+    "ListInstanceProfilesResponseTypeDef",
     {
-        "InstanceProfiles": List[InstanceProfileOutputTypeDef],
+        "InstanceProfiles": List[InstanceProfileTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RoleDetailOutputTypeDef = TypedDict(
-    "RoleDetailOutputTypeDef",
+RoleDetailTypeDef = TypedDict(
+    "RoleDetailTypeDef",
     {
         "Path": str,
         "RoleName": str,
         "RoleId": str,
         "Arn": str,
         "CreateDate": datetime,
         "AssumeRolePolicyDocument": str,
-        "InstanceProfileList": List[InstanceProfileOutputTypeDef],
-        "RolePolicyList": List[PolicyDetailOutputTypeDef],
-        "AttachedManagedPolicies": List[AttachedPolicyOutputTypeDef],
-        "PermissionsBoundary": AttachedPermissionsBoundaryOutputTypeDef,
+        "InstanceProfileList": List[InstanceProfileTypeDef],
+        "RolePolicyList": List[PolicyDetailTypeDef],
+        "AttachedManagedPolicies": List[AttachedPolicyTypeDef],
+        "PermissionsBoundary": AttachedPermissionsBoundaryTypeDef,
         "Tags": List[TagOutputTypeDef],
-        "RoleLastUsed": RoleLastUsedOutputTypeDef,
+        "RoleLastUsed": RoleLastUsedTypeDef,
     },
 )
 
-SimulatePolicyResponseOutputTypeDef = TypedDict(
-    "SimulatePolicyResponseOutputTypeDef",
+SimulatePolicyResponseTypeDef = TypedDict(
+    "SimulatePolicyResponseTypeDef",
     {
-        "EvaluationResults": List[EvaluationResultOutputTypeDef],
+        "EvaluationResults": List[EvaluationResultTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-GetAccountAuthorizationDetailsResponseOutputTypeDef = TypedDict(
-    "GetAccountAuthorizationDetailsResponseOutputTypeDef",
+GetAccountAuthorizationDetailsResponseTypeDef = TypedDict(
+    "GetAccountAuthorizationDetailsResponseTypeDef",
     {
-        "UserDetailList": List[UserDetailOutputTypeDef],
-        "GroupDetailList": List[GroupDetailOutputTypeDef],
-        "RoleDetailList": List[RoleDetailOutputTypeDef],
-        "Policies": List[ManagedPolicyDetailOutputTypeDef],
+        "UserDetailList": List[UserDetailTypeDef],
+        "GroupDetailList": List[GroupDetailTypeDef],
+        "RoleDetailList": List[RoleDetailTypeDef],
+        "Policies": List[ManagedPolicyDetailTypeDef],
         "IsTruncated": bool,
         "Marker": str,
         "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/waiter.py` & `mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam/waiter.pyi` & `mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/PKG-INFO` & `mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iam
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.IAM 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.IAM 1.28.3 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.7](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iam docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iam/).
 
 See how it helps to find and fix potential bugs:
 
@@ -639,18 +639,18 @@
 ### Typed dictionaries
 
 `mypy_boto3_iam.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iam.type_defs import (
-    AccessDetailOutputTypeDef,
-    AccessKeyLastUsedOutputTypeDef,
-    AccessKeyMetadataOutputTypeDef,
-    AccessKeyOutputTypeDef,
+    AccessDetailTypeDef,
+    AccessKeyLastUsedTypeDef,
+    AccessKeyMetadataTypeDef,
+    AccessKeyTypeDef,
     AddClientIDToOpenIDConnectProviderRequestRequestTypeDef,
     AddRoleToInstanceProfileRequestInstanceProfileAddRoleTypeDef,
     AddRoleToInstanceProfileRequestRequestTypeDef,
     AddUserToGroupRequestGroupAddUserTypeDef,
     AddUserToGroupRequestRequestTypeDef,
     AddUserToGroupRequestUserAddGroupTypeDef,
     AttachGroupPolicyRequestGroupAttachPolicyTypeDef,
@@ -658,39 +658,39 @@
     AttachGroupPolicyRequestRequestTypeDef,
     AttachRolePolicyRequestPolicyAttachRoleTypeDef,
     AttachRolePolicyRequestRequestTypeDef,
     AttachRolePolicyRequestRoleAttachPolicyTypeDef,
     AttachUserPolicyRequestPolicyAttachUserTypeDef,
     AttachUserPolicyRequestRequestTypeDef,
     AttachUserPolicyRequestUserAttachPolicyTypeDef,
-    AttachedPermissionsBoundaryOutputTypeDef,
     AttachedPermissionsBoundaryResponseMetadataTypeDef,
-    AttachedPolicyOutputTypeDef,
+    AttachedPermissionsBoundaryTypeDef,
+    AttachedPolicyTypeDef,
     ChangePasswordRequestRequestTypeDef,
     ChangePasswordRequestServiceResourceChangePasswordTypeDef,
     ContextEntryTypeDef,
     CreateAccessKeyRequestRequestTypeDef,
     CreateAccountAliasRequestRequestTypeDef,
     CreateAccountAliasRequestServiceResourceCreateAccountAliasTypeDef,
     CreateGroupRequestGroupCreateTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateGroupRequestServiceResourceCreateGroupTypeDef,
-    GroupOutputTypeDef,
+    GroupTypeDef,
     TagTypeDef,
     CreateLoginProfileRequestLoginProfileCreateTypeDef,
     CreateLoginProfileRequestRequestTypeDef,
     CreateLoginProfileRequestUserCreateLoginProfileTypeDef,
-    LoginProfileOutputTypeDef,
+    LoginProfileTypeDef,
     TagOutputTypeDef,
     CreatePolicyVersionRequestPolicyCreateVersionTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
-    PolicyVersionOutputTypeDef,
+    PolicyVersionTypeDef,
     CreateServiceLinkedRoleRequestRequestTypeDef,
     CreateServiceSpecificCredentialRequestRequestTypeDef,
-    ServiceSpecificCredentialOutputTypeDef,
+    ServiceSpecificCredentialTypeDef,
     DeactivateMFADeviceRequestRequestTypeDef,
     DeleteAccessKeyRequestRequestTypeDef,
     DeleteAccountAliasRequestRequestTypeDef,
     DeleteGroupPolicyRequestRequestTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteInstanceProfileRequestRequestTypeDef,
     DeleteLoginProfileRequestRequestTypeDef,
@@ -700,159 +700,159 @@
     DeleteRolePermissionsBoundaryRequestRequestTypeDef,
     DeleteRolePolicyRequestRequestTypeDef,
     DeleteRoleRequestRequestTypeDef,
     DeleteSAMLProviderRequestRequestTypeDef,
     DeleteSSHPublicKeyRequestRequestTypeDef,
     DeleteServerCertificateRequestRequestTypeDef,
     DeleteServiceLinkedRoleRequestRequestTypeDef,
-    DeleteServiceLinkedRoleResponseOutputTypeDef,
+    DeleteServiceLinkedRoleResponseTypeDef,
     DeleteServiceSpecificCredentialRequestRequestTypeDef,
     DeleteSigningCertificateRequestRequestTypeDef,
     DeleteUserPermissionsBoundaryRequestRequestTypeDef,
     DeleteUserPolicyRequestRequestTypeDef,
     DeleteUserRequestRequestTypeDef,
     DeleteVirtualMFADeviceRequestRequestTypeDef,
-    RoleUsageTypeOutputTypeDef,
+    RoleUsageTypeTypeDef,
     DetachGroupPolicyRequestGroupDetachPolicyTypeDef,
     DetachGroupPolicyRequestPolicyDetachGroupTypeDef,
     DetachGroupPolicyRequestRequestTypeDef,
     DetachRolePolicyRequestPolicyDetachRoleTypeDef,
     DetachRolePolicyRequestRequestTypeDef,
     DetachRolePolicyRequestRoleDetachPolicyTypeDef,
     DetachUserPolicyRequestPolicyDetachUserTypeDef,
     DetachUserPolicyRequestRequestTypeDef,
     DetachUserPolicyRequestUserDetachPolicyTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableMFADeviceRequestMfaDeviceAssociateTypeDef,
     EnableMFADeviceRequestRequestTypeDef,
     EnableMFADeviceRequestUserEnableMfaTypeDef,
-    EntityInfoOutputTypeDef,
-    ErrorDetailsOutputTypeDef,
-    OrganizationsDecisionDetailOutputTypeDef,
-    PermissionsBoundaryDecisionDetailOutputTypeDef,
-    GenerateCredentialReportResponseOutputTypeDef,
+    EntityInfoTypeDef,
+    ErrorDetailsTypeDef,
+    OrganizationsDecisionDetailTypeDef,
+    PermissionsBoundaryDecisionDetailTypeDef,
+    GenerateCredentialReportResponseTypeDef,
     GenerateOrganizationsAccessReportRequestRequestTypeDef,
-    GenerateOrganizationsAccessReportResponseOutputTypeDef,
+    GenerateOrganizationsAccessReportResponseTypeDef,
     GenerateServiceLastAccessedDetailsRequestRequestTypeDef,
-    GenerateServiceLastAccessedDetailsResponseOutputTypeDef,
+    GenerateServiceLastAccessedDetailsResponseTypeDef,
     GetAccessKeyLastUsedRequestRequestTypeDef,
     GetAccountAuthorizationDetailsRequestGetAccountAuthorizationDetailsPaginateTypeDef,
     GetAccountAuthorizationDetailsRequestRequestTypeDef,
-    PasswordPolicyOutputTypeDef,
-    GetAccountSummaryResponseOutputTypeDef,
+    PasswordPolicyTypeDef,
+    GetAccountSummaryResponseTypeDef,
     GetContextKeysForCustomPolicyRequestRequestTypeDef,
-    GetContextKeysForPolicyResponseOutputTypeDef,
+    GetContextKeysForPolicyResponseTypeDef,
     GetContextKeysForPrincipalPolicyRequestRequestTypeDef,
-    GetCredentialReportResponseOutputTypeDef,
+    GetCredentialReportResponseTypeDef,
     GetGroupPolicyRequestRequestTypeDef,
-    GetGroupPolicyResponseOutputTypeDef,
+    GetGroupPolicyResponseTypeDef,
     GetGroupRequestGetGroupPaginateTypeDef,
     GetGroupRequestRequestTypeDef,
     WaiterConfigTypeDef,
     GetInstanceProfileRequestRequestTypeDef,
     GetLoginProfileRequestRequestTypeDef,
     GetMFADeviceRequestRequestTypeDef,
-    GetMFADeviceResponseOutputTypeDef,
+    GetMFADeviceResponseTypeDef,
     GetOpenIDConnectProviderRequestRequestTypeDef,
     GetOrganizationsAccessReportRequestRequestTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetPolicyVersionRequestRequestTypeDef,
     GetRolePolicyRequestRequestTypeDef,
-    GetRolePolicyResponseOutputTypeDef,
+    GetRolePolicyResponseTypeDef,
     GetRoleRequestRequestTypeDef,
     GetSAMLProviderRequestRequestTypeDef,
     GetSSHPublicKeyRequestRequestTypeDef,
-    SSHPublicKeyOutputTypeDef,
+    SSHPublicKeyTypeDef,
     GetServerCertificateRequestRequestTypeDef,
     GetServiceLastAccessedDetailsRequestRequestTypeDef,
     GetServiceLastAccessedDetailsWithEntitiesRequestRequestTypeDef,
     GetServiceLinkedRoleDeletionStatusRequestRequestTypeDef,
     GetUserPolicyRequestRequestTypeDef,
-    GetUserPolicyResponseOutputTypeDef,
+    GetUserPolicyResponseTypeDef,
     GetUserRequestRequestTypeDef,
-    PolicyDetailOutputTypeDef,
+    PolicyDetailTypeDef,
     ListAccessKeysRequestListAccessKeysPaginateTypeDef,
     ListAccessKeysRequestRequestTypeDef,
     ListAccountAliasesRequestListAccountAliasesPaginateTypeDef,
     ListAccountAliasesRequestRequestTypeDef,
-    ListAccountAliasesResponseOutputTypeDef,
+    ListAccountAliasesResponseTypeDef,
     ListAttachedGroupPoliciesRequestListAttachedGroupPoliciesPaginateTypeDef,
     ListAttachedGroupPoliciesRequestRequestTypeDef,
     ListAttachedRolePoliciesRequestListAttachedRolePoliciesPaginateTypeDef,
     ListAttachedRolePoliciesRequestRequestTypeDef,
     ListAttachedUserPoliciesRequestListAttachedUserPoliciesPaginateTypeDef,
     ListAttachedUserPoliciesRequestRequestTypeDef,
     ListEntitiesForPolicyRequestListEntitiesForPolicyPaginateTypeDef,
     ListEntitiesForPolicyRequestRequestTypeDef,
-    PolicyGroupOutputTypeDef,
-    PolicyRoleOutputTypeDef,
-    PolicyUserOutputTypeDef,
+    PolicyGroupTypeDef,
+    PolicyRoleTypeDef,
+    PolicyUserTypeDef,
     ListGroupPoliciesRequestListGroupPoliciesPaginateTypeDef,
     ListGroupPoliciesRequestRequestTypeDef,
-    ListGroupPoliciesResponseOutputTypeDef,
+    ListGroupPoliciesResponseTypeDef,
     ListGroupsForUserRequestListGroupsForUserPaginateTypeDef,
     ListGroupsForUserRequestRequestTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListInstanceProfileTagsRequestListInstanceProfileTagsPaginateTypeDef,
     ListInstanceProfileTagsRequestRequestTypeDef,
     ListInstanceProfilesForRoleRequestListInstanceProfilesForRolePaginateTypeDef,
     ListInstanceProfilesForRoleRequestRequestTypeDef,
     ListInstanceProfilesRequestListInstanceProfilesPaginateTypeDef,
     ListInstanceProfilesRequestRequestTypeDef,
     ListMFADeviceTagsRequestListMFADeviceTagsPaginateTypeDef,
     ListMFADeviceTagsRequestRequestTypeDef,
     ListMFADevicesRequestListMFADevicesPaginateTypeDef,
     ListMFADevicesRequestRequestTypeDef,
-    MFADeviceOutputTypeDef,
+    MFADeviceTypeDef,
     ListOpenIDConnectProviderTagsRequestListOpenIDConnectProviderTagsPaginateTypeDef,
     ListOpenIDConnectProviderTagsRequestRequestTypeDef,
-    OpenIDConnectProviderListEntryOutputTypeDef,
-    PolicyGrantingServiceAccessOutputTypeDef,
+    OpenIDConnectProviderListEntryTypeDef,
+    PolicyGrantingServiceAccessTypeDef,
     ListPoliciesGrantingServiceAccessRequestRequestTypeDef,
     ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
     ListPolicyTagsRequestListPolicyTagsPaginateTypeDef,
     ListPolicyTagsRequestRequestTypeDef,
     ListPolicyVersionsRequestListPolicyVersionsPaginateTypeDef,
     ListPolicyVersionsRequestRequestTypeDef,
     ListRolePoliciesRequestListRolePoliciesPaginateTypeDef,
     ListRolePoliciesRequestRequestTypeDef,
-    ListRolePoliciesResponseOutputTypeDef,
+    ListRolePoliciesResponseTypeDef,
     ListRoleTagsRequestListRoleTagsPaginateTypeDef,
     ListRoleTagsRequestRequestTypeDef,
     ListRolesRequestListRolesPaginateTypeDef,
     ListRolesRequestRequestTypeDef,
     ListSAMLProviderTagsRequestListSAMLProviderTagsPaginateTypeDef,
     ListSAMLProviderTagsRequestRequestTypeDef,
-    SAMLProviderListEntryOutputTypeDef,
+    SAMLProviderListEntryTypeDef,
     ListSSHPublicKeysRequestListSSHPublicKeysPaginateTypeDef,
     ListSSHPublicKeysRequestRequestTypeDef,
-    SSHPublicKeyMetadataOutputTypeDef,
+    SSHPublicKeyMetadataTypeDef,
     ListServerCertificateTagsRequestListServerCertificateTagsPaginateTypeDef,
     ListServerCertificateTagsRequestRequestTypeDef,
     ListServerCertificatesRequestListServerCertificatesPaginateTypeDef,
     ListServerCertificatesRequestRequestTypeDef,
-    ServerCertificateMetadataOutputTypeDef,
+    ServerCertificateMetadataTypeDef,
     ListServiceSpecificCredentialsRequestRequestTypeDef,
-    ServiceSpecificCredentialMetadataOutputTypeDef,
+    ServiceSpecificCredentialMetadataTypeDef,
     ListSigningCertificatesRequestListSigningCertificatesPaginateTypeDef,
     ListSigningCertificatesRequestRequestTypeDef,
-    SigningCertificateOutputTypeDef,
+    SigningCertificateTypeDef,
     ListUserPoliciesRequestListUserPoliciesPaginateTypeDef,
     ListUserPoliciesRequestRequestTypeDef,
-    ListUserPoliciesResponseOutputTypeDef,
+    ListUserPoliciesResponseTypeDef,
     ListUserTagsRequestListUserTagsPaginateTypeDef,
     ListUserTagsRequestRequestTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     ListVirtualMFADevicesRequestListVirtualMFADevicesPaginateTypeDef,
     ListVirtualMFADevicesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    PositionOutputTypeDef,
+    PositionTypeDef,
     PutGroupPolicyRequestGroupCreatePolicyTypeDef,
     PutGroupPolicyRequestGroupPolicyPutTypeDef,
     PutGroupPolicyRequestRequestTypeDef,
     PutRolePermissionsBoundaryRequestRequestTypeDef,
     PutRolePolicyRequestRequestTypeDef,
     PutRolePolicyRequestRolePolicyPutTypeDef,
     PutUserPermissionsBoundaryRequestRequestTypeDef,
@@ -865,18 +865,18 @@
     RemoveUserFromGroupRequestGroupRemoveUserTypeDef,
     RemoveUserFromGroupRequestRequestTypeDef,
     RemoveUserFromGroupRequestUserRemoveGroupTypeDef,
     ResetServiceSpecificCredentialRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ResyncMFADeviceRequestMfaDeviceResyncTypeDef,
     ResyncMFADeviceRequestRequestTypeDef,
-    RoleLastUsedOutputTypeDef,
+    RoleLastUsedTypeDef,
     RoleLastUsedResponseMetadataTypeDef,
     ServerCertificateMetadataResponseMetadataTypeDef,
-    TrackedActionLastAccessedOutputTypeDef,
+    TrackedActionLastAccessedTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetSecurityTokenServicePreferencesRequestRequestTypeDef,
     UntagInstanceProfileRequestRequestTypeDef,
     UntagMFADeviceRequestRequestTypeDef,
     UntagOpenIDConnectProviderRequestRequestTypeDef,
     UntagPolicyRequestRequestTypeDef,
     UntagRoleRequestRequestTypeDef,
@@ -898,40 +898,40 @@
     UpdateLoginProfileRequestLoginProfileUpdateTypeDef,
     UpdateLoginProfileRequestRequestTypeDef,
     UpdateOpenIDConnectProviderThumbprintRequestRequestTypeDef,
     UpdateRoleDescriptionRequestRequestTypeDef,
     UpdateRoleRequestRequestTypeDef,
     UpdateSAMLProviderRequestRequestTypeDef,
     UpdateSAMLProviderRequestSamlProviderUpdateTypeDef,
-    UpdateSAMLProviderResponseOutputTypeDef,
+    UpdateSAMLProviderResponseTypeDef,
     UpdateSSHPublicKeyRequestRequestTypeDef,
     UpdateServerCertificateRequestRequestTypeDef,
     UpdateServerCertificateRequestServerCertificateUpdateTypeDef,
     UpdateServiceSpecificCredentialRequestRequestTypeDef,
     UpdateSigningCertificateRequestRequestTypeDef,
     UpdateSigningCertificateRequestSigningCertificateActivateTypeDef,
     UpdateSigningCertificateRequestSigningCertificateDeactivateTypeDef,
     UpdateUserRequestRequestTypeDef,
     UpdateUserRequestUserUpdateTypeDef,
     UploadSSHPublicKeyRequestRequestTypeDef,
     UploadSigningCertificateRequestRequestTypeDef,
     UploadSigningCertificateRequestServiceResourceCreateSigningCertificateTypeDef,
-    GetAccessKeyLastUsedResponseOutputTypeDef,
-    ListAccessKeysResponseOutputTypeDef,
-    CreateAccessKeyResponseOutputTypeDef,
-    ListAttachedGroupPoliciesResponseOutputTypeDef,
-    ListAttachedRolePoliciesResponseOutputTypeDef,
-    ListAttachedUserPoliciesResponseOutputTypeDef,
+    GetAccessKeyLastUsedResponseTypeDef,
+    ListAccessKeysResponseTypeDef,
+    CreateAccessKeyResponseTypeDef,
+    ListAttachedGroupPoliciesResponseTypeDef,
+    ListAttachedRolePoliciesResponseTypeDef,
+    ListAttachedUserPoliciesResponseTypeDef,
     SimulateCustomPolicyRequestRequestTypeDef,
     SimulateCustomPolicyRequestSimulateCustomPolicyPaginateTypeDef,
     SimulatePrincipalPolicyRequestRequestTypeDef,
     SimulatePrincipalPolicyRequestSimulatePrincipalPolicyPaginateTypeDef,
-    CreateGroupResponseOutputTypeDef,
-    ListGroupsForUserResponseOutputTypeDef,
-    ListGroupsResponseOutputTypeDef,
+    CreateGroupResponseTypeDef,
+    ListGroupsForUserResponseTypeDef,
+    ListGroupsResponseTypeDef,
     CreateInstanceProfileRequestRequestTypeDef,
     CreateInstanceProfileRequestServiceResourceCreateInstanceProfileTypeDef,
     CreateOpenIDConnectProviderRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreatePolicyRequestServiceResourceCreatePolicyTypeDef,
     CreateRoleRequestRequestTypeDef,
     CreateRoleRequestServiceResourceCreateRoleTypeDef,
@@ -948,98 +948,98 @@
     TagPolicyRequestRequestTypeDef,
     TagRoleRequestRequestTypeDef,
     TagSAMLProviderRequestRequestTypeDef,
     TagServerCertificateRequestRequestTypeDef,
     TagUserRequestRequestTypeDef,
     UploadServerCertificateRequestRequestTypeDef,
     UploadServerCertificateRequestServiceResourceCreateServerCertificateTypeDef,
-    CreateLoginProfileResponseOutputTypeDef,
-    GetLoginProfileResponseOutputTypeDef,
-    CreateOpenIDConnectProviderResponseOutputTypeDef,
-    CreateSAMLProviderResponseOutputTypeDef,
-    GetOpenIDConnectProviderResponseOutputTypeDef,
-    GetSAMLProviderResponseOutputTypeDef,
-    ListInstanceProfileTagsResponseOutputTypeDef,
-    ListMFADeviceTagsResponseOutputTypeDef,
-    ListOpenIDConnectProviderTagsResponseOutputTypeDef,
-    ListPolicyTagsResponseOutputTypeDef,
-    ListRoleTagsResponseOutputTypeDef,
-    ListSAMLProviderTagsResponseOutputTypeDef,
-    ListServerCertificateTagsResponseOutputTypeDef,
-    ListUserTagsResponseOutputTypeDef,
-    PolicyOutputTypeDef,
-    UserOutputTypeDef,
+    CreateLoginProfileResponseTypeDef,
+    GetLoginProfileResponseTypeDef,
+    CreateOpenIDConnectProviderResponseTypeDef,
+    CreateSAMLProviderResponseTypeDef,
+    GetOpenIDConnectProviderResponseTypeDef,
+    GetSAMLProviderResponseTypeDef,
+    ListInstanceProfileTagsResponseTypeDef,
+    ListMFADeviceTagsResponseTypeDef,
+    ListOpenIDConnectProviderTagsResponseTypeDef,
+    ListPolicyTagsResponseTypeDef,
+    ListRoleTagsResponseTypeDef,
+    ListSAMLProviderTagsResponseTypeDef,
+    ListServerCertificateTagsResponseTypeDef,
+    ListUserTagsResponseTypeDef,
+    PolicyTypeDef,
     UserResponseMetadataTypeDef,
-    CreatePolicyVersionResponseOutputTypeDef,
-    GetPolicyVersionResponseOutputTypeDef,
-    ListPolicyVersionsResponseOutputTypeDef,
-    ManagedPolicyDetailOutputTypeDef,
-    CreateServiceSpecificCredentialResponseOutputTypeDef,
-    ResetServiceSpecificCredentialResponseOutputTypeDef,
-    DeletionTaskFailureReasonTypeOutputTypeDef,
-    EntityDetailsOutputTypeDef,
-    GetOrganizationsAccessReportResponseOutputTypeDef,
-    GetAccountPasswordPolicyResponseOutputTypeDef,
+    UserTypeDef,
+    CreatePolicyVersionResponseTypeDef,
+    GetPolicyVersionResponseTypeDef,
+    ListPolicyVersionsResponseTypeDef,
+    ManagedPolicyDetailTypeDef,
+    CreateServiceSpecificCredentialResponseTypeDef,
+    ResetServiceSpecificCredentialResponseTypeDef,
+    DeletionTaskFailureReasonTypeTypeDef,
+    EntityDetailsTypeDef,
+    GetOrganizationsAccessReportResponseTypeDef,
+    GetAccountPasswordPolicyResponseTypeDef,
     GetInstanceProfileRequestInstanceProfileExistsWaitTypeDef,
     GetPolicyRequestPolicyExistsWaitTypeDef,
     GetRoleRequestRoleExistsWaitTypeDef,
     GetUserRequestUserExistsWaitTypeDef,
-    GetSSHPublicKeyResponseOutputTypeDef,
-    UploadSSHPublicKeyResponseOutputTypeDef,
-    GroupDetailOutputTypeDef,
-    UserDetailOutputTypeDef,
-    ListEntitiesForPolicyResponseOutputTypeDef,
-    ListMFADevicesResponseOutputTypeDef,
-    ListOpenIDConnectProvidersResponseOutputTypeDef,
-    ListPoliciesGrantingServiceAccessEntryOutputTypeDef,
-    ListSAMLProvidersResponseOutputTypeDef,
-    ListSSHPublicKeysResponseOutputTypeDef,
-    ListServerCertificatesResponseOutputTypeDef,
-    ServerCertificateOutputTypeDef,
-    UploadServerCertificateResponseOutputTypeDef,
-    ListServiceSpecificCredentialsResponseOutputTypeDef,
-    ListSigningCertificatesResponseOutputTypeDef,
-    UploadSigningCertificateResponseOutputTypeDef,
-    StatementOutputTypeDef,
-    RoleOutputTypeDef,
-    ServiceLastAccessedOutputTypeDef,
-    CreatePolicyResponseOutputTypeDef,
-    GetPolicyResponseOutputTypeDef,
-    ListPoliciesResponseOutputTypeDef,
-    CreateUserResponseOutputTypeDef,
-    GetGroupResponseOutputTypeDef,
-    GetUserResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
-    VirtualMFADeviceOutputTypeDef,
-    GetServiceLinkedRoleDeletionStatusResponseOutputTypeDef,
-    GetServiceLastAccessedDetailsWithEntitiesResponseOutputTypeDef,
-    ListPoliciesGrantingServiceAccessResponseOutputTypeDef,
-    GetServerCertificateResponseOutputTypeDef,
-    ResourceSpecificResultOutputTypeDef,
-    CreateRoleResponseOutputTypeDef,
-    CreateServiceLinkedRoleResponseOutputTypeDef,
-    GetRoleResponseOutputTypeDef,
-    InstanceProfileOutputTypeDef,
-    ListRolesResponseOutputTypeDef,
-    UpdateRoleDescriptionResponseOutputTypeDef,
-    GetServiceLastAccessedDetailsResponseOutputTypeDef,
-    CreateVirtualMFADeviceResponseOutputTypeDef,
-    ListVirtualMFADevicesResponseOutputTypeDef,
-    EvaluationResultOutputTypeDef,
-    CreateInstanceProfileResponseOutputTypeDef,
-    GetInstanceProfileResponseOutputTypeDef,
-    ListInstanceProfilesForRoleResponseOutputTypeDef,
-    ListInstanceProfilesResponseOutputTypeDef,
-    RoleDetailOutputTypeDef,
-    SimulatePolicyResponseOutputTypeDef,
-    GetAccountAuthorizationDetailsResponseOutputTypeDef,
+    GetSSHPublicKeyResponseTypeDef,
+    UploadSSHPublicKeyResponseTypeDef,
+    GroupDetailTypeDef,
+    UserDetailTypeDef,
+    ListEntitiesForPolicyResponseTypeDef,
+    ListMFADevicesResponseTypeDef,
+    ListOpenIDConnectProvidersResponseTypeDef,
+    ListPoliciesGrantingServiceAccessEntryTypeDef,
+    ListSAMLProvidersResponseTypeDef,
+    ListSSHPublicKeysResponseTypeDef,
+    ListServerCertificatesResponseTypeDef,
+    ServerCertificateTypeDef,
+    UploadServerCertificateResponseTypeDef,
+    ListServiceSpecificCredentialsResponseTypeDef,
+    ListSigningCertificatesResponseTypeDef,
+    UploadSigningCertificateResponseTypeDef,
+    StatementTypeDef,
+    RoleTypeDef,
+    ServiceLastAccessedTypeDef,
+    CreatePolicyResponseTypeDef,
+    GetPolicyResponseTypeDef,
+    ListPoliciesResponseTypeDef,
+    CreateUserResponseTypeDef,
+    GetGroupResponseTypeDef,
+    GetUserResponseTypeDef,
+    ListUsersResponseTypeDef,
+    VirtualMFADeviceTypeDef,
+    GetServiceLinkedRoleDeletionStatusResponseTypeDef,
+    GetServiceLastAccessedDetailsWithEntitiesResponseTypeDef,
+    ListPoliciesGrantingServiceAccessResponseTypeDef,
+    GetServerCertificateResponseTypeDef,
+    ResourceSpecificResultTypeDef,
+    CreateRoleResponseTypeDef,
+    CreateServiceLinkedRoleResponseTypeDef,
+    GetRoleResponseTypeDef,
+    InstanceProfileTypeDef,
+    ListRolesResponseTypeDef,
+    UpdateRoleDescriptionResponseTypeDef,
+    GetServiceLastAccessedDetailsResponseTypeDef,
+    CreateVirtualMFADeviceResponseTypeDef,
+    ListVirtualMFADevicesResponseTypeDef,
+    EvaluationResultTypeDef,
+    CreateInstanceProfileResponseTypeDef,
+    GetInstanceProfileResponseTypeDef,
+    ListInstanceProfilesForRoleResponseTypeDef,
+    ListInstanceProfilesResponseTypeDef,
+    RoleDetailTypeDef,
+    SimulatePolicyResponseTypeDef,
+    GetAccountAuthorizationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> AccessDetailOutputTypeDef:
+def get_structure() -> AccessDetailTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iam-1.28.3.post1/mypy_boto3_iam.egg-info/SOURCES.txt` & `mypy-boto3-iam-1.28.3.post2/mypy_boto3_iam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iam-1.28.3.post1/setup.py` & `mypy-boto3-iam-1.28.3.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iam",
-    version="1.28.3.post1",
+    version="1.28.3.post2",
     packages=["mypy_boto3_iam"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IAM 1.28.3 service generated with mypy-boto3-builder 7.14.7"
+        "Type annotations for boto3.IAM 1.28.3 service generated with mypy-boto3-builder 7.15.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

