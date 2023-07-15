# Comparing `tmp/mostats-1.0.6-py3-none-any.whl.zip` & `tmp/mostats-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 17134 bytes, number of entries: 8
+Zip file size: 18774 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 08:19 mostats/__init__.py
--rw-r--r--  2.0 unx     8340 b- defN 23-Jul-14 11:28 mostats/getCluster.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jul-14 11:32 mostats-1.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     3759 b- defN 23-Jul-14 11:32 mostats-1.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 11:32 mostats-1.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jul-14 11:32 mostats-1.0.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-14 11:32 mostats-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      632 b- defN 23-Jul-14 11:32 mostats-1.0.6.dist-info/RECORD
-8 files, 48032 bytes uncompressed, 16026 bytes compressed:  66.6%
+-rw-r--r--  2.0 unx    13141 b- defN 23-Jul-15 18:02 mostats/getCluster.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-15 18:12 mostats-1.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5555 b- defN 23-Jul-15 18:12 mostats-1.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-15 18:12 mostats-1.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-15 18:12 mostats-1.0.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-15 18:12 mostats-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      633 b- defN 23-Jul-15 18:12 mostats-1.0.7.dist-info/RECORD
+8 files, 54630 bytes uncompressed, 17666 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: mostats/__init__.py
 Comment: 
 
 Filename: mostats/getCluster.py
 Comment: 
 
-Filename: mostats-1.0.6.dist-info/LICENSE
+Filename: mostats-1.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: mostats-1.0.6.dist-info/METADATA
+Filename: mostats-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: mostats-1.0.6.dist-info/WHEEL
+Filename: mostats-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: mostats-1.0.6.dist-info/entry_points.txt
+Filename: mostats-1.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: mostats-1.0.6.dist-info/top_level.txt
+Filename: mostats-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: mostats-1.0.6.dist-info/RECORD
+Filename: mostats-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mostats/getCluster.py

