# Comparing `tmp/mypy-boto3-cognito-idp-1.28.3.post1.tar.gz` & `tmp/mypy-boto3-cognito-idp-1.28.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cognito-idp-1.28.3.post1.tar", last modified: Fri Jul 14 16:17:59 2023, max compression
+gzip compressed data, was "mypy-boto3-cognito-idp-1.28.3.post2.tar", last modified: Sat Jul 15 06:38:32 2023, max compression
```

## Comparing `mypy-boto3-cognito-idp-1.28.3.post1.tar` & `mypy-boto3-cognito-idp-1.28.3.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.903361 mypy-boto3-cognito-idp-1.28.3.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27194 2023-07-14 16:17:59.899361 mypy-boto3-cognito-idp-1.28.3.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25675 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.891360 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79559 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    79442 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-07-14 16:15:17.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-14 16:15:17.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   108255 2023-07-14 16:15:20.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   108118 2023-07-14 16:15:18.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 16:15:16.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:17:59.899361 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27194 2023-07-14 16:17:59.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-14 16:17:59.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:17:59.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 16:17:59.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 16:17:59.000000 mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:17:59.903361 mypy-boto3-cognito-idp-1.28.3.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-14 16:15:15.000000 mypy-boto3-cognito-idp-1.28.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.318243 mypy-boto3-cognito-idp-1.28.3.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 06:35:43.000000 mypy-boto3-cognito-idp-1.28.3.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26702 2023-07-15 06:38:32.318243 mypy-boto3-cognito-idp-1.28.3.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25183 2023-07-15 06:35:43.000000 mypy-boto3-cognito-idp-1.28.3.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.298242 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-15 06:35:43.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-15 06:35:43.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-15 06:35:43.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78755 2023-07-15 06:35:44.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78638 2023-07-15 06:35:43.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-07-15 06:35:45.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-15 06:35:44.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-07-15 06:35:44.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-07-15 06:35:44.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:35:43.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   106461 2023-07-15 06:35:48.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106324 2023-07-15 06:35:46.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-15 06:35:43.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:32.314243 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26702 2023-07-15 06:38:32.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-15 06:38:32.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:32.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:32.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-15 06:38:32.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 06:38:32.000000 mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:38:32.318243 mypy-boto3-cognito-idp-1.28.3.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-15 06:35:43.000000 mypy-boto3-cognito-idp-1.28.3.post2/setup.py
```

### Comparing `mypy-boto3-cognito-idp-1.28.3.post1/LICENSE` & `mypy-boto3-cognito-idp-1.28.3.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.3.post1/PKG-INFO` & `mypy-boto3-cognito-idp-1.28.3.post2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-idp
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.CognitoIdentityProvider 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.CognitoIdentityProvider 1.28.3 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/
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
 [mypy-boto3-cognito-idp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
 
@@ -418,46 +418,46 @@
     AdminGetUserRequestRequestTypeDef,
     AttributeTypeOutputTypeDef,
     MFAOptionTypeOutputTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AdminListDevicesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     AdminListGroupsForUserRequestRequestTypeDef,
-    GroupTypeOutputTypeDef,
+    GroupTypeTypeDef,
     AdminListUserAuthEventsRequestRequestTypeDef,
     AdminRemoveUserFromGroupRequestRequestTypeDef,
     AdminResetUserPasswordRequestRequestTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
     AdminSetUserPasswordRequestRequestTypeDef,
     MFAOptionTypeTypeDef,
     AdminUpdateAuthEventFeedbackRequestRequestTypeDef,
     AdminUpdateDeviceStatusRequestRequestTypeDef,
     AdminUserGlobalSignOutRequestRequestTypeDef,
     AnalyticsConfigurationTypeOutputTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AssociateSoftwareTokenRequestRequestTypeDef,
-    ChallengeResponseTypeOutputTypeDef,
-    EventContextDataTypeOutputTypeDef,
-    EventFeedbackTypeOutputTypeDef,
-    EventRiskTypeOutputTypeDef,
-    NewDeviceMetadataTypeOutputTypeDef,
+    ChallengeResponseTypeTypeDef,
+    EventContextDataTypeTypeDef,
+    EventFeedbackTypeTypeDef,
+    EventRiskTypeTypeDef,
+    NewDeviceMetadataTypeTypeDef,
     ChangePasswordRequestRequestTypeDef,
-    CodeDeliveryDetailsTypeOutputTypeDef,
+    CodeDeliveryDetailsTypeTypeDef,
     CompromisedCredentialsActionsTypeOutputTypeDef,
     CompromisedCredentialsActionsTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
     UserContextDataTypeTypeDef,
     HttpHeaderTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
-    IdentityProviderTypeOutputTypeDef,
+    IdentityProviderTypeTypeDef,
     ResourceServerScopeTypeTypeDef,
     CreateUserImportJobRequestRequestTypeDef,
-    UserImportJobTypeOutputTypeDef,
+    UserImportJobTypeTypeDef,
     TokenValidityUnitsTypeTypeDef,
     CustomDomainConfigTypeTypeDef,
     DeviceConfigurationTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     SmsConfigurationTypeTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
@@ -488,29 +488,29 @@
     ForgetDeviceRequestRequestTypeDef,
     GetCSVHeaderRequestRequestTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GetIdentityProviderByIdentifierRequestRequestTypeDef,
     GetSigningCertificateRequestRequestTypeDef,
     GetUICustomizationRequestRequestTypeDef,
-    UICustomizationTypeOutputTypeDef,
+    UICustomizationTypeTypeDef,
     GetUserAttributeVerificationCodeRequestRequestTypeDef,
     GetUserPoolMfaConfigRequestRequestTypeDef,
     SoftwareTokenMfaConfigTypeOutputTypeDef,
     GetUserRequestRequestTypeDef,
     GlobalSignOutRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
-    ProviderDescriptionOutputTypeDef,
+    ProviderDescriptionTypeDef,
     ListResourceServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListUserImportJobsRequestRequestTypeDef,
     ListUserPoolClientsRequestRequestTypeDef,
-    UserPoolClientDescriptionOutputTypeDef,
+    UserPoolClientDescriptionTypeDef,
     ListUserPoolsRequestRequestTypeDef,
     ListUsersInGroupRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
     NotifyEmailTypeOutputTypeDef,
     NotifyEmailTypeTypeDef,
     NumberAttributeConstraintsTypeOutputTypeDef,
     NumberAttributeConstraintsTypeTypeDef,
@@ -545,136 +545,136 @@
     AccountTakeoverActionsTypeOutputTypeDef,
     AccountTakeoverActionsTypeTypeDef,
     AdminCreateUserConfigTypeOutputTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserRequestRequestTypeDef,
     AdminUpdateUserAttributesRequestRequestTypeDef,
     UpdateUserAttributesRequestRequestTypeDef,
-    AssociateSoftwareTokenResponseOutputTypeDef,
-    ConfirmDeviceResponseOutputTypeDef,
-    CreateUserPoolDomainResponseOutputTypeDef,
+    AssociateSoftwareTokenResponseTypeDef,
+    ConfirmDeviceResponseTypeDef,
+    CreateUserPoolDomainResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetCSVHeaderResponseOutputTypeDef,
-    GetSigningCertificateResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    UpdateUserPoolDomainResponseOutputTypeDef,
-    VerifySoftwareTokenResponseOutputTypeDef,
+    GetCSVHeaderResponseTypeDef,
+    GetSigningCertificateResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateUserPoolDomainResponseTypeDef,
+    VerifySoftwareTokenResponseTypeDef,
     AdminDisableProviderForUserRequestRequestTypeDef,
     AdminLinkProviderForUserRequestRequestTypeDef,
-    DeviceTypeOutputTypeDef,
-    AdminGetUserResponseOutputTypeDef,
-    GetUserResponseOutputTypeDef,
-    UserTypeOutputTypeDef,
+    DeviceTypeTypeDef,
+    AdminGetUserResponseTypeDef,
+    GetUserResponseTypeDef,
+    UserTypeTypeDef,
     AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
     AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListResourceServersRequestListResourceServersPaginateTypeDef,
     ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
     ListUserPoolsRequestListUserPoolsPaginateTypeDef,
     ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
-    AdminListGroupsForUserResponseOutputTypeDef,
-    CreateGroupResponseOutputTypeDef,
-    GetGroupResponseOutputTypeDef,
-    ListGroupsResponseOutputTypeDef,
-    UpdateGroupResponseOutputTypeDef,
+    AdminListGroupsForUserResponseTypeDef,
+    CreateGroupResponseTypeDef,
+    GetGroupResponseTypeDef,
+    ListGroupsResponseTypeDef,
+    UpdateGroupResponseTypeDef,
     AdminSetUserMFAPreferenceRequestRequestTypeDef,
     SetUserMFAPreferenceRequestRequestTypeDef,
     AdminSetUserSettingsRequestRequestTypeDef,
     SetUserSettingsRequestRequestTypeDef,
-    AuthEventTypeOutputTypeDef,
-    AuthenticationResultTypeOutputTypeDef,
-    ForgotPasswordResponseOutputTypeDef,
-    GetUserAttributeVerificationCodeResponseOutputTypeDef,
-    ResendConfirmationCodeResponseOutputTypeDef,
-    SignUpResponseOutputTypeDef,
-    UpdateUserAttributesResponseOutputTypeDef,
+    AuthEventTypeTypeDef,
+    AuthenticationResultTypeTypeDef,
+    ForgotPasswordResponseTypeDef,
+    GetUserAttributeVerificationCodeResponseTypeDef,
+    ResendConfirmationCodeResponseTypeDef,
+    SignUpResponseTypeDef,
+    UpdateUserAttributesResponseTypeDef,
     CompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
     CompromisedCredentialsRiskConfigurationTypeTypeDef,
     ConfirmDeviceRequestRequestTypeDef,
     ConfirmForgotPasswordRequestRequestTypeDef,
     ConfirmSignUpRequestRequestTypeDef,
     ForgotPasswordRequestRequestTypeDef,
     InitiateAuthRequestRequestTypeDef,
     ResendConfirmationCodeRequestRequestTypeDef,
     RespondToAuthChallengeRequestRequestTypeDef,
     SignUpRequestRequestTypeDef,
     ContextDataTypeTypeDef,
-    CreateIdentityProviderResponseOutputTypeDef,
-    DescribeIdentityProviderResponseOutputTypeDef,
-    GetIdentityProviderByIdentifierResponseOutputTypeDef,
-    UpdateIdentityProviderResponseOutputTypeDef,
+    CreateIdentityProviderResponseTypeDef,
+    DescribeIdentityProviderResponseTypeDef,
+    GetIdentityProviderByIdentifierResponseTypeDef,
+    UpdateIdentityProviderResponseTypeDef,
     CreateResourceServerRequestRequestTypeDef,
     UpdateResourceServerRequestRequestTypeDef,
-    CreateUserImportJobResponseOutputTypeDef,
-    DescribeUserImportJobResponseOutputTypeDef,
-    ListUserImportJobsResponseOutputTypeDef,
-    StartUserImportJobResponseOutputTypeDef,
-    StopUserImportJobResponseOutputTypeDef,
+    CreateUserImportJobResponseTypeDef,
+    DescribeUserImportJobResponseTypeDef,
+    ListUserImportJobsResponseTypeDef,
+    StartUserImportJobResponseTypeDef,
+    StopUserImportJobResponseTypeDef,
     CreateUserPoolClientRequestRequestTypeDef,
     UpdateUserPoolClientRequestRequestTypeDef,
     CreateUserPoolDomainRequestRequestTypeDef,
     UpdateUserPoolDomainRequestRequestTypeDef,
     SmsMfaConfigTypeTypeDef,
-    DomainDescriptionTypeOutputTypeDef,
+    DomainDescriptionTypeTypeDef,
     LambdaConfigTypeOutputTypeDef,
     LambdaConfigTypeTypeDef,
-    GetUICustomizationResponseOutputTypeDef,
-    SetUICustomizationResponseOutputTypeDef,
-    ListIdentityProvidersResponseOutputTypeDef,
-    ListUserPoolClientsResponseOutputTypeDef,
+    GetUICustomizationResponseTypeDef,
+    SetUICustomizationResponseTypeDef,
+    ListIdentityProvidersResponseTypeDef,
+    ListUserPoolClientsResponseTypeDef,
     NotifyConfigurationTypeOutputTypeDef,
     NotifyConfigurationTypeTypeDef,
     UserPoolPolicyTypeOutputTypeDef,
     UserPoolPolicyTypeTypeDef,
-    ResourceServerTypeOutputTypeDef,
+    ResourceServerTypeTypeDef,
     SchemaAttributeTypeOutputTypeDef,
     SchemaAttributeTypeTypeDef,
     SmsMfaConfigTypeOutputTypeDef,
-    UserPoolClientTypeOutputTypeDef,
-    AdminGetDeviceResponseOutputTypeDef,
-    AdminListDevicesResponseOutputTypeDef,
-    GetDeviceResponseOutputTypeDef,
-    ListDevicesResponseOutputTypeDef,
-    AdminCreateUserResponseOutputTypeDef,
-    ListUsersInGroupResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
-    AdminListUserAuthEventsResponseOutputTypeDef,
-    AdminInitiateAuthResponseOutputTypeDef,
-    AdminRespondToAuthChallengeResponseOutputTypeDef,
-    InitiateAuthResponseOutputTypeDef,
-    RespondToAuthChallengeResponseOutputTypeDef,
+    UserPoolClientTypeTypeDef,
+    AdminGetDeviceResponseTypeDef,
+    AdminListDevicesResponseTypeDef,
+    GetDeviceResponseTypeDef,
+    ListDevicesResponseTypeDef,
+    AdminCreateUserResponseTypeDef,
+    ListUsersInGroupResponseTypeDef,
+    ListUsersResponseTypeDef,
+    AdminListUserAuthEventsResponseTypeDef,
+    AdminInitiateAuthResponseTypeDef,
+    AdminRespondToAuthChallengeResponseTypeDef,
+    InitiateAuthResponseTypeDef,
+    RespondToAuthChallengeResponseTypeDef,
     AdminInitiateAuthRequestRequestTypeDef,
     AdminRespondToAuthChallengeRequestRequestTypeDef,
     SetUserPoolMfaConfigRequestRequestTypeDef,
-    DescribeUserPoolDomainResponseOutputTypeDef,
-    UserPoolDescriptionTypeOutputTypeDef,
+    DescribeUserPoolDomainResponseTypeDef,
+    UserPoolDescriptionTypeTypeDef,
     AccountTakeoverRiskConfigurationTypeOutputTypeDef,
     AccountTakeoverRiskConfigurationTypeTypeDef,
     UpdateUserPoolRequestRequestTypeDef,
-    CreateResourceServerResponseOutputTypeDef,
-    DescribeResourceServerResponseOutputTypeDef,
-    ListResourceServersResponseOutputTypeDef,
-    UpdateResourceServerResponseOutputTypeDef,
-    UserPoolTypeOutputTypeDef,
+    CreateResourceServerResponseTypeDef,
+    DescribeResourceServerResponseTypeDef,
+    ListResourceServersResponseTypeDef,
+    UpdateResourceServerResponseTypeDef,
+    UserPoolTypeTypeDef,
     AddCustomAttributesRequestRequestTypeDef,
     CreateUserPoolRequestRequestTypeDef,
-    GetUserPoolMfaConfigResponseOutputTypeDef,
-    SetUserPoolMfaConfigResponseOutputTypeDef,
-    CreateUserPoolClientResponseOutputTypeDef,
-    DescribeUserPoolClientResponseOutputTypeDef,
-    UpdateUserPoolClientResponseOutputTypeDef,
-    ListUserPoolsResponseOutputTypeDef,
-    RiskConfigurationTypeOutputTypeDef,
+    GetUserPoolMfaConfigResponseTypeDef,
+    SetUserPoolMfaConfigResponseTypeDef,
+    CreateUserPoolClientResponseTypeDef,
+    DescribeUserPoolClientResponseTypeDef,
+    UpdateUserPoolClientResponseTypeDef,
+    ListUserPoolsResponseTypeDef,
+    RiskConfigurationTypeTypeDef,
     SetRiskConfigurationRequestRequestTypeDef,
-    CreateUserPoolResponseOutputTypeDef,
-    DescribeUserPoolResponseOutputTypeDef,
-    DescribeRiskConfigurationResponseOutputTypeDef,
-    SetRiskConfigurationResponseOutputTypeDef,
+    CreateUserPoolResponseTypeDef,
+    DescribeUserPoolResponseTypeDef,
+    DescribeRiskConfigurationResponseTypeDef,
+    SetRiskConfigurationResponseTypeDef,
 )
 
 
 def get_structure() -> RecoveryOptionTypeOutputTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-cognito-idp-1.28.3.post1/README.md` & `mypy-boto3-cognito-idp-1.28.3.post2/README.md`

 * *Files 11% similar despite different names*

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
 [mypy-boto3-cognito-idp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
 
@@ -386,46 +386,46 @@
     AdminGetUserRequestRequestTypeDef,
     AttributeTypeOutputTypeDef,
     MFAOptionTypeOutputTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AdminListDevicesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     AdminListGroupsForUserRequestRequestTypeDef,
-    GroupTypeOutputTypeDef,
+    GroupTypeTypeDef,
     AdminListUserAuthEventsRequestRequestTypeDef,
     AdminRemoveUserFromGroupRequestRequestTypeDef,
     AdminResetUserPasswordRequestRequestTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
     AdminSetUserPasswordRequestRequestTypeDef,
     MFAOptionTypeTypeDef,
     AdminUpdateAuthEventFeedbackRequestRequestTypeDef,
     AdminUpdateDeviceStatusRequestRequestTypeDef,
     AdminUserGlobalSignOutRequestRequestTypeDef,
     AnalyticsConfigurationTypeOutputTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AssociateSoftwareTokenRequestRequestTypeDef,
-    ChallengeResponseTypeOutputTypeDef,
-    EventContextDataTypeOutputTypeDef,
-    EventFeedbackTypeOutputTypeDef,
-    EventRiskTypeOutputTypeDef,
-    NewDeviceMetadataTypeOutputTypeDef,
+    ChallengeResponseTypeTypeDef,
+    EventContextDataTypeTypeDef,
+    EventFeedbackTypeTypeDef,
+    EventRiskTypeTypeDef,
+    NewDeviceMetadataTypeTypeDef,
     ChangePasswordRequestRequestTypeDef,
-    CodeDeliveryDetailsTypeOutputTypeDef,
+    CodeDeliveryDetailsTypeTypeDef,
     CompromisedCredentialsActionsTypeOutputTypeDef,
     CompromisedCredentialsActionsTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
     UserContextDataTypeTypeDef,
     HttpHeaderTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
-    IdentityProviderTypeOutputTypeDef,
+    IdentityProviderTypeTypeDef,
     ResourceServerScopeTypeTypeDef,
     CreateUserImportJobRequestRequestTypeDef,
-    UserImportJobTypeOutputTypeDef,
+    UserImportJobTypeTypeDef,
     TokenValidityUnitsTypeTypeDef,
     CustomDomainConfigTypeTypeDef,
     DeviceConfigurationTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     SmsConfigurationTypeTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
@@ -456,29 +456,29 @@
     ForgetDeviceRequestRequestTypeDef,
     GetCSVHeaderRequestRequestTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GetIdentityProviderByIdentifierRequestRequestTypeDef,
     GetSigningCertificateRequestRequestTypeDef,
     GetUICustomizationRequestRequestTypeDef,
-    UICustomizationTypeOutputTypeDef,
+    UICustomizationTypeTypeDef,
     GetUserAttributeVerificationCodeRequestRequestTypeDef,
     GetUserPoolMfaConfigRequestRequestTypeDef,
     SoftwareTokenMfaConfigTypeOutputTypeDef,
     GetUserRequestRequestTypeDef,
     GlobalSignOutRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
-    ProviderDescriptionOutputTypeDef,
+    ProviderDescriptionTypeDef,
     ListResourceServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListUserImportJobsRequestRequestTypeDef,
     ListUserPoolClientsRequestRequestTypeDef,
-    UserPoolClientDescriptionOutputTypeDef,
+    UserPoolClientDescriptionTypeDef,
     ListUserPoolsRequestRequestTypeDef,
     ListUsersInGroupRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
     NotifyEmailTypeOutputTypeDef,
     NotifyEmailTypeTypeDef,
     NumberAttributeConstraintsTypeOutputTypeDef,
     NumberAttributeConstraintsTypeTypeDef,
@@ -513,136 +513,136 @@
     AccountTakeoverActionsTypeOutputTypeDef,
     AccountTakeoverActionsTypeTypeDef,
     AdminCreateUserConfigTypeOutputTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserRequestRequestTypeDef,
     AdminUpdateUserAttributesRequestRequestTypeDef,
     UpdateUserAttributesRequestRequestTypeDef,
-    AssociateSoftwareTokenResponseOutputTypeDef,
-    ConfirmDeviceResponseOutputTypeDef,
-    CreateUserPoolDomainResponseOutputTypeDef,
+    AssociateSoftwareTokenResponseTypeDef,
+    ConfirmDeviceResponseTypeDef,
+    CreateUserPoolDomainResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetCSVHeaderResponseOutputTypeDef,
-    GetSigningCertificateResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    UpdateUserPoolDomainResponseOutputTypeDef,
-    VerifySoftwareTokenResponseOutputTypeDef,
+    GetCSVHeaderResponseTypeDef,
+    GetSigningCertificateResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateUserPoolDomainResponseTypeDef,
+    VerifySoftwareTokenResponseTypeDef,
     AdminDisableProviderForUserRequestRequestTypeDef,
     AdminLinkProviderForUserRequestRequestTypeDef,
-    DeviceTypeOutputTypeDef,
-    AdminGetUserResponseOutputTypeDef,
-    GetUserResponseOutputTypeDef,
-    UserTypeOutputTypeDef,
+    DeviceTypeTypeDef,
+    AdminGetUserResponseTypeDef,
+    GetUserResponseTypeDef,
+    UserTypeTypeDef,
     AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
     AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListResourceServersRequestListResourceServersPaginateTypeDef,
     ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
     ListUserPoolsRequestListUserPoolsPaginateTypeDef,
     ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
-    AdminListGroupsForUserResponseOutputTypeDef,
-    CreateGroupResponseOutputTypeDef,
-    GetGroupResponseOutputTypeDef,
-    ListGroupsResponseOutputTypeDef,
-    UpdateGroupResponseOutputTypeDef,
+    AdminListGroupsForUserResponseTypeDef,
+    CreateGroupResponseTypeDef,
+    GetGroupResponseTypeDef,
+    ListGroupsResponseTypeDef,
+    UpdateGroupResponseTypeDef,
     AdminSetUserMFAPreferenceRequestRequestTypeDef,
     SetUserMFAPreferenceRequestRequestTypeDef,
     AdminSetUserSettingsRequestRequestTypeDef,
     SetUserSettingsRequestRequestTypeDef,
-    AuthEventTypeOutputTypeDef,
-    AuthenticationResultTypeOutputTypeDef,
-    ForgotPasswordResponseOutputTypeDef,
-    GetUserAttributeVerificationCodeResponseOutputTypeDef,
-    ResendConfirmationCodeResponseOutputTypeDef,
-    SignUpResponseOutputTypeDef,
-    UpdateUserAttributesResponseOutputTypeDef,
+    AuthEventTypeTypeDef,
+    AuthenticationResultTypeTypeDef,
+    ForgotPasswordResponseTypeDef,
+    GetUserAttributeVerificationCodeResponseTypeDef,
+    ResendConfirmationCodeResponseTypeDef,
+    SignUpResponseTypeDef,
+    UpdateUserAttributesResponseTypeDef,
     CompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
     CompromisedCredentialsRiskConfigurationTypeTypeDef,
     ConfirmDeviceRequestRequestTypeDef,
     ConfirmForgotPasswordRequestRequestTypeDef,
     ConfirmSignUpRequestRequestTypeDef,
     ForgotPasswordRequestRequestTypeDef,
     InitiateAuthRequestRequestTypeDef,
     ResendConfirmationCodeRequestRequestTypeDef,
     RespondToAuthChallengeRequestRequestTypeDef,
     SignUpRequestRequestTypeDef,
     ContextDataTypeTypeDef,
-    CreateIdentityProviderResponseOutputTypeDef,
-    DescribeIdentityProviderResponseOutputTypeDef,
-    GetIdentityProviderByIdentifierResponseOutputTypeDef,
-    UpdateIdentityProviderResponseOutputTypeDef,
+    CreateIdentityProviderResponseTypeDef,
+    DescribeIdentityProviderResponseTypeDef,
+    GetIdentityProviderByIdentifierResponseTypeDef,
+    UpdateIdentityProviderResponseTypeDef,
     CreateResourceServerRequestRequestTypeDef,
     UpdateResourceServerRequestRequestTypeDef,
-    CreateUserImportJobResponseOutputTypeDef,
-    DescribeUserImportJobResponseOutputTypeDef,
-    ListUserImportJobsResponseOutputTypeDef,
-    StartUserImportJobResponseOutputTypeDef,
-    StopUserImportJobResponseOutputTypeDef,
+    CreateUserImportJobResponseTypeDef,
+    DescribeUserImportJobResponseTypeDef,
+    ListUserImportJobsResponseTypeDef,
+    StartUserImportJobResponseTypeDef,
+    StopUserImportJobResponseTypeDef,
     CreateUserPoolClientRequestRequestTypeDef,
     UpdateUserPoolClientRequestRequestTypeDef,
     CreateUserPoolDomainRequestRequestTypeDef,
     UpdateUserPoolDomainRequestRequestTypeDef,
     SmsMfaConfigTypeTypeDef,
-    DomainDescriptionTypeOutputTypeDef,
+    DomainDescriptionTypeTypeDef,
     LambdaConfigTypeOutputTypeDef,
     LambdaConfigTypeTypeDef,
-    GetUICustomizationResponseOutputTypeDef,
-    SetUICustomizationResponseOutputTypeDef,
-    ListIdentityProvidersResponseOutputTypeDef,
-    ListUserPoolClientsResponseOutputTypeDef,
+    GetUICustomizationResponseTypeDef,
+    SetUICustomizationResponseTypeDef,
+    ListIdentityProvidersResponseTypeDef,
+    ListUserPoolClientsResponseTypeDef,
     NotifyConfigurationTypeOutputTypeDef,
     NotifyConfigurationTypeTypeDef,
     UserPoolPolicyTypeOutputTypeDef,
     UserPoolPolicyTypeTypeDef,
-    ResourceServerTypeOutputTypeDef,
+    ResourceServerTypeTypeDef,
     SchemaAttributeTypeOutputTypeDef,
     SchemaAttributeTypeTypeDef,
     SmsMfaConfigTypeOutputTypeDef,
-    UserPoolClientTypeOutputTypeDef,
-    AdminGetDeviceResponseOutputTypeDef,
-    AdminListDevicesResponseOutputTypeDef,
-    GetDeviceResponseOutputTypeDef,
-    ListDevicesResponseOutputTypeDef,
-    AdminCreateUserResponseOutputTypeDef,
-    ListUsersInGroupResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
-    AdminListUserAuthEventsResponseOutputTypeDef,
-    AdminInitiateAuthResponseOutputTypeDef,
-    AdminRespondToAuthChallengeResponseOutputTypeDef,
-    InitiateAuthResponseOutputTypeDef,
-    RespondToAuthChallengeResponseOutputTypeDef,
+    UserPoolClientTypeTypeDef,
+    AdminGetDeviceResponseTypeDef,
+    AdminListDevicesResponseTypeDef,
+    GetDeviceResponseTypeDef,
+    ListDevicesResponseTypeDef,
+    AdminCreateUserResponseTypeDef,
+    ListUsersInGroupResponseTypeDef,
+    ListUsersResponseTypeDef,
+    AdminListUserAuthEventsResponseTypeDef,
+    AdminInitiateAuthResponseTypeDef,
+    AdminRespondToAuthChallengeResponseTypeDef,
+    InitiateAuthResponseTypeDef,
+    RespondToAuthChallengeResponseTypeDef,
     AdminInitiateAuthRequestRequestTypeDef,
     AdminRespondToAuthChallengeRequestRequestTypeDef,
     SetUserPoolMfaConfigRequestRequestTypeDef,
-    DescribeUserPoolDomainResponseOutputTypeDef,
-    UserPoolDescriptionTypeOutputTypeDef,
+    DescribeUserPoolDomainResponseTypeDef,
+    UserPoolDescriptionTypeTypeDef,
     AccountTakeoverRiskConfigurationTypeOutputTypeDef,
     AccountTakeoverRiskConfigurationTypeTypeDef,
     UpdateUserPoolRequestRequestTypeDef,
-    CreateResourceServerResponseOutputTypeDef,
-    DescribeResourceServerResponseOutputTypeDef,
-    ListResourceServersResponseOutputTypeDef,
-    UpdateResourceServerResponseOutputTypeDef,
-    UserPoolTypeOutputTypeDef,
+    CreateResourceServerResponseTypeDef,
+    DescribeResourceServerResponseTypeDef,
+    ListResourceServersResponseTypeDef,
+    UpdateResourceServerResponseTypeDef,
+    UserPoolTypeTypeDef,
     AddCustomAttributesRequestRequestTypeDef,
     CreateUserPoolRequestRequestTypeDef,
-    GetUserPoolMfaConfigResponseOutputTypeDef,
-    SetUserPoolMfaConfigResponseOutputTypeDef,
-    CreateUserPoolClientResponseOutputTypeDef,
-    DescribeUserPoolClientResponseOutputTypeDef,
-    UpdateUserPoolClientResponseOutputTypeDef,
-    ListUserPoolsResponseOutputTypeDef,
-    RiskConfigurationTypeOutputTypeDef,
+    GetUserPoolMfaConfigResponseTypeDef,
+    SetUserPoolMfaConfigResponseTypeDef,
+    CreateUserPoolClientResponseTypeDef,
+    DescribeUserPoolClientResponseTypeDef,
+    UpdateUserPoolClientResponseTypeDef,
+    ListUserPoolsResponseTypeDef,
+    RiskConfigurationTypeTypeDef,
     SetRiskConfigurationRequestRequestTypeDef,
-    CreateUserPoolResponseOutputTypeDef,
-    DescribeUserPoolResponseOutputTypeDef,
-    DescribeRiskConfigurationResponseOutputTypeDef,
-    SetRiskConfigurationResponseOutputTypeDef,
+    CreateUserPoolResponseTypeDef,
+    DescribeUserPoolResponseTypeDef,
+    DescribeRiskConfigurationResponseTypeDef,
+    SetRiskConfigurationResponseTypeDef,
 )
 
 
 def get_structure() -> RecoveryOptionTypeOutputTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/__init__.py` & `mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/__init__.pyi` & `mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/__main__.py` & `mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for boto3.CognitoIdentityProvider 1.28.3\nVersion:        "
-        " 1.28.3.post1\nBuilder version: 7.14.7\nDocs:           "
+        " 1.28.3.post2\nBuilder version: 7.15.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider\nOther"
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

### Comparing `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/client.py` & `mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,102 +47,102 @@
     ListUsersInGroupPaginator,
     ListUsersPaginator,
 )
 from .type_defs import (
     AccountRecoverySettingTypeTypeDef,
     AccountTakeoverRiskConfigurationTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
-    AdminCreateUserResponseOutputTypeDef,
-    AdminGetDeviceResponseOutputTypeDef,
-    AdminGetUserResponseOutputTypeDef,
-    AdminInitiateAuthResponseOutputTypeDef,
-    AdminListDevicesResponseOutputTypeDef,
-    AdminListGroupsForUserResponseOutputTypeDef,
-    AdminListUserAuthEventsResponseOutputTypeDef,
-    AdminRespondToAuthChallengeResponseOutputTypeDef,
+    AdminCreateUserResponseTypeDef,
+    AdminGetDeviceResponseTypeDef,
+    AdminGetUserResponseTypeDef,
+    AdminInitiateAuthResponseTypeDef,
+    AdminListDevicesResponseTypeDef,
+    AdminListGroupsForUserResponseTypeDef,
+    AdminListUserAuthEventsResponseTypeDef,
+    AdminRespondToAuthChallengeResponseTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
-    AssociateSoftwareTokenResponseOutputTypeDef,
+    AssociateSoftwareTokenResponseTypeDef,
     AttributeTypeTypeDef,
     CompromisedCredentialsRiskConfigurationTypeTypeDef,
-    ConfirmDeviceResponseOutputTypeDef,
+    ConfirmDeviceResponseTypeDef,
     ContextDataTypeTypeDef,
-    CreateGroupResponseOutputTypeDef,
-    CreateIdentityProviderResponseOutputTypeDef,
-    CreateResourceServerResponseOutputTypeDef,
-    CreateUserImportJobResponseOutputTypeDef,
-    CreateUserPoolClientResponseOutputTypeDef,
-    CreateUserPoolDomainResponseOutputTypeDef,
-    CreateUserPoolResponseOutputTypeDef,
+    CreateGroupResponseTypeDef,
+    CreateIdentityProviderResponseTypeDef,
+    CreateResourceServerResponseTypeDef,
+    CreateUserImportJobResponseTypeDef,
+    CreateUserPoolClientResponseTypeDef,
+    CreateUserPoolDomainResponseTypeDef,
+    CreateUserPoolResponseTypeDef,
     CustomDomainConfigTypeTypeDef,
-    DescribeIdentityProviderResponseOutputTypeDef,
-    DescribeResourceServerResponseOutputTypeDef,
-    DescribeRiskConfigurationResponseOutputTypeDef,
-    DescribeUserImportJobResponseOutputTypeDef,
-    DescribeUserPoolClientResponseOutputTypeDef,
-    DescribeUserPoolDomainResponseOutputTypeDef,
-    DescribeUserPoolResponseOutputTypeDef,
+    DescribeIdentityProviderResponseTypeDef,
+    DescribeResourceServerResponseTypeDef,
+    DescribeRiskConfigurationResponseTypeDef,
+    DescribeUserImportJobResponseTypeDef,
+    DescribeUserPoolClientResponseTypeDef,
+    DescribeUserPoolDomainResponseTypeDef,
+    DescribeUserPoolResponseTypeDef,
     DeviceConfigurationTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     EmptyResponseMetadataTypeDef,
-    ForgotPasswordResponseOutputTypeDef,
-    GetCSVHeaderResponseOutputTypeDef,
-    GetDeviceResponseOutputTypeDef,
-    GetGroupResponseOutputTypeDef,
-    GetIdentityProviderByIdentifierResponseOutputTypeDef,
-    GetSigningCertificateResponseOutputTypeDef,
-    GetUICustomizationResponseOutputTypeDef,
-    GetUserAttributeVerificationCodeResponseOutputTypeDef,
-    GetUserPoolMfaConfigResponseOutputTypeDef,
-    GetUserResponseOutputTypeDef,
-    InitiateAuthResponseOutputTypeDef,
+    ForgotPasswordResponseTypeDef,
+    GetCSVHeaderResponseTypeDef,
+    GetDeviceResponseTypeDef,
+    GetGroupResponseTypeDef,
+    GetIdentityProviderByIdentifierResponseTypeDef,
+    GetSigningCertificateResponseTypeDef,
+    GetUICustomizationResponseTypeDef,
+    GetUserAttributeVerificationCodeResponseTypeDef,
+    GetUserPoolMfaConfigResponseTypeDef,
+    GetUserResponseTypeDef,
+    InitiateAuthResponseTypeDef,
     LambdaConfigTypeTypeDef,
-    ListDevicesResponseOutputTypeDef,
-    ListGroupsResponseOutputTypeDef,
-    ListIdentityProvidersResponseOutputTypeDef,
-    ListResourceServersResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ListUserImportJobsResponseOutputTypeDef,
-    ListUserPoolClientsResponseOutputTypeDef,
-    ListUserPoolsResponseOutputTypeDef,
-    ListUsersInGroupResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
+    ListDevicesResponseTypeDef,
+    ListGroupsResponseTypeDef,
+    ListIdentityProvidersResponseTypeDef,
+    ListResourceServersResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListUserImportJobsResponseTypeDef,
+    ListUserPoolClientsResponseTypeDef,
+    ListUserPoolsResponseTypeDef,
+    ListUsersInGroupResponseTypeDef,
+    ListUsersResponseTypeDef,
     MFAOptionTypeTypeDef,
     ProviderUserIdentifierTypeTypeDef,
-    ResendConfirmationCodeResponseOutputTypeDef,
+    ResendConfirmationCodeResponseTypeDef,
     ResourceServerScopeTypeTypeDef,
-    RespondToAuthChallengeResponseOutputTypeDef,
+    RespondToAuthChallengeResponseTypeDef,
     RiskExceptionConfigurationTypeTypeDef,
     SchemaAttributeTypeTypeDef,
-    SetRiskConfigurationResponseOutputTypeDef,
-    SetUICustomizationResponseOutputTypeDef,
-    SetUserPoolMfaConfigResponseOutputTypeDef,
-    SignUpResponseOutputTypeDef,
+    SetRiskConfigurationResponseTypeDef,
+    SetUICustomizationResponseTypeDef,
+    SetUserPoolMfaConfigResponseTypeDef,
+    SignUpResponseTypeDef,
     SmsConfigurationTypeTypeDef,
     SmsMfaConfigTypeTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaConfigTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
-    StartUserImportJobResponseOutputTypeDef,
-    StopUserImportJobResponseOutputTypeDef,
+    StartUserImportJobResponseTypeDef,
+    StopUserImportJobResponseTypeDef,
     TokenValidityUnitsTypeTypeDef,
-    UpdateGroupResponseOutputTypeDef,
-    UpdateIdentityProviderResponseOutputTypeDef,
-    UpdateResourceServerResponseOutputTypeDef,
-    UpdateUserAttributesResponseOutputTypeDef,
-    UpdateUserPoolClientResponseOutputTypeDef,
-    UpdateUserPoolDomainResponseOutputTypeDef,
+    UpdateGroupResponseTypeDef,
+    UpdateIdentityProviderResponseTypeDef,
+    UpdateResourceServerResponseTypeDef,
+    UpdateUserAttributesResponseTypeDef,
+    UpdateUserPoolClientResponseTypeDef,
+    UpdateUserPoolDomainResponseTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserContextDataTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UserPoolPolicyTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
-    VerifySoftwareTokenResponseOutputTypeDef,
+    VerifySoftwareTokenResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -258,15 +258,15 @@
         UserAttributes: Sequence[AttributeTypeTypeDef] = ...,
         ValidationData: Sequence[AttributeTypeTypeDef] = ...,
         TemporaryPassword: str = ...,
         ForceAliasCreation: bool = ...,
         MessageAction: MessageActionTypeType = ...,
         DesiredDeliveryMediums: Sequence[DeliveryMediumTypeType] = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> AdminCreateUserResponseOutputTypeDef:
+    ) -> AdminCreateUserResponseTypeDef:
         """
         Creates a new user in the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_create_user)
         """
 
