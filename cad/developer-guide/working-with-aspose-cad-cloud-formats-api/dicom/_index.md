﻿---
title: "DICOM API"
type: docs
url: /working-with-aspose-cad-cloud-formats-api/dicom/
weight: 20
---

# **Introduction**
This article explains how to work with the DICOM API. Using the following APIs, you can work with an image in the storage and process new ones:

1. [PUT /cad/{name}/dicom](https://reference.aspose.cloud/cad/#!/Dicom/PutDrawingDicom)
1. [POST /cad/dicom](https://reference.aspose.cloud/cad/#!/Dicom/PostDrawingDicom)

## **Resource URI**
[Swagger UI](https://reference.aspose.cloud/cad/) lets you call Aspose.CAD REST APIs directly from the browser.

## **cURL Example**
**Export drawing to DICOM format**

{{< tabs tabTotal="2" tabID="1" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get Access Token
// Get App Key and App SID from https://dashboard.aspose.cloud/

 curl -v "https://api.aspose.cloud/connect/token" \
 -X POST \
 -d 'grant_type=client_credentials&client_id=xxxx&client_secret=xxxx' \
 -H "Content-Type: application/x-www-form-urlencoded" \
 -H "Accept: application/json"



// cURL example to export Drawing to DICOM format

curl -v "https://api.aspose.cloud/v3.0/cad/dicom" \
-X PUT \
-H "Content-Type: multipart/form-data" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>" \
-F "drawingData=file.dxf" \
-o result.dicom

// cURL example to export an existing drawing to DICOM format with export settings specified

curl -v "https://api.aspose.cloud/v3.0/cad/dicom" \
-X POST \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>" \
-d "options=DICOM options passed as a JSON" \
-o result.dicom

Export an existing drawing to
```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

DICOM file 

```

{{< /tab >}}

{{< /tabs >}}
            
# **SDKs**
Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Checkout our [GitHub repository](https://github.com/aspose-cad-cloud) for a complete list of Aspose.CAD SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/cad/available-sdks/) article to learn how to add an SDK to your project.
## **SDK Examples**
**Export drawing to DICOM format.**
{{< tabs tabTotal="2" tabID="2" tabName1="C#" tabName2="Python">}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cad-gists" "08d6d4c55fe96b77e1e9c57a2f36d6ba" "Example-cad-cloud-net-put-dicom.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cad-gists" "7fd0ee4ef54697f442abdcbb41abbe10" "Example-cad-cloud-python-put-dicom.py" >}}

{{< /tab >}}
{{< /tabs >}}


**Export an existing drawing to DICOM format with export settings specified.**
{{< tabs tabTotal="2" tabID="3" tabName1="C#" tabName2="Python">}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cad-gists" "08d6d4c55fe96b77e1e9c57a2f36d6ba" "Example-cad-cloud-net-post-dicom.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cad-gists" "7fd0ee4ef54697f442abdcbb41abbe10" "Example-cad-cloud-python-post-dicom.py" >}}

{{< /tab >}}
{{< /tabs >}}