```diff
@@ -1,85 +1,113 @@
 from pymongo import MongoClient
 from urllib.parse import urlparse
 import pandas as pd
 import csv
 import argparse
 import sys
 import os
+from openpyxl import load_workbook
 
 output = []
 cluster_stats = []
+db_sizing = []
 
 def main():
 
     argparser = argparse.ArgumentParser(description='Get the MongoDB database statistic '
-                                                    'to a local CSV file')
+                                                    'to an excel file')
     argparser.add_argument('-u', '--url', nargs='+', default="mongodb://127.0.0.1",
                             help='MongoDB cluster URL, default is "mongodb://127.0.0.1". \nExample: "mongodb+srv://<<username>>:<<password>>@cluster.zqqqy.mongodb.net/?retryWrites=true&w=majority". For multiple server please use the space and "" to seperate example:"mongodb+srv://<<username>>:<<password>>@cluster1.zqqqy.mongodb.net/?retryWrites=true&w=majority" "mongodb+srv://<<username>>:<<password>>@cluster2.zqqqy.mongodb.net/?retryWrites=true&w=majority" ')
-    argparser.add_argument('-c', '--csv', default="cluster-data.csv",
-                            help='CSV filename, default "cluster-data.csv" \n')
+    argparser.add_argument('-uf', '--urlfile', default="",
+                            help='Get the MongoDB cluster URL from a file. It will read each line as one MongoDB cluster URL')
+    argparser.add_argument('-e', '--excelfile', default="Cluster-info.xlsx",
+                            help='Excel filename, default "Cluster-info.xlsx" \n')
     argparser.add_argument('-n', '--name', nargs='+', default="",
                             help='Cluster name, default value first subdomain example: mongodb+srv://clustername.cl0.mongodb.net will be clustername. For multiple server please use the space and "" to seperate example:"cluster1" "cluster2"  \n')
+    argparser.add_argument('-nf', '--namefile', default="",
+                            help='Get the cluster name from a file. It will read each line as one cluster name \n')
     argparser.add_argument('-m', '--moreinfo', default=False,
                             help='Getting the host information, uptime, total number of command, read, and insert \n')
+    argparser.add_argument('-fa', '--fa', default="",
+                            help='Frequently access ratio in percent (input number only)\n')
+    argparser.add_argument('-iops', '--iops', default="",
+                            help='Expected IOPS\n')
     args = argparser.parse_args()
     
-    print('\nMostats - Get the MongoDB database statistic to a local CSV file\nPlease follow the instruction by run mostats -h\n')
+    print('\nMostats - Get the MongoDB database statistic to an excel file\nPlease follow the instruction by run mostats -h\n')
+
+    if args.namefile != "":
+        cname = read_file(args.namefile)
+    elif args.name != "": 
+        cname = args.name
+
+    if args.urlfile != "":
+        conn_pool = read_file(args.urlfile)          
+    else: 
+        conn_pool = args.url       
+
     if args.name == "":
-        print(f'Get the database information from : "{args.url}" and save to "{args.csv}"')
+        print(f'Get the database information from : "{conn_pool}" and save to "{args.excelfile}"')
     else:
-        print(f'Get the database information from : "{args.url}" with cluster name "{args.name}" and save to "{args.csv}"')
-    print('\n')
-    print("Please wait as it might take a while...")
-    conn_pool = args.url
+        print(f'Get the database information from : "{conn_pool}" with cluster name "{args.name}" and save to "{args.excelfile}"')
+    #print('\n')
+    print('\nPlease wait as it might take a while...')
+
     more_info = args.moreinfo
-    counter = 0    
+    counter = 0
+
+    if(len(conn_pool) != len(cname)) and (len(cname) >0 ):
+        raise Exception(f'The number of MongoDB URL "{len(conn_pool)}" doesnt match with the number of cluster name "{len(cname)}"')
+    
     try:
         for conn in conn_pool:
+            print(f'Getting database information from {conn}. Progress: {counter+1}/{len(conn_pool)}')
             totalindex = 0
             totalindexsize =0
+            totaluniqueindex =0
+            frequentlyaccess = 0
             totaldocuments = 0
             totalstoragesize = 0
             totalsize = 0            
             parsed_uri = urlparse(conn)
             if args.name == "":
                 cluster_name = parsed_uri.hostname.split('.')[0]
             else:
-                cluster_name = args.name[counter]
+                cluster_name = cname[counter]
             client = MongoClient(conn)
             if more_info:               
                 data = client.admin.command("hostInfo")
                 cstat = {
-                    "cluster_name" : cluster_name,
-                    "hostname" : data["system"]["hostname"],
-                    "memSizeMB" : data["system"]["memSizeMB"],
-                    "numCores" : data["system"]["numCores"], 
-                    "numPhysicalCores" : data["system"]["numPhysicalCores"],
-                    "cpuArch" : data["system"]["cpuArch"]            
+                    "Cluster name" : cluster_name,
+                    "Hostname" : data["system"]["hostname"],
+                    "Memory size(MB)" : data["system"]["memSizeMB"],
+                    "CPU Cores" : data["system"]["numCores"], 
+                    "CPU physicalCores" : data["system"]["numPhysicalCores"],
+                    "CPU arch" : data["system"]["cpuArch"]            
                 }
                 server_status = client.admin.command("serverStatus")
 
                 cstat.update({
-                    "uptime" : server_status["uptime"],
-                    "opc_insert" : server_status["opcounters"]["insert"], 
-                    "opc_query" : server_status["opcounters"]["query"],
-                    "opc_update" : server_status["opcounters"]["update"],
-                    "opc_delete" : server_status["opcounters"]["delete"], 
-                    "opc_getmore" : server_status["opcounters"]["getmore"],
-                    "opc_command" : server_status["opcounters"]["command"],
-                    "est_insert_per_sec" : round((server_status["opcounters"]["insert"])/ server_status["uptime"],2),
-                    "est_query_per_sec" : round((server_status["opcounters"]["query"])/ server_status["uptime"],2),
-                    "est_update_per_sec" : round((server_status["opcounters"]["update"])/ server_status["uptime"],2),
-                    "est_delete_per_sec" : round((server_status["opcounters"]["delete"])/ server_status["uptime"],2),
-                    "est_getmore_per_sec" : round((server_status["opcounters"]["getmore"])/ server_status["uptime"],2),
-                    "est_command_per_sec" : round((server_status["opcounters"]["command"])/ server_status["uptime"],2),           
+                    "Uptime" : server_status["uptime"],
+                    "Opc insert" : server_status["opcounters"]["insert"], 
+                    "Opc query" : server_status["opcounters"]["query"],
+                    "Opc update" : server_status["opcounters"]["update"],
+                    "Opc delete" : server_status["opcounters"]["delete"], 
+                    "Opc getmore" : server_status["opcounters"]["getmore"],
+                    "Opc command" : server_status["opcounters"]["command"],
+                    "Est insert per sec" : round((server_status["opcounters"]["insert"])/ server_status["uptime"],2),
+                    "Est query per sec" : round((server_status["opcounters"]["query"])/ server_status["uptime"],2),
+                    "Est update per sec" : round((server_status["opcounters"]["update"])/ server_status["uptime"],2),
+                    "Est delete per sec" : round((server_status["opcounters"]["delete"])/ server_status["uptime"],2),
+                    "Est getmore per sec" : round((server_status["opcounters"]["getmore"])/ server_status["uptime"],2),
+                    "Est command per sec" : round((server_status["opcounters"]["command"])/ server_status["uptime"],2),           
                 })
-                total_operation_sec = cstat["est_insert_per_sec"] + cstat["est_query_per_sec"] + (cstat["est_update_per_sec"] *2) + (cstat["est_delete_per_sec"] *2) + cstat["est_getmore_per_sec"] + cstat["est_command_per_sec"]
+                total_operation_sec = cstat["Est insert per sec"] + cstat["Est query per sec"] + (cstat["Est update per sec"] *2) + (cstat["Est delete per sec"] *2) + cstat["Est getmore per sec"] + cstat["Est command per sec"]
                 cstat.update({
-                    "est_total_ops_per_sec" : total_operation_sec
+                    "Est total ops per sec" : total_operation_sec
                 })
                 
                 cluster_stats.append(cstat)
 
             for db in client.list_database_names():
                 if db not in ["admin", "config", "local"]:
                     for coll in client[db].list_collections():
@@ -91,54 +119,129 @@
                                 avgObjSize = 0
                             try:
                                 num_doc = client[db].command(
                                     "collStats", coll["name"])["count"]
                             except KeyError:
                                 num_doc = 0
                             coll_stat = {
-                                "cluster_name": cluster_name,
-                                "db_name": db,
-                                "coll_name": coll["name"],
-                                "coll_size_MB": client[db].command("collStats", coll["name"], scale=1024*1024)["size"],
-                                "avg_obj_size_Bytes": avgObjSize,
-                                "num_doc": num_doc,
-                                "storage_size_MB": client[db].command("collStats", coll["name"], scale=1024*1024)["storageSize"],
-                                "num_idx": client[db].command("collStats", coll["name"])["nindexes"],
-                                "idx_size_MB": client[db].command("collStats", coll["name"], scale=1024*1024)["totalIndexSize"],
-                                "total_size_MB": client[db].command("collStats", coll["name"], scale=1024*1024)["totalSize"],
+                                "Cluster name": cluster_name,
+                                "Database name": db,
+                                "Collection name": coll["name"],
+                                "Collection size(MB)": client[db].command("collStats", coll["name"], scale=1024*1024)["size"],
+                                "Average object size(Bytes)": avgObjSize,
+                                "Total number of document": num_doc,
+                                "Storage size(MB)": client[db].command("collStats", coll["name"], scale=1024*1024)["storageSize"],
+                                "Total number of index": client[db].command("collStats", coll["name"])["nindexes"],
+                                "Total index size(MB)": client[db].command("collStats", coll["name"], scale=1024*1024)["totalIndexSize"],
+                                "Total size(MB)": client[db].command("collStats", coll["name"], scale=1024*1024)["totalSize"],
                             }
                             if more_info:
-                                totalindex += coll_stat["num_idx"]
-                                totalindexsize += coll_stat["idx_size_MB"]
-                                totaldocuments += coll_stat["num_doc"]
-                                totalstoragesize += coll_stat["storage_size_MB"]
-                                totalsize += coll_stat["total_size_MB"]                                
+                                totalindex += coll_stat["Total number of index"]
+                                if coll_stat["Total number of index"] != 0:
+                                    totaluniqueindex += coll_stat["Total number of index"] -1
+                                if args.fa != "":
+                                    frequentlyaccess = ((int(args.fa) /100) * (coll_stat["Average object size(Bytes)"]* coll_stat["Total number of document"]))
+                                totalindexsize += coll_stat["Total index size(MB)"]
+                                totaldocuments += coll_stat["Total number of document"]
+                                totalstoragesize += coll_stat["Storage size(MB)"]
+                                totalsize += coll_stat["Total size(MB)"]                                
                             output.append(coll_stat)                                                                                 
             counter = counter + 1
             client.close()
-            if more_info: 
+            if more_info:
+                    if args.fa != "":
+                        cstat.update({  
+                            "Frequently access file(MB)" :frequentlyaccess
+                        }) 
                     cstat.update({
-                        "total_index" : totalindex,
-                        "total_indexsizeMB" : totalindexsize,
-                        "total_documents" : totaldocuments,
-                        "total_storagesizeMB" : totalstoragesize,
-                        "total_sizeMB" : totalsize,
-                        "est_compression_ratio_percent" : round(((totalsize-totalstoragesize)/totalsize) *100,2)
-                    })                           
-        df = pd.json_normalize(output)
-        df.to_csv(args.csv, quoting=csv.QUOTE_NONNUMERIC, index=False)
+                        "Total number of index" : totalindex,
+                        "Total unique index" : totaluniqueindex,
+                        "Total index size(MB)" : totalindexsize,
+                        "Total number of document" : totaldocuments,
+                        "Storage size(MB)" : totalstoragesize,
+                        "Total size(MB)" : totalsize,
+                        "Estimate compression ratio(%)" : round(((totalsize-totalstoragesize)/totalsize) *100,2)
+                    })
+                         
+                    if args.fa != "":                        
+                        if args.iops != "":
+                            recommendcpu = round((args.iops / (12500) * ((1-0.05) ** cstat["Total unique index"])),5)
+                        else:
+                            recommendcpu = round((cstat["Est total ops per sec"] / ((12500) * ((1-0.05) ** cstat["Total unique index"]))),5)                                                
+                        dbs = {
+                            "Cluster name" : str(cstat["Cluster name"]),
+                            "Hostname" : cstat["Hostname"],
+                            "Memory size(GB)" : round(cstat["Memory size(MB)"]/1024,2),
+                            "CPU Cores" : cstat["CPU Cores"], 
+                            "CPU physicalCores" : cstat["CPU physicalCores"],
+                            "Required harddisk size(GB)" : round(cstat["Storage size(MB)"]/1024,2),
+                            "Recommended memory(GB)" : round(((cstat["Frequently access file(MB)"] + cstat["Total index size(MB)"]) *2)/1024,2),
+                            "Recommended CPU core" : recommendcpu
+                        }
+                        db_sizing.append(dbs)  
+
+        write_json_to_excel(output, args.excelfile, "Cluster Data")
+
         if more_info:
-            df = pd.json_normalize(cluster_stats)
-            df.to_csv("cluster-info.csv", quoting=csv.QUOTE_NONNUMERIC, index=False)
-        print("Getting cluster information - completed successfully")
+            write_json_to_excel(cluster_stats, args.excelfile, "Cluster Info")
+
+        if args.fa != "":                  
+            write_json_to_excel(db_sizing, args.excelfile, "Cluster Sizing")
+
+        print('\nGetting all databases information - completed successfully')
     except KeyboardInterrupt:
         shutdown()
     except Exception as e:
         print("Exception:", str(e))
 
+def write_json_to_excel(json_data, output_file, worksheet):
+    # Convert JSON data to a pandas DataFrame
+    df = pd.DataFrame(json_data)
+
+    if file_exists(output_file):   
+        with pd.ExcelWriter(output_file, engine='openpyxl', mode='a', if_sheet_exists="replace") as writer:
+            # Write the data to the specified sheet
+            df.to_excel(writer, sheet_name=worksheet, index=False)
+            
+    else: 
+        df.to_excel(output_file, sheet_name=worksheet, index=False)
+
+    # Load the workbook
+    workbook = load_workbook(output_file)
+
+    # Access the active worksheet
+    worksheet = workbook[worksheet]
+
+    # Expand column widths based on the content of the first row
+    for column_cells in worksheet.columns:
+        max_length = 0
+        column = column_cells[0].column_letter  # Get the column letter
+        for cell in column_cells:
+            try:
+                if len(str(cell.value)) > max_length:
+                    max_length = len(cell.value)
+            except:
+                pass
+        adjusted_width = (max_length + 2) * 1  # Adjust the width factor as needed
+        worksheet.column_dimensions[column].width = adjusted_width
+
+    # Save the modified workbook
+    workbook.save(output_file)
+
+def file_exists(file_path):
+    return os.path.isfile(file_path)
+
+def read_file(file_path):
+    lines = []
+    with open(file_path, 'r') as file:
+        for line in file:
+            line = line.strip()
+            lines.append(line)
+    return lines
+
 def shutdown():
     print()
 
     try:
         sys.exit(0)
     except SystemExit as e:
         os._exit(0)
```

