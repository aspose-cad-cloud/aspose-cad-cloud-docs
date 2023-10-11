---
title: "Working with Aspose.CAD Cloud Live API"
type: docs
url: /working-with-aspose-cad-cloud-live-api/
weight: 50
---

## **Introduction**
Aspose.CAD Cloud provides support functions for working with files such as conversion, adding a watermark and working with metadata.

### **Convert CAD drawing**
#### **API Information**

|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/cad/Convert|POST|Convert CAD drawing to DXF, DWG, DGN, DWF, DWFX, IFC, STL, DWT, IGES, PLT, CF2, OBJ, HPGL, IGS, PCL, FBX, PDF, SVG format|[ConvertFile](https://apireference.aspose.cloud/cad/#/Live/Convert)|
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
-X POST "https://api.aspose.cloud/v3.0/cad/Convert?outputFormat=pdf" 
-H "Content-Type: multipart/form-data" 
-H "Authorization: Bearer <jwt token>" 
-H "Accept: application/json"
-d @path/to/data.dxf https://aspose.com/file

```

{{< /tab >}}
{{< /tabs >}}

### **Add watermark to drawing**
#### **API Information**
|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/cad/Watermark|POST|Add watermark to drawing|[Watermark](https://apireference.aspose.cloud/cad/#/Live/Watermark)|

#### **cURL Example**
{{< tabs tabTotal="1" tabID="2" tabName1="Request" >}}

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
-X POST "https://api.aspose.cloud/v3.0/cad/Watermark?outputFormat=pdf" 
-H "Content-Type: multipart/form-data" 
-H "Authorization: Bearer <jwt token>" 
-H "Accept: application/json"

```

{{< /tab >}}
{{< /tabs >}}

### **Extract Text from CAD drawing to txt file**
#### **API Information**
|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/cad/ExtractText|POST|Extract Text from CAD drawing to txt file|[ExtractText](https://apireference.aspose.cloud/cad/#/Live/ExtractText)|

#### **cURL Example**
{{< tabs tabTotal="1" tabID="3" tabName1="Request" >}}

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
-X POST "https://api.aspose.cloud/v3.0/cad/ExtractText" 
-H "Content-Type: multipart/form-data" 
-H "Authorization: Bearer <jwt token>" 
-H "Accept: application/json"
-d @path/to/data.dxf https://aspose.com/file

```

{{< /tab >}}
{{< /tabs >}}


### **Extract Metadata from CAD drawing to txt, xml or json file**
#### **API Information**
|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/cad/ExtractMetadata|POST|Extract Metadata from CAD drawing to txt, xml or json file|[ExtractMetadata](https://apireference.aspose.cloud/cad/#/Live/ExtractMetadata)|

#### **cURL Example**
{{< tabs tabTotal="1" tabID="4" tabName2="Request" >}}

{{< tab tabNum="2" >}}

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
-X POST "https://api.aspose.cloud/v3.0/cad/ExtractMetadata?outputFormat=txt" 
-H "Content-Type: multipart/form-data" 
-H "Authorization: Bearer <jwt token>" 
-H "Accept: application/json"
-d @path/to/data.dxf https://aspose.com/file

```

{{< /tab >}}
{{< /tabs >}}


### **Return file for viewer**
#### **API Information**
|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/cad/Viewer|POST|Return file for viewer|[Viewer](https://apireference.aspose.cloud/cad/#/Live/Viewer)|

#### **cURL Example**
{{< tabs tabTotal="1" tabID="5" tabName1="Request" >}}

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
-X POST "https://api.aspose.cloud/v3.0/cad/Viewer?outputFormat=png" 
-H "Content-Type: multipart/form-data" 
-H "Authorization: Bearer <jwt token>" 
-H "Accept: application/json"
-d @path/to/data.dxf https://aspose.com/file

```

{{< /tab >}}
{{< /tabs >}}


### **Get Metadata info**
#### **API Information**
|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/cad/EditMetadata|POST|Get Metadata info|[EditMetadata](https://apireference.aspose.cloud/cad/#/Live/EditMetadata)|

#### **cURL Example**
{{< tabs tabTotal="1" tabID="6" tabName1="Request" >}}

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
-X POST "https://api.aspose.cloud/v3.0/cad/EditMetadata" 
-H "Content-Type: multipart/form-data" 
-H "Authorization: Bearer <jwt token>" 
-H "Accept: application/json"

```

{{< /tab >}}
{{< /tabs >}}


### **Save Metadata**
#### **API Information**
|**API**|**Type**|**Description**|**Swagger Link**|
| :- | :- | :- | :- |
|/cad/EditMetadata|PUT|Save Metadata|[EditMetadata](https://apireference.aspose.cloud/cad/#/Live/EditMetadata2)|

#### **cURL Example**
{{< tabs tabTotal="1" tabID="7" tabName1="Request" >}}

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
-X PUT "https://api.aspose.cloud/v3.0/cad/EditMetadata" 
-H "Content-Type: multipart/form-data" 
-H "Authorization: Bearer <jwt token>" 
-H "Accept: application/json"

```

{{< /tab >}}
{{< /tabs >}}