@@ -323,25 +323,23 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_forget_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_forget_device)
         """
 
     def admin_get_device(
         self, *, DeviceKey: str, UserPoolId: str, Username: str
-    ) -> AdminGetDeviceResponseOutputTypeDef:
+    ) -> AdminGetDeviceResponseTypeDef:
         """
         Gets the device, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_get_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_get_device)
         """
 
-    def admin_get_user(
-        self, *, UserPoolId: str, Username: str
-    ) -> AdminGetUserResponseOutputTypeDef:
+    def admin_get_user(self, *, UserPoolId: str, Username: str) -> AdminGetUserResponseTypeDef:
         """
         Gets the specified user by user name in a user pool as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_get_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_get_user)
         """
 
@@ -351,15 +349,15 @@
         UserPoolId: str,
         ClientId: str,
         AuthFlow: AuthFlowTypeType,
         AuthParameters: Mapping[str, str] = ...,
         ClientMetadata: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ContextData: ContextDataTypeTypeDef = ...
-    ) -> AdminInitiateAuthResponseOutputTypeDef:
+    ) -> AdminInitiateAuthResponseTypeDef:
         """
         Initiates the authentication flow, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_initiate_auth)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_initiate_auth)
         """
 
@@ -377,35 +375,35 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_link_provider_for_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_link_provider_for_user)
         """
 
     def admin_list_devices(
         self, *, UserPoolId: str, Username: str, Limit: int = ..., PaginationToken: str = ...
-    ) -> AdminListDevicesResponseOutputTypeDef:
+    ) -> AdminListDevicesResponseTypeDef:
         """
         Lists devices, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_list_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_list_devices)
         """
 
     def admin_list_groups_for_user(
         self, *, Username: str, UserPoolId: str, Limit: int = ..., NextToken: str = ...
-    ) -> AdminListGroupsForUserResponseOutputTypeDef:
+    ) -> AdminListGroupsForUserResponseTypeDef:
         """
         Lists the groups that the user belongs to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_list_groups_for_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_list_groups_for_user)
         """
 
     def admin_list_user_auth_events(
         self, *, UserPoolId: str, Username: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> AdminListUserAuthEventsResponseOutputTypeDef:
+    ) -> AdminListUserAuthEventsResponseTypeDef:
         """
         A history of user activity and any risks detected as part of Amazon Cognito
         advanced security.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_list_user_auth_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_list_user_auth_events)
         """
@@ -437,15 +435,15 @@
         ClientId: str,
         ChallengeName: ChallengeNameTypeType,
         ChallengeResponses: Mapping[str, str] = ...,
         Session: str = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ContextData: ContextDataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> AdminRespondToAuthChallengeResponseOutputTypeDef:
+    ) -> AdminRespondToAuthChallengeResponseTypeDef:
         """
         Responds to an authentication challenge, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_respond_to_auth_challenge)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_respond_to_auth_challenge)
         """
 
@@ -533,15 +531,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_user_global_sign_out)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_user_global_sign_out)
         """
 
     def associate_software_token(
         self, *, AccessToken: str = ..., Session: str = ...
-    ) -> AssociateSoftwareTokenResponseOutputTypeDef:
+    ) -> AssociateSoftwareTokenResponseTypeDef:
         """
         Begins setup of time-based one-time password (TOTP) multi-factor authentication
         (MFA) for a user, with a unique private key that Amazon Cognito generates and
         returns in the API response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.associate_software_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#associate_software_token)
@@ -576,15 +574,15 @@
     def confirm_device(
         self,
         *,
         AccessToken: str,
         DeviceKey: str,
         DeviceSecretVerifierConfig: DeviceSecretVerifierConfigTypeTypeDef = ...,
         DeviceName: str = ...
-    ) -> ConfirmDeviceResponseOutputTypeDef:
+    ) -> ConfirmDeviceResponseTypeDef:
         """
         Confirms tracking of the device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.confirm_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#confirm_device)
         """
 
@@ -630,15 +628,15 @@
         self,
         *,
         GroupName: str,
         UserPoolId: str,
         Description: str = ...,
         RoleArn: str = ...,
         Precedence: int = ...
-    ) -> CreateGroupResponseOutputTypeDef:
+    ) -> CreateGroupResponseTypeDef:
         """
         Creates a new group in the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_group)
         """
 
@@ -647,40 +645,40 @@
         *,
         UserPoolId: str,
         ProviderName: str,
         ProviderType: IdentityProviderTypeTypeType,
         ProviderDetails: Mapping[str, str],
         AttributeMapping: Mapping[str, str] = ...,
         IdpIdentifiers: Sequence[str] = ...
-    ) -> CreateIdentityProviderResponseOutputTypeDef:
+    ) -> CreateIdentityProviderResponseTypeDef:
         """
         Creates an IdP for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_identity_provider)
         """
 
     def create_resource_server(
         self,
         *,
         UserPoolId: str,
         Identifier: str,
         Name: str,
         Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...
-    ) -> CreateResourceServerResponseOutputTypeDef:
+    ) -> CreateResourceServerResponseTypeDef:
         """
         Creates a new OAuth2.0 resource server and defines custom scopes within it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_resource_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_resource_server)
         """
 
     def create_user_import_job(
         self, *, JobName: str, UserPoolId: str, CloudWatchLogsRoleArn: str
-    ) -> CreateUserImportJobResponseOutputTypeDef:
+    ) -> CreateUserImportJobResponseTypeDef:
         """
         Creates the user import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_import_job)
         """
 
@@ -706,15 +704,15 @@
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         Schema: Sequence[SchemaAttributeTypeTypeDef] = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
         UsernameConfiguration: UsernameConfigurationTypeTypeDef = ...,
         AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...
-    ) -> CreateUserPoolResponseOutputTypeDef:
+    ) -> CreateUserPoolResponseTypeDef:
         """
         Creates a new Amazon Cognito user pool and sets the password policy for the
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_pool)
         """
@@ -740,29 +738,29 @@
         AllowedOAuthScopes: Sequence[str] = ...,
         AllowedOAuthFlowsUserPoolClient: bool = ...,
         AnalyticsConfiguration: AnalyticsConfigurationTypeTypeDef = ...,
         PreventUserExistenceErrors: PreventUserExistenceErrorTypesType = ...,
         EnableTokenRevocation: bool = ...,
         EnablePropagateAdditionalUserContextData: bool = ...,
         AuthSessionValidity: int = ...
-    ) -> CreateUserPoolClientResponseOutputTypeDef:
+    ) -> CreateUserPoolClientResponseTypeDef:
         """
         Creates the user pool client.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool_client)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_pool_client)
         """
 
     def create_user_pool_domain(
         self,
         *,
         Domain: str,
         UserPoolId: str,
         CustomDomainConfig: CustomDomainConfigTypeTypeDef = ...
-    ) -> CreateUserPoolDomainResponseOutputTypeDef:
+    ) -> CreateUserPoolDomainResponseTypeDef:
         """
         Creates a new domain for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_pool_domain)
         """
 
@@ -836,74 +834,72 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.delete_user_pool_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#delete_user_pool_domain)
         """
 
     def describe_identity_provider(
         self, *, UserPoolId: str, ProviderName: str
-    ) -> DescribeIdentityProviderResponseOutputTypeDef:
+    ) -> DescribeIdentityProviderResponseTypeDef:
         """
         Gets information about a specific IdP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_identity_provider)
         """
 
     def describe_resource_server(
         self, *, UserPoolId: str, Identifier: str
-    ) -> DescribeResourceServerResponseOutputTypeDef:
+    ) -> DescribeResourceServerResponseTypeDef:
         """
         Describes a resource server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_resource_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_resource_server)
         """
 
     def describe_risk_configuration(
         self, *, UserPoolId: str, ClientId: str = ...
-    ) -> DescribeRiskConfigurationResponseOutputTypeDef:
+    ) -> DescribeRiskConfigurationResponseTypeDef:
         """
         Describes the risk configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_risk_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_risk_configuration)
         """
 
     def describe_user_import_job(
         self, *, UserPoolId: str, JobId: str
-    ) -> DescribeUserImportJobResponseOutputTypeDef:
+    ) -> DescribeUserImportJobResponseTypeDef:
         """
         Describes the user import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_user_import_job)
         """
 
-    def describe_user_pool(self, *, UserPoolId: str) -> DescribeUserPoolResponseOutputTypeDef:
+    def describe_user_pool(self, *, UserPoolId: str) -> DescribeUserPoolResponseTypeDef:
         """
         Returns the configuration information and metadata of the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_user_pool)
         """
 
     def describe_user_pool_client(
         self, *, UserPoolId: str, ClientId: str
-    ) -> DescribeUserPoolClientResponseOutputTypeDef:
+    ) -> DescribeUserPoolClientResponseTypeDef:
         """
         Client method for returning the configuration information and metadata of the
         specified user pool app client.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_pool_client)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_user_pool_client)
         """
 
-    def describe_user_pool_domain(
-        self, *, Domain: str
-    ) -> DescribeUserPoolDomainResponseOutputTypeDef:
+    def describe_user_pool_domain(self, *, Domain: str) -> DescribeUserPoolDomainResponseTypeDef:
         """
         Gets information about a domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_pool_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_user_pool_domain)
         """
 
@@ -922,15 +918,15 @@
         *,
         ClientId: str,
         Username: str,
         SecretHash: str = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> ForgotPasswordResponseOutputTypeDef:
+    ) -> ForgotPasswordResponseTypeDef:
         """
         Calling this API causes a message to be sent to the end user with a confirmation
         code that is required to change the user's password.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.forgot_password)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#forgot_password)
         """
@@ -945,93 +941,87 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#generate_presigned_url)
         """
 
-    def get_csv_header(self, *, UserPoolId: str) -> GetCSVHeaderResponseOutputTypeDef:
+    def get_csv_header(self, *, UserPoolId: str) -> GetCSVHeaderResponseTypeDef:
         """
         Gets the header information for the comma-separated value (CSV) file to be used
         as input for the user import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_csv_header)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_csv_header)
         """
 
-    def get_device(
-        self, *, DeviceKey: str, AccessToken: str = ...
-    ) -> GetDeviceResponseOutputTypeDef:
+    def get_device(self, *, DeviceKey: str, AccessToken: str = ...) -> GetDeviceResponseTypeDef:
         """
         Gets the device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_device)
         """
 
-    def get_group(self, *, GroupName: str, UserPoolId: str) -> GetGroupResponseOutputTypeDef:
+    def get_group(self, *, GroupName: str, UserPoolId: str) -> GetGroupResponseTypeDef:
         """
         Gets a group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_group)
         """
 
     def get_identity_provider_by_identifier(
         self, *, UserPoolId: str, IdpIdentifier: str
-    ) -> GetIdentityProviderByIdentifierResponseOutputTypeDef:
+    ) -> GetIdentityProviderByIdentifierResponseTypeDef:
         """
         Gets the specified IdP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_identity_provider_by_identifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_identity_provider_by_identifier)
         """
 
-    def get_signing_certificate(
-        self, *, UserPoolId: str
-    ) -> GetSigningCertificateResponseOutputTypeDef:
+    def get_signing_certificate(self, *, UserPoolId: str) -> GetSigningCertificateResponseTypeDef:
         """
         This method takes a user pool ID, and returns the signing certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_signing_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_signing_certificate)
         """
 
     def get_ui_customization(
         self, *, UserPoolId: str, ClientId: str = ...
-    ) -> GetUICustomizationResponseOutputTypeDef:
+    ) -> GetUICustomizationResponseTypeDef:
         """
         Gets the user interface (UI) Customization information for a particular app
         client's app UI, if any such information exists for the client.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_ui_customization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_ui_customization)
         """
 
-    def get_user(self, *, AccessToken: str) -> GetUserResponseOutputTypeDef:
+    def get_user(self, *, AccessToken: str) -> GetUserResponseTypeDef:
         """
         Gets the user attributes and metadata for a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_user)
         """
 
     def get_user_attribute_verification_code(
         self, *, AccessToken: str, AttributeName: str, ClientMetadata: Mapping[str, str] = ...
-    ) -> GetUserAttributeVerificationCodeResponseOutputTypeDef:
+    ) -> GetUserAttributeVerificationCodeResponseTypeDef:
         """
         Generates a user attribute verification code for the specified attribute name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_user_attribute_verification_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_user_attribute_verification_code)
         """
 
-    def get_user_pool_mfa_config(
-        self, *, UserPoolId: str
-    ) -> GetUserPoolMfaConfigResponseOutputTypeDef:
+    def get_user_pool_mfa_config(self, *, UserPoolId: str) -> GetUserPoolMfaConfigResponseTypeDef:
         """
         Gets the user pool multi-factor authentication (MFA) configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_user_pool_mfa_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_user_pool_mfa_config)
         """
 
@@ -1048,96 +1038,94 @@
         *,
         AuthFlow: AuthFlowTypeType,
         ClientId: str,
         AuthParameters: Mapping[str, str] = ...,
         ClientMetadata: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...
-    ) -> InitiateAuthResponseOutputTypeDef:
+    ) -> InitiateAuthResponseTypeDef:
         """
         Initiates sign-in for a user in the Amazon Cognito user directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.initiate_auth)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#initiate_auth)
         """
 
     def list_devices(
         self, *, AccessToken: str, Limit: int = ..., PaginationToken: str = ...
-    ) -> ListDevicesResponseOutputTypeDef:
+    ) -> ListDevicesResponseTypeDef:
         """
         Lists the sign-in devices that Amazon Cognito has registered to the current
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_devices)
         """
 
     def list_groups(
         self, *, UserPoolId: str, Limit: int = ..., NextToken: str = ...
-    ) -> ListGroupsResponseOutputTypeDef:
+    ) -> ListGroupsResponseTypeDef:
         """
         Lists the groups associated with a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_groups)
         """
 
     def list_identity_providers(
         self, *, UserPoolId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListIdentityProvidersResponseOutputTypeDef:
+    ) -> ListIdentityProvidersResponseTypeDef:
         """
         Lists information about all IdPs for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_identity_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_identity_providers)
         """
 
     def list_resource_servers(
         self, *, UserPoolId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListResourceServersResponseOutputTypeDef:
+    ) -> ListResourceServersResponseTypeDef:
         """
         Lists the resource servers for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_resource_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_resource_servers)
         """
 