## Comparing `mostats-1.0.6.dist-info/LICENSE` & `mostats-1.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mostats-1.0.6.dist-info/METADATA` & `mostats-1.0.7.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,84 +1,131 @@
 Metadata-Version: 2.1
 Name: mostats
-Version: 1.0.6
+Version: 1.0.7
 Summary: Get the MongoDB database statistic to a local CSV file
 Home-page: https://github.com/pix3lize/mostats
 Author: Hendri Tjipto
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pymongo
 Requires-Dist: pandas
 Requires-Dist: argparse
+Requires-Dist: openpyxl
 
 # Mostats 📊
 
 ---
 
 ![PyPI](https://img.shields.io/pypi/v/mostats) [![Downloads](https://static.pepy.tech/personalized-badge/mostats?period=month&units=international_system&left_color=brightgreen&right_color=grey&left_text=Downloads)](https://pepy.tech/project/mostats) ![GitHub repo size](https://img.shields.io/github/repo-size/pix3lize/mostats) ![GitHub last commit (by committer)](https://img.shields.io/github/last-commit/pix3lize/mostats)
 
-Get the MongoDB database statistic e.g : database name, collection, index size, and collection size to a local CSV file.
+Get the MongoDB database statistic e.g : database name, collection, index size, and collection size to a an excel file.
 
-New version support multiple server instance and getting additional host information, uptime, total number of command, read, getmore, command, insert, and summarise the cluster report. Host information will be save as cluster-info.csv on the same folder
+New version support multiple server instance and getting additional host information, uptime, total number of command, read, getmore, command, insert, summarise the cluster report, and recommended sizing. Host information will be save as "Cluster-info.xlsx" on the same folder
+
+To get host information :
 
 ```python
 mostats -u "mongodb+srv://username:password@cluster1.cluster.mongodb.net/" -m True
 ```
 
+To get sizing information (specify frequenly access data in percentage -fa) below is the sample of 5% :
+
+```python
+mostats -u "mongodb+srv://username:password@cluster1.cluster.mongodb.net/" -fa 5 -m True
+```
+
 #### Install
 
 Run this command, please choose pip or pip3
 
 ```terminal
 pip3 install mostats
 pip install mostats
 ```
 
 #### How to use
 
 Please check on the guide below:
 
 ```terminal
-usage: getCluster.py [-h] [-u URL [URL ...]] [-c CSV] [-n NAME [NAME ...]] [-m MOREINFO]
+usage: getCluster.py [-h] [-u URL [URL ...]] [-uf URLFILE] [-e EXCELFILE] [-n NAME [NAME ...]] [-nf NAMEFILE] [-m MOREINFO] [-fa FA] [-iops IOPS]
 
-Get the MongoDB database statistic to a local CSV file
+Get the MongoDB database statistic to an excel file
 
 options:
   -h, --help            show this help message and exit
   -u URL [URL ...], --url URL [URL ...]
                         MongoDB cluster URL, default is "mongodb://127.0.0.1". Example:
-                        "mongodb+srv://<<username>>:<<password>>@cluster.zqqqy.mongodb.net/?retryWrites=true&w=majority". For multiple server
-                        please use the space and "" to seperate
+                        "mongodb+srv://<<username>>:<<password>>@cluster.zqqqy.mongodb.net/?retryWrites=true&w=majority". For multiple server please
+                        use the space and "" to seperate
                         example:"mongodb+srv://<<username>>:<<password>>@cluster1.zqqqy.mongodb.net/?retryWrites=true&w=majority"
                         "mongodb+srv://<<username>>:<<password>>@cluster2.zqqqy.mongodb.net/?retryWrites=true&w=majority"
-  -c CSV, --csv CSV     CSV filename, default "cluster-data.csv"
+  -uf URLFILE, --urlfile URLFILE
+                        Get the MongoDB cluster URL from a file. It will read each line as one MongoDB cluster URL
+  -e EXCELFILE, --excelfile EXCELFILE
+                        Excel filename, default "Cluster-info.xlsx"
   -n NAME [NAME ...], --name NAME [NAME ...]
                         Cluster name, default value first subdomain example: mongodb+srv://clustername.cl0.mongodb.net will be clustername. For
                         multiple server please use the space and "" to seperate example:"cluster1" "cluster2"
+  -nf NAMEFILE, --namefile NAMEFILE
+                        Get the cluster name from a file. It will read each line as one cluster name
   -m MOREINFO, --moreinfo MOREINFO
                         Getting the host information, uptime, total number of command, read, and insert
+  -fa FA, --fa FA       Frequently access ratio in percent (input number only)
+  -iops IOPS, --iops IOPS
+                        Expected IOPS
 ```
 
 #### Example
 
 For MongoDB Atlas please leave the cluster name empty
 
 ```python
 mostats -u "mongodb+srv://username:password@cluster0.cluster.mongodb.net/?retryWrites=true&w=majority" -c "cluster-info.csv"
 ```
 
 Specify custom cluster name for MongoDB Community or Enterprise Edition installation only when MongogDB installed without FQDN
 
 ```python
-mostats -u "mongodb+srv://username:password@cluster0.cluster.mongodb.net/?retryWrites=true&w=majority" -c "cluster-info.csv"
+mostats -u "mongodb+srv://username:password@cluster0.cluster.mongodb.net/?retryWrites=true&w=majority" -n "Cluster1" -c "Custom-file.xlsx"
 ```
 
-Getting more host information on multiple cluster with custom cluster name. Please leave it empty when getting the data from MongoDB atlas
+Getting host information on multiple cluster with custom cluster name. Please leave it empty when getting the data from MongoDB atlas
 
 ```python
 mostats -u "mongodb+srv://username:password@cluster1.cluster.mongodb.net/" "mongodb+srv://username:password@cluster2.cluster.mongodb.net/" -n "Cluster 1" "Cluster 2" -m True
 ```
+
+Getting host information and sizing on multiple cluster with custom cluster name. Specify frequently access file by adding parameter -fa. Please leave it empty when getting the data from MongoDB atlas. Below are the sample code for adding frequently access data equal to 5%
+
+```python
+mostats -u "mongodb+srv://username:password@cluster1.cluster.mongodb.net/" "mongodb+srv://username:password@cluster2.cluster.mongodb.net/" -n "Cluster 1" "Cluster 2" -fa 5 -m True
+```
+
+#### Getting more than one MongoDB cluster with external file
+
+Mostats can read external files to specify both MongoDB URL and custom name. It will read each line as one MongoDB URL and one cluster name.
+
+Sample mongourl.txt
+
+```txt
+mongodb+srv://username:password@cluster1.cluster.mongodb.net/
+mongodb+srv://username:password@cluster2.cluster.mongodb.net/
+```
+
+Sample name.txt
+
+```txt
+Cluster 1
+Cluster 2
+```
+
+Below are the sample script:
+
+```python
+mostats -uf "mongourl.txt" -nf "name.txt" -fa 0 -m True
+```
```

