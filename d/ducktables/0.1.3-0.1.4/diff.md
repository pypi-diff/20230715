# Comparing `tmp/ducktables-0.1.3.tar.gz` & `tmp/ducktables-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ducktables-0.1.3.tar", last modified: Wed Jun  7 20:25:06 2023, max compression
+gzip compressed data, was "ducktables-0.1.4.tar", last modified: Sat Jul 15 04:20:41 2023, max compression
```

## Comparing `ducktables-0.1.3.tar` & `ducktables-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-06-07 20:25:06.162996 ducktables-0.1.3/
--rw-rw-r--   0 mark      (4000) mark      (4000)     7625 2023-06-07 20:25:06.158996 ducktables-0.1.3/PKG-INFO
--rw-rw-r--   0 mark      (4000) mark      (4000)     6364 2023-06-07 20:22:38.000000 ducktables-0.1.3/README.md
-drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-06-07 20:25:06.158996 ducktables-0.1.3/ducktables/
--rw-rw-r--   0 mark      (4000) mark      (4000)        3 2023-05-26 22:15:50.000000 ducktables-0.1.3/ducktables/__init__.py
--rw-rw-r--   0 mark      (4000) mark      (4000)     3915 2023-06-07 20:22:38.000000 ducktables-0.1.3/ducktables/aws.py
--rw-rw-r--   0 mark      (4000) mark      (4000)      358 2023-05-23 17:02:10.000000 ducktables-0.1.3/ducktables/github.py
-drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-06-07 20:25:06.158996 ducktables-0.1.3/ducktables/google/
--rw-rw-r--   0 mark      (4000) mark      (4000)     3917 2023-06-07 20:22:38.000000 ducktables-0.1.3/ducktables/google/__init__.py
--rw-rw-r--   0 mark      (4000) mark      (4000)     3479 2023-05-19 19:34:59.000000 ducktables-0.1.3/ducktables/google/analytics.py
--rw-rw-r--   0 mark      (4000) mark      (4000)     1044 2023-06-07 20:22:38.000000 ducktables-0.1.3/ducktables/openai.py
-drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-06-07 20:25:06.158996 ducktables-0.1.3/ducktables.egg-info/
--rw-rw-r--   0 mark      (4000) mark      (4000)     7625 2023-06-07 20:25:06.000000 ducktables-0.1.3/ducktables.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (4000) mark      (4000)      331 2023-06-07 20:25:06.000000 ducktables-0.1.3/ducktables.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (4000) mark      (4000)        1 2023-06-07 20:25:06.000000 ducktables-0.1.3/ducktables.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (4000) mark      (4000)      267 2023-06-07 20:25:06.000000 ducktables-0.1.3/ducktables.egg-info/requires.txt
--rw-rw-r--   0 mark      (4000) mark      (4000)       11 2023-06-07 20:25:06.000000 ducktables-0.1.3/ducktables.egg-info/top_level.txt
--rw-rw-r--   0 mark      (4000) mark      (4000)       38 2023-06-07 20:25:06.162996 ducktables-0.1.3/setup.cfg
--rw-rw-r--   0 mark      (4000) mark      (4000)      543 2023-06-07 20:24:40.000000 ducktables-0.1.3/setup.py
+drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-07-15 04:20:41.662872 ducktables-0.1.4/
+-rw-rw-r--   0 mark      (4000) mark      (4000)     7210 2023-07-15 04:20:41.662872 ducktables-0.1.4/PKG-INFO
+-rw-rw-r--   0 mark      (4000) mark      (4000)     5997 2023-07-14 22:29:19.000000 ducktables-0.1.4/README.md
+drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-07-15 04:20:41.658872 ducktables-0.1.4/ducktables/
+-rw-rw-r--   0 mark      (4000) mark      (4000)     2342 2023-07-14 19:54:14.000000 ducktables-0.1.4/ducktables/__init__.py
+-rw-rw-r--   0 mark      (4000) mark      (4000)     3692 2023-07-14 19:54:14.000000 ducktables-0.1.4/ducktables/aws.py
+-rw-rw-r--   0 mark      (4000) mark      (4000)     2543 2023-07-14 22:51:22.000000 ducktables-0.1.4/ducktables/github.py
+drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-07-15 04:20:41.658872 ducktables-0.1.4/ducktables/google/
+-rw-rw-r--   0 mark      (4000) mark      (4000)     3917 2023-06-16 22:18:31.000000 ducktables-0.1.4/ducktables/google/__init__.py
+-rw-rw-r--   0 mark      (4000) mark      (4000)     3479 2023-05-19 19:34:59.000000 ducktables-0.1.4/ducktables/google/analytics.py
+-rw-rw-r--   0 mark      (4000) mark      (4000)     1052 2023-07-14 19:54:14.000000 ducktables-0.1.4/ducktables/openai.py
+drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-07-15 04:20:41.658872 ducktables-0.1.4/ducktables.egg-info/
+-rw-rw-r--   0 mark      (4000) mark      (4000)     7210 2023-07-15 04:20:41.000000 ducktables-0.1.4/ducktables.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (4000) mark      (4000)      331 2023-07-15 04:20:41.000000 ducktables-0.1.4/ducktables.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (4000) mark      (4000)        1 2023-07-15 04:20:41.000000 ducktables-0.1.4/ducktables.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (4000) mark      (4000)      267 2023-07-15 04:20:41.000000 ducktables-0.1.4/ducktables.egg-info/requires.txt
+-rw-rw-r--   0 mark      (4000) mark      (4000)       11 2023-07-15 04:20:41.000000 ducktables-0.1.4/ducktables.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (4000) mark      (4000)       38 2023-07-15 04:20:41.662872 ducktables-0.1.4/setup.cfg
+-rw-rw-r--   0 mark      (4000) mark      (4000)      543 2023-06-16 22:18:31.000000 ducktables-0.1.4/setup.py
```

### Comparing `ducktables-0.1.3/PKG-INFO` & `ducktables-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ducktables
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python Table Functions for DuckDB
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # DuckTables: Python Functions for DuckDB
         
         DuckTables is Python library that provides out of the box functions for the [DuckDB PyTables](https://github.com/MarkRoddy/duckdb-pytables) extension.
         
@@ -50,65 +50,59 @@
         These queries assume you've already installed the [PyTables](https://github.com/MarkRoddy/duckdb-pytables) extension in a DuckDB session. See the extensions [installation guide](https://github.com/MarkRoddy/duckdb-pytables#installation) if you have not.
         
         ## AWS
         Note that all queries will assume to run in the region you have specified in your configuration file. Set the `AWS_DEFAULT_REGION` to override this behavior.
         ### EC2 Instances
         Returns the results of a [DescribeInstances](https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstances.html) API call.
         ```sql
-            SELECT * FROM pytable('aws:ec2_instances',
-              columns = {
-                'instance_id': 'VARCHAR',
-                'name': 'VARCHAR',
-                'instance_type': 'VARCHAR',
-                'state': 'VARCHAR',
-                'key_pair': 'VARCHAR',
-                'platform': 'VARCHAR',
-                'architecture': 'VARCHAR',
-                'vpc_id': 'VARCHAR',
-                'subnet_id': 'VARCHAR',
-                'public_dns': 'VARCHAR',
-                'public_ip': 'VARCHAR',
-                'private_dns': 'VARCHAR',
-                'private_ip': 'VARCHAR'
-                });
+            SELECT * FROM pytable('ducktables.aws:ec2_instances');
         ```
         
         ### S3 Buckets
         Returns the results of a [ListBuckets](https://docs.aws.amazon.com/AmazonS3/latest/API/API_ListBuckets.html) API call.
         ```SQL
-        SELECT * FROM pytable('aws:s3_buckets', 
-          columns={'name': 'VARCHAR', 'creation_date': 'VARCHAR'}
-        );
+        SELECT * FROM pytable('ducktables.aws:s3_buckets');
         ```
         
         ### S3 Objects
         This only includes metadata about the objects themselves, not their contents. See the [httpfs](https://duckdb.org/docs/guides/import/s3_import.html) DuckDB extension if you're interested in loading data from objects on S3.
         
         Note that the second argument, the prefix path, is optional and can be omitted.
         ```SQL
-        SELECT * FROM pytable('aws:s3_objects', 'bucket-name', 'foo/bar/prefix',
-          columns = { 'key': 'VARCHAR', 'last_modified': 'VARCHAR', 'size': 'INT', 'storage_class': 'VARCHAR'}
-        );
+        SELECT * FROM pytable('ducktables.aws:s3_objects', 'bucket-name', 'foo/bar/prefix');
         ```
         
         ## Github
+        
+        ### Repositories
         Enumerates all repositories for the named user or organization.
         ```SQL
-        SELECT * FROM pytable('ghub:repos_for', 'duckdb',
-          columns = {'repo': 'VARCHAR', 'description': 'VARCHAR', 'language': 'VARCHAR'}
-        );
+        SELECT * FROM pytable('ducktables.githb:repos_for', 'duckdb');
+        ```
+        
+        ### Workflows
+        Enumerate each Github Actions Workflow associated with a repository
+        ```SQL
+        SELECT * FROM pytable('ducktables.github:workflows', 'MarkRoddy/duckdb-pytables')
+        ```
+        
+        ### Workflow Runs
+        List each execution of every Github Actions Workflow run on a repository.
+        ```SQL
+        SELECT * FROM pytable('ducktables.github:workflow_runs', 'MarkRoddy/duckdb-pytables')
         ```
         
+        
+        
         ## Open AI
         
         ### ChatGPT
         Given a prompt and a number of desired responses, will generate a table with the model's response.
         ```SQL
-        SELECT * FROM pytable('chatgpt:prompt', 'Write a limerick poem about how much you love SQL', 2,
-          columns = {'index': 'INT','message': 'VARCHAR', 'message_role': 'VARCHAR', 'finish_reason': 'VARCHAR'},
+        SELECT * FROM pytable('chatgpt:prompt', 'Write a limerick poem about how much you love SQL', 2)
         );
         ```
         
         ## Google
         
         ### Sheets
         Pulls data from a Google Sheet. Note that you'll either need user account authorization, or if you use a service account, the
```

### Comparing `ducktables-0.1.3/README.md` & `ducktables-0.1.4/ducktables.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,132 +1,135 @@
-# DuckTables: Python Functions for DuckDB
-
-DuckTables is Python library that provides out of the box functions for the [DuckDB PyTables](https://github.com/MarkRoddy/duckdb-pytables) extension.
-
-
-# Installation
-
-```shell
-pip install ducktables
-```
-
-# Authentication
-DuckTables interacts with a number of different services, and each has their own authentication and configuration mechanism. Note that you only have to configure the services that you plan on using.
-
-## AWS
-Follow the [auth instructions](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/quickstart.html#configuration) for Boto3, the library that ducktables uses to interface with AWS apis. Note that if you're already using boto3 or the AWS CLI, your existing authentication configuration will be utilized, and you don't need to do anything.
-
-## Github
-When starting your DuckDB client (such as the DuckDB cli), set an environment variable named `GITHUB_ACCESS_TOKEN`. From the command line, this will look like:
-
-```shell
-GITHUB_ACCESS_TOKEN=<token> duckdb -unsigned
-```
-
-To obtain an API token, log into github.com, and create one [here](https://github.com/settings/tokens).
-
-## OpenAI
-To use OpenAI functions you will need a valid API key and organization id. If you're logged in, you can create an API key [here](https://platform.openai.com/account/api-keys), and your organization id can be found [here](https://platform.openai.com/account/org-settings).
-
-To specify these values, you'll need to set two environment variables when running DuckDB: `OPENAI_ORG_ID` and `OPENAI_API_KEY`. This may look something like:
-```shell
-OPENAI_ORG_ID=<orid> OPENAI_API_KEY=<apikey> duckdb -unsigned
-```
-
-## Google
-Google related functions assume you have a json applications credentials file on disk where you're running DuckDB. The user or service account assoicated with the file will need to have the necessary permissions to interact with services associated with any functions you may use.
-
-To specify the path to the credentials file, set an evironment variable named `GOOGLE_APPLICATION_CREDENTIALS` when running DuckDB. That may look something like:
-```shell
-GOOGLE_APPLICATION_CREDENTIALS=~/.gcloud/some-file.json duckdb -unsigned
-```
-
-# Example Queries
-These queries assume you've already installed the [PyTables](https://github.com/MarkRoddy/duckdb-pytables) extension in a DuckDB session. See the extensions [installation guide](https://github.com/MarkRoddy/duckdb-pytables#installation) if you have not.
-
-## AWS
-Note that all queries will assume to run in the region you have specified in your configuration file. Set the `AWS_DEFAULT_REGION` to override this behavior.
-### EC2 Instances
-Returns the results of a [DescribeInstances](https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstances.html) API call.
-```sql
-    SELECT * FROM pytable('aws:ec2_instances',
-      columns = {
-        'instance_id': 'VARCHAR',
-        'name': 'VARCHAR',
-        'instance_type': 'VARCHAR',
-        'state': 'VARCHAR',
-        'key_pair': 'VARCHAR',
-        'platform': 'VARCHAR',
-        'architecture': 'VARCHAR',
-        'vpc_id': 'VARCHAR',
-        'subnet_id': 'VARCHAR',
-        'public_dns': 'VARCHAR',
-        'public_ip': 'VARCHAR',
-        'private_dns': 'VARCHAR',
-        'private_ip': 'VARCHAR'
-        });
-```
-
-### S3 Buckets
-Returns the results of a [ListBuckets](https://docs.aws.amazon.com/AmazonS3/latest/API/API_ListBuckets.html) API call.
-```SQL
-SELECT * FROM pytable('aws:s3_buckets', 
-  columns={'name': 'VARCHAR', 'creation_date': 'VARCHAR'}
-);
-```
-
-### S3 Objects
-This only includes metadata about the objects themselves, not their contents. See the [httpfs](https://duckdb.org/docs/guides/import/s3_import.html) DuckDB extension if you're interested in loading data from objects on S3.
-
-Note that the second argument, the prefix path, is optional and can be omitted.
-```SQL
-SELECT * FROM pytable('aws:s3_objects', 'bucket-name', 'foo/bar/prefix',
-  columns = { 'key': 'VARCHAR', 'last_modified': 'VARCHAR', 'size': 'INT', 'storage_class': 'VARCHAR'}
-);
-```
-
-## Github
-Enumerates all repositories for the named user or organization.
-```SQL
-SELECT * FROM pytable('ghub:repos_for', 'duckdb',
-  columns = {'repo': 'VARCHAR', 'description': 'VARCHAR', 'language': 'VARCHAR'}
-);
-```
-
-## Open AI
-
-### ChatGPT
-Given a prompt and a number of desired responses, will generate a table with the model's response.
-```SQL
-SELECT * FROM pytable('chatgpt:prompt', 'Write a limerick poem about how much you love SQL', 2,
-  columns = {'index': 'INT','message': 'VARCHAR', 'message_role': 'VARCHAR', 'finish_reason': 'VARCHAR'},
-);
-```
-
-## Google
-
-### Sheets
-Pulls data from a Google Sheet. Note that you'll either need user account authorization, or if you use a service account, the
-account will need read permissions on the sheet in question if it is private.
-
-This example query pulls from a Google provided example spreadsheet. You can see the sheet [here](https://docs.google.com/spreadsheets/d/1BxiMVs0XRA5nFMdKvBdBZjgmUUqptlbs74OgvE2upms/edit#gid=0). Note that despite this sheet being public, you will still need Google Cloud authorization configured on your local machine.
-```SQL
-SELECT *
-FROM pytable('google:sheet', '1BxiMVs0XRA5nFMdKvBdBZjgmUUqptlbs74OgvE2upms', 'Class Data!A2:F31',
-  columns = {
-    'name': 'VARCHAR', 'gender': 'VARCHAR', 'class_level': 'VARCHAR',
-    'state': 'VARCHAR', 'major': 'VARCHAR', 'extracurricular': 'VARCHAR'}
-);
-```
-
-### Analytics
-This query has three required parameters. The ViewID you wish to query, and the start/end date range for your query. See [this post](https://stackoverflow.com/a/47921777) for an explanation of finding your view ID. Start and end dates should be strings in a 'YYYY-MM-DD' format. Note you can alos override the set of Dimensions and Metrics, but this requires understanding how to adjust the `columns` argument to account for the change in schema that will occur as a result.
-```SQL
-    SELECT * FROM pytable('ducktables.google.analytics:metrics', '<view-id>', '<start-date>', '<end-date>',
-      columns = {
-        -- Dimensions
-        'date': 'VARCHAR', 'hour': 'VARCHAR', 'pagePath': 'VARCHAR', 'source': 'VARCHAR', 'medium': 'VARCHAR',
-        -- Metrics
-        'sessions': 'INT', 'users': 'INT', 'pageviews': 'INT', 'avgSessionDuration': 'FLOAT', 'bounceRate': 'FLOAT'
-        });
-```
-
+Metadata-Version: 2.1
+Name: ducktables
+Version: 0.1.4
+Summary: Python Table Functions for DuckDB
+Home-page: UNKNOWN
+License: UNKNOWN
+Description: # DuckTables: Python Functions for DuckDB
+        
+        DuckTables is Python library that provides out of the box functions for the [DuckDB PyTables](https://github.com/MarkRoddy/duckdb-pytables) extension.
+        
+        
+        # Installation
+        
+        ```shell
+        pip install ducktables
+        ```
+        
+        # Authentication
+        DuckTables interacts with a number of different services, and each has their own authentication and configuration mechanism. Note that you only have to configure the services that you plan on using.
+        
+        ## AWS
+        Follow the [auth instructions](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/quickstart.html#configuration) for Boto3, the library that ducktables uses to interface with AWS apis. Note that if you're already using boto3 or the AWS CLI, your existing authentication configuration will be utilized, and you don't need to do anything.
+        
+        ## Github
+        When starting your DuckDB client (such as the DuckDB cli), set an environment variable named `GITHUB_ACCESS_TOKEN`. From the command line, this will look like:
+        
+        ```shell
+        GITHUB_ACCESS_TOKEN=<token> duckdb -unsigned
+        ```
+        
+        To obtain an API token, log into github.com, and create one [here](https://github.com/settings/tokens).
+        
+        ## OpenAI
+        To use OpenAI functions you will need a valid API key and organization id. If you're logged in, you can create an API key [here](https://platform.openai.com/account/api-keys), and your organization id can be found [here](https://platform.openai.com/account/org-settings).
+        
+        To specify these values, you'll need to set two environment variables when running DuckDB: `OPENAI_ORG_ID` and `OPENAI_API_KEY`. This may look something like:
+        ```shell
+        OPENAI_ORG_ID=<orid> OPENAI_API_KEY=<apikey> duckdb -unsigned
+        ```
+        
+        ## Google
+        Google related functions assume you have a json applications credentials file on disk where you're running DuckDB. The user or service account assoicated with the file will need to have the necessary permissions to interact with services associated with any functions you may use.
+        
+        To specify the path to the credentials file, set an evironment variable named `GOOGLE_APPLICATION_CREDENTIALS` when running DuckDB. That may look something like:
+        ```shell
+        GOOGLE_APPLICATION_CREDENTIALS=~/.gcloud/some-file.json duckdb -unsigned
+        ```
+        
+        # Example Queries
+        These queries assume you've already installed the [PyTables](https://github.com/MarkRoddy/duckdb-pytables) extension in a DuckDB session. See the extensions [installation guide](https://github.com/MarkRoddy/duckdb-pytables#installation) if you have not.
+        
+        ## AWS
+        Note that all queries will assume to run in the region you have specified in your configuration file. Set the `AWS_DEFAULT_REGION` to override this behavior.
+        ### EC2 Instances
+        Returns the results of a [DescribeInstances](https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeInstances.html) API call.
+        ```sql
+            SELECT * FROM pytable('ducktables.aws:ec2_instances');
+        ```
+        
+        ### S3 Buckets
+        Returns the results of a [ListBuckets](https://docs.aws.amazon.com/AmazonS3/latest/API/API_ListBuckets.html) API call.
+        ```SQL
+        SELECT * FROM pytable('ducktables.aws:s3_buckets');
+        ```
+        
+        ### S3 Objects
+        This only includes metadata about the objects themselves, not their contents. See the [httpfs](https://duckdb.org/docs/guides/import/s3_import.html) DuckDB extension if you're interested in loading data from objects on S3.
+        
+        Note that the second argument, the prefix path, is optional and can be omitted.
+        ```SQL
+        SELECT * FROM pytable('ducktables.aws:s3_objects', 'bucket-name', 'foo/bar/prefix');
+        ```
+        
+        ## Github
+        
+        ### Repositories
+        Enumerates all repositories for the named user or organization.
+        ```SQL
+        SELECT * FROM pytable('ducktables.githb:repos_for', 'duckdb');
+        ```
+        
+        ### Workflows
+        Enumerate each Github Actions Workflow associated with a repository
+        ```SQL
+        SELECT * FROM pytable('ducktables.github:workflows', 'MarkRoddy/duckdb-pytables')
+        ```
+        
+        ### Workflow Runs
+        List each execution of every Github Actions Workflow run on a repository.
+        ```SQL
+        SELECT * FROM pytable('ducktables.github:workflow_runs', 'MarkRoddy/duckdb-pytables')
+        ```
+        
+        
+        
+        ## Open AI
+        
+        ### ChatGPT
+        Given a prompt and a number of desired responses, will generate a table with the model's response.
+        ```SQL
+        SELECT * FROM pytable('chatgpt:prompt', 'Write a limerick poem about how much you love SQL', 2)
+        );
+        ```
+        
+        ## Google
+        
+        ### Sheets
+        Pulls data from a Google Sheet. Note that you'll either need user account authorization, or if you use a service account, the
+        account will need read permissions on the sheet in question if it is private.
+        
+        This example query pulls from a Google provided example spreadsheet. You can see the sheet [here](https://docs.google.com/spreadsheets/d/1BxiMVs0XRA5nFMdKvBdBZjgmUUqptlbs74OgvE2upms/edit#gid=0). Note that despite this sheet being public, you will still need Google Cloud authorization configured on your local machine.
+        ```SQL
+        SELECT *
+        FROM pytable('google:sheet', '1BxiMVs0XRA5nFMdKvBdBZjgmUUqptlbs74OgvE2upms', 'Class Data!A2:F31',
+          columns = {
+            'name': 'VARCHAR', 'gender': 'VARCHAR', 'class_level': 'VARCHAR',
+            'state': 'VARCHAR', 'major': 'VARCHAR', 'extracurricular': 'VARCHAR'}
+        );
+        ```
+        
+        ### Analytics
+        This query has three required parameters. The ViewID you wish to query, and the start/end date range for your query. See [this post](https://stackoverflow.com/a/47921777) for an explanation of finding your view ID. Start and end dates should be strings in a 'YYYY-MM-DD' format. Note you can alos override the set of Dimensions and Metrics, but this requires understanding how to adjust the `columns` argument to account for the change in schema that will occur as a result.
+        ```SQL
+            SELECT * FROM pytable('ducktables.google.analytics:metrics', '<view-id>', '<start-date>', '<end-date>',
+              columns = {
+                -- Dimensions
+                'date': 'VARCHAR', 'hour': 'VARCHAR', 'pagePath': 'VARCHAR', 'source': 'VARCHAR', 'medium': 'VARCHAR',
+                -- Metrics
+                'sessions': 'INT', 'users': 'INT', 'pageviews': 'INT', 'avgSessionDuration': 'FLOAT', 'bounceRate': 'FLOAT'
+                });
+        ```
+        
+        
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `ducktables-0.1.3/ducktables/aws.py` & `ducktables-0.1.4/ducktables/aws.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 
 import boto3
+from ducktables import ducktable
 
-
+_ec2_instances_schema = {
+    'instance_id': str,
+    'name': str,
+    'instance_type': str,
+    'state': str,
+    'key_pair': str,
+    'platform': str,
+    'architecture': str,
+    'vpc_id': str,
+    'subnet_id': str,
+    'public_dns': str,
+    'public_ip': str,
+    'private_dns': str,
+    'private_ip': str,
+    }
+@ducktable(**_ec2_instances_schema)
 def ec2_instances():
     """
     SQL Usage:
-    SELECT * FROM pytable('aws:ec2_instances',
-      columns = {
-        'instance_id': 'VARCHAR',
-        'name': 'VARCHAR',
-        'instance_type': 'VARCHAR',
-        'state': 'VARCHAR',
-        'key_pair': 'VARCHAR',
-        'platform': 'VARCHAR',
-        'architecture': 'VARCHAR',
-        'vpc_id': 'VARCHAR',
-        'subnet_id': 'VARCHAR',
-        'public_dns': 'VARCHAR',
-        'public_ip': 'VARCHAR',
-        'private_dns': 'VARCHAR',
-        'private_ip': 'VARCHAR'
-        });
+    SELECT * FROM pytable('aws:ec2_instances'));
     """
     def response_to_rows(response):
         for resv in response['Reservations']:
             resv_id = resv['ReservationId']
             instances = resv['Instances']
             for i in instances:
                 instance_name = None
@@ -55,38 +56,34 @@
     token = response.get('NextToken')
     while token:
         response = client.describe_instances(NextToken = token)
         yield from response_to_rows(response)
         token = response.get('NextToken')
         
         
-
+@ducktable(name = str, creation_date = str)
 def s3_buckets():
     """
     SQL Usage:
-    SELECT * FROM pytable('aws:s3_buckets', columns={'name': 'VARCHAR', 'creation_date': 'VARCHAR'});
+    SELECT * FROM pytable('aws:s3_buckets');
     """
     client = boto3.client('s3')
     response = client.list_buckets()
     for bucket in response['Buckets']:
         yield (bucket['Name'], bucket['CreationDate'].strftime('%m/%d/%Y'))
     
-
+@ducktable(key = str, last_modified = str, size = int, storage_class = str)
 def s3_objects(bucket, prefix = None):
     """
     SQL Usage:
-    SELECT * FROM pytable('aws:s3_objects', 'bucket-name', 'foo/bar/prefix',
-      columns = { 'key': 'VARCHAR', 'last_modified': 'VARCHAR', 'size': 'INT', 'storage_class': 'VARCHAR'}
-    );
+    SELECT * FROM pytable('aws:s3_objects', 'bucket-name', 'foo/bar/prefix');
 
     Note that the final prefix argument is optional, and you don't need to specify it in
     your SQL query. To list all objects:
-    SELECT * FROM python_table('aws', 's3_objects',
-      { 'key': 'VARCHAR', 'last_modified': 'VARCHAR', 'size': 'INT', 'storage_class': 'VARCHAR'},
-      ['bucket-name']);
+    SELECT * FROM pytable('aws:s3_objects', 'bucket-name');
     """
     def to_row(obj):
         return (obj['Key'],
                 obj['LastModified'].strftime('%m/%d/%Y'),
                 obj['Size'],
                 obj['StorageClass'])
```

### Comparing `ducktables-0.1.3/ducktables/google/__init__.py` & `ducktables-0.1.4/ducktables/google/__init__.py`

 * *Files identical despite different names*

### Comparing `ducktables-0.1.3/ducktables/google/analytics.py` & `ducktables-0.1.4/ducktables/google/analytics.py`

 * *Files identical despite different names*

### Comparing `ducktables-0.1.3/ducktables/openai.py` & `ducktables-0.1.4/ducktables/openai.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 import os, sys
 import openai
 
 openai.organization = os.getenv("OPENAI_ORG_ID")
 openai.api_key = os.getenv("OPENAI_API_KEY")
 
+from ducktables import ducktable
+
+@ducktable(index = int, message = str, message_role = str, finish_reason = str)
 def prompt(input_phrase, num_responses = 5):
     """
     SQL Usage:
-    SELECT * FROM pytable('chatgpt:prompt', 'Write a limerick poem about how much you love SQL', 2,
-      columns = {'index': 'INT','message': 'VARCHAR', 'message_role': 'VARCHAR', 'finish_reason': 'VARCHAR'},
-    );
+    SELECT * FROM pytable('ducktables.openai:prompt', 'Write a limerick poem about how much you love SQL', 2);
     """
     completion = openai.ChatCompletion.create(
         model="gpt-3.5-turbo",
         # Complains when getting int like things so we explicitly cast
         n = int(num_responses),
         messages=[
             {"role": "user", "content": input_phrase}
```

### Comparing `ducktables-0.1.3/setup.py` & `ducktables-0.1.4/setup.py`

 * *Files identical despite different names*