-    def list_tags_for_resource(
-        self, *, ResourceArn: str
-    ) -> ListTagsForResourceResponseOutputTypeDef:
+    def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags that are assigned to an Amazon Cognito user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_tags_for_resource)
         """
 
     def list_user_import_jobs(
         self, *, UserPoolId: str, MaxResults: int, PaginationToken: str = ...
-    ) -> ListUserImportJobsResponseOutputTypeDef:
+    ) -> ListUserImportJobsResponseTypeDef:
         """
         Lists the user import jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_user_import_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_user_import_jobs)
         """
 
     def list_user_pool_clients(
         self, *, UserPoolId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListUserPoolClientsResponseOutputTypeDef:
+    ) -> ListUserPoolClientsResponseTypeDef:
         """
         Lists the clients that have been created for the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_user_pool_clients)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_user_pool_clients)
         """
 
     def list_user_pools(
         self, *, MaxResults: int, NextToken: str = ...
-    ) -> ListUserPoolsResponseOutputTypeDef:
+    ) -> ListUserPoolsResponseTypeDef:
         """
         Lists the user pools associated with an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_user_pools)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_user_pools)
         """
 
@@ -1145,25 +1133,25 @@
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         PaginationToken: str = ...,
         Filter: str = ...
-    ) -> ListUsersResponseOutputTypeDef:
+    ) -> ListUsersResponseTypeDef:
         """
         Lists the users in the Amazon Cognito user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_users)
         """
 
     def list_users_in_group(
         self, *, UserPoolId: str, GroupName: str, Limit: int = ..., NextToken: str = ...
-    ) -> ListUsersInGroupResponseOutputTypeDef:
+    ) -> ListUsersInGroupResponseTypeDef:
         """
         Lists the users in the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_users_in_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_users_in_group)
         """
 
@@ -1172,15 +1160,15 @@
         *,
         ClientId: str,
         Username: str,
         SecretHash: str = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> ResendConfirmationCodeResponseOutputTypeDef:
+    ) -> ResendConfirmationCodeResponseTypeDef:
         """
         Resends the confirmation (for confirmation of registration) to a specific user
         in the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.resend_confirmation_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#resend_confirmation_code)
         """
@@ -1191,15 +1179,15 @@
         ClientId: str,
         ChallengeName: ChallengeNameTypeType,
         Session: str = ...,
         ChallengeResponses: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> RespondToAuthChallengeResponseOutputTypeDef:
+    ) -> RespondToAuthChallengeResponseTypeDef:
         """
         Responds to the authentication challenge.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.respond_to_auth_challenge)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#respond_to_auth_challenge)
         """
 
@@ -1216,30 +1204,30 @@
         self,
         *,
         UserPoolId: str,
         ClientId: str = ...,
         CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeTypeDef = ...,
         AccountTakeoverRiskConfiguration: AccountTakeoverRiskConfigurationTypeTypeDef = ...,
         RiskExceptionConfiguration: RiskExceptionConfigurationTypeTypeDef = ...
-    ) -> SetRiskConfigurationResponseOutputTypeDef:
+    ) -> SetRiskConfigurationResponseTypeDef:
         """
         Configures actions on detected risks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_risk_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#set_risk_configuration)
         """
 
     def set_ui_customization(
         self,
         *,
         UserPoolId: str,
         ClientId: str = ...,
         CSS: str = ...,
         ImageFile: Union[str, bytes, IO[Any], StreamingBody] = ...
-    ) -> SetUICustomizationResponseOutputTypeDef:
+    ) -> SetUICustomizationResponseTypeDef:
         """
         Sets the user interface (UI) customization information for a user pool's built-
         in app UI.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_ui_customization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#set_ui_customization)
         """
@@ -1262,15 +1250,15 @@
     def set_user_pool_mfa_config(
         self,
         *,
         UserPoolId: str,
         SmsMfaConfiguration: SmsMfaConfigTypeTypeDef = ...,
         SoftwareTokenMfaConfiguration: SoftwareTokenMfaConfigTypeTypeDef = ...,
         MfaConfiguration: UserPoolMfaTypeType = ...
-    ) -> SetUserPoolMfaConfigResponseOutputTypeDef:
+    ) -> SetUserPoolMfaConfigResponseTypeDef:
         """
         Sets the user pool multi-factor authentication (MFA) configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_user_pool_mfa_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#set_user_pool_mfa_config)
         """
 
@@ -1292,36 +1280,36 @@
         Password: str,
         SecretHash: str = ...,
         UserAttributes: Sequence[AttributeTypeTypeDef] = ...,
         ValidationData: Sequence[AttributeTypeTypeDef] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> SignUpResponseOutputTypeDef:
+    ) -> SignUpResponseTypeDef:
         """
         Registers the user in the specified user pool and creates a user name, password,
         and user attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.sign_up)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#sign_up)
         """
 
     def start_user_import_job(
         self, *, UserPoolId: str, JobId: str
-    ) -> StartUserImportJobResponseOutputTypeDef:
+    ) -> StartUserImportJobResponseTypeDef:
         """
         Starts the user import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.start_user_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#start_user_import_job)
         """
 
     def stop_user_import_job(
         self, *, UserPoolId: str, JobId: str
-    ) -> StopUserImportJobResponseOutputTypeDef:
+    ) -> StopUserImportJobResponseTypeDef:
         """
         Stops the user import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.stop_user_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#stop_user_import_job)
         """
 
@@ -1376,15 +1364,15 @@
         self,
         *,
         GroupName: str,
         UserPoolId: str,
         Description: str = ...,
         RoleArn: str = ...,
         Precedence: int = ...
-    ) -> UpdateGroupResponseOutputTypeDef:
+    ) -> UpdateGroupResponseTypeDef:
         """
         Updates the specified group with the specified attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_group)
         """
 
@@ -1392,44 +1380,44 @@
         self,
         *,
         UserPoolId: str,
         ProviderName: str,
         ProviderDetails: Mapping[str, str] = ...,
         AttributeMapping: Mapping[str, str] = ...,
         IdpIdentifiers: Sequence[str] = ...
-    ) -> UpdateIdentityProviderResponseOutputTypeDef:
+    ) -> UpdateIdentityProviderResponseTypeDef:
         """
         Updates IdP information for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_identity_provider)
         """
 
     def update_resource_server(
         self,
         *,
         UserPoolId: str,
         Identifier: str,
         Name: str,
         Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...
-    ) -> UpdateResourceServerResponseOutputTypeDef:
+    ) -> UpdateResourceServerResponseTypeDef:
         """
         Updates the name and scopes of resource server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_resource_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_resource_server)
         """
 
     def update_user_attributes(
         self,
         *,
         UserAttributes: Sequence[AttributeTypeTypeDef],
         AccessToken: str,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> UpdateUserAttributesResponseOutputTypeDef:
+    ) -> UpdateUserAttributesResponseTypeDef:
         """
         Allows a user to update a specific attribute (one at a time).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_user_attributes)
         """
 
@@ -1484,25 +1472,25 @@
         AllowedOAuthScopes: Sequence[str] = ...,
         AllowedOAuthFlowsUserPoolClient: bool = ...,
         AnalyticsConfiguration: AnalyticsConfigurationTypeTypeDef = ...,
         PreventUserExistenceErrors: PreventUserExistenceErrorTypesType = ...,
         EnableTokenRevocation: bool = ...,
         EnablePropagateAdditionalUserContextData: bool = ...,
         AuthSessionValidity: int = ...
-    ) -> UpdateUserPoolClientResponseOutputTypeDef:
+    ) -> UpdateUserPoolClientResponseTypeDef:
         """
         Updates the specified user pool app client with the specified attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool_client)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_user_pool_client)
         """
 
     def update_user_pool_domain(
         self, *, Domain: str, UserPoolId: str, CustomDomainConfig: CustomDomainConfigTypeTypeDef
-    ) -> UpdateUserPoolDomainResponseOutputTypeDef:
+    ) -> UpdateUserPoolDomainResponseTypeDef:
         """
         Updates the Secure Sockets Layer (SSL) certificate for the custom domain for
         your user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_user_pool_domain)
         """
@@ -1510,15 +1498,15 @@
     def verify_software_token(
         self,
         *,
         UserCode: str,
         AccessToken: str = ...,
         Session: str = ...,
         FriendlyDeviceName: str = ...
-    ) -> VerifySoftwareTokenResponseOutputTypeDef:
+    ) -> VerifySoftwareTokenResponseTypeDef:
         """
         Use this API to register a user's entered time-based one-time password (TOTP)
         code and mark the user's software token MFA status as "verified" if successful.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.verify_software_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#verify_software_token)
         """
```

### Comparing `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/client.pyi` & `mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/client.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -47,102 +47,102 @@
     ListUsersInGroupPaginator,
     ListUsersPaginator,
 )
 from .type_defs import (
     AccountRecoverySettingTypeTypeDef,
     AccountTakeoverRiskConfigurationTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
-    AdminCreateUserResponseOutputTypeDef,
-    AdminGetDeviceResponseOutputTypeDef,
-    AdminGetUserResponseOutputTypeDef,
-    AdminInitiateAuthResponseOutputTypeDef,
-    AdminListDevicesResponseOutputTypeDef,
-    AdminListGroupsForUserResponseOutputTypeDef,
-    AdminListUserAuthEventsResponseOutputTypeDef,
-    AdminRespondToAuthChallengeResponseOutputTypeDef,
+    AdminCreateUserResponseTypeDef,
+    AdminGetDeviceResponseTypeDef,
+    AdminGetUserResponseTypeDef,
+    AdminInitiateAuthResponseTypeDef,
+    AdminListDevicesResponseTypeDef,
+    AdminListGroupsForUserResponseTypeDef,
+    AdminListUserAuthEventsResponseTypeDef,
+    AdminRespondToAuthChallengeResponseTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
-    AssociateSoftwareTokenResponseOutputTypeDef,
+    AssociateSoftwareTokenResponseTypeDef,
     AttributeTypeTypeDef,
     CompromisedCredentialsRiskConfigurationTypeTypeDef,
-    ConfirmDeviceResponseOutputTypeDef,
+    ConfirmDeviceResponseTypeDef,
     ContextDataTypeTypeDef,
-    CreateGroupResponseOutputTypeDef,
-    CreateIdentityProviderResponseOutputTypeDef,
-    CreateResourceServerResponseOutputTypeDef,
-    CreateUserImportJobResponseOutputTypeDef,
-    CreateUserPoolClientResponseOutputTypeDef,
-    CreateUserPoolDomainResponseOutputTypeDef,
-    CreateUserPoolResponseOutputTypeDef,
+    CreateGroupResponseTypeDef,
+    CreateIdentityProviderResponseTypeDef,
+    CreateResourceServerResponseTypeDef,
+    CreateUserImportJobResponseTypeDef,
+    CreateUserPoolClientResponseTypeDef,
+    CreateUserPoolDomainResponseTypeDef,
+    CreateUserPoolResponseTypeDef,
     CustomDomainConfigTypeTypeDef,
-    DescribeIdentityProviderResponseOutputTypeDef,
-    DescribeResourceServerResponseOutputTypeDef,
-    DescribeRiskConfigurationResponseOutputTypeDef,
-    DescribeUserImportJobResponseOutputTypeDef,
-    DescribeUserPoolClientResponseOutputTypeDef,
-    DescribeUserPoolDomainResponseOutputTypeDef,
-    DescribeUserPoolResponseOutputTypeDef,
+    DescribeIdentityProviderResponseTypeDef,
+    DescribeResourceServerResponseTypeDef,
+    DescribeRiskConfigurationResponseTypeDef,
+    DescribeUserImportJobResponseTypeDef,
+    DescribeUserPoolClientResponseTypeDef,
+    DescribeUserPoolDomainResponseTypeDef,
+    DescribeUserPoolResponseTypeDef,
     DeviceConfigurationTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     EmptyResponseMetadataTypeDef,
-    ForgotPasswordResponseOutputTypeDef,
-    GetCSVHeaderResponseOutputTypeDef,
-    GetDeviceResponseOutputTypeDef,
-    GetGroupResponseOutputTypeDef,
-    GetIdentityProviderByIdentifierResponseOutputTypeDef,
-    GetSigningCertificateResponseOutputTypeDef,
-    GetUICustomizationResponseOutputTypeDef,
-    GetUserAttributeVerificationCodeResponseOutputTypeDef,
-    GetUserPoolMfaConfigResponseOutputTypeDef,
-    GetUserResponseOutputTypeDef,
-    InitiateAuthResponseOutputTypeDef,
+    ForgotPasswordResponseTypeDef,
+    GetCSVHeaderResponseTypeDef,
+    GetDeviceResponseTypeDef,
+    GetGroupResponseTypeDef,
+    GetIdentityProviderByIdentifierResponseTypeDef,
+    GetSigningCertificateResponseTypeDef,
+    GetUICustomizationResponseTypeDef,
+    GetUserAttributeVerificationCodeResponseTypeDef,
+    GetUserPoolMfaConfigResponseTypeDef,
+    GetUserResponseTypeDef,
+    InitiateAuthResponseTypeDef,
     LambdaConfigTypeTypeDef,
-    ListDevicesResponseOutputTypeDef,
-    ListGroupsResponseOutputTypeDef,
-    ListIdentityProvidersResponseOutputTypeDef,
-    ListResourceServersResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    ListUserImportJobsResponseOutputTypeDef,
-    ListUserPoolClientsResponseOutputTypeDef,
-    ListUserPoolsResponseOutputTypeDef,
-    ListUsersInGroupResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
+    ListDevicesResponseTypeDef,
+    ListGroupsResponseTypeDef,
+    ListIdentityProvidersResponseTypeDef,
+    ListResourceServersResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListUserImportJobsResponseTypeDef,
+    ListUserPoolClientsResponseTypeDef,
+    ListUserPoolsResponseTypeDef,
+    ListUsersInGroupResponseTypeDef,
+    ListUsersResponseTypeDef,
     MFAOptionTypeTypeDef,
     ProviderUserIdentifierTypeTypeDef,
-    ResendConfirmationCodeResponseOutputTypeDef,
+    ResendConfirmationCodeResponseTypeDef,
     ResourceServerScopeTypeTypeDef,
-    RespondToAuthChallengeResponseOutputTypeDef,
+    RespondToAuthChallengeResponseTypeDef,
     RiskExceptionConfigurationTypeTypeDef,
     SchemaAttributeTypeTypeDef,
-    SetRiskConfigurationResponseOutputTypeDef,
-    SetUICustomizationResponseOutputTypeDef,
-    SetUserPoolMfaConfigResponseOutputTypeDef,
-    SignUpResponseOutputTypeDef,
+    SetRiskConfigurationResponseTypeDef,
+    SetUICustomizationResponseTypeDef,
+    SetUserPoolMfaConfigResponseTypeDef,
+    SignUpResponseTypeDef,
     SmsConfigurationTypeTypeDef,
     SmsMfaConfigTypeTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaConfigTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
-    StartUserImportJobResponseOutputTypeDef,
-    StopUserImportJobResponseOutputTypeDef,
+    StartUserImportJobResponseTypeDef,
+    StopUserImportJobResponseTypeDef,
     TokenValidityUnitsTypeTypeDef,
-    UpdateGroupResponseOutputTypeDef,
-    UpdateIdentityProviderResponseOutputTypeDef,
-    UpdateResourceServerResponseOutputTypeDef,
-    UpdateUserAttributesResponseOutputTypeDef,
-    UpdateUserPoolClientResponseOutputTypeDef,
-    UpdateUserPoolDomainResponseOutputTypeDef,
+    UpdateGroupResponseTypeDef,
+    UpdateIdentityProviderResponseTypeDef,
+    UpdateResourceServerResponseTypeDef,
+    UpdateUserAttributesResponseTypeDef,
+    UpdateUserPoolClientResponseTypeDef,
+    UpdateUserPoolDomainResponseTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserContextDataTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UserPoolPolicyTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
-    VerifySoftwareTokenResponseOutputTypeDef,
+    VerifySoftwareTokenResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -250,15 +250,15 @@
         UserAttributes: Sequence[AttributeTypeTypeDef] = ...,
         ValidationData: Sequence[AttributeTypeTypeDef] = ...,
         TemporaryPassword: str = ...,
         ForceAliasCreation: bool = ...,
         MessageAction: MessageActionTypeType = ...,
         DesiredDeliveryMediums: Sequence[DeliveryMediumTypeType] = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> AdminCreateUserResponseOutputTypeDef:
+    ) -> AdminCreateUserResponseTypeDef:
         """
         Creates a new user in the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_create_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_create_user)
         """
     def admin_delete_user(self, *, UserPoolId: str, Username: str) -> EmptyResponseMetadataTypeDef:
@@ -308,24 +308,22 @@
         Forgets the device, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_forget_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_forget_device)
         """
     def admin_get_device(
         self, *, DeviceKey: str, UserPoolId: str, Username: str
-    ) -> AdminGetDeviceResponseOutputTypeDef:
+    ) -> AdminGetDeviceResponseTypeDef:
         """
         Gets the device, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_get_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_get_device)
         """
-    def admin_get_user(
-        self, *, UserPoolId: str, Username: str
-    ) -> AdminGetUserResponseOutputTypeDef:
+    def admin_get_user(self, *, UserPoolId: str, Username: str) -> AdminGetUserResponseTypeDef:
         """
         Gets the specified user by user name in a user pool as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_get_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_get_user)
         """
     def admin_initiate_auth(
@@ -334,15 +332,15 @@
         UserPoolId: str,
         ClientId: str,
         AuthFlow: AuthFlowTypeType,
         AuthParameters: Mapping[str, str] = ...,
         ClientMetadata: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ContextData: ContextDataTypeTypeDef = ...
-    ) -> AdminInitiateAuthResponseOutputTypeDef:
+    ) -> AdminInitiateAuthResponseTypeDef:
         """
         Initiates the authentication flow, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_initiate_auth)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_initiate_auth)
         """
     def admin_link_provider_for_user(
@@ -358,33 +356,33 @@
         name and value from the external IdP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_link_provider_for_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_link_provider_for_user)
         """
     def admin_list_devices(
         self, *, UserPoolId: str, Username: str, Limit: int = ..., PaginationToken: str = ...
-    ) -> AdminListDevicesResponseOutputTypeDef:
+    ) -> AdminListDevicesResponseTypeDef:
         """
         Lists devices, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_list_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_list_devices)
         """
     def admin_list_groups_for_user(
         self, *, Username: str, UserPoolId: str, Limit: int = ..., NextToken: str = ...
-    ) -> AdminListGroupsForUserResponseOutputTypeDef:
+    ) -> AdminListGroupsForUserResponseTypeDef:
         """
         Lists the groups that the user belongs to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_list_groups_for_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_list_groups_for_user)
         """
     def admin_list_user_auth_events(
         self, *, UserPoolId: str, Username: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> AdminListUserAuthEventsResponseOutputTypeDef:
+    ) -> AdminListUserAuthEventsResponseTypeDef:
         """
         A history of user activity and any risks detected as part of Amazon Cognito
         advanced security.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_list_user_auth_events)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_list_user_auth_events)
         """
@@ -413,15 +411,15 @@
         ClientId: str,
         ChallengeName: ChallengeNameTypeType,
         ChallengeResponses: Mapping[str, str] = ...,
         Session: str = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ContextData: ContextDataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> AdminRespondToAuthChallengeResponseOutputTypeDef:
+    ) -> AdminRespondToAuthChallengeResponseTypeDef:
         """
         Responds to an authentication challenge, as an administrator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_respond_to_auth_challenge)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_respond_to_auth_challenge)
         """
     def admin_set_user_mfa_preference(
@@ -501,15 +499,15 @@
         Signs out a user from all devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.admin_user_global_sign_out)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#admin_user_global_sign_out)
         """
     def associate_software_token(
         self, *, AccessToken: str = ..., Session: str = ...
-    ) -> AssociateSoftwareTokenResponseOutputTypeDef:
+    ) -> AssociateSoftwareTokenResponseTypeDef:
         """
         Begins setup of time-based one-time password (TOTP) multi-factor authentication
         (MFA) for a user, with a unique private key that Amazon Cognito generates and
         returns in the API response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.associate_software_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#associate_software_token)
@@ -540,15 +538,15 @@
     def confirm_device(
         self,
         *,
         AccessToken: str,
         DeviceKey: str,
         DeviceSecretVerifierConfig: DeviceSecretVerifierConfigTypeTypeDef = ...,
         DeviceName: str = ...
-    ) -> ConfirmDeviceResponseOutputTypeDef:
+    ) -> ConfirmDeviceResponseTypeDef:
         """
         Confirms tracking of the device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.confirm_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#confirm_device)
         """
     def confirm_forgot_password(
@@ -591,15 +589,15 @@
         self,
         *,
         GroupName: str,
         UserPoolId: str,
         Description: str = ...,
         RoleArn: str = ...,
         Precedence: int = ...
-    ) -> CreateGroupResponseOutputTypeDef:
+    ) -> CreateGroupResponseTypeDef:
         """
         Creates a new group in the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_group)
         """
     def create_identity_provider(
@@ -607,38 +605,38 @@
         *,
         UserPoolId: str,
         ProviderName: str,
         ProviderType: IdentityProviderTypeTypeType,
         ProviderDetails: Mapping[str, str],
         AttributeMapping: Mapping[str, str] = ...,
         IdpIdentifiers: Sequence[str] = ...
-    ) -> CreateIdentityProviderResponseOutputTypeDef:
+    ) -> CreateIdentityProviderResponseTypeDef:
         """
         Creates an IdP for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_identity_provider)
         """
     def create_resource_server(
         self,
         *,
         UserPoolId: str,
         Identifier: str,
         Name: str,
         Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...
-    ) -> CreateResourceServerResponseOutputTypeDef:
+    ) -> CreateResourceServerResponseTypeDef:
         """
         Creates a new OAuth2.0 resource server and defines custom scopes within it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_resource_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_resource_server)
         """
     def create_user_import_job(
         self, *, JobName: str, UserPoolId: str, CloudWatchLogsRoleArn: str
-    ) -> CreateUserImportJobResponseOutputTypeDef:
+    ) -> CreateUserImportJobResponseTypeDef:
         """
         Creates the user import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_import_job)
         """
     def create_user_pool(
@@ -663,15 +661,15 @@
         SmsConfiguration: SmsConfigurationTypeTypeDef = ...,
         UserPoolTags: Mapping[str, str] = ...,
         AdminCreateUserConfig: AdminCreateUserConfigTypeTypeDef = ...,
         Schema: Sequence[SchemaAttributeTypeTypeDef] = ...,
         UserPoolAddOns: UserPoolAddOnsTypeTypeDef = ...,
         UsernameConfiguration: UsernameConfigurationTypeTypeDef = ...,
         AccountRecoverySetting: AccountRecoverySettingTypeTypeDef = ...
-    ) -> CreateUserPoolResponseOutputTypeDef:
+    ) -> CreateUserPoolResponseTypeDef:
         """
         Creates a new Amazon Cognito user pool and sets the password policy for the
         pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_pool)
         """
@@ -696,28 +694,28 @@
         AllowedOAuthScopes: Sequence[str] = ...,
         AllowedOAuthFlowsUserPoolClient: bool = ...,
         AnalyticsConfiguration: AnalyticsConfigurationTypeTypeDef = ...,
         PreventUserExistenceErrors: PreventUserExistenceErrorTypesType = ...,
         EnableTokenRevocation: bool = ...,
         EnablePropagateAdditionalUserContextData: bool = ...,
         AuthSessionValidity: int = ...
-    ) -> CreateUserPoolClientResponseOutputTypeDef:
+    ) -> CreateUserPoolClientResponseTypeDef:
         """
         Creates the user pool client.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool_client)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_pool_client)
         """
     def create_user_pool_domain(
         self,
         *,
         Domain: str,
         UserPoolId: str,
         CustomDomainConfig: CustomDomainConfigTypeTypeDef = ...
-    ) -> CreateUserPoolDomainResponseOutputTypeDef:
+    ) -> CreateUserPoolDomainResponseTypeDef:
         """
         Creates a new domain for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.create_user_pool_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#create_user_pool_domain)
         """
     def delete_group(self, *, GroupName: str, UserPoolId: str) -> EmptyResponseMetadataTypeDef:
@@ -782,68 +780,66 @@
         Deletes a domain for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.delete_user_pool_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#delete_user_pool_domain)
         """
     def describe_identity_provider(
         self, *, UserPoolId: str, ProviderName: str
-    ) -> DescribeIdentityProviderResponseOutputTypeDef:
+    ) -> DescribeIdentityProviderResponseTypeDef:
         """
         Gets information about a specific IdP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_identity_provider)
         """
     def describe_resource_server(
         self, *, UserPoolId: str, Identifier: str
-    ) -> DescribeResourceServerResponseOutputTypeDef:
+    ) -> DescribeResourceServerResponseTypeDef:
         """
         Describes a resource server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_resource_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_resource_server)
         """
     def describe_risk_configuration(
         self, *, UserPoolId: str, ClientId: str = ...
-    ) -> DescribeRiskConfigurationResponseOutputTypeDef:
+    ) -> DescribeRiskConfigurationResponseTypeDef:
         """
         Describes the risk configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_risk_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_risk_configuration)
         """
     def describe_user_import_job(
         self, *, UserPoolId: str, JobId: str
-    ) -> DescribeUserImportJobResponseOutputTypeDef:
+    ) -> DescribeUserImportJobResponseTypeDef:
         """
         Describes the user import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_user_import_job)
         """
-    def describe_user_pool(self, *, UserPoolId: str) -> DescribeUserPoolResponseOutputTypeDef:
+    def describe_user_pool(self, *, UserPoolId: str) -> DescribeUserPoolResponseTypeDef:
         """
         Returns the configuration information and metadata of the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_pool)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_user_pool)
         """
     def describe_user_pool_client(
         self, *, UserPoolId: str, ClientId: str
-    ) -> DescribeUserPoolClientResponseOutputTypeDef:
+    ) -> DescribeUserPoolClientResponseTypeDef:
         """
         Client method for returning the configuration information and metadata of the
         specified user pool app client.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_pool_client)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_user_pool_client)
         """
-    def describe_user_pool_domain(
-        self, *, Domain: str
-    ) -> DescribeUserPoolDomainResponseOutputTypeDef:
+    def describe_user_pool_domain(self, *, Domain: str) -> DescribeUserPoolDomainResponseTypeDef:
         """
         Gets information about a domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.describe_user_pool_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#describe_user_pool_domain)
         """
     def forget_device(
@@ -860,15 +856,15 @@
         *,
         ClientId: str,
         Username: str,
         SecretHash: str = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> ForgotPasswordResponseOutputTypeDef:
+    ) -> ForgotPasswordResponseTypeDef:
         """
         Calling this API causes a message to be sent to the end user with a confirmation
         code that is required to change the user's password.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.forgot_password)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#forgot_password)
         """
