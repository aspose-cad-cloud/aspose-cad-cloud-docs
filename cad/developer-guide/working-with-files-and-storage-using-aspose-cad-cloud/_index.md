---
title: "Working with Files and Storage using Aspose.CAD Cloud"
type: docs
url: /working-with-files-and-storage-using-aspose-cad-cloud/
weight: 60
---

## **Introduction**
Aspose.CAD Cloud provides helper functions to work with files uploaded to Aspose.CAD Cloud Storage or any other Cloud Storage of your choice. If you need any help getting started with setting third party storage please refer to [Aspose Cloud UI Help Topics](https://docs.aspose.cloud/display/totalcloud/Aspose+Cloud+UI+Help+Topics).
### **Download a file from Cloud Storage**
#### **API Information**

|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/cad/storage/file/{path}|GET|Download a File from Storage|[DownloadFile](https://apireference.aspose.cloud/cad/#/File/DownloadFile)|
#### **cURL Example**
{{< tabs tabTotal="1" tabID="1" tabName1="Request" >}}

{{< tab tabNum="1" >}}

**Create Request Token**

```java

curl -v "https://api.aspose.cloud/connect/token" 
-X POST 
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" 
-H "Content-Type: application/x-www-form-urlencoded" 
-H "Accept: application/json"

```

```java

curl
-X GET "https://api.aspose.cloud/v3.0/cad/storage/file/presentation_images.dxf" 
-H "Content-Type: application/json" 
-H "Authorization: Bearer <jwt token>" 
-H "Accept: multipart/form-data"

```

{{< /tab >}}

{{< /tabs >}}
### **Uploading a file from Cloud Storage**
#### **API Information**

|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/cad/storage/file/{path}|PUT|Upload a file to Cloud Storage|[UploadFile](https://apireference.aspose.cloud/cad/#/File/UploadFile)|
#### **cURL Example**
{{< tabs tabTotal="2" tabID="4" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

**Create Request Token**

```java

curl -v "https://api.aspose.cloud/connect/token" 
-X POST -d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" 
-H "Content-Type: application/x-www-form-urlencoded" 
-H "Accept: application/json"

```

```java

curl
-X PUT "https://api.aspose.cloud/v3.0/cad/storage/file/presentation_images_1.dxf" 
-H "Content-Type:application/octet-stream" 
-H "Authorization: Bearer <jwt token>" 
-H "Content-Type: multipart/form-data"
-d @path/to/data.dxf https://aspose.com/file

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

{

   "uploaded":[

      "input_1.dxf"

   ],

   "errors":[

   ]

}

```

{{< /tab >}}

{{< /tabs >}}
### **Copying a file to a new location on Cloud Storage**
#### **API Information**

|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/cad/storage/file/copy/{srcPath}|PUT|Duplicate a file to a new location on Cloud Storage|[CopyFile](https://apireference.aspose.cloud/cad/#/File/CopyFile)|
#### **cURL Example**
{{< tabs tabTotal="1" tabID="8" tabName1="Request" >}}

{{< tab tabNum="1" >}}

**Create Request Token**

```java

curl 
-v "https://api.aspose.cloud/connect/token" 
-X POST 
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" 
-H "Content-Type: application/x-www-form-urlencoded" 
-H "Accept: application/json"

```

```java

curl
-X PUT "https://api.aspose.cloud/v3.0/cad/storage/file/copy/input.dxf?destPath=destinationPath" 
-H "Content-Type:application/json" 
-H "Authorization: Bearer <jwt token>" 
-H "Accept: application/json"
```

{{< /tab >}}

{{< /tabs >}}
### **Moving a file to a new location on Cloud Storage**
#### **API Information**

|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/cad/storage/file/move/{srcPath}|PUT|Move a file to a new location on Cloud Storage|[MoveFile](https://apireference.aspose.cloud/cad/#/File/MoveFile)|
#### **cURL Example**
{{< tabs tabTotal="1" tabID="11" tabName1="Request" >}}

{{< tab tabNum="1" >}}

**Create Request Token**

```java

curl 
-v "https://api.aspose.cloud/connect/token" 
-X POST 
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" 
-H "Content-Type: application/x-www-form-urlencoded" 
-H "Accept: application/json"

```

```java

curl
-X PUT "https://api.aspose.cloud/v3.0/cad/storage/file/move/input.dxf?destPath=destinationPath" 
-H "Content-Type:application/json" 
-H "Authorization: Bearer <jwt token>"
-H "Accept: application/json"
```

{{< /tab >}}

{{< /tabs >}}
### **Deleting a file on Cloud Storage**
#### **API Information**

|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/cad/storage/file/{path}|DELETE|Delete a file from Cloud Storage|[DeleteFile](https://apireference.aspose.cloud/cad/#/File/DeleteFile)|
#### **cURL Example**
{{< tabs tabTotal="1" tabID="14" tabName1="Request" >}}

{{< tab tabNum="1" >}}

**Create Request Token**

```java

curl 
-v "https://api.aspose.cloud/connect/token" 
-X POST 
-d "grant_type=client_credentials&client_id=xxxx&client_secret=xxxx" 
-H "Content-Type: application/x-www-form-urlencoded" 
-H "Accept: application/json"

```

```java

curl
-X DELETE "https://api.aspose.cloud/v3.0/cad/storage/file/sample.dxf" 
-H "Content-Type:application/json" 
-H "Authorization: Bearer <jwt token>"

```

{{< /tab >}}

{{< /tabs >}}