@@ -881,85 +877,79 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#generate_presigned_url)
         """
-    def get_csv_header(self, *, UserPoolId: str) -> GetCSVHeaderResponseOutputTypeDef:
+    def get_csv_header(self, *, UserPoolId: str) -> GetCSVHeaderResponseTypeDef:
         """
         Gets the header information for the comma-separated value (CSV) file to be used
         as input for the user import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_csv_header)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_csv_header)
         """
-    def get_device(
-        self, *, DeviceKey: str, AccessToken: str = ...
-    ) -> GetDeviceResponseOutputTypeDef:
+    def get_device(self, *, DeviceKey: str, AccessToken: str = ...) -> GetDeviceResponseTypeDef:
         """
         Gets the device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_device)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_device)
         """
-    def get_group(self, *, GroupName: str, UserPoolId: str) -> GetGroupResponseOutputTypeDef:
+    def get_group(self, *, GroupName: str, UserPoolId: str) -> GetGroupResponseTypeDef:
         """
         Gets a group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_group)
         """
     def get_identity_provider_by_identifier(
         self, *, UserPoolId: str, IdpIdentifier: str
-    ) -> GetIdentityProviderByIdentifierResponseOutputTypeDef:
+    ) -> GetIdentityProviderByIdentifierResponseTypeDef:
         """
         Gets the specified IdP.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_identity_provider_by_identifier)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_identity_provider_by_identifier)
         """
-    def get_signing_certificate(
-        self, *, UserPoolId: str
-    ) -> GetSigningCertificateResponseOutputTypeDef:
+    def get_signing_certificate(self, *, UserPoolId: str) -> GetSigningCertificateResponseTypeDef:
         """
         This method takes a user pool ID, and returns the signing certificate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_signing_certificate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_signing_certificate)
         """
     def get_ui_customization(
         self, *, UserPoolId: str, ClientId: str = ...
-    ) -> GetUICustomizationResponseOutputTypeDef:
+    ) -> GetUICustomizationResponseTypeDef:
         """
         Gets the user interface (UI) Customization information for a particular app
         client's app UI, if any such information exists for the client.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_ui_customization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_ui_customization)
         """
-    def get_user(self, *, AccessToken: str) -> GetUserResponseOutputTypeDef:
+    def get_user(self, *, AccessToken: str) -> GetUserResponseTypeDef:
         """
         Gets the user attributes and metadata for a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_user)
         """
     def get_user_attribute_verification_code(
         self, *, AccessToken: str, AttributeName: str, ClientMetadata: Mapping[str, str] = ...
-    ) -> GetUserAttributeVerificationCodeResponseOutputTypeDef:
+    ) -> GetUserAttributeVerificationCodeResponseTypeDef:
         """
         Generates a user attribute verification code for the specified attribute name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_user_attribute_verification_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_user_attribute_verification_code)
         """
-    def get_user_pool_mfa_config(
-        self, *, UserPoolId: str
-    ) -> GetUserPoolMfaConfigResponseOutputTypeDef:
+    def get_user_pool_mfa_config(self, *, UserPoolId: str) -> GetUserPoolMfaConfigResponseTypeDef:
         """
         Gets the user pool multi-factor authentication (MFA) configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.get_user_pool_mfa_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#get_user_pool_mfa_config)
         """
     def global_sign_out(self, *, AccessToken: str) -> Dict[str, Any]:
@@ -974,112 +964,110 @@
         *,
         AuthFlow: AuthFlowTypeType,
         ClientId: str,
         AuthParameters: Mapping[str, str] = ...,
         ClientMetadata: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...
-    ) -> InitiateAuthResponseOutputTypeDef:
+    ) -> InitiateAuthResponseTypeDef:
         """
         Initiates sign-in for a user in the Amazon Cognito user directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.initiate_auth)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#initiate_auth)
         """
     def list_devices(
         self, *, AccessToken: str, Limit: int = ..., PaginationToken: str = ...
-    ) -> ListDevicesResponseOutputTypeDef:
+    ) -> ListDevicesResponseTypeDef:
         """
         Lists the sign-in devices that Amazon Cognito has registered to the current
         user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_devices)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_devices)
         """
     def list_groups(
         self, *, UserPoolId: str, Limit: int = ..., NextToken: str = ...
-    ) -> ListGroupsResponseOutputTypeDef:
+    ) -> ListGroupsResponseTypeDef:
         """
         Lists the groups associated with a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_groups)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_groups)
         """
     def list_identity_providers(
         self, *, UserPoolId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListIdentityProvidersResponseOutputTypeDef:
+    ) -> ListIdentityProvidersResponseTypeDef:
         """
         Lists information about all IdPs for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_identity_providers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_identity_providers)
         """
     def list_resource_servers(
         self, *, UserPoolId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListResourceServersResponseOutputTypeDef:
+    ) -> ListResourceServersResponseTypeDef:
         """
         Lists the resource servers for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_resource_servers)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_resource_servers)
         """
-    def list_tags_for_resource(
-        self, *, ResourceArn: str
-    ) -> ListTagsForResourceResponseOutputTypeDef:
+    def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags that are assigned to an Amazon Cognito user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_tags_for_resource)
         """
     def list_user_import_jobs(
         self, *, UserPoolId: str, MaxResults: int, PaginationToken: str = ...
-    ) -> ListUserImportJobsResponseOutputTypeDef:
+    ) -> ListUserImportJobsResponseTypeDef:
         """
         Lists the user import jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_user_import_jobs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_user_import_jobs)
         """
     def list_user_pool_clients(
         self, *, UserPoolId: str, MaxResults: int = ..., NextToken: str = ...
-    ) -> ListUserPoolClientsResponseOutputTypeDef:
+    ) -> ListUserPoolClientsResponseTypeDef:
         """
         Lists the clients that have been created for the specified user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_user_pool_clients)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_user_pool_clients)
         """
     def list_user_pools(
         self, *, MaxResults: int, NextToken: str = ...
-    ) -> ListUserPoolsResponseOutputTypeDef:
+    ) -> ListUserPoolsResponseTypeDef:
         """
         Lists the user pools associated with an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_user_pools)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_user_pools)
         """
     def list_users(
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Limit: int = ...,
         PaginationToken: str = ...,
         Filter: str = ...
-    ) -> ListUsersResponseOutputTypeDef:
+    ) -> ListUsersResponseTypeDef:
         """
         Lists the users in the Amazon Cognito user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_users)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_users)
         """
     def list_users_in_group(
         self, *, UserPoolId: str, GroupName: str, Limit: int = ..., NextToken: str = ...
-    ) -> ListUsersInGroupResponseOutputTypeDef:
+    ) -> ListUsersInGroupResponseTypeDef:
         """
         Lists the users in the specified group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.list_users_in_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#list_users_in_group)
         """
     def resend_confirmation_code(
@@ -1087,15 +1075,15 @@
         *,
         ClientId: str,
         Username: str,
         SecretHash: str = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> ResendConfirmationCodeResponseOutputTypeDef:
+    ) -> ResendConfirmationCodeResponseTypeDef:
         """
         Resends the confirmation (for confirmation of registration) to a specific user
         in the user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.resend_confirmation_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#resend_confirmation_code)
         """
@@ -1105,15 +1093,15 @@
         ClientId: str,
         ChallengeName: ChallengeNameTypeType,
         Session: str = ...,
         ChallengeResponses: Mapping[str, str] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> RespondToAuthChallengeResponseOutputTypeDef:
+    ) -> RespondToAuthChallengeResponseTypeDef:
         """
         Responds to the authentication challenge.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.respond_to_auth_challenge)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#respond_to_auth_challenge)
         """
     def revoke_token(self, *, Token: str, ClientId: str, ClientSecret: str = ...) -> Dict[str, Any]:
@@ -1128,29 +1116,29 @@
         self,
         *,
         UserPoolId: str,
         ClientId: str = ...,
         CompromisedCredentialsRiskConfiguration: CompromisedCredentialsRiskConfigurationTypeTypeDef = ...,
         AccountTakeoverRiskConfiguration: AccountTakeoverRiskConfigurationTypeTypeDef = ...,
         RiskExceptionConfiguration: RiskExceptionConfigurationTypeTypeDef = ...
-    ) -> SetRiskConfigurationResponseOutputTypeDef:
+    ) -> SetRiskConfigurationResponseTypeDef:
         """
         Configures actions on detected risks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_risk_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#set_risk_configuration)
         """
     def set_ui_customization(
         self,
         *,
         UserPoolId: str,
         ClientId: str = ...,
         CSS: str = ...,
         ImageFile: Union[str, bytes, IO[Any], StreamingBody] = ...
-    ) -> SetUICustomizationResponseOutputTypeDef:
+    ) -> SetUICustomizationResponseTypeDef:
         """
         Sets the user interface (UI) customization information for a user pool's built-
         in app UI.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_ui_customization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#set_ui_customization)
         """
@@ -1171,15 +1159,15 @@
     def set_user_pool_mfa_config(
         self,
         *,
         UserPoolId: str,
         SmsMfaConfiguration: SmsMfaConfigTypeTypeDef = ...,
         SoftwareTokenMfaConfiguration: SoftwareTokenMfaConfigTypeTypeDef = ...,
         MfaConfiguration: UserPoolMfaTypeType = ...
-    ) -> SetUserPoolMfaConfigResponseOutputTypeDef:
+    ) -> SetUserPoolMfaConfigResponseTypeDef:
         """
         Sets the user pool multi-factor authentication (MFA) configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.set_user_pool_mfa_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#set_user_pool_mfa_config)
         """
     def set_user_settings(
@@ -1199,34 +1187,34 @@
         Password: str,
         SecretHash: str = ...,
         UserAttributes: Sequence[AttributeTypeTypeDef] = ...,
         ValidationData: Sequence[AttributeTypeTypeDef] = ...,
         AnalyticsMetadata: AnalyticsMetadataTypeTypeDef = ...,
         UserContextData: UserContextDataTypeTypeDef = ...,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> SignUpResponseOutputTypeDef:
+    ) -> SignUpResponseTypeDef:
         """
         Registers the user in the specified user pool and creates a user name, password,
         and user attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.sign_up)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#sign_up)
         """
     def start_user_import_job(
         self, *, UserPoolId: str, JobId: str
-    ) -> StartUserImportJobResponseOutputTypeDef:
+    ) -> StartUserImportJobResponseTypeDef:
         """
         Starts the user import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.start_user_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#start_user_import_job)
         """
     def stop_user_import_job(
         self, *, UserPoolId: str, JobId: str
-    ) -> StopUserImportJobResponseOutputTypeDef:
+    ) -> StopUserImportJobResponseTypeDef:
         """
         Stops the user import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.stop_user_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#stop_user_import_job)
         """
     def tag_resource(self, *, ResourceArn: str, Tags: Mapping[str, str]) -> Dict[str, Any]:
@@ -1276,57 +1264,57 @@
         self,
         *,
         GroupName: str,
         UserPoolId: str,
         Description: str = ...,
         RoleArn: str = ...,
         Precedence: int = ...
-    ) -> UpdateGroupResponseOutputTypeDef:
+    ) -> UpdateGroupResponseTypeDef:
         """
         Updates the specified group with the specified attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_group)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_group)
         """
     def update_identity_provider(
         self,
         *,
         UserPoolId: str,
         ProviderName: str,
         ProviderDetails: Mapping[str, str] = ...,
         AttributeMapping: Mapping[str, str] = ...,
         IdpIdentifiers: Sequence[str] = ...
-    ) -> UpdateIdentityProviderResponseOutputTypeDef:
+    ) -> UpdateIdentityProviderResponseTypeDef:
         """
         Updates IdP information for a user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_identity_provider)
         """
     def update_resource_server(
         self,
         *,
         UserPoolId: str,
         Identifier: str,
         Name: str,
         Scopes: Sequence[ResourceServerScopeTypeTypeDef] = ...
-    ) -> UpdateResourceServerResponseOutputTypeDef:
+    ) -> UpdateResourceServerResponseTypeDef:
         """
         Updates the name and scopes of resource server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_resource_server)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_resource_server)
         """
     def update_user_attributes(
         self,
         *,
         UserAttributes: Sequence[AttributeTypeTypeDef],
         AccessToken: str,
         ClientMetadata: Mapping[str, str] = ...
-    ) -> UpdateUserAttributesResponseOutputTypeDef:
+    ) -> UpdateUserAttributesResponseTypeDef:
         """
         Allows a user to update a specific attribute (one at a time).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_user_attributes)
         """
     def update_user_pool(
@@ -1379,39 +1367,39 @@
         AllowedOAuthScopes: Sequence[str] = ...,
         AllowedOAuthFlowsUserPoolClient: bool = ...,
         AnalyticsConfiguration: AnalyticsConfigurationTypeTypeDef = ...,
         PreventUserExistenceErrors: PreventUserExistenceErrorTypesType = ...,
         EnableTokenRevocation: bool = ...,
         EnablePropagateAdditionalUserContextData: bool = ...,
         AuthSessionValidity: int = ...
-    ) -> UpdateUserPoolClientResponseOutputTypeDef:
+    ) -> UpdateUserPoolClientResponseTypeDef:
         """
         Updates the specified user pool app client with the specified attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool_client)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_user_pool_client)
         """
     def update_user_pool_domain(
         self, *, Domain: str, UserPoolId: str, CustomDomainConfig: CustomDomainConfigTypeTypeDef
-    ) -> UpdateUserPoolDomainResponseOutputTypeDef:
+    ) -> UpdateUserPoolDomainResponseTypeDef:
         """
         Updates the Secure Sockets Layer (SSL) certificate for the custom domain for
         your user pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.update_user_pool_domain)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#update_user_pool_domain)
         """
     def verify_software_token(
         self,
         *,
         UserCode: str,
         AccessToken: str = ...,
         Session: str = ...,
         FriendlyDeviceName: str = ...
-    ) -> VerifySoftwareTokenResponseOutputTypeDef:
+    ) -> VerifySoftwareTokenResponseTypeDef:
         """
         Use this API to register a user's entered time-based one-time password (TOTP)
         code and mark the user's software token MFA status as "verified" if successful.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Client.verify_software_token)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/client/#verify_software_token)
         """
```

### Comparing `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/literals.py` & `mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/literals.pyi` & `mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/paginator.py` & `mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,23 +36,23 @@
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    AdminListGroupsForUserResponseOutputTypeDef,
-    AdminListUserAuthEventsResponseOutputTypeDef,
-    ListGroupsResponseOutputTypeDef,
-    ListIdentityProvidersResponseOutputTypeDef,
-    ListResourceServersResponseOutputTypeDef,
-    ListUserPoolClientsResponseOutputTypeDef,
-    ListUserPoolsResponseOutputTypeDef,
-    ListUsersInGroupResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
+    AdminListGroupsForUserResponseTypeDef,
+    AdminListUserAuthEventsResponseTypeDef,
+    ListGroupsResponseTypeDef,
+    ListIdentityProvidersResponseTypeDef,
+    ListResourceServersResponseTypeDef,
+    ListUserPoolClientsResponseTypeDef,
+    ListUserPoolsResponseTypeDef,
+    ListUsersInGroupResponseTypeDef,
+    ListUsersResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "AdminListGroupsForUserPaginator",
     "AdminListUserAuthEventsPaginator",
     "ListGroupsPaginator",
@@ -79,105 +79,105 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
     """
 
     def paginate(
         self, *, Username: str, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[AdminListGroupsForUserResponseOutputTypeDef]:
+    ) -> _PageIterator[AdminListGroupsForUserResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
         """
 
 
 class AdminListUserAuthEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistuserautheventspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, Username: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[AdminListUserAuthEventsResponseOutputTypeDef]:
+    ) -> _PageIterator[AdminListUserAuthEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistuserautheventspaginator)
         """
 
 
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListGroupsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listgroupspaginator)
         """
 
 
 class ListIdentityProvidersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listidentityproviderspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListIdentityProvidersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListIdentityProvidersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listidentityproviderspaginator)
         """
 
 
 class ListResourceServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listresourceserverspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListResourceServersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListResourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listresourceserverspaginator)
         """
 
 
 class ListUserPoolClientsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolclientspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListUserPoolClientsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUserPoolClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolclientspaginator)
         """
 
 
 class ListUserPoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListUserPoolsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUserPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolspaginator)
         """
 
 
 class ListUsersPaginator(Paginator):
@@ -189,27 +189,27 @@
     def paginate(
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Filter: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListUsersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserspaginator)
         """
 
 
 class ListUsersInGroupPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listusersingrouppaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, GroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListUsersInGroupResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUsersInGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listusersingrouppaginator)
         """
```

### Comparing `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/paginator.pyi` & `mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/paginator.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -36,23 +36,23 @@
     ```
 """
 from typing import Generic, Iterator, Sequence, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
-    AdminListGroupsForUserResponseOutputTypeDef,
-    AdminListUserAuthEventsResponseOutputTypeDef,
-    ListGroupsResponseOutputTypeDef,
-    ListIdentityProvidersResponseOutputTypeDef,
-    ListResourceServersResponseOutputTypeDef,
-    ListUserPoolClientsResponseOutputTypeDef,
-    ListUserPoolsResponseOutputTypeDef,
-    ListUsersInGroupResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
+    AdminListGroupsForUserResponseTypeDef,
+    AdminListUserAuthEventsResponseTypeDef,
+    ListGroupsResponseTypeDef,
+    ListIdentityProvidersResponseTypeDef,
+    ListResourceServersResponseTypeDef,
+    ListUserPoolClientsResponseTypeDef,
+    ListUserPoolsResponseTypeDef,
+    ListUsersInGroupResponseTypeDef,
+    ListUsersResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "AdminListGroupsForUserPaginator",
     "AdminListUserAuthEventsPaginator",
     "ListGroupsPaginator",
@@ -76,99 +76,99 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
     """
 
     def paginate(
         self, *, Username: str, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[AdminListGroupsForUserResponseOutputTypeDef]:
+    ) -> _PageIterator[AdminListGroupsForUserResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
         """
 
 class AdminListUserAuthEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistuserautheventspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, Username: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[AdminListUserAuthEventsResponseOutputTypeDef]:
+    ) -> _PageIterator[AdminListUserAuthEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistuserautheventspaginator)
         """
 
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListGroupsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listgroupspaginator)
         """
 
 class ListIdentityProvidersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listidentityproviderspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListIdentityProvidersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListIdentityProvidersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listidentityproviderspaginator)
         """
 
 class ListResourceServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listresourceserverspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListResourceServersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListResourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listresourceserverspaginator)
         """
 
 class ListUserPoolClientsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolclientspaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListUserPoolClientsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUserPoolClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolclientspaginator)
         """
 
 class ListUserPoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListUserPoolsResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUserPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolspaginator)
         """
 
 class ListUsersPaginator(Paginator):
     """
@@ -179,26 +179,26 @@
     def paginate(
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Filter: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListUsersResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserspaginator)
         """
 
 class ListUsersInGroupPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listusersingrouppaginator)
     """
 
     def paginate(
         self, *, UserPoolId: str, GroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListUsersInGroupResponseOutputTypeDef]:
+    ) -> _PageIterator[ListUsersInGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listusersingrouppaginator)
         """
```

### Comparing `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/type_defs.py` & `mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -86,46 +86,46 @@
     "AdminGetUserRequestRequestTypeDef",
     "AttributeTypeOutputTypeDef",
     "MFAOptionTypeOutputTypeDef",
     "AnalyticsMetadataTypeTypeDef",
     "AdminListDevicesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "AdminListGroupsForUserRequestRequestTypeDef",
-    "GroupTypeOutputTypeDef",
+    "GroupTypeTypeDef",
     "AdminListUserAuthEventsRequestRequestTypeDef",
     "AdminRemoveUserFromGroupRequestRequestTypeDef",
     "AdminResetUserPasswordRequestRequestTypeDef",
     "SMSMfaSettingsTypeTypeDef",
     "SoftwareTokenMfaSettingsTypeTypeDef",
     "AdminSetUserPasswordRequestRequestTypeDef",
     "MFAOptionTypeTypeDef",
     "AdminUpdateAuthEventFeedbackRequestRequestTypeDef",
     "AdminUpdateDeviceStatusRequestRequestTypeDef",
     "AdminUserGlobalSignOutRequestRequestTypeDef",
     "AnalyticsConfigurationTypeOutputTypeDef",
     "AnalyticsConfigurationTypeTypeDef",
     "AssociateSoftwareTokenRequestRequestTypeDef",
-    "ChallengeResponseTypeOutputTypeDef",
-    "EventContextDataTypeOutputTypeDef",
-    "EventFeedbackTypeOutputTypeDef",
-    "EventRiskTypeOutputTypeDef",
-    "NewDeviceMetadataTypeOutputTypeDef",
+    "ChallengeResponseTypeTypeDef",
+    "EventContextDataTypeTypeDef",
+    "EventFeedbackTypeTypeDef",
+    "EventRiskTypeTypeDef",
+    "NewDeviceMetadataTypeTypeDef",
     "ChangePasswordRequestRequestTypeDef",
-    "CodeDeliveryDetailsTypeOutputTypeDef",
+    "CodeDeliveryDetailsTypeTypeDef",
     "CompromisedCredentialsActionsTypeOutputTypeDef",
     "CompromisedCredentialsActionsTypeTypeDef",
     "DeviceSecretVerifierConfigTypeTypeDef",
     "UserContextDataTypeTypeDef",
     "HttpHeaderTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
-    "IdentityProviderTypeOutputTypeDef",
+    "IdentityProviderTypeTypeDef",
     "ResourceServerScopeTypeTypeDef",
     "CreateUserImportJobRequestRequestTypeDef",
-    "UserImportJobTypeOutputTypeDef",
+    "UserImportJobTypeTypeDef",
     "TokenValidityUnitsTypeTypeDef",
     "CustomDomainConfigTypeTypeDef",
     "DeviceConfigurationTypeTypeDef",
     "EmailConfigurationTypeTypeDef",
     "SmsConfigurationTypeTypeDef",
     "UserAttributeUpdateSettingsTypeTypeDef",
     "UserPoolAddOnsTypeTypeDef",
@@ -156,29 +156,29 @@
     "ForgetDeviceRequestRequestTypeDef",
     "GetCSVHeaderRequestRequestTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GetIdentityProviderByIdentifierRequestRequestTypeDef",
     "GetSigningCertificateRequestRequestTypeDef",
     "GetUICustomizationRequestRequestTypeDef",
-    "UICustomizationTypeOutputTypeDef",
+    "UICustomizationTypeTypeDef",
     "GetUserAttributeVerificationCodeRequestRequestTypeDef",
     "GetUserPoolMfaConfigRequestRequestTypeDef",
     "SoftwareTokenMfaConfigTypeOutputTypeDef",
     "GetUserRequestRequestTypeDef",
     "GlobalSignOutRequestRequestTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
-    "ProviderDescriptionOutputTypeDef",
+    "ProviderDescriptionTypeDef",
     "ListResourceServersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListUserImportJobsRequestRequestTypeDef",
     "ListUserPoolClientsRequestRequestTypeDef",
-    "UserPoolClientDescriptionOutputTypeDef",
+    "UserPoolClientDescriptionTypeDef",
     "ListUserPoolsRequestRequestTypeDef",
     "ListUsersInGroupRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "NotifyEmailTypeOutputTypeDef",
     "NotifyEmailTypeTypeDef",
     "NumberAttributeConstraintsTypeOutputTypeDef",
     "NumberAttributeConstraintsTypeTypeDef",
@@ -213,136 +213,136 @@
     "AccountTakeoverActionsTypeOutputTypeDef",
     "AccountTakeoverActionsTypeTypeDef",
     "AdminCreateUserConfigTypeOutputTypeDef",
     "AdminCreateUserConfigTypeTypeDef",
     "AdminCreateUserRequestRequestTypeDef",
     "AdminUpdateUserAttributesRequestRequestTypeDef",
     "UpdateUserAttributesRequestRequestTypeDef",
-    "AssociateSoftwareTokenResponseOutputTypeDef",
-    "ConfirmDeviceResponseOutputTypeDef",
-    "CreateUserPoolDomainResponseOutputTypeDef",
+    "AssociateSoftwareTokenResponseTypeDef",
+    "ConfirmDeviceResponseTypeDef",
+    "CreateUserPoolDomainResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "GetCSVHeaderResponseOutputTypeDef",
-    "GetSigningCertificateResponseOutputTypeDef",
-    "ListTagsForResourceResponseOutputTypeDef",
-    "UpdateUserPoolDomainResponseOutputTypeDef",
-    "VerifySoftwareTokenResponseOutputTypeDef",
+    "GetCSVHeaderResponseTypeDef",
+    "GetSigningCertificateResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateUserPoolDomainResponseTypeDef",
+    "VerifySoftwareTokenResponseTypeDef",
     "AdminDisableProviderForUserRequestRequestTypeDef",
     "AdminLinkProviderForUserRequestRequestTypeDef",
-    "DeviceTypeOutputTypeDef",
-    "AdminGetUserResponseOutputTypeDef",
-    "GetUserResponseOutputTypeDef",
-    "UserTypeOutputTypeDef",
+    "DeviceTypeTypeDef",
+    "AdminGetUserResponseTypeDef",
+    "GetUserResponseTypeDef",
+    "UserTypeTypeDef",
     "AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
     "AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListResourceServersRequestListResourceServersPaginateTypeDef",
     "ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
     "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
     "ListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
-    "AdminListGroupsForUserResponseOutputTypeDef",
-    "CreateGroupResponseOutputTypeDef",
-    "GetGroupResponseOutputTypeDef",
-    "ListGroupsResponseOutputTypeDef",
-    "UpdateGroupResponseOutputTypeDef",
+    "AdminListGroupsForUserResponseTypeDef",
+    "CreateGroupResponseTypeDef",
+    "GetGroupResponseTypeDef",
+    "ListGroupsResponseTypeDef",
+    "UpdateGroupResponseTypeDef",
     "AdminSetUserMFAPreferenceRequestRequestTypeDef",
     "SetUserMFAPreferenceRequestRequestTypeDef",
     "AdminSetUserSettingsRequestRequestTypeDef",
     "SetUserSettingsRequestRequestTypeDef",
-    "AuthEventTypeOutputTypeDef",
-    "AuthenticationResultTypeOutputTypeDef",
-    "ForgotPasswordResponseOutputTypeDef",
-    "GetUserAttributeVerificationCodeResponseOutputTypeDef",
-    "ResendConfirmationCodeResponseOutputTypeDef",
-    "SignUpResponseOutputTypeDef",
-    "UpdateUserAttributesResponseOutputTypeDef",
+    "AuthEventTypeTypeDef",
+    "AuthenticationResultTypeTypeDef",
+    "ForgotPasswordResponseTypeDef",
+    "GetUserAttributeVerificationCodeResponseTypeDef",
+    "ResendConfirmationCodeResponseTypeDef",
+    "SignUpResponseTypeDef",
+    "UpdateUserAttributesResponseTypeDef",
     "CompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
     "CompromisedCredentialsRiskConfigurationTypeTypeDef",
     "ConfirmDeviceRequestRequestTypeDef",
     "ConfirmForgotPasswordRequestRequestTypeDef",
     "ConfirmSignUpRequestRequestTypeDef",
     "ForgotPasswordRequestRequestTypeDef",
     "InitiateAuthRequestRequestTypeDef",
     "ResendConfirmationCodeRequestRequestTypeDef",
     "RespondToAuthChallengeRequestRequestTypeDef",
     "SignUpRequestRequestTypeDef",
     "ContextDataTypeTypeDef",
-    "CreateIdentityProviderResponseOutputTypeDef",
-    "DescribeIdentityProviderResponseOutputTypeDef",
-    "GetIdentityProviderByIdentifierResponseOutputTypeDef",
-    "UpdateIdentityProviderResponseOutputTypeDef",
+    "CreateIdentityProviderResponseTypeDef",
+    "DescribeIdentityProviderResponseTypeDef",
+    "GetIdentityProviderByIdentifierResponseTypeDef",
+    "UpdateIdentityProviderResponseTypeDef",
     "CreateResourceServerRequestRequestTypeDef",
     "UpdateResourceServerRequestRequestTypeDef",
-    "CreateUserImportJobResponseOutputTypeDef",
-    "DescribeUserImportJobResponseOutputTypeDef",
-    "ListUserImportJobsResponseOutputTypeDef",
-    "StartUserImportJobResponseOutputTypeDef",
-    "StopUserImportJobResponseOutputTypeDef",
+    "CreateUserImportJobResponseTypeDef",
+    "DescribeUserImportJobResponseTypeDef",
+    "ListUserImportJobsResponseTypeDef",
+    "StartUserImportJobResponseTypeDef",
+    "StopUserImportJobResponseTypeDef",
     "CreateUserPoolClientRequestRequestTypeDef",
     "UpdateUserPoolClientRequestRequestTypeDef",
     "CreateUserPoolDomainRequestRequestTypeDef",
     "UpdateUserPoolDomainRequestRequestTypeDef",
     "SmsMfaConfigTypeTypeDef",
-    "DomainDescriptionTypeOutputTypeDef",
+    "DomainDescriptionTypeTypeDef",
     "LambdaConfigTypeOutputTypeDef",
     "LambdaConfigTypeTypeDef",
-    "GetUICustomizationResponseOutputTypeDef",
-    "SetUICustomizationResponseOutputTypeDef",
-    "ListIdentityProvidersResponseOutputTypeDef",
-    "ListUserPoolClientsResponseOutputTypeDef",
+    "GetUICustomizationResponseTypeDef",
+    "SetUICustomizationResponseTypeDef",
+    "ListIdentityProvidersResponseTypeDef",
+    "ListUserPoolClientsResponseTypeDef",
     "NotifyConfigurationTypeOutputTypeDef",
     "NotifyConfigurationTypeTypeDef",
     "UserPoolPolicyTypeOutputTypeDef",
     "UserPoolPolicyTypeTypeDef",
-    "ResourceServerTypeOutputTypeDef",
+    "ResourceServerTypeTypeDef",
     "SchemaAttributeTypeOutputTypeDef",
     "SchemaAttributeTypeTypeDef",
     "SmsMfaConfigTypeOutputTypeDef",
-    "UserPoolClientTypeOutputTypeDef",
-    "AdminGetDeviceResponseOutputTypeDef",
-    "AdminListDevicesResponseOutputTypeDef",
-    "GetDeviceResponseOutputTypeDef",
-    "ListDevicesResponseOutputTypeDef",
-    "AdminCreateUserResponseOutputTypeDef",
-    "ListUsersInGroupResponseOutputTypeDef",
-    "ListUsersResponseOutputTypeDef",
-    "AdminListUserAuthEventsResponseOutputTypeDef",
-    "AdminInitiateAuthResponseOutputTypeDef",
-    "AdminRespondToAuthChallengeResponseOutputTypeDef",
-    "InitiateAuthResponseOutputTypeDef",
-    "RespondToAuthChallengeResponseOutputTypeDef",
+    "UserPoolClientTypeTypeDef",
+    "AdminGetDeviceResponseTypeDef",
+    "AdminListDevicesResponseTypeDef",
+    "GetDeviceResponseTypeDef",
+    "ListDevicesResponseTypeDef",
+    "AdminCreateUserResponseTypeDef",
+    "ListUsersInGroupResponseTypeDef",
+    "ListUsersResponseTypeDef",
+    "AdminListUserAuthEventsResponseTypeDef",
+    "AdminInitiateAuthResponseTypeDef",
+    "AdminRespondToAuthChallengeResponseTypeDef",
+    "InitiateAuthResponseTypeDef",
+    "RespondToAuthChallengeResponseTypeDef",
     "AdminInitiateAuthRequestRequestTypeDef",
     "AdminRespondToAuthChallengeRequestRequestTypeDef",
     "SetUserPoolMfaConfigRequestRequestTypeDef",
-    "DescribeUserPoolDomainResponseOutputTypeDef",
-    "UserPoolDescriptionTypeOutputTypeDef",
+    "DescribeUserPoolDomainResponseTypeDef",
+    "UserPoolDescriptionTypeTypeDef",
     "AccountTakeoverRiskConfigurationTypeOutputTypeDef",
     "AccountTakeoverRiskConfigurationTypeTypeDef",
     "UpdateUserPoolRequestRequestTypeDef",
-    "CreateResourceServerResponseOutputTypeDef",
-    "DescribeResourceServerResponseOutputTypeDef",
-    "ListResourceServersResponseOutputTypeDef",
-    "UpdateResourceServerResponseOutputTypeDef",
-    "UserPoolTypeOutputTypeDef",
+    "CreateResourceServerResponseTypeDef",
+    "DescribeResourceServerResponseTypeDef",
+    "ListResourceServersResponseTypeDef",
+    "UpdateResourceServerResponseTypeDef",
+    "UserPoolTypeTypeDef",
     "AddCustomAttributesRequestRequestTypeDef",
     "CreateUserPoolRequestRequestTypeDef",
-    "GetUserPoolMfaConfigResponseOutputTypeDef",
-    "SetUserPoolMfaConfigResponseOutputTypeDef",
-    "CreateUserPoolClientResponseOutputTypeDef",
-    "DescribeUserPoolClientResponseOutputTypeDef",
-    "UpdateUserPoolClientResponseOutputTypeDef",
-    "ListUserPoolsResponseOutputTypeDef",
-    "RiskConfigurationTypeOutputTypeDef",
+    "GetUserPoolMfaConfigResponseTypeDef",
+    "SetUserPoolMfaConfigResponseTypeDef",
+    "CreateUserPoolClientResponseTypeDef",
+    "DescribeUserPoolClientResponseTypeDef",
+    "UpdateUserPoolClientResponseTypeDef",
+    "ListUserPoolsResponseTypeDef",
+    "RiskConfigurationTypeTypeDef",
     "SetRiskConfigurationRequestRequestTypeDef",
-    "CreateUserPoolResponseOutputTypeDef",
-    "DescribeUserPoolResponseOutputTypeDef",
-    "DescribeRiskConfigurationResponseOutputTypeDef",
-    "SetRiskConfigurationResponseOutputTypeDef",
+    "CreateUserPoolResponseTypeDef",
+    "DescribeUserPoolResponseTypeDef",
+    "DescribeRiskConfigurationResponseTypeDef",
+    "SetRiskConfigurationResponseTypeDef",
 )
 
 RecoveryOptionTypeOutputTypeDef = TypedDict(
     "RecoveryOptionTypeOutputTypeDef",
     {
         "Priority": int,
         "Name": RecoveryOptionNameTypeType,
@@ -600,16 +600,16 @@
 class AdminListGroupsForUserRequestRequestTypeDef(
     _RequiredAdminListGroupsForUserRequestRequestTypeDef,
     _OptionalAdminListGroupsForUserRequestRequestTypeDef,
 ):
     pass
 
 
-GroupTypeOutputTypeDef = TypedDict(
-    "GroupTypeOutputTypeDef",
+GroupTypeTypeDef = TypedDict(
+    "GroupTypeTypeDef",
     {
         "GroupName": str,
         "UserPoolId": str,
         "Description": str,
         "RoleArn": str,
         "Precedence": int,
         "LastModifiedDate": datetime,
@@ -794,53 +794,53 @@
     {
         "AccessToken": str,
         "Session": str,
     },
     total=False,
 )
 
-ChallengeResponseTypeOutputTypeDef = TypedDict(
-    "ChallengeResponseTypeOutputTypeDef",
+ChallengeResponseTypeTypeDef = TypedDict(
+    "ChallengeResponseTypeTypeDef",
     {
         "ChallengeName": ChallengeNameType,
         "ChallengeResponse": ChallengeResponseType,
     },
 )
 
-EventContextDataTypeOutputTypeDef = TypedDict(
-    "EventContextDataTypeOutputTypeDef",
+EventContextDataTypeTypeDef = TypedDict(
+    "EventContextDataTypeTypeDef",
     {
         "IpAddress": str,
         "DeviceName": str,
         "Timezone": str,
         "City": str,
         "Country": str,
     },
 )
 
-EventFeedbackTypeOutputTypeDef = TypedDict(
-    "EventFeedbackTypeOutputTypeDef",
+EventFeedbackTypeTypeDef = TypedDict(
+    "EventFeedbackTypeTypeDef",
     {
         "FeedbackValue": FeedbackValueTypeType,
         "Provider": str,
         "FeedbackDate": datetime,
     },
 )
 
-EventRiskTypeOutputTypeDef = TypedDict(
-    "EventRiskTypeOutputTypeDef",
+EventRiskTypeTypeDef = TypedDict(
+    "EventRiskTypeTypeDef",
     {
         "RiskDecision": RiskDecisionTypeType,
         "RiskLevel": RiskLevelTypeType,
         "CompromisedCredentialsDetected": bool,
     },
 )
 
-NewDeviceMetadataTypeOutputTypeDef = TypedDict(
-    "NewDeviceMetadataTypeOutputTypeDef",
+NewDeviceMetadataTypeTypeDef = TypedDict(
+    "NewDeviceMetadataTypeTypeDef",
     {
         "DeviceKey": str,
         "DeviceGroupKey": str,
     },
 )
 
 ChangePasswordRequestRequestTypeDef = TypedDict(
@@ -848,16 +848,16 @@
     {
         "PreviousPassword": str,
         "ProposedPassword": str,
         "AccessToken": str,
     },
 )
 
-CodeDeliveryDetailsTypeOutputTypeDef = TypedDict(
-    "CodeDeliveryDetailsTypeOutputTypeDef",
+CodeDeliveryDetailsTypeTypeDef = TypedDict(
+    "CodeDeliveryDetailsTypeTypeDef",
     {
         "Destination": str,
         "DeliveryMedium": DeliveryMediumTypeType,
         "AttributeName": str,
     },
 )
 
@@ -948,16 +948,16 @@
 class CreateIdentityProviderRequestRequestTypeDef(
     _RequiredCreateIdentityProviderRequestRequestTypeDef,
     _OptionalCreateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
 
-IdentityProviderTypeOutputTypeDef = TypedDict(
-    "IdentityProviderTypeOutputTypeDef",
+IdentityProviderTypeTypeDef = TypedDict(
+    "IdentityProviderTypeTypeDef",
     {
         "UserPoolId": str,
         "ProviderName": str,
         "ProviderType": IdentityProviderTypeTypeType,
         "ProviderDetails": Dict[str, str],
         "AttributeMapping": Dict[str, str],
         "IdpIdentifiers": List[str],
@@ -979,16 +979,16 @@
     {
         "JobName": str,
         "UserPoolId": str,
         "CloudWatchLogsRoleArn": str,
     },
 )
 
-UserImportJobTypeOutputTypeDef = TypedDict(
-    "UserImportJobTypeOutputTypeDef",
+UserImportJobTypeTypeDef = TypedDict(
+    "UserImportJobTypeTypeDef",
     {
         "JobName": str,
         "JobId": str,
         "UserPoolId": str,
         "PreSignedUrl": str,
         "CreationDate": datetime,
         "StartDate": datetime,
@@ -1375,16 +1375,16 @@
 class GetUICustomizationRequestRequestTypeDef(
     _RequiredGetUICustomizationRequestRequestTypeDef,
     _OptionalGetUICustomizationRequestRequestTypeDef,
 ):
     pass
 
 
-UICustomizationTypeOutputTypeDef = TypedDict(
-    "UICustomizationTypeOutputTypeDef",
+UICustomizationTypeTypeDef = TypedDict(
+    "UICustomizationTypeTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "ImageUrl": str,
         "CSS": str,
         "CSSVersion": str,
         "LastModifiedDate": datetime,
@@ -1506,16 +1506,16 @@
 class ListIdentityProvidersRequestRequestTypeDef(
     _RequiredListIdentityProvidersRequestRequestTypeDef,
     _OptionalListIdentityProvidersRequestRequestTypeDef,
 ):
     pass
 
 
-ProviderDescriptionOutputTypeDef = TypedDict(
-    "ProviderDescriptionOutputTypeDef",
+ProviderDescriptionTypeDef = TypedDict(
+    "ProviderDescriptionTypeDef",
     {
         "ProviderName": str,
         "ProviderType": IdentityProviderTypeTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
 )
@@ -1592,16 +1592,16 @@
 class ListUserPoolClientsRequestRequestTypeDef(
     _RequiredListUserPoolClientsRequestRequestTypeDef,
     _OptionalListUserPoolClientsRequestRequestTypeDef,
 ):
     pass
 
 
-UserPoolClientDescriptionOutputTypeDef = TypedDict(
-    "UserPoolClientDescriptionOutputTypeDef",
+UserPoolClientDescriptionTypeDef = TypedDict(
+    "UserPoolClientDescriptionTypeDef",
     {
         "ClientId": str,
         "UserPoolId": str,
         "ClientName": str,
     },
 )
 
@@ -2163,81 +2163,81 @@
 class UpdateUserAttributesRequestRequestTypeDef(
     _RequiredUpdateUserAttributesRequestRequestTypeDef,
     _OptionalUpdateUserAttributesRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateSoftwareTokenResponseOutputTypeDef = TypedDict(
-    "AssociateSoftwareTokenResponseOutputTypeDef",
+AssociateSoftwareTokenResponseTypeDef = TypedDict(
+    "AssociateSoftwareTokenResponseTypeDef",
     {
         "SecretCode": str,
         "Session": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfirmDeviceResponseOutputTypeDef = TypedDict(
-    "ConfirmDeviceResponseOutputTypeDef",
+ConfirmDeviceResponseTypeDef = TypedDict(
+    "ConfirmDeviceResponseTypeDef",
     {
         "UserConfirmationNecessary": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateUserPoolDomainResponseOutputTypeDef = TypedDict(
-    "CreateUserPoolDomainResponseOutputTypeDef",
+CreateUserPoolDomainResponseTypeDef = TypedDict(
+    "CreateUserPoolDomainResponseTypeDef",
     {
         "CloudFrontDomain": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetCSVHeaderResponseOutputTypeDef = TypedDict(
-    "GetCSVHeaderResponseOutputTypeDef",
+GetCSVHeaderResponseTypeDef = TypedDict(
+    "GetCSVHeaderResponseTypeDef",
     {
         "UserPoolId": str,
         "CSVHeader": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetSigningCertificateResponseOutputTypeDef = TypedDict(
-    "GetSigningCertificateResponseOutputTypeDef",
+GetSigningCertificateResponseTypeDef = TypedDict(
+    "GetSigningCertificateResponseTypeDef",
     {
         "Certificate": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseOutputTypeDef = TypedDict(
-    "ListTagsForResourceResponseOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateUserPoolDomainResponseOutputTypeDef = TypedDict(
-    "UpdateUserPoolDomainResponseOutputTypeDef",
+UpdateUserPoolDomainResponseTypeDef = TypedDict(
+    "UpdateUserPoolDomainResponseTypeDef",
     {
         "CloudFrontDomain": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VerifySoftwareTokenResponseOutputTypeDef = TypedDict(
-    "VerifySoftwareTokenResponseOutputTypeDef",
+VerifySoftwareTokenResponseTypeDef = TypedDict(
+    "VerifySoftwareTokenResponseTypeDef",
     {
         "Status": VerifySoftwareTokenResponseTypeType,
         "Session": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -2254,55 +2254,55 @@
     {
         "UserPoolId": str,
         "DestinationUser": ProviderUserIdentifierTypeTypeDef,
         "SourceUser": ProviderUserIdentifierTypeTypeDef,
     },
 )
 
-DeviceTypeOutputTypeDef = TypedDict(
-    "DeviceTypeOutputTypeDef",
+DeviceTypeTypeDef = TypedDict(
+    "DeviceTypeTypeDef",
     {
         "DeviceKey": str,
         "DeviceAttributes": List[AttributeTypeOutputTypeDef],
         "DeviceCreateDate": datetime,
         "DeviceLastModifiedDate": datetime,
         "DeviceLastAuthenticatedDate": datetime,
     },
 )
 
-AdminGetUserResponseOutputTypeDef = TypedDict(
-    "AdminGetUserResponseOutputTypeDef",
+AdminGetUserResponseTypeDef = TypedDict(
+    "AdminGetUserResponseTypeDef",
     {
         "Username": str,
         "UserAttributes": List[AttributeTypeOutputTypeDef],
         "UserCreateDate": datetime,
         "UserLastModifiedDate": datetime,
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
         "MFAOptions": List[MFAOptionTypeOutputTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetUserResponseOutputTypeDef = TypedDict(
-    "GetUserResponseOutputTypeDef",
+GetUserResponseTypeDef = TypedDict(
+    "GetUserResponseTypeDef",
     {
         "Username": str,
         "UserAttributes": List[AttributeTypeOutputTypeDef],
         "MFAOptions": List[MFAOptionTypeOutputTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UserTypeOutputTypeDef = TypedDict(
-    "UserTypeOutputTypeDef",
+UserTypeTypeDef = TypedDict(
+    "UserTypeTypeDef",
     {
         "Username": str,
         "Attributes": List[AttributeTypeOutputTypeDef],
         "UserCreateDate": datetime,
         "UserLastModifiedDate": datetime,
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
@@ -2495,52 +2495,52 @@
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
 
-AdminListGroupsForUserResponseOutputTypeDef = TypedDict(
-    "AdminListGroupsForUserResponseOutputTypeDef",
+AdminListGroupsForUserResponseTypeDef = TypedDict(
+    "AdminListGroupsForUserResponseTypeDef",
     {
-        "Groups": List[GroupTypeOutputTypeDef],
+        "Groups": List[GroupTypeTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateGroupResponseOutputTypeDef = TypedDict(
-    "CreateGroupResponseOutputTypeDef",
+CreateGroupResponseTypeDef = TypedDict(
+    "CreateGroupResponseTypeDef",
     {
-        "Group": GroupTypeOutputTypeDef,
+        "Group": GroupTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetGroupResponseOutputTypeDef = TypedDict(
-    "GetGroupResponseOutputTypeDef",
+GetGroupResponseTypeDef = TypedDict(
+    "GetGroupResponseTypeDef",
     {
-        "Group": GroupTypeOutputTypeDef,
+        "Group": GroupTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListGroupsResponseOutputTypeDef = TypedDict(
-    "ListGroupsResponseOutputTypeDef",
+ListGroupsResponseTypeDef = TypedDict(
+    "ListGroupsResponseTypeDef",
     {
-        "Groups": List[GroupTypeOutputTypeDef],
+        "Groups": List[GroupTypeTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateGroupResponseOutputTypeDef = TypedDict(
-    "UpdateGroupResponseOutputTypeDef",
+UpdateGroupResponseTypeDef = TypedDict(
+    "UpdateGroupResponseTypeDef",
     {
-        "Group": GroupTypeOutputTypeDef,
+        "Group": GroupTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef = TypedDict(
     "_RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef",
     {
@@ -2601,78 +2601,78 @@
     "SetUserSettingsRequestRequestTypeDef",
     {
         "AccessToken": str,
         "MFAOptions": Sequence[MFAOptionTypeTypeDef],
     },
 )
 
-AuthEventTypeOutputTypeDef = TypedDict(
-    "AuthEventTypeOutputTypeDef",
+AuthEventTypeTypeDef = TypedDict(
+    "AuthEventTypeTypeDef",
     {
         "EventId": str,
         "EventType": EventTypeType,
         "CreationDate": datetime,
         "EventResponse": EventResponseTypeType,
-        "EventRisk": EventRiskTypeOutputTypeDef,
-        "ChallengeResponses": List[ChallengeResponseTypeOutputTypeDef],
-        "EventContextData": EventContextDataTypeOutputTypeDef,
-        "EventFeedback": EventFeedbackTypeOutputTypeDef,
+        "EventRisk": EventRiskTypeTypeDef,
+        "ChallengeResponses": List[ChallengeResponseTypeTypeDef],
+        "EventContextData": EventContextDataTypeTypeDef,
+        "EventFeedback": EventFeedbackTypeTypeDef,
     },
 )
 
-AuthenticationResultTypeOutputTypeDef = TypedDict(
-    "AuthenticationResultTypeOutputTypeDef",
+AuthenticationResultTypeTypeDef = TypedDict(
+    "AuthenticationResultTypeTypeDef",
     {
         "AccessToken": str,
         "ExpiresIn": int,
         "TokenType": str,
         "RefreshToken": str,
         "IdToken": str,
-        "NewDeviceMetadata": NewDeviceMetadataTypeOutputTypeDef,
+        "NewDeviceMetadata": NewDeviceMetadataTypeTypeDef,
     },
 )
 
-ForgotPasswordResponseOutputTypeDef = TypedDict(
-    "ForgotPasswordResponseOutputTypeDef",
+ForgotPasswordResponseTypeDef = TypedDict(
+    "ForgotPasswordResponseTypeDef",
     {
-        "CodeDeliveryDetails": CodeDeliveryDetailsTypeOutputTypeDef,
+        "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetUserAttributeVerificationCodeResponseOutputTypeDef = TypedDict(
-    "GetUserAttributeVerificationCodeResponseOutputTypeDef",
+GetUserAttributeVerificationCodeResponseTypeDef = TypedDict(
+    "GetUserAttributeVerificationCodeResponseTypeDef",
     {
-        "CodeDeliveryDetails": CodeDeliveryDetailsTypeOutputTypeDef,
+        "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResendConfirmationCodeResponseOutputTypeDef = TypedDict(
-    "ResendConfirmationCodeResponseOutputTypeDef",
+ResendConfirmationCodeResponseTypeDef = TypedDict(
+    "ResendConfirmationCodeResponseTypeDef",
     {
-        "CodeDeliveryDetails": CodeDeliveryDetailsTypeOutputTypeDef,
+        "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SignUpResponseOutputTypeDef = TypedDict(
-    "SignUpResponseOutputTypeDef",
+SignUpResponseTypeDef = TypedDict(
+    "SignUpResponseTypeDef",
     {
         "UserConfirmed": bool,
-        "CodeDeliveryDetails": CodeDeliveryDetailsTypeOutputTypeDef,
+        "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
         "UserSub": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateUserAttributesResponseOutputTypeDef = TypedDict(
-    "UpdateUserAttributesResponseOutputTypeDef",
+UpdateUserAttributesResponseTypeDef = TypedDict(
+    "UpdateUserAttributesResponseTypeDef",
     {
-        "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeOutputTypeDef],
+        "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompromisedCredentialsRiskConfigurationTypeOutputTypeDef = TypedDict(
     "CompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
     {
@@ -2930,42 +2930,42 @@
 )
 
 
 class ContextDataTypeTypeDef(_RequiredContextDataTypeTypeDef, _OptionalContextDataTypeTypeDef):
     pass
 
 
-CreateIdentityProviderResponseOutputTypeDef = TypedDict(
-    "CreateIdentityProviderResponseOutputTypeDef",
+CreateIdentityProviderResponseTypeDef = TypedDict(
+    "CreateIdentityProviderResponseTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeOutputTypeDef,
+        "IdentityProvider": IdentityProviderTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeIdentityProviderResponseOutputTypeDef = TypedDict(
-    "DescribeIdentityProviderResponseOutputTypeDef",
+DescribeIdentityProviderResponseTypeDef = TypedDict(
+    "DescribeIdentityProviderResponseTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeOutputTypeDef,
+        "IdentityProvider": IdentityProviderTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetIdentityProviderByIdentifierResponseOutputTypeDef = TypedDict(
-    "GetIdentityProviderByIdentifierResponseOutputTypeDef",
+GetIdentityProviderByIdentifierResponseTypeDef = TypedDict(
+    "GetIdentityProviderByIdentifierResponseTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeOutputTypeDef,
+        "IdentityProvider": IdentityProviderTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateIdentityProviderResponseOutputTypeDef = TypedDict(
-    "UpdateIdentityProviderResponseOutputTypeDef",
+UpdateIdentityProviderResponseTypeDef = TypedDict(
+    "UpdateIdentityProviderResponseTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeOutputTypeDef,
+        "IdentityProvider": IdentityProviderTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateResourceServerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceServerRequestRequestTypeDef",
     {
@@ -3010,51 +3010,51 @@
 class UpdateResourceServerRequestRequestTypeDef(
     _RequiredUpdateResourceServerRequestRequestTypeDef,
     _OptionalUpdateResourceServerRequestRequestTypeDef,
 ):
     pass
 
 
-CreateUserImportJobResponseOutputTypeDef = TypedDict(
-    "CreateUserImportJobResponseOutputTypeDef",
+CreateUserImportJobResponseTypeDef = TypedDict(
+    "CreateUserImportJobResponseTypeDef",
     {
-        "UserImportJob": UserImportJobTypeOutputTypeDef,
+        "UserImportJob": UserImportJobTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeUserImportJobResponseOutputTypeDef = TypedDict(
-    "DescribeUserImportJobResponseOutputTypeDef",
+DescribeUserImportJobResponseTypeDef = TypedDict(
+    "DescribeUserImportJobResponseTypeDef",
     {
-        "UserImportJob": UserImportJobTypeOutputTypeDef,
+        "UserImportJob": UserImportJobTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUserImportJobsResponseOutputTypeDef = TypedDict(
-    "ListUserImportJobsResponseOutputTypeDef",
+ListUserImportJobsResponseTypeDef = TypedDict(
+    "ListUserImportJobsResponseTypeDef",
     {
-        "UserImportJobs": List[UserImportJobTypeOutputTypeDef],
+        "UserImportJobs": List[UserImportJobTypeTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartUserImportJobResponseOutputTypeDef = TypedDict(
-    "StartUserImportJobResponseOutputTypeDef",
+StartUserImportJobResponseTypeDef = TypedDict(
+    "StartUserImportJobResponseTypeDef",
     {
-        "UserImportJob": UserImportJobTypeOutputTypeDef,
+        "UserImportJob": UserImportJobTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopUserImportJobResponseOutputTypeDef = TypedDict(
-    "StopUserImportJobResponseOutputTypeDef",
+StopUserImportJobResponseTypeDef = TypedDict(
+    "StopUserImportJobResponseTypeDef",
     {
-        "UserImportJob": UserImportJobTypeOutputTypeDef,
+        "UserImportJob": UserImportJobTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUserPoolClientRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserPoolClientRequestRequestTypeDef",
     {
@@ -3176,16 +3176,16 @@
     {
         "SmsAuthenticationMessage": str,
         "SmsConfiguration": SmsConfigurationTypeTypeDef,
     },
     total=False,
 )
 
-DomainDescriptionTypeOutputTypeDef = TypedDict(
-    "DomainDescriptionTypeOutputTypeDef",
+DomainDescriptionTypeTypeDef = TypedDict(
+    "DomainDescriptionTypeTypeDef",
     {
         "UserPoolId": str,
         "AWSAccountId": str,
         "Domain": str,
         "S3Bucket": str,
         "CloudFrontDistribution": str,
         "Version": str,
@@ -3229,43 +3229,43 @@
         "CustomSMSSender": CustomSMSLambdaVersionConfigTypeTypeDef,
         "CustomEmailSender": CustomEmailLambdaVersionConfigTypeTypeDef,
         "KMSKeyID": str,
     },
     total=False,
 )
 
-GetUICustomizationResponseOutputTypeDef = TypedDict(
-    "GetUICustomizationResponseOutputTypeDef",
+GetUICustomizationResponseTypeDef = TypedDict(
+    "GetUICustomizationResponseTypeDef",
     {
-        "UICustomization": UICustomizationTypeOutputTypeDef,
+        "UICustomization": UICustomizationTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SetUICustomizationResponseOutputTypeDef = TypedDict(
-    "SetUICustomizationResponseOutputTypeDef",
+SetUICustomizationResponseTypeDef = TypedDict(
+    "SetUICustomizationResponseTypeDef",
     {
-        "UICustomization": UICustomizationTypeOutputTypeDef,
+        "UICustomization": UICustomizationTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListIdentityProvidersResponseOutputTypeDef = TypedDict(
-    "ListIdentityProvidersResponseOutputTypeDef",
+ListIdentityProvidersResponseTypeDef = TypedDict(
+    "ListIdentityProvidersResponseTypeDef",
     {
-        "Providers": List[ProviderDescriptionOutputTypeDef],
+        "Providers": List[ProviderDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUserPoolClientsResponseOutputTypeDef = TypedDict(
-    "ListUserPoolClientsResponseOutputTypeDef",
+ListUserPoolClientsResponseTypeDef = TypedDict(
+    "ListUserPoolClientsResponseTypeDef",
     {
-        "UserPoolClients": List[UserPoolClientDescriptionOutputTypeDef],
+        "UserPoolClients": List[UserPoolClientDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotifyConfigurationTypeOutputTypeDef = TypedDict(
     "NotifyConfigurationTypeOutputTypeDef",
@@ -3315,16 +3315,16 @@
     "UserPoolPolicyTypeTypeDef",
     {
         "PasswordPolicy": PasswordPolicyTypeTypeDef,
     },
     total=False,
 )
 
-ResourceServerTypeOutputTypeDef = TypedDict(
-    "ResourceServerTypeOutputTypeDef",
+ResourceServerTypeTypeDef = TypedDict(
+    "ResourceServerTypeTypeDef",
     {
         "UserPoolId": str,
         "Identifier": str,
         "Name": str,
         "Scopes": List[ResourceServerScopeTypeOutputTypeDef],
     },
 )
@@ -3360,16 +3360,16 @@
     "SmsMfaConfigTypeOutputTypeDef",
     {
         "SmsAuthenticationMessage": str,
         "SmsConfiguration": SmsConfigurationTypeOutputTypeDef,
     },
 )
 
-UserPoolClientTypeOutputTypeDef = TypedDict(
-    "UserPoolClientTypeOutputTypeDef",
+UserPoolClientTypeTypeDef = TypedDict(
+    "UserPoolClientTypeTypeDef",
     {
         "UserPoolId": str,
         "ClientName": str,
         "ClientId": str,
         "ClientSecret": str,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
@@ -3391,123 +3391,123 @@
         "PreventUserExistenceErrors": PreventUserExistenceErrorTypesType,
         "EnableTokenRevocation": bool,
         "EnablePropagateAdditionalUserContextData": bool,
         "AuthSessionValidity": int,
     },
 )
 
-AdminGetDeviceResponseOutputTypeDef = TypedDict(
-    "AdminGetDeviceResponseOutputTypeDef",
+AdminGetDeviceResponseTypeDef = TypedDict(
+    "AdminGetDeviceResponseTypeDef",
     {
-        "Device": DeviceTypeOutputTypeDef,
+        "Device": DeviceTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminListDevicesResponseOutputTypeDef = TypedDict(
-    "AdminListDevicesResponseOutputTypeDef",
+AdminListDevicesResponseTypeDef = TypedDict(
+    "AdminListDevicesResponseTypeDef",
     {
-        "Devices": List[DeviceTypeOutputTypeDef],
+        "Devices": List[DeviceTypeTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetDeviceResponseOutputTypeDef = TypedDict(
-    "GetDeviceResponseOutputTypeDef",
+GetDeviceResponseTypeDef = TypedDict(
+    "GetDeviceResponseTypeDef",
     {
-        "Device": DeviceTypeOutputTypeDef,
+        "Device": DeviceTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDevicesResponseOutputTypeDef = TypedDict(
-    "ListDevicesResponseOutputTypeDef",
+ListDevicesResponseTypeDef = TypedDict(
+    "ListDevicesResponseTypeDef",
     {
-        "Devices": List[DeviceTypeOutputTypeDef],
+        "Devices": List[DeviceTypeTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminCreateUserResponseOutputTypeDef = TypedDict(
-    "AdminCreateUserResponseOutputTypeDef",
+AdminCreateUserResponseTypeDef = TypedDict(
+    "AdminCreateUserResponseTypeDef",
     {
-        "User": UserTypeOutputTypeDef,
+        "User": UserTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUsersInGroupResponseOutputTypeDef = TypedDict(
-    "ListUsersInGroupResponseOutputTypeDef",
+ListUsersInGroupResponseTypeDef = TypedDict(
+    "ListUsersInGroupResponseTypeDef",
     {
-        "Users": List[UserTypeOutputTypeDef],
+        "Users": List[UserTypeTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUsersResponseOutputTypeDef = TypedDict(
-    "ListUsersResponseOutputTypeDef",
+ListUsersResponseTypeDef = TypedDict(
+    "ListUsersResponseTypeDef",
     {
-        "Users": List[UserTypeOutputTypeDef],
+        "Users": List[UserTypeTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminListUserAuthEventsResponseOutputTypeDef = TypedDict(
-    "AdminListUserAuthEventsResponseOutputTypeDef",
+AdminListUserAuthEventsResponseTypeDef = TypedDict(
+    "AdminListUserAuthEventsResponseTypeDef",
     {
-        "AuthEvents": List[AuthEventTypeOutputTypeDef],
+        "AuthEvents": List[AuthEventTypeTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminInitiateAuthResponseOutputTypeDef = TypedDict(
-    "AdminInitiateAuthResponseOutputTypeDef",
+AdminInitiateAuthResponseTypeDef = TypedDict(
+    "AdminInitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
-        "AuthenticationResult": AuthenticationResultTypeOutputTypeDef,
+        "AuthenticationResult": AuthenticationResultTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminRespondToAuthChallengeResponseOutputTypeDef = TypedDict(
-    "AdminRespondToAuthChallengeResponseOutputTypeDef",
+AdminRespondToAuthChallengeResponseTypeDef = TypedDict(
+    "AdminRespondToAuthChallengeResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
-        "AuthenticationResult": AuthenticationResultTypeOutputTypeDef,
+        "AuthenticationResult": AuthenticationResultTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InitiateAuthResponseOutputTypeDef = TypedDict(
-    "InitiateAuthResponseOutputTypeDef",
+InitiateAuthResponseTypeDef = TypedDict(
+    "InitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
-        "AuthenticationResult": AuthenticationResultTypeOutputTypeDef,
+        "AuthenticationResult": AuthenticationResultTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RespondToAuthChallengeResponseOutputTypeDef = TypedDict(
-    "RespondToAuthChallengeResponseOutputTypeDef",
+RespondToAuthChallengeResponseTypeDef = TypedDict(
+    "RespondToAuthChallengeResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
-        "AuthenticationResult": AuthenticationResultTypeOutputTypeDef,
+        "AuthenticationResult": AuthenticationResultTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAdminInitiateAuthRequestRequestTypeDef = TypedDict(
     "_RequiredAdminInitiateAuthRequestRequestTypeDef",
     {
@@ -3582,24 +3582,24 @@
 class SetUserPoolMfaConfigRequestRequestTypeDef(
     _RequiredSetUserPoolMfaConfigRequestRequestTypeDef,
     _OptionalSetUserPoolMfaConfigRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeUserPoolDomainResponseOutputTypeDef = TypedDict(
-    "DescribeUserPoolDomainResponseOutputTypeDef",
+DescribeUserPoolDomainResponseTypeDef = TypedDict(
+    "DescribeUserPoolDomainResponseTypeDef",
     {
-        "DomainDescription": DomainDescriptionTypeOutputTypeDef,
+        "DomainDescription": DomainDescriptionTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UserPoolDescriptionTypeOutputTypeDef = TypedDict(
-    "UserPoolDescriptionTypeOutputTypeDef",
+UserPoolDescriptionTypeTypeDef = TypedDict(
+    "UserPoolDescriptionTypeTypeDef",
     {
         "Id": str,
         "Name": str,
         "LambdaConfig": LambdaConfigTypeOutputTypeDef,
         "Status": StatusTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
@@ -3670,49 +3670,49 @@
 
 class UpdateUserPoolRequestRequestTypeDef(
     _RequiredUpdateUserPoolRequestRequestTypeDef, _OptionalUpdateUserPoolRequestRequestTypeDef
 ):
     pass
 
 
-CreateResourceServerResponseOutputTypeDef = TypedDict(
-    "CreateResourceServerResponseOutputTypeDef",
+CreateResourceServerResponseTypeDef = TypedDict(
+    "CreateResourceServerResponseTypeDef",
     {
-        "ResourceServer": ResourceServerTypeOutputTypeDef,
+        "ResourceServer": ResourceServerTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeResourceServerResponseOutputTypeDef = TypedDict(
-    "DescribeResourceServerResponseOutputTypeDef",
+DescribeResourceServerResponseTypeDef = TypedDict(
+    "DescribeResourceServerResponseTypeDef",
     {
-        "ResourceServer": ResourceServerTypeOutputTypeDef,
+        "ResourceServer": ResourceServerTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListResourceServersResponseOutputTypeDef = TypedDict(
-    "ListResourceServersResponseOutputTypeDef",
+ListResourceServersResponseTypeDef = TypedDict(
+    "ListResourceServersResponseTypeDef",
     {
-        "ResourceServers": List[ResourceServerTypeOutputTypeDef],
+        "ResourceServers": List[ResourceServerTypeTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateResourceServerResponseOutputTypeDef = TypedDict(
-    "UpdateResourceServerResponseOutputTypeDef",
+UpdateResourceServerResponseTypeDef = TypedDict(
+    "UpdateResourceServerResponseTypeDef",
     {
-        "ResourceServer": ResourceServerTypeOutputTypeDef,
+        "ResourceServer": ResourceServerTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UserPoolTypeOutputTypeDef = TypedDict(
-    "UserPoolTypeOutputTypeDef",
+UserPoolTypeTypeDef = TypedDict(
+    "UserPoolTypeTypeDef",
     {
         "Id": str,
         "Name": str,
         "Policies": UserPoolPolicyTypeOutputTypeDef,
         "DeletionProtection": DeletionProtectionTypeType,
         "LambdaConfig": LambdaConfigTypeOutputTypeDef,
         "Status": StatusTypeType,
@@ -3792,69 +3792,69 @@
 
 class CreateUserPoolRequestRequestTypeDef(
     _RequiredCreateUserPoolRequestRequestTypeDef, _OptionalCreateUserPoolRequestRequestTypeDef
 ):
     pass
 
 
-GetUserPoolMfaConfigResponseOutputTypeDef = TypedDict(
-    "GetUserPoolMfaConfigResponseOutputTypeDef",
+GetUserPoolMfaConfigResponseTypeDef = TypedDict(
+    "GetUserPoolMfaConfigResponseTypeDef",
     {
         "SmsMfaConfiguration": SmsMfaConfigTypeOutputTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeOutputTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SetUserPoolMfaConfigResponseOutputTypeDef = TypedDict(
-    "SetUserPoolMfaConfigResponseOutputTypeDef",
+SetUserPoolMfaConfigResponseTypeDef = TypedDict(
+    "SetUserPoolMfaConfigResponseTypeDef",
     {
         "SmsMfaConfiguration": SmsMfaConfigTypeOutputTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeOutputTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateUserPoolClientResponseOutputTypeDef = TypedDict(
-    "CreateUserPoolClientResponseOutputTypeDef",
+CreateUserPoolClientResponseTypeDef = TypedDict(
+    "CreateUserPoolClientResponseTypeDef",
     {
-        "UserPoolClient": UserPoolClientTypeOutputTypeDef,
+        "UserPoolClient": UserPoolClientTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeUserPoolClientResponseOutputTypeDef = TypedDict(
-    "DescribeUserPoolClientResponseOutputTypeDef",
+DescribeUserPoolClientResponseTypeDef = TypedDict(
+    "DescribeUserPoolClientResponseTypeDef",
     {
-        "UserPoolClient": UserPoolClientTypeOutputTypeDef,
+        "UserPoolClient": UserPoolClientTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateUserPoolClientResponseOutputTypeDef = TypedDict(
-    "UpdateUserPoolClientResponseOutputTypeDef",
+UpdateUserPoolClientResponseTypeDef = TypedDict(
+    "UpdateUserPoolClientResponseTypeDef",
     {
-        "UserPoolClient": UserPoolClientTypeOutputTypeDef,
+        "UserPoolClient": UserPoolClientTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUserPoolsResponseOutputTypeDef = TypedDict(
-    "ListUserPoolsResponseOutputTypeDef",
+ListUserPoolsResponseTypeDef = TypedDict(
+    "ListUserPoolsResponseTypeDef",
     {
-        "UserPools": List[UserPoolDescriptionTypeOutputTypeDef],
+        "UserPools": List[UserPoolDescriptionTypeTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RiskConfigurationTypeOutputTypeDef = TypedDict(
-    "RiskConfigurationTypeOutputTypeDef",
+RiskConfigurationTypeTypeDef = TypedDict(
+    "RiskConfigurationTypeTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "CompromisedCredentialsRiskConfiguration": (
             CompromisedCredentialsRiskConfigurationTypeOutputTypeDef
         ),
         "AccountTakeoverRiskConfiguration": AccountTakeoverRiskConfigurationTypeOutputTypeDef,
@@ -3886,38 +3886,38 @@
 class SetRiskConfigurationRequestRequestTypeDef(
     _RequiredSetRiskConfigurationRequestRequestTypeDef,
     _OptionalSetRiskConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-CreateUserPoolResponseOutputTypeDef = TypedDict(
-    "CreateUserPoolResponseOutputTypeDef",
+CreateUserPoolResponseTypeDef = TypedDict(
+    "CreateUserPoolResponseTypeDef",
     {
-        "UserPool": UserPoolTypeOutputTypeDef,
+        "UserPool": UserPoolTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeUserPoolResponseOutputTypeDef = TypedDict(
-    "DescribeUserPoolResponseOutputTypeDef",
+DescribeUserPoolResponseTypeDef = TypedDict(
+    "DescribeUserPoolResponseTypeDef",
     {
-        "UserPool": UserPoolTypeOutputTypeDef,
+        "UserPool": UserPoolTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeRiskConfigurationResponseOutputTypeDef = TypedDict(
-    "DescribeRiskConfigurationResponseOutputTypeDef",
+DescribeRiskConfigurationResponseTypeDef = TypedDict(
+    "DescribeRiskConfigurationResponseTypeDef",
     {
-        "RiskConfiguration": RiskConfigurationTypeOutputTypeDef,
+        "RiskConfiguration": RiskConfigurationTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SetRiskConfigurationResponseOutputTypeDef = TypedDict(
-    "SetRiskConfigurationResponseOutputTypeDef",
+SetRiskConfigurationResponseTypeDef = TypedDict(
+    "SetRiskConfigurationResponseTypeDef",
     {
-        "RiskConfiguration": RiskConfigurationTypeOutputTypeDef,
+        "RiskConfiguration": RiskConfigurationTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp/type_defs.pyi` & `mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -85,46 +85,46 @@
     "AdminGetUserRequestRequestTypeDef",
     "AttributeTypeOutputTypeDef",
     "MFAOptionTypeOutputTypeDef",
     "AnalyticsMetadataTypeTypeDef",
     "AdminListDevicesRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "AdminListGroupsForUserRequestRequestTypeDef",
-    "GroupTypeOutputTypeDef",
+    "GroupTypeTypeDef",
     "AdminListUserAuthEventsRequestRequestTypeDef",
     "AdminRemoveUserFromGroupRequestRequestTypeDef",
     "AdminResetUserPasswordRequestRequestTypeDef",
     "SMSMfaSettingsTypeTypeDef",
     "SoftwareTokenMfaSettingsTypeTypeDef",
     "AdminSetUserPasswordRequestRequestTypeDef",
     "MFAOptionTypeTypeDef",
     "AdminUpdateAuthEventFeedbackRequestRequestTypeDef",
     "AdminUpdateDeviceStatusRequestRequestTypeDef",
     "AdminUserGlobalSignOutRequestRequestTypeDef",
     "AnalyticsConfigurationTypeOutputTypeDef",
     "AnalyticsConfigurationTypeTypeDef",
     "AssociateSoftwareTokenRequestRequestTypeDef",
-    "ChallengeResponseTypeOutputTypeDef",
-    "EventContextDataTypeOutputTypeDef",
-    "EventFeedbackTypeOutputTypeDef",
-    "EventRiskTypeOutputTypeDef",
-    "NewDeviceMetadataTypeOutputTypeDef",
+    "ChallengeResponseTypeTypeDef",
+    "EventContextDataTypeTypeDef",
+    "EventFeedbackTypeTypeDef",
+    "EventRiskTypeTypeDef",
+    "NewDeviceMetadataTypeTypeDef",
     "ChangePasswordRequestRequestTypeDef",
-    "CodeDeliveryDetailsTypeOutputTypeDef",
+    "CodeDeliveryDetailsTypeTypeDef",
     "CompromisedCredentialsActionsTypeOutputTypeDef",
     "CompromisedCredentialsActionsTypeTypeDef",
     "DeviceSecretVerifierConfigTypeTypeDef",
     "UserContextDataTypeTypeDef",
     "HttpHeaderTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
-    "IdentityProviderTypeOutputTypeDef",
+    "IdentityProviderTypeTypeDef",
     "ResourceServerScopeTypeTypeDef",
     "CreateUserImportJobRequestRequestTypeDef",
-    "UserImportJobTypeOutputTypeDef",
+    "UserImportJobTypeTypeDef",
     "TokenValidityUnitsTypeTypeDef",
     "CustomDomainConfigTypeTypeDef",
     "DeviceConfigurationTypeTypeDef",
     "EmailConfigurationTypeTypeDef",
     "SmsConfigurationTypeTypeDef",
     "UserAttributeUpdateSettingsTypeTypeDef",
     "UserPoolAddOnsTypeTypeDef",
@@ -155,29 +155,29 @@
     "ForgetDeviceRequestRequestTypeDef",
     "GetCSVHeaderRequestRequestTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GetIdentityProviderByIdentifierRequestRequestTypeDef",
     "GetSigningCertificateRequestRequestTypeDef",
     "GetUICustomizationRequestRequestTypeDef",
-    "UICustomizationTypeOutputTypeDef",
+    "UICustomizationTypeTypeDef",
     "GetUserAttributeVerificationCodeRequestRequestTypeDef",
     "GetUserPoolMfaConfigRequestRequestTypeDef",
     "SoftwareTokenMfaConfigTypeOutputTypeDef",
     "GetUserRequestRequestTypeDef",
     "GlobalSignOutRequestRequestTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListGroupsRequestRequestTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
-    "ProviderDescriptionOutputTypeDef",
+    "ProviderDescriptionTypeDef",
     "ListResourceServersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListUserImportJobsRequestRequestTypeDef",
     "ListUserPoolClientsRequestRequestTypeDef",
-    "UserPoolClientDescriptionOutputTypeDef",
+    "UserPoolClientDescriptionTypeDef",
     "ListUserPoolsRequestRequestTypeDef",
     "ListUsersInGroupRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "NotifyEmailTypeOutputTypeDef",
     "NotifyEmailTypeTypeDef",
     "NumberAttributeConstraintsTypeOutputTypeDef",
     "NumberAttributeConstraintsTypeTypeDef",
@@ -212,136 +212,136 @@
     "AccountTakeoverActionsTypeOutputTypeDef",
     "AccountTakeoverActionsTypeTypeDef",
     "AdminCreateUserConfigTypeOutputTypeDef",
     "AdminCreateUserConfigTypeTypeDef",
     "AdminCreateUserRequestRequestTypeDef",
     "AdminUpdateUserAttributesRequestRequestTypeDef",
     "UpdateUserAttributesRequestRequestTypeDef",
-    "AssociateSoftwareTokenResponseOutputTypeDef",
-    "ConfirmDeviceResponseOutputTypeDef",
-    "CreateUserPoolDomainResponseOutputTypeDef",
+    "AssociateSoftwareTokenResponseTypeDef",
+    "ConfirmDeviceResponseTypeDef",
+    "CreateUserPoolDomainResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "GetCSVHeaderResponseOutputTypeDef",
-    "GetSigningCertificateResponseOutputTypeDef",
-    "ListTagsForResourceResponseOutputTypeDef",
-    "UpdateUserPoolDomainResponseOutputTypeDef",
-    "VerifySoftwareTokenResponseOutputTypeDef",
+    "GetCSVHeaderResponseTypeDef",
+    "GetSigningCertificateResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateUserPoolDomainResponseTypeDef",
+    "VerifySoftwareTokenResponseTypeDef",
     "AdminDisableProviderForUserRequestRequestTypeDef",
     "AdminLinkProviderForUserRequestRequestTypeDef",
-    "DeviceTypeOutputTypeDef",
-    "AdminGetUserResponseOutputTypeDef",
-    "GetUserResponseOutputTypeDef",
-    "UserTypeOutputTypeDef",
+    "DeviceTypeTypeDef",
+    "AdminGetUserResponseTypeDef",
+    "GetUserResponseTypeDef",
+    "UserTypeTypeDef",
     "AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
     "AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
     "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListResourceServersRequestListResourceServersPaginateTypeDef",
     "ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
     "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
     "ListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
-    "AdminListGroupsForUserResponseOutputTypeDef",
-    "CreateGroupResponseOutputTypeDef",
-    "GetGroupResponseOutputTypeDef",
-    "ListGroupsResponseOutputTypeDef",
-    "UpdateGroupResponseOutputTypeDef",
+    "AdminListGroupsForUserResponseTypeDef",
+    "CreateGroupResponseTypeDef",
+    "GetGroupResponseTypeDef",
+    "ListGroupsResponseTypeDef",
+    "UpdateGroupResponseTypeDef",
     "AdminSetUserMFAPreferenceRequestRequestTypeDef",
     "SetUserMFAPreferenceRequestRequestTypeDef",
     "AdminSetUserSettingsRequestRequestTypeDef",
     "SetUserSettingsRequestRequestTypeDef",
-    "AuthEventTypeOutputTypeDef",
-    "AuthenticationResultTypeOutputTypeDef",
-    "ForgotPasswordResponseOutputTypeDef",
-    "GetUserAttributeVerificationCodeResponseOutputTypeDef",
-    "ResendConfirmationCodeResponseOutputTypeDef",
-    "SignUpResponseOutputTypeDef",
-    "UpdateUserAttributesResponseOutputTypeDef",
+    "AuthEventTypeTypeDef",
+    "AuthenticationResultTypeTypeDef",
+    "ForgotPasswordResponseTypeDef",
+    "GetUserAttributeVerificationCodeResponseTypeDef",
+    "ResendConfirmationCodeResponseTypeDef",
+    "SignUpResponseTypeDef",
+    "UpdateUserAttributesResponseTypeDef",
     "CompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
     "CompromisedCredentialsRiskConfigurationTypeTypeDef",
     "ConfirmDeviceRequestRequestTypeDef",
     "ConfirmForgotPasswordRequestRequestTypeDef",
     "ConfirmSignUpRequestRequestTypeDef",
     "ForgotPasswordRequestRequestTypeDef",
     "InitiateAuthRequestRequestTypeDef",
     "ResendConfirmationCodeRequestRequestTypeDef",
     "RespondToAuthChallengeRequestRequestTypeDef",
     "SignUpRequestRequestTypeDef",
     "ContextDataTypeTypeDef",
-    "CreateIdentityProviderResponseOutputTypeDef",
-    "DescribeIdentityProviderResponseOutputTypeDef",
-    "GetIdentityProviderByIdentifierResponseOutputTypeDef",
-    "UpdateIdentityProviderResponseOutputTypeDef",
+    "CreateIdentityProviderResponseTypeDef",
+    "DescribeIdentityProviderResponseTypeDef",
+    "GetIdentityProviderByIdentifierResponseTypeDef",
+    "UpdateIdentityProviderResponseTypeDef",
     "CreateResourceServerRequestRequestTypeDef",
     "UpdateResourceServerRequestRequestTypeDef",
-    "CreateUserImportJobResponseOutputTypeDef",
-    "DescribeUserImportJobResponseOutputTypeDef",
-    "ListUserImportJobsResponseOutputTypeDef",
-    "StartUserImportJobResponseOutputTypeDef",
-    "StopUserImportJobResponseOutputTypeDef",
+    "CreateUserImportJobResponseTypeDef",
+    "DescribeUserImportJobResponseTypeDef",
+    "ListUserImportJobsResponseTypeDef",
+    "StartUserImportJobResponseTypeDef",
+    "StopUserImportJobResponseTypeDef",
     "CreateUserPoolClientRequestRequestTypeDef",
     "UpdateUserPoolClientRequestRequestTypeDef",
     "CreateUserPoolDomainRequestRequestTypeDef",
     "UpdateUserPoolDomainRequestRequestTypeDef",
     "SmsMfaConfigTypeTypeDef",
-    "DomainDescriptionTypeOutputTypeDef",
+    "DomainDescriptionTypeTypeDef",
     "LambdaConfigTypeOutputTypeDef",
     "LambdaConfigTypeTypeDef",
-    "GetUICustomizationResponseOutputTypeDef",
-    "SetUICustomizationResponseOutputTypeDef",
-    "ListIdentityProvidersResponseOutputTypeDef",
-    "ListUserPoolClientsResponseOutputTypeDef",
+    "GetUICustomizationResponseTypeDef",
+    "SetUICustomizationResponseTypeDef",
+    "ListIdentityProvidersResponseTypeDef",
+    "ListUserPoolClientsResponseTypeDef",
     "NotifyConfigurationTypeOutputTypeDef",
     "NotifyConfigurationTypeTypeDef",
     "UserPoolPolicyTypeOutputTypeDef",
     "UserPoolPolicyTypeTypeDef",
-    "ResourceServerTypeOutputTypeDef",
+    "ResourceServerTypeTypeDef",
     "SchemaAttributeTypeOutputTypeDef",
     "SchemaAttributeTypeTypeDef",
     "SmsMfaConfigTypeOutputTypeDef",
-    "UserPoolClientTypeOutputTypeDef",
-    "AdminGetDeviceResponseOutputTypeDef",
-    "AdminListDevicesResponseOutputTypeDef",
-    "GetDeviceResponseOutputTypeDef",
-    "ListDevicesResponseOutputTypeDef",
-    "AdminCreateUserResponseOutputTypeDef",
-    "ListUsersInGroupResponseOutputTypeDef",
-    "ListUsersResponseOutputTypeDef",
-    "AdminListUserAuthEventsResponseOutputTypeDef",
-    "AdminInitiateAuthResponseOutputTypeDef",
-    "AdminRespondToAuthChallengeResponseOutputTypeDef",
-    "InitiateAuthResponseOutputTypeDef",
-    "RespondToAuthChallengeResponseOutputTypeDef",
+    "UserPoolClientTypeTypeDef",
+    "AdminGetDeviceResponseTypeDef",
+    "AdminListDevicesResponseTypeDef",
+    "GetDeviceResponseTypeDef",
+    "ListDevicesResponseTypeDef",
+    "AdminCreateUserResponseTypeDef",
+    "ListUsersInGroupResponseTypeDef",
+    "ListUsersResponseTypeDef",
+    "AdminListUserAuthEventsResponseTypeDef",
+    "AdminInitiateAuthResponseTypeDef",
+    "AdminRespondToAuthChallengeResponseTypeDef",
+    "InitiateAuthResponseTypeDef",
+    "RespondToAuthChallengeResponseTypeDef",
     "AdminInitiateAuthRequestRequestTypeDef",
     "AdminRespondToAuthChallengeRequestRequestTypeDef",
     "SetUserPoolMfaConfigRequestRequestTypeDef",
-    "DescribeUserPoolDomainResponseOutputTypeDef",
-    "UserPoolDescriptionTypeOutputTypeDef",
+    "DescribeUserPoolDomainResponseTypeDef",
+    "UserPoolDescriptionTypeTypeDef",
     "AccountTakeoverRiskConfigurationTypeOutputTypeDef",
     "AccountTakeoverRiskConfigurationTypeTypeDef",
     "UpdateUserPoolRequestRequestTypeDef",
-    "CreateResourceServerResponseOutputTypeDef",
-    "DescribeResourceServerResponseOutputTypeDef",
-    "ListResourceServersResponseOutputTypeDef",
-    "UpdateResourceServerResponseOutputTypeDef",
-    "UserPoolTypeOutputTypeDef",
+    "CreateResourceServerResponseTypeDef",
+    "DescribeResourceServerResponseTypeDef",
+    "ListResourceServersResponseTypeDef",
+    "UpdateResourceServerResponseTypeDef",
+    "UserPoolTypeTypeDef",
     "AddCustomAttributesRequestRequestTypeDef",
     "CreateUserPoolRequestRequestTypeDef",
-    "GetUserPoolMfaConfigResponseOutputTypeDef",
-    "SetUserPoolMfaConfigResponseOutputTypeDef",
-    "CreateUserPoolClientResponseOutputTypeDef",
-    "DescribeUserPoolClientResponseOutputTypeDef",
-    "UpdateUserPoolClientResponseOutputTypeDef",
-    "ListUserPoolsResponseOutputTypeDef",
-    "RiskConfigurationTypeOutputTypeDef",
+    "GetUserPoolMfaConfigResponseTypeDef",
+    "SetUserPoolMfaConfigResponseTypeDef",
+    "CreateUserPoolClientResponseTypeDef",
+    "DescribeUserPoolClientResponseTypeDef",
+    "UpdateUserPoolClientResponseTypeDef",
+    "ListUserPoolsResponseTypeDef",
+    "RiskConfigurationTypeTypeDef",
     "SetRiskConfigurationRequestRequestTypeDef",
-    "CreateUserPoolResponseOutputTypeDef",
-    "DescribeUserPoolResponseOutputTypeDef",
-    "DescribeRiskConfigurationResponseOutputTypeDef",
-    "SetRiskConfigurationResponseOutputTypeDef",
+    "CreateUserPoolResponseTypeDef",
+    "DescribeUserPoolResponseTypeDef",
+    "DescribeRiskConfigurationResponseTypeDef",
+    "SetRiskConfigurationResponseTypeDef",
 )
 
 RecoveryOptionTypeOutputTypeDef = TypedDict(
     "RecoveryOptionTypeOutputTypeDef",
     {
         "Priority": int,
         "Name": RecoveryOptionNameTypeType,
@@ -591,16 +591,16 @@
 
 class AdminListGroupsForUserRequestRequestTypeDef(
     _RequiredAdminListGroupsForUserRequestRequestTypeDef,
     _OptionalAdminListGroupsForUserRequestRequestTypeDef,
 ):
     pass
 
-GroupTypeOutputTypeDef = TypedDict(
-    "GroupTypeOutputTypeDef",
+GroupTypeTypeDef = TypedDict(
+    "GroupTypeTypeDef",
     {
         "GroupName": str,
         "UserPoolId": str,
         "Description": str,
         "RoleArn": str,
         "Precedence": int,
         "LastModifiedDate": datetime,
@@ -777,53 +777,53 @@
     {
         "AccessToken": str,
         "Session": str,
     },
     total=False,
 )
 
-ChallengeResponseTypeOutputTypeDef = TypedDict(
-    "ChallengeResponseTypeOutputTypeDef",
+ChallengeResponseTypeTypeDef = TypedDict(
+    "ChallengeResponseTypeTypeDef",
     {
         "ChallengeName": ChallengeNameType,
         "ChallengeResponse": ChallengeResponseType,
     },
 )
 
-EventContextDataTypeOutputTypeDef = TypedDict(
-    "EventContextDataTypeOutputTypeDef",
+EventContextDataTypeTypeDef = TypedDict(
+    "EventContextDataTypeTypeDef",
     {
         "IpAddress": str,
         "DeviceName": str,
         "Timezone": str,
         "City": str,
         "Country": str,
     },
 )
 
-EventFeedbackTypeOutputTypeDef = TypedDict(
-    "EventFeedbackTypeOutputTypeDef",
+EventFeedbackTypeTypeDef = TypedDict(
+    "EventFeedbackTypeTypeDef",
     {
         "FeedbackValue": FeedbackValueTypeType,
         "Provider": str,
         "FeedbackDate": datetime,
     },
 )
 
-EventRiskTypeOutputTypeDef = TypedDict(
-    "EventRiskTypeOutputTypeDef",
+EventRiskTypeTypeDef = TypedDict(
+    "EventRiskTypeTypeDef",
     {
         "RiskDecision": RiskDecisionTypeType,
         "RiskLevel": RiskLevelTypeType,
         "CompromisedCredentialsDetected": bool,
     },
 )
 
-NewDeviceMetadataTypeOutputTypeDef = TypedDict(
-    "NewDeviceMetadataTypeOutputTypeDef",
+NewDeviceMetadataTypeTypeDef = TypedDict(
+    "NewDeviceMetadataTypeTypeDef",
     {
         "DeviceKey": str,
         "DeviceGroupKey": str,
     },
 )
 
 ChangePasswordRequestRequestTypeDef = TypedDict(
@@ -831,16 +831,16 @@
     {
         "PreviousPassword": str,
         "ProposedPassword": str,
         "AccessToken": str,
     },
 )
 
-CodeDeliveryDetailsTypeOutputTypeDef = TypedDict(
-    "CodeDeliveryDetailsTypeOutputTypeDef",
+CodeDeliveryDetailsTypeTypeDef = TypedDict(
+    "CodeDeliveryDetailsTypeTypeDef",
     {
         "Destination": str,
         "DeliveryMedium": DeliveryMediumTypeType,
         "AttributeName": str,
     },
 )
 
@@ -927,16 +927,16 @@
 
 class CreateIdentityProviderRequestRequestTypeDef(
     _RequiredCreateIdentityProviderRequestRequestTypeDef,
     _OptionalCreateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
-IdentityProviderTypeOutputTypeDef = TypedDict(
-    "IdentityProviderTypeOutputTypeDef",
+IdentityProviderTypeTypeDef = TypedDict(
+    "IdentityProviderTypeTypeDef",
     {
         "UserPoolId": str,
         "ProviderName": str,
         "ProviderType": IdentityProviderTypeTypeType,
         "ProviderDetails": Dict[str, str],
         "AttributeMapping": Dict[str, str],
         "IdpIdentifiers": List[str],
@@ -958,16 +958,16 @@
     {
         "JobName": str,
         "UserPoolId": str,
         "CloudWatchLogsRoleArn": str,
     },
 )
 
-UserImportJobTypeOutputTypeDef = TypedDict(
-    "UserImportJobTypeOutputTypeDef",
+UserImportJobTypeTypeDef = TypedDict(
+    "UserImportJobTypeTypeDef",
     {
         "JobName": str,
         "JobId": str,
         "UserPoolId": str,
         "PreSignedUrl": str,
         "CreationDate": datetime,
         "StartDate": datetime,
@@ -1344,16 +1344,16 @@
 
 class GetUICustomizationRequestRequestTypeDef(
     _RequiredGetUICustomizationRequestRequestTypeDef,
     _OptionalGetUICustomizationRequestRequestTypeDef,
 ):
     pass
 
-UICustomizationTypeOutputTypeDef = TypedDict(
-    "UICustomizationTypeOutputTypeDef",
+UICustomizationTypeTypeDef = TypedDict(
+    "UICustomizationTypeTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "ImageUrl": str,
         "CSS": str,
         "CSSVersion": str,
         "LastModifiedDate": datetime,
@@ -1467,16 +1467,16 @@
 
 class ListIdentityProvidersRequestRequestTypeDef(
     _RequiredListIdentityProvidersRequestRequestTypeDef,
     _OptionalListIdentityProvidersRequestRequestTypeDef,
 ):
     pass
 
-ProviderDescriptionOutputTypeDef = TypedDict(
-    "ProviderDescriptionOutputTypeDef",
+ProviderDescriptionTypeDef = TypedDict(
+    "ProviderDescriptionTypeDef",
     {
         "ProviderName": str,
         "ProviderType": IdentityProviderTypeTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
 )
@@ -1547,16 +1547,16 @@
 
 class ListUserPoolClientsRequestRequestTypeDef(
     _RequiredListUserPoolClientsRequestRequestTypeDef,
     _OptionalListUserPoolClientsRequestRequestTypeDef,
 ):
     pass
 
-UserPoolClientDescriptionOutputTypeDef = TypedDict(
-    "UserPoolClientDescriptionOutputTypeDef",
+UserPoolClientDescriptionTypeDef = TypedDict(
+    "UserPoolClientDescriptionTypeDef",
     {
         "ClientId": str,
         "UserPoolId": str,
         "ClientName": str,
     },
 )
 
@@ -2092,81 +2092,81 @@
 
 class UpdateUserAttributesRequestRequestTypeDef(
     _RequiredUpdateUserAttributesRequestRequestTypeDef,
     _OptionalUpdateUserAttributesRequestRequestTypeDef,
 ):
     pass
 
-AssociateSoftwareTokenResponseOutputTypeDef = TypedDict(
-    "AssociateSoftwareTokenResponseOutputTypeDef",
+AssociateSoftwareTokenResponseTypeDef = TypedDict(
+    "AssociateSoftwareTokenResponseTypeDef",
     {
         "SecretCode": str,
         "Session": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfirmDeviceResponseOutputTypeDef = TypedDict(
-    "ConfirmDeviceResponseOutputTypeDef",
+ConfirmDeviceResponseTypeDef = TypedDict(
+    "ConfirmDeviceResponseTypeDef",
     {
         "UserConfirmationNecessary": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateUserPoolDomainResponseOutputTypeDef = TypedDict(
-    "CreateUserPoolDomainResponseOutputTypeDef",
+CreateUserPoolDomainResponseTypeDef = TypedDict(
+    "CreateUserPoolDomainResponseTypeDef",
     {
         "CloudFrontDomain": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetCSVHeaderResponseOutputTypeDef = TypedDict(
-    "GetCSVHeaderResponseOutputTypeDef",
+GetCSVHeaderResponseTypeDef = TypedDict(
+    "GetCSVHeaderResponseTypeDef",
     {
         "UserPoolId": str,
         "CSVHeader": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetSigningCertificateResponseOutputTypeDef = TypedDict(
-    "GetSigningCertificateResponseOutputTypeDef",
+GetSigningCertificateResponseTypeDef = TypedDict(
+    "GetSigningCertificateResponseTypeDef",
     {
         "Certificate": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseOutputTypeDef = TypedDict(
-    "ListTagsForResourceResponseOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateUserPoolDomainResponseOutputTypeDef = TypedDict(
-    "UpdateUserPoolDomainResponseOutputTypeDef",
+UpdateUserPoolDomainResponseTypeDef = TypedDict(
+    "UpdateUserPoolDomainResponseTypeDef",
     {
         "CloudFrontDomain": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VerifySoftwareTokenResponseOutputTypeDef = TypedDict(
-    "VerifySoftwareTokenResponseOutputTypeDef",
+VerifySoftwareTokenResponseTypeDef = TypedDict(
+    "VerifySoftwareTokenResponseTypeDef",
     {
         "Status": VerifySoftwareTokenResponseTypeType,
         "Session": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -2183,55 +2183,55 @@
     {
         "UserPoolId": str,
         "DestinationUser": ProviderUserIdentifierTypeTypeDef,
         "SourceUser": ProviderUserIdentifierTypeTypeDef,
     },
 )
 
-DeviceTypeOutputTypeDef = TypedDict(
-    "DeviceTypeOutputTypeDef",
+DeviceTypeTypeDef = TypedDict(
+    "DeviceTypeTypeDef",
     {
         "DeviceKey": str,
         "DeviceAttributes": List[AttributeTypeOutputTypeDef],
         "DeviceCreateDate": datetime,
         "DeviceLastModifiedDate": datetime,
         "DeviceLastAuthenticatedDate": datetime,
     },
 )
 
-AdminGetUserResponseOutputTypeDef = TypedDict(
-    "AdminGetUserResponseOutputTypeDef",
+AdminGetUserResponseTypeDef = TypedDict(
+    "AdminGetUserResponseTypeDef",
     {
         "Username": str,
         "UserAttributes": List[AttributeTypeOutputTypeDef],
         "UserCreateDate": datetime,
         "UserLastModifiedDate": datetime,
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
         "MFAOptions": List[MFAOptionTypeOutputTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetUserResponseOutputTypeDef = TypedDict(
-    "GetUserResponseOutputTypeDef",
+GetUserResponseTypeDef = TypedDict(
+    "GetUserResponseTypeDef",
     {
         "Username": str,
         "UserAttributes": List[AttributeTypeOutputTypeDef],
         "MFAOptions": List[MFAOptionTypeOutputTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UserTypeOutputTypeDef = TypedDict(
-    "UserTypeOutputTypeDef",
+UserTypeTypeDef = TypedDict(
+    "UserTypeTypeDef",
     {
         "Username": str,
         "Attributes": List[AttributeTypeOutputTypeDef],
         "UserCreateDate": datetime,
         "UserLastModifiedDate": datetime,
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
@@ -2408,52 +2408,52 @@
 
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
-AdminListGroupsForUserResponseOutputTypeDef = TypedDict(
-    "AdminListGroupsForUserResponseOutputTypeDef",
+AdminListGroupsForUserResponseTypeDef = TypedDict(
+    "AdminListGroupsForUserResponseTypeDef",
     {
-        "Groups": List[GroupTypeOutputTypeDef],
+        "Groups": List[GroupTypeTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateGroupResponseOutputTypeDef = TypedDict(
-    "CreateGroupResponseOutputTypeDef",
+CreateGroupResponseTypeDef = TypedDict(
+    "CreateGroupResponseTypeDef",
     {
-        "Group": GroupTypeOutputTypeDef,
+        "Group": GroupTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetGroupResponseOutputTypeDef = TypedDict(
-    "GetGroupResponseOutputTypeDef",
+GetGroupResponseTypeDef = TypedDict(
+    "GetGroupResponseTypeDef",
     {
-        "Group": GroupTypeOutputTypeDef,
+        "Group": GroupTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListGroupsResponseOutputTypeDef = TypedDict(
-    "ListGroupsResponseOutputTypeDef",
+ListGroupsResponseTypeDef = TypedDict(
+    "ListGroupsResponseTypeDef",
     {
-        "Groups": List[GroupTypeOutputTypeDef],
+        "Groups": List[GroupTypeTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateGroupResponseOutputTypeDef = TypedDict(
-    "UpdateGroupResponseOutputTypeDef",
+UpdateGroupResponseTypeDef = TypedDict(
+    "UpdateGroupResponseTypeDef",
     {
-        "Group": GroupTypeOutputTypeDef,
+        "Group": GroupTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef = TypedDict(
     "_RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef",
     {
@@ -2510,78 +2510,78 @@
     "SetUserSettingsRequestRequestTypeDef",
     {
         "AccessToken": str,
         "MFAOptions": Sequence[MFAOptionTypeTypeDef],
     },
 )
 
-AuthEventTypeOutputTypeDef = TypedDict(
-    "AuthEventTypeOutputTypeDef",
+AuthEventTypeTypeDef = TypedDict(
+    "AuthEventTypeTypeDef",
     {
         "EventId": str,
         "EventType": EventTypeType,
         "CreationDate": datetime,
         "EventResponse": EventResponseTypeType,
-        "EventRisk": EventRiskTypeOutputTypeDef,
-        "ChallengeResponses": List[ChallengeResponseTypeOutputTypeDef],
-        "EventContextData": EventContextDataTypeOutputTypeDef,
-        "EventFeedback": EventFeedbackTypeOutputTypeDef,
+        "EventRisk": EventRiskTypeTypeDef,
+        "ChallengeResponses": List[ChallengeResponseTypeTypeDef],
+        "EventContextData": EventContextDataTypeTypeDef,
+        "EventFeedback": EventFeedbackTypeTypeDef,
     },
 )
 
-AuthenticationResultTypeOutputTypeDef = TypedDict(
-    "AuthenticationResultTypeOutputTypeDef",
+AuthenticationResultTypeTypeDef = TypedDict(
+    "AuthenticationResultTypeTypeDef",
     {
         "AccessToken": str,
         "ExpiresIn": int,
         "TokenType": str,
         "RefreshToken": str,
         "IdToken": str,
-        "NewDeviceMetadata": NewDeviceMetadataTypeOutputTypeDef,
+        "NewDeviceMetadata": NewDeviceMetadataTypeTypeDef,
     },
 )
 
-ForgotPasswordResponseOutputTypeDef = TypedDict(
-    "ForgotPasswordResponseOutputTypeDef",
+ForgotPasswordResponseTypeDef = TypedDict(
+    "ForgotPasswordResponseTypeDef",
     {
-        "CodeDeliveryDetails": CodeDeliveryDetailsTypeOutputTypeDef,
+        "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetUserAttributeVerificationCodeResponseOutputTypeDef = TypedDict(
-    "GetUserAttributeVerificationCodeResponseOutputTypeDef",
+GetUserAttributeVerificationCodeResponseTypeDef = TypedDict(
+    "GetUserAttributeVerificationCodeResponseTypeDef",
     {
-        "CodeDeliveryDetails": CodeDeliveryDetailsTypeOutputTypeDef,
+        "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResendConfirmationCodeResponseOutputTypeDef = TypedDict(
-    "ResendConfirmationCodeResponseOutputTypeDef",
+ResendConfirmationCodeResponseTypeDef = TypedDict(
+    "ResendConfirmationCodeResponseTypeDef",
     {
-        "CodeDeliveryDetails": CodeDeliveryDetailsTypeOutputTypeDef,
+        "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SignUpResponseOutputTypeDef = TypedDict(
-    "SignUpResponseOutputTypeDef",
+SignUpResponseTypeDef = TypedDict(
+    "SignUpResponseTypeDef",
     {
         "UserConfirmed": bool,
-        "CodeDeliveryDetails": CodeDeliveryDetailsTypeOutputTypeDef,
+        "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
         "UserSub": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateUserAttributesResponseOutputTypeDef = TypedDict(
-    "UpdateUserAttributesResponseOutputTypeDef",
+UpdateUserAttributesResponseTypeDef = TypedDict(
+    "UpdateUserAttributesResponseTypeDef",
     {
-        "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeOutputTypeDef],
+        "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CompromisedCredentialsRiskConfigurationTypeOutputTypeDef = TypedDict(
     "CompromisedCredentialsRiskConfigurationTypeOutputTypeDef",
     {
@@ -2819,42 +2819,42 @@
     },
     total=False,
 )
 
 class ContextDataTypeTypeDef(_RequiredContextDataTypeTypeDef, _OptionalContextDataTypeTypeDef):
     pass
 
-CreateIdentityProviderResponseOutputTypeDef = TypedDict(
-    "CreateIdentityProviderResponseOutputTypeDef",
+CreateIdentityProviderResponseTypeDef = TypedDict(
+    "CreateIdentityProviderResponseTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeOutputTypeDef,
+        "IdentityProvider": IdentityProviderTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeIdentityProviderResponseOutputTypeDef = TypedDict(
-    "DescribeIdentityProviderResponseOutputTypeDef",
+DescribeIdentityProviderResponseTypeDef = TypedDict(
+    "DescribeIdentityProviderResponseTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeOutputTypeDef,
+        "IdentityProvider": IdentityProviderTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetIdentityProviderByIdentifierResponseOutputTypeDef = TypedDict(
-    "GetIdentityProviderByIdentifierResponseOutputTypeDef",
+GetIdentityProviderByIdentifierResponseTypeDef = TypedDict(
+    "GetIdentityProviderByIdentifierResponseTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeOutputTypeDef,
+        "IdentityProvider": IdentityProviderTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateIdentityProviderResponseOutputTypeDef = TypedDict(
-    "UpdateIdentityProviderResponseOutputTypeDef",
+UpdateIdentityProviderResponseTypeDef = TypedDict(
+    "UpdateIdentityProviderResponseTypeDef",
     {
-        "IdentityProvider": IdentityProviderTypeOutputTypeDef,
+        "IdentityProvider": IdentityProviderTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateResourceServerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceServerRequestRequestTypeDef",
     {
@@ -2895,51 +2895,51 @@
 
 class UpdateResourceServerRequestRequestTypeDef(
     _RequiredUpdateResourceServerRequestRequestTypeDef,
     _OptionalUpdateResourceServerRequestRequestTypeDef,
 ):
     pass
 
-CreateUserImportJobResponseOutputTypeDef = TypedDict(
-    "CreateUserImportJobResponseOutputTypeDef",
+CreateUserImportJobResponseTypeDef = TypedDict(
+    "CreateUserImportJobResponseTypeDef",
     {
-        "UserImportJob": UserImportJobTypeOutputTypeDef,
+        "UserImportJob": UserImportJobTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeUserImportJobResponseOutputTypeDef = TypedDict(
-    "DescribeUserImportJobResponseOutputTypeDef",
+DescribeUserImportJobResponseTypeDef = TypedDict(
+    "DescribeUserImportJobResponseTypeDef",
     {
-        "UserImportJob": UserImportJobTypeOutputTypeDef,
+        "UserImportJob": UserImportJobTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUserImportJobsResponseOutputTypeDef = TypedDict(
-    "ListUserImportJobsResponseOutputTypeDef",
+ListUserImportJobsResponseTypeDef = TypedDict(
+    "ListUserImportJobsResponseTypeDef",
     {
-        "UserImportJobs": List[UserImportJobTypeOutputTypeDef],
+        "UserImportJobs": List[UserImportJobTypeTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartUserImportJobResponseOutputTypeDef = TypedDict(
-    "StartUserImportJobResponseOutputTypeDef",
+StartUserImportJobResponseTypeDef = TypedDict(
+    "StartUserImportJobResponseTypeDef",
     {
-        "UserImportJob": UserImportJobTypeOutputTypeDef,
+        "UserImportJob": UserImportJobTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StopUserImportJobResponseOutputTypeDef = TypedDict(
-    "StopUserImportJobResponseOutputTypeDef",
+StopUserImportJobResponseTypeDef = TypedDict(
+    "StopUserImportJobResponseTypeDef",
     {
-        "UserImportJob": UserImportJobTypeOutputTypeDef,
+        "UserImportJob": UserImportJobTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUserPoolClientRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserPoolClientRequestRequestTypeDef",
     {
@@ -3055,16 +3055,16 @@
     {
         "SmsAuthenticationMessage": str,
         "SmsConfiguration": SmsConfigurationTypeTypeDef,
     },
     total=False,
 )
 
-DomainDescriptionTypeOutputTypeDef = TypedDict(
-    "DomainDescriptionTypeOutputTypeDef",
+DomainDescriptionTypeTypeDef = TypedDict(
+    "DomainDescriptionTypeTypeDef",
     {
         "UserPoolId": str,
         "AWSAccountId": str,
         "Domain": str,
         "S3Bucket": str,
         "CloudFrontDistribution": str,
         "Version": str,
@@ -3108,43 +3108,43 @@
         "CustomSMSSender": CustomSMSLambdaVersionConfigTypeTypeDef,
         "CustomEmailSender": CustomEmailLambdaVersionConfigTypeTypeDef,
         "KMSKeyID": str,
     },
     total=False,
 )
 
-GetUICustomizationResponseOutputTypeDef = TypedDict(
-    "GetUICustomizationResponseOutputTypeDef",
+GetUICustomizationResponseTypeDef = TypedDict(
+    "GetUICustomizationResponseTypeDef",
     {
-        "UICustomization": UICustomizationTypeOutputTypeDef,
+        "UICustomization": UICustomizationTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SetUICustomizationResponseOutputTypeDef = TypedDict(
-    "SetUICustomizationResponseOutputTypeDef",
+SetUICustomizationResponseTypeDef = TypedDict(
+    "SetUICustomizationResponseTypeDef",
     {
-        "UICustomization": UICustomizationTypeOutputTypeDef,
+        "UICustomization": UICustomizationTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListIdentityProvidersResponseOutputTypeDef = TypedDict(
-    "ListIdentityProvidersResponseOutputTypeDef",
+ListIdentityProvidersResponseTypeDef = TypedDict(
+    "ListIdentityProvidersResponseTypeDef",
     {
-        "Providers": List[ProviderDescriptionOutputTypeDef],
+        "Providers": List[ProviderDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUserPoolClientsResponseOutputTypeDef = TypedDict(
-    "ListUserPoolClientsResponseOutputTypeDef",
+ListUserPoolClientsResponseTypeDef = TypedDict(
+    "ListUserPoolClientsResponseTypeDef",
     {
-        "UserPoolClients": List[UserPoolClientDescriptionOutputTypeDef],
+        "UserPoolClients": List[UserPoolClientDescriptionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotifyConfigurationTypeOutputTypeDef = TypedDict(
     "NotifyConfigurationTypeOutputTypeDef",
@@ -3192,16 +3192,16 @@
     "UserPoolPolicyTypeTypeDef",
     {
         "PasswordPolicy": PasswordPolicyTypeTypeDef,
     },
     total=False,
 )
 
-ResourceServerTypeOutputTypeDef = TypedDict(
-    "ResourceServerTypeOutputTypeDef",
+ResourceServerTypeTypeDef = TypedDict(
+    "ResourceServerTypeTypeDef",
     {
         "UserPoolId": str,
         "Identifier": str,
         "Name": str,
         "Scopes": List[ResourceServerScopeTypeOutputTypeDef],
     },
 )
@@ -3237,16 +3237,16 @@
     "SmsMfaConfigTypeOutputTypeDef",
     {
         "SmsAuthenticationMessage": str,
         "SmsConfiguration": SmsConfigurationTypeOutputTypeDef,
     },
 )
 
-UserPoolClientTypeOutputTypeDef = TypedDict(
-    "UserPoolClientTypeOutputTypeDef",
+UserPoolClientTypeTypeDef = TypedDict(
+    "UserPoolClientTypeTypeDef",
     {
         "UserPoolId": str,
         "ClientName": str,
         "ClientId": str,
         "ClientSecret": str,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
@@ -3268,123 +3268,123 @@
         "PreventUserExistenceErrors": PreventUserExistenceErrorTypesType,
         "EnableTokenRevocation": bool,
         "EnablePropagateAdditionalUserContextData": bool,
         "AuthSessionValidity": int,
     },
 )
 
-AdminGetDeviceResponseOutputTypeDef = TypedDict(
-    "AdminGetDeviceResponseOutputTypeDef",
+AdminGetDeviceResponseTypeDef = TypedDict(
+    "AdminGetDeviceResponseTypeDef",
     {
-        "Device": DeviceTypeOutputTypeDef,
+        "Device": DeviceTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminListDevicesResponseOutputTypeDef = TypedDict(
-    "AdminListDevicesResponseOutputTypeDef",
+AdminListDevicesResponseTypeDef = TypedDict(
+    "AdminListDevicesResponseTypeDef",
     {
-        "Devices": List[DeviceTypeOutputTypeDef],
+        "Devices": List[DeviceTypeTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetDeviceResponseOutputTypeDef = TypedDict(
-    "GetDeviceResponseOutputTypeDef",
+GetDeviceResponseTypeDef = TypedDict(
+    "GetDeviceResponseTypeDef",
     {
-        "Device": DeviceTypeOutputTypeDef,
+        "Device": DeviceTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDevicesResponseOutputTypeDef = TypedDict(
-    "ListDevicesResponseOutputTypeDef",
+ListDevicesResponseTypeDef = TypedDict(
+    "ListDevicesResponseTypeDef",
     {
-        "Devices": List[DeviceTypeOutputTypeDef],
+        "Devices": List[DeviceTypeTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminCreateUserResponseOutputTypeDef = TypedDict(
-    "AdminCreateUserResponseOutputTypeDef",
+AdminCreateUserResponseTypeDef = TypedDict(
+    "AdminCreateUserResponseTypeDef",
     {
-        "User": UserTypeOutputTypeDef,
+        "User": UserTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUsersInGroupResponseOutputTypeDef = TypedDict(
-    "ListUsersInGroupResponseOutputTypeDef",
+ListUsersInGroupResponseTypeDef = TypedDict(
+    "ListUsersInGroupResponseTypeDef",
     {
-        "Users": List[UserTypeOutputTypeDef],
+        "Users": List[UserTypeTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUsersResponseOutputTypeDef = TypedDict(
-    "ListUsersResponseOutputTypeDef",
+ListUsersResponseTypeDef = TypedDict(
+    "ListUsersResponseTypeDef",
     {
-        "Users": List[UserTypeOutputTypeDef],
+        "Users": List[UserTypeTypeDef],
         "PaginationToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminListUserAuthEventsResponseOutputTypeDef = TypedDict(
-    "AdminListUserAuthEventsResponseOutputTypeDef",
+AdminListUserAuthEventsResponseTypeDef = TypedDict(
+    "AdminListUserAuthEventsResponseTypeDef",
     {
-        "AuthEvents": List[AuthEventTypeOutputTypeDef],
+        "AuthEvents": List[AuthEventTypeTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminInitiateAuthResponseOutputTypeDef = TypedDict(
-    "AdminInitiateAuthResponseOutputTypeDef",
+AdminInitiateAuthResponseTypeDef = TypedDict(
+    "AdminInitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
-        "AuthenticationResult": AuthenticationResultTypeOutputTypeDef,
+        "AuthenticationResult": AuthenticationResultTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdminRespondToAuthChallengeResponseOutputTypeDef = TypedDict(
-    "AdminRespondToAuthChallengeResponseOutputTypeDef",
+AdminRespondToAuthChallengeResponseTypeDef = TypedDict(
+    "AdminRespondToAuthChallengeResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
-        "AuthenticationResult": AuthenticationResultTypeOutputTypeDef,
+        "AuthenticationResult": AuthenticationResultTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InitiateAuthResponseOutputTypeDef = TypedDict(
-    "InitiateAuthResponseOutputTypeDef",
+InitiateAuthResponseTypeDef = TypedDict(
+    "InitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
-        "AuthenticationResult": AuthenticationResultTypeOutputTypeDef,
+        "AuthenticationResult": AuthenticationResultTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RespondToAuthChallengeResponseOutputTypeDef = TypedDict(
-    "RespondToAuthChallengeResponseOutputTypeDef",
+RespondToAuthChallengeResponseTypeDef = TypedDict(
+    "RespondToAuthChallengeResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
-        "AuthenticationResult": AuthenticationResultTypeOutputTypeDef,
+        "AuthenticationResult": AuthenticationResultTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAdminInitiateAuthRequestRequestTypeDef = TypedDict(
     "_RequiredAdminInitiateAuthRequestRequestTypeDef",
     {
@@ -3453,24 +3453,24 @@
 
 class SetUserPoolMfaConfigRequestRequestTypeDef(
     _RequiredSetUserPoolMfaConfigRequestRequestTypeDef,
     _OptionalSetUserPoolMfaConfigRequestRequestTypeDef,
 ):
     pass
 
-DescribeUserPoolDomainResponseOutputTypeDef = TypedDict(
-    "DescribeUserPoolDomainResponseOutputTypeDef",
+DescribeUserPoolDomainResponseTypeDef = TypedDict(
+    "DescribeUserPoolDomainResponseTypeDef",
     {
-        "DomainDescription": DomainDescriptionTypeOutputTypeDef,
+        "DomainDescription": DomainDescriptionTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UserPoolDescriptionTypeOutputTypeDef = TypedDict(
-    "UserPoolDescriptionTypeOutputTypeDef",
+UserPoolDescriptionTypeTypeDef = TypedDict(
+    "UserPoolDescriptionTypeTypeDef",
     {
         "Id": str,
         "Name": str,
         "LambdaConfig": LambdaConfigTypeOutputTypeDef,
         "Status": StatusTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
@@ -3537,49 +3537,49 @@
 )
 
 class UpdateUserPoolRequestRequestTypeDef(
     _RequiredUpdateUserPoolRequestRequestTypeDef, _OptionalUpdateUserPoolRequestRequestTypeDef
 ):
     pass
 
-CreateResourceServerResponseOutputTypeDef = TypedDict(
-    "CreateResourceServerResponseOutputTypeDef",
+CreateResourceServerResponseTypeDef = TypedDict(
+    "CreateResourceServerResponseTypeDef",
     {
-        "ResourceServer": ResourceServerTypeOutputTypeDef,
+        "ResourceServer": ResourceServerTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeResourceServerResponseOutputTypeDef = TypedDict(
-    "DescribeResourceServerResponseOutputTypeDef",
+DescribeResourceServerResponseTypeDef = TypedDict(
+    "DescribeResourceServerResponseTypeDef",
     {
-        "ResourceServer": ResourceServerTypeOutputTypeDef,
+        "ResourceServer": ResourceServerTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListResourceServersResponseOutputTypeDef = TypedDict(
-    "ListResourceServersResponseOutputTypeDef",
+ListResourceServersResponseTypeDef = TypedDict(
+    "ListResourceServersResponseTypeDef",
     {
-        "ResourceServers": List[ResourceServerTypeOutputTypeDef],
+        "ResourceServers": List[ResourceServerTypeTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateResourceServerResponseOutputTypeDef = TypedDict(
-    "UpdateResourceServerResponseOutputTypeDef",
+UpdateResourceServerResponseTypeDef = TypedDict(
+    "UpdateResourceServerResponseTypeDef",
     {
-        "ResourceServer": ResourceServerTypeOutputTypeDef,
+        "ResourceServer": ResourceServerTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UserPoolTypeOutputTypeDef = TypedDict(
-    "UserPoolTypeOutputTypeDef",
+UserPoolTypeTypeDef = TypedDict(
+    "UserPoolTypeTypeDef",
     {
         "Id": str,
         "Name": str,
         "Policies": UserPoolPolicyTypeOutputTypeDef,
         "DeletionProtection": DeletionProtectionTypeType,
         "LambdaConfig": LambdaConfigTypeOutputTypeDef,
         "Status": StatusTypeType,
@@ -3657,69 +3657,69 @@
 )
 
 class CreateUserPoolRequestRequestTypeDef(
     _RequiredCreateUserPoolRequestRequestTypeDef, _OptionalCreateUserPoolRequestRequestTypeDef
 ):
     pass
 
-GetUserPoolMfaConfigResponseOutputTypeDef = TypedDict(
-    "GetUserPoolMfaConfigResponseOutputTypeDef",
+GetUserPoolMfaConfigResponseTypeDef = TypedDict(
+    "GetUserPoolMfaConfigResponseTypeDef",
     {
         "SmsMfaConfiguration": SmsMfaConfigTypeOutputTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeOutputTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SetUserPoolMfaConfigResponseOutputTypeDef = TypedDict(
-    "SetUserPoolMfaConfigResponseOutputTypeDef",
+SetUserPoolMfaConfigResponseTypeDef = TypedDict(
+    "SetUserPoolMfaConfigResponseTypeDef",
     {
         "SmsMfaConfiguration": SmsMfaConfigTypeOutputTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeOutputTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateUserPoolClientResponseOutputTypeDef = TypedDict(
-    "CreateUserPoolClientResponseOutputTypeDef",
+CreateUserPoolClientResponseTypeDef = TypedDict(
+    "CreateUserPoolClientResponseTypeDef",
     {
-        "UserPoolClient": UserPoolClientTypeOutputTypeDef,
+        "UserPoolClient": UserPoolClientTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeUserPoolClientResponseOutputTypeDef = TypedDict(
-    "DescribeUserPoolClientResponseOutputTypeDef",
+DescribeUserPoolClientResponseTypeDef = TypedDict(
+    "DescribeUserPoolClientResponseTypeDef",
     {
-        "UserPoolClient": UserPoolClientTypeOutputTypeDef,
+        "UserPoolClient": UserPoolClientTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateUserPoolClientResponseOutputTypeDef = TypedDict(
-    "UpdateUserPoolClientResponseOutputTypeDef",
+UpdateUserPoolClientResponseTypeDef = TypedDict(
+    "UpdateUserPoolClientResponseTypeDef",
     {
-        "UserPoolClient": UserPoolClientTypeOutputTypeDef,
+        "UserPoolClient": UserPoolClientTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListUserPoolsResponseOutputTypeDef = TypedDict(
-    "ListUserPoolsResponseOutputTypeDef",
+ListUserPoolsResponseTypeDef = TypedDict(
+    "ListUserPoolsResponseTypeDef",
     {
-        "UserPools": List[UserPoolDescriptionTypeOutputTypeDef],
+        "UserPools": List[UserPoolDescriptionTypeTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RiskConfigurationTypeOutputTypeDef = TypedDict(
-    "RiskConfigurationTypeOutputTypeDef",
+RiskConfigurationTypeTypeDef = TypedDict(
+    "RiskConfigurationTypeTypeDef",
     {
         "UserPoolId": str,
         "ClientId": str,
         "CompromisedCredentialsRiskConfiguration": (
             CompromisedCredentialsRiskConfigurationTypeOutputTypeDef
         ),
         "AccountTakeoverRiskConfiguration": AccountTakeoverRiskConfigurationTypeOutputTypeDef,
@@ -3749,38 +3749,38 @@
 
 class SetRiskConfigurationRequestRequestTypeDef(
     _RequiredSetRiskConfigurationRequestRequestTypeDef,
     _OptionalSetRiskConfigurationRequestRequestTypeDef,
 ):
     pass
 
-CreateUserPoolResponseOutputTypeDef = TypedDict(
-    "CreateUserPoolResponseOutputTypeDef",
+CreateUserPoolResponseTypeDef = TypedDict(
+    "CreateUserPoolResponseTypeDef",
     {
-        "UserPool": UserPoolTypeOutputTypeDef,
+        "UserPool": UserPoolTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeUserPoolResponseOutputTypeDef = TypedDict(
-    "DescribeUserPoolResponseOutputTypeDef",
+DescribeUserPoolResponseTypeDef = TypedDict(
+    "DescribeUserPoolResponseTypeDef",
     {
-        "UserPool": UserPoolTypeOutputTypeDef,
+        "UserPool": UserPoolTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeRiskConfigurationResponseOutputTypeDef = TypedDict(
-    "DescribeRiskConfigurationResponseOutputTypeDef",
+DescribeRiskConfigurationResponseTypeDef = TypedDict(
+    "DescribeRiskConfigurationResponseTypeDef",
     {
-        "RiskConfiguration": RiskConfigurationTypeOutputTypeDef,
+        "RiskConfiguration": RiskConfigurationTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SetRiskConfigurationResponseOutputTypeDef = TypedDict(
-    "SetRiskConfigurationResponseOutputTypeDef",
+SetRiskConfigurationResponseTypeDef = TypedDict(
+    "SetRiskConfigurationResponseTypeDef",
     {
-        "RiskConfiguration": RiskConfigurationTypeOutputTypeDef,
+        "RiskConfiguration": RiskConfigurationTypeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/PKG-INFO` & `mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-idp
-Version: 1.28.3.post1
-Summary: Type annotations for boto3.CognitoIdentityProvider 1.28.3 service generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3.CognitoIdentityProvider 1.28.3 service generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/
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
 [mypy-boto3-cognito-idp docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/).
 
 See how it helps to find and fix potential bugs:
 
@@ -418,46 +418,46 @@
     AdminGetUserRequestRequestTypeDef,
     AttributeTypeOutputTypeDef,
     MFAOptionTypeOutputTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AdminListDevicesRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     AdminListGroupsForUserRequestRequestTypeDef,
-    GroupTypeOutputTypeDef,
+    GroupTypeTypeDef,
     AdminListUserAuthEventsRequestRequestTypeDef,
     AdminRemoveUserFromGroupRequestRequestTypeDef,
     AdminResetUserPasswordRequestRequestTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
     AdminSetUserPasswordRequestRequestTypeDef,
     MFAOptionTypeTypeDef,
     AdminUpdateAuthEventFeedbackRequestRequestTypeDef,
     AdminUpdateDeviceStatusRequestRequestTypeDef,
     AdminUserGlobalSignOutRequestRequestTypeDef,
     AnalyticsConfigurationTypeOutputTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AssociateSoftwareTokenRequestRequestTypeDef,
-    ChallengeResponseTypeOutputTypeDef,
-    EventContextDataTypeOutputTypeDef,
-    EventFeedbackTypeOutputTypeDef,
-    EventRiskTypeOutputTypeDef,
-    NewDeviceMetadataTypeOutputTypeDef,
+    ChallengeResponseTypeTypeDef,
+    EventContextDataTypeTypeDef,
+    EventFeedbackTypeTypeDef,
+    EventRiskTypeTypeDef,
+    NewDeviceMetadataTypeTypeDef,
     ChangePasswordRequestRequestTypeDef,
-    CodeDeliveryDetailsTypeOutputTypeDef,
+    CodeDeliveryDetailsTypeTypeDef,
     CompromisedCredentialsActionsTypeOutputTypeDef,
     CompromisedCredentialsActionsTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
     UserContextDataTypeTypeDef,
     HttpHeaderTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
-    IdentityProviderTypeOutputTypeDef,
+    IdentityProviderTypeTypeDef,
     ResourceServerScopeTypeTypeDef,
     CreateUserImportJobRequestRequestTypeDef,
-    UserImportJobTypeOutputTypeDef,
+    UserImportJobTypeTypeDef,
     TokenValidityUnitsTypeTypeDef,
     CustomDomainConfigTypeTypeDef,
     DeviceConfigurationTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     SmsConfigurationTypeTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
@@ -488,29 +488,29 @@
     ForgetDeviceRequestRequestTypeDef,
     GetCSVHeaderRequestRequestTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GetIdentityProviderByIdentifierRequestRequestTypeDef,
     GetSigningCertificateRequestRequestTypeDef,
     GetUICustomizationRequestRequestTypeDef,
-    UICustomizationTypeOutputTypeDef,
+    UICustomizationTypeTypeDef,
     GetUserAttributeVerificationCodeRequestRequestTypeDef,
     GetUserPoolMfaConfigRequestRequestTypeDef,
     SoftwareTokenMfaConfigTypeOutputTypeDef,
     GetUserRequestRequestTypeDef,
     GlobalSignOutRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListGroupsRequestRequestTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
-    ProviderDescriptionOutputTypeDef,
+    ProviderDescriptionTypeDef,
     ListResourceServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListUserImportJobsRequestRequestTypeDef,
     ListUserPoolClientsRequestRequestTypeDef,
-    UserPoolClientDescriptionOutputTypeDef,
+    UserPoolClientDescriptionTypeDef,
     ListUserPoolsRequestRequestTypeDef,
     ListUsersInGroupRequestRequestTypeDef,
     ListUsersRequestRequestTypeDef,
     NotifyEmailTypeOutputTypeDef,
     NotifyEmailTypeTypeDef,
     NumberAttributeConstraintsTypeOutputTypeDef,
     NumberAttributeConstraintsTypeTypeDef,
@@ -545,136 +545,136 @@
     AccountTakeoverActionsTypeOutputTypeDef,
     AccountTakeoverActionsTypeTypeDef,
     AdminCreateUserConfigTypeOutputTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserRequestRequestTypeDef,
     AdminUpdateUserAttributesRequestRequestTypeDef,
     UpdateUserAttributesRequestRequestTypeDef,
-    AssociateSoftwareTokenResponseOutputTypeDef,
-    ConfirmDeviceResponseOutputTypeDef,
-    CreateUserPoolDomainResponseOutputTypeDef,
+    AssociateSoftwareTokenResponseTypeDef,
+    ConfirmDeviceResponseTypeDef,
+    CreateUserPoolDomainResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    GetCSVHeaderResponseOutputTypeDef,
-    GetSigningCertificateResponseOutputTypeDef,
-    ListTagsForResourceResponseOutputTypeDef,
-    UpdateUserPoolDomainResponseOutputTypeDef,
-    VerifySoftwareTokenResponseOutputTypeDef,
+    GetCSVHeaderResponseTypeDef,
+    GetSigningCertificateResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateUserPoolDomainResponseTypeDef,
+    VerifySoftwareTokenResponseTypeDef,
     AdminDisableProviderForUserRequestRequestTypeDef,
     AdminLinkProviderForUserRequestRequestTypeDef,
-    DeviceTypeOutputTypeDef,
-    AdminGetUserResponseOutputTypeDef,
-    GetUserResponseOutputTypeDef,
-    UserTypeOutputTypeDef,
+    DeviceTypeTypeDef,
+    AdminGetUserResponseTypeDef,
+    GetUserResponseTypeDef,
+    UserTypeTypeDef,
     AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
     AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
     ListGroupsRequestListGroupsPaginateTypeDef,
     ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListResourceServersRequestListResourceServersPaginateTypeDef,
     ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
     ListUserPoolsRequestListUserPoolsPaginateTypeDef,
     ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
     ListUsersRequestListUsersPaginateTypeDef,
-    AdminListGroupsForUserResponseOutputTypeDef,
-    CreateGroupResponseOutputTypeDef,
-    GetGroupResponseOutputTypeDef,
-    ListGroupsResponseOutputTypeDef,
-    UpdateGroupResponseOutputTypeDef,
+    AdminListGroupsForUserResponseTypeDef,
+    CreateGroupResponseTypeDef,
+    GetGroupResponseTypeDef,
+    ListGroupsResponseTypeDef,
+    UpdateGroupResponseTypeDef,
     AdminSetUserMFAPreferenceRequestRequestTypeDef,
     SetUserMFAPreferenceRequestRequestTypeDef,
     AdminSetUserSettingsRequestRequestTypeDef,
     SetUserSettingsRequestRequestTypeDef,
-    AuthEventTypeOutputTypeDef,
-    AuthenticationResultTypeOutputTypeDef,
-    ForgotPasswordResponseOutputTypeDef,
-    GetUserAttributeVerificationCodeResponseOutputTypeDef,
-    ResendConfirmationCodeResponseOutputTypeDef,
-    SignUpResponseOutputTypeDef,
-    UpdateUserAttributesResponseOutputTypeDef,
+    AuthEventTypeTypeDef,
+    AuthenticationResultTypeTypeDef,
+    ForgotPasswordResponseTypeDef,
+    GetUserAttributeVerificationCodeResponseTypeDef,
+    ResendConfirmationCodeResponseTypeDef,
+    SignUpResponseTypeDef,
+    UpdateUserAttributesResponseTypeDef,
     CompromisedCredentialsRiskConfigurationTypeOutputTypeDef,
     CompromisedCredentialsRiskConfigurationTypeTypeDef,
     ConfirmDeviceRequestRequestTypeDef,
     ConfirmForgotPasswordRequestRequestTypeDef,
     ConfirmSignUpRequestRequestTypeDef,
     ForgotPasswordRequestRequestTypeDef,
     InitiateAuthRequestRequestTypeDef,
     ResendConfirmationCodeRequestRequestTypeDef,
     RespondToAuthChallengeRequestRequestTypeDef,
     SignUpRequestRequestTypeDef,
     ContextDataTypeTypeDef,
-    CreateIdentityProviderResponseOutputTypeDef,
-    DescribeIdentityProviderResponseOutputTypeDef,
-    GetIdentityProviderByIdentifierResponseOutputTypeDef,
-    UpdateIdentityProviderResponseOutputTypeDef,
+    CreateIdentityProviderResponseTypeDef,
+    DescribeIdentityProviderResponseTypeDef,
+    GetIdentityProviderByIdentifierResponseTypeDef,
+    UpdateIdentityProviderResponseTypeDef,
     CreateResourceServerRequestRequestTypeDef,
     UpdateResourceServerRequestRequestTypeDef,
-    CreateUserImportJobResponseOutputTypeDef,
-    DescribeUserImportJobResponseOutputTypeDef,
-    ListUserImportJobsResponseOutputTypeDef,
-    StartUserImportJobResponseOutputTypeDef,
-    StopUserImportJobResponseOutputTypeDef,
+    CreateUserImportJobResponseTypeDef,
+    DescribeUserImportJobResponseTypeDef,
+    ListUserImportJobsResponseTypeDef,
+    StartUserImportJobResponseTypeDef,
+    StopUserImportJobResponseTypeDef,
     CreateUserPoolClientRequestRequestTypeDef,
     UpdateUserPoolClientRequestRequestTypeDef,
     CreateUserPoolDomainRequestRequestTypeDef,
     UpdateUserPoolDomainRequestRequestTypeDef,
     SmsMfaConfigTypeTypeDef,
-    DomainDescriptionTypeOutputTypeDef,
+    DomainDescriptionTypeTypeDef,
     LambdaConfigTypeOutputTypeDef,
     LambdaConfigTypeTypeDef,
-    GetUICustomizationResponseOutputTypeDef,
-    SetUICustomizationResponseOutputTypeDef,
-    ListIdentityProvidersResponseOutputTypeDef,
-    ListUserPoolClientsResponseOutputTypeDef,
+    GetUICustomizationResponseTypeDef,
+    SetUICustomizationResponseTypeDef,
+    ListIdentityProvidersResponseTypeDef,
+    ListUserPoolClientsResponseTypeDef,
     NotifyConfigurationTypeOutputTypeDef,
     NotifyConfigurationTypeTypeDef,
     UserPoolPolicyTypeOutputTypeDef,
     UserPoolPolicyTypeTypeDef,
-    ResourceServerTypeOutputTypeDef,
+    ResourceServerTypeTypeDef,
     SchemaAttributeTypeOutputTypeDef,
     SchemaAttributeTypeTypeDef,
     SmsMfaConfigTypeOutputTypeDef,
-    UserPoolClientTypeOutputTypeDef,
-    AdminGetDeviceResponseOutputTypeDef,
-    AdminListDevicesResponseOutputTypeDef,
-    GetDeviceResponseOutputTypeDef,
-    ListDevicesResponseOutputTypeDef,
-    AdminCreateUserResponseOutputTypeDef,
-    ListUsersInGroupResponseOutputTypeDef,
-    ListUsersResponseOutputTypeDef,
-    AdminListUserAuthEventsResponseOutputTypeDef,
-    AdminInitiateAuthResponseOutputTypeDef,
-    AdminRespondToAuthChallengeResponseOutputTypeDef,
-    InitiateAuthResponseOutputTypeDef,
-    RespondToAuthChallengeResponseOutputTypeDef,
+    UserPoolClientTypeTypeDef,
+    AdminGetDeviceResponseTypeDef,
+    AdminListDevicesResponseTypeDef,
+    GetDeviceResponseTypeDef,
+    ListDevicesResponseTypeDef,
+    AdminCreateUserResponseTypeDef,
+    ListUsersInGroupResponseTypeDef,
+    ListUsersResponseTypeDef,
+    AdminListUserAuthEventsResponseTypeDef,
+    AdminInitiateAuthResponseTypeDef,
+    AdminRespondToAuthChallengeResponseTypeDef,
+    InitiateAuthResponseTypeDef,
+    RespondToAuthChallengeResponseTypeDef,
     AdminInitiateAuthRequestRequestTypeDef,
     AdminRespondToAuthChallengeRequestRequestTypeDef,
     SetUserPoolMfaConfigRequestRequestTypeDef,
-    DescribeUserPoolDomainResponseOutputTypeDef,
-    UserPoolDescriptionTypeOutputTypeDef,
+    DescribeUserPoolDomainResponseTypeDef,
+    UserPoolDescriptionTypeTypeDef,
     AccountTakeoverRiskConfigurationTypeOutputTypeDef,
     AccountTakeoverRiskConfigurationTypeTypeDef,
     UpdateUserPoolRequestRequestTypeDef,
-    CreateResourceServerResponseOutputTypeDef,
-    DescribeResourceServerResponseOutputTypeDef,
-    ListResourceServersResponseOutputTypeDef,
-    UpdateResourceServerResponseOutputTypeDef,
-    UserPoolTypeOutputTypeDef,
+    CreateResourceServerResponseTypeDef,
+    DescribeResourceServerResponseTypeDef,
+    ListResourceServersResponseTypeDef,
+    UpdateResourceServerResponseTypeDef,
+    UserPoolTypeTypeDef,
     AddCustomAttributesRequestRequestTypeDef,
     CreateUserPoolRequestRequestTypeDef,
-    GetUserPoolMfaConfigResponseOutputTypeDef,
-    SetUserPoolMfaConfigResponseOutputTypeDef,
-    CreateUserPoolClientResponseOutputTypeDef,
-    DescribeUserPoolClientResponseOutputTypeDef,
-    UpdateUserPoolClientResponseOutputTypeDef,
-    ListUserPoolsResponseOutputTypeDef,
-    RiskConfigurationTypeOutputTypeDef,
+    GetUserPoolMfaConfigResponseTypeDef,
+    SetUserPoolMfaConfigResponseTypeDef,
+    CreateUserPoolClientResponseTypeDef,
+    DescribeUserPoolClientResponseTypeDef,
+    UpdateUserPoolClientResponseTypeDef,
+    ListUserPoolsResponseTypeDef,
+    RiskConfigurationTypeTypeDef,
     SetRiskConfigurationRequestRequestTypeDef,
-    CreateUserPoolResponseOutputTypeDef,
-    DescribeUserPoolResponseOutputTypeDef,
-    DescribeRiskConfigurationResponseOutputTypeDef,
-    SetRiskConfigurationResponseOutputTypeDef,
+    CreateUserPoolResponseTypeDef,
+    DescribeUserPoolResponseTypeDef,
+    DescribeRiskConfigurationResponseTypeDef,
+    SetRiskConfigurationResponseTypeDef,
 )
 
 
 def get_structure() -> RecoveryOptionTypeOutputTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-cognito-idp-1.28.3.post1/mypy_boto3_cognito_idp.egg-info/SOURCES.txt` & `mypy-boto3-cognito-idp-1.28.3.post2/mypy_boto3_cognito_idp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.3.post1/setup.py` & `mypy-boto3-cognito-idp-1.28.3.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cognito-idp",
-    version="1.28.3.post1",
+    version="1.28.3.post2",
     packages=["mypy_boto3_cognito_idp"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for boto3.CognitoIdentityProvider 1.28.3 service generated with"
-        " mypy-boto3-builder 7.14.7"
+        " mypy-boto3-builder 7.15.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

