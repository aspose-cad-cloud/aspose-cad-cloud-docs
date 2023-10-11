---
title: "Convert CAD Drawings to PDF Format"
type: docs
url: /convert-cad-drawings-to-pdf-format/
weight: 40
---

# **Introduction**
This article explains how to convert CAD drawing/image to another format. You can convert CAD Drawings to Portable Document Format (PDF). Aspose.CAD provides the following two APIs to perform the said task:

1. [GET /cad/{name}/saveAs](https://apireference.aspose.cloud/cad/#/SaveAs/GetDrawingSaveAs)
1. [POST /cad/saveAs](https://apireference.aspose.cloud/cad/#/SaveAs/PostDrawingSaveAs)
## **Resource URI**
[Aspose.CAD Cloud APIs Swagger UI](https://apireference.aspose.cloud/cad/) lets you call these APIs directly from the browser. The description of the APIs and their parameters are also given there.
## **cURL Example**
**Option 1: Export existing drawing to another format**


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


// cURL example to export Drawing to another format

curl -v "https://api.aspose.cloud/v3.0/cad/910609.dxf/saveAs/pdf" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>" \
-o 910609.pdf

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

PDF Document 

```

{{< /tab >}}

{{< /tabs >}}

**Option 2: Export existing an image to PDF format. Image is passed as a request body**

**Input Document:** 

**Output Document:**

{{< tabs tabTotal="2" tabID="4" tabName1="Request" tabName2="Response" >}}

{{< tab tabNum="1" >}}

```java

// First get Access Token
// Get App Key and App SID from https://dashboard.aspose.cloud/

curl -v "https://api.aspose.cloud/connect/token" \
-X POST \
-d 'grant_type=client_credentials&client_id=xxxx&client_secret=xxxx' \
-H "Content-Type: application/x-www-form-urlencoded" \
-H "Accept: application/json"



// cURL example to export Drawing to another format. Image is passed as request body

curl -v "https://api.aspose.cloud/v3.0/cad/saveAs/pdf" \
-X POST \
-H "Content-Type: multipart/form-data" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>" \
-d @path/to/data.dxf https://aspose.com/file
-o 910609.pdf

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

PDF Document 

```

{{< /tab >}}

{{< /tabs >}}
# **SDKs**
Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Checkout our [GitHub repository](https://github.com/aspose-cad-cloud) for a complete list of Aspose.CAD SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/cad/available-sdks/) article to learn how to add an SDK to your project.
## **SDK Examples**
**Option 1: Export existing drawing to PDF format**

{{< tabs tabTotal="5" tabID="7" tabName1="C#" tabName2="PHP" tabName3="Ruby" tabName4="Python" tabName5="Node.js" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "c8bd6d4c37d5c3f13814621654f144a2" "Examples-.NET-GetImageSaveAs.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "771038f7ed5885cfde27c52a9fa2de33" "Examples-CAD-PHP-Scale-CAD-Result-In-Storage.php" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "4622acaf999d638b0735551bd1aa2709" "Examples-CAD-PHP-Render-CAD-to-PDF-Result-in-Storage.rb" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "6c0182692bf71c98fc3266e1d77490c3" "CAD-to-PDF-Result-in-Storage.py" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "49dc674a9de19e007289548bd69e1486" "Save-As-PDF.js" >}}

{{< /tab >}}

{{< /tabs >}}

**Option 2: Export existing image to PDF format, where Image is passed as a request body**

{{< tabs tabTotal="5" tabID="8" tabName1="C#" tabName2="PHP" tabName3="Ruby" tabName4="Python" tabName5="Node.js" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "c8bd6d4c37d5c3f13814621654f144a2" "Examples-.NET-PostImageSaveAs.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "771038f7ed5885cfde27c52a9fa2de33" "Examples-CAD-PHP-Scale-CAD-Result-In-Response.php" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "4622acaf999d638b0735551bd1aa2709" "Examples-CAD-PHP-Render-CAD-to-PDF-Result-in-Response.rb" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "6c0182692bf71c98fc3266e1d77490c3" "CAD-to-PDF-Result-in-Response.py" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "49dc674a9de19e007289548bd69e1486" "Save-As-PDF-from-Stream.js" >}}

{{< /tab >}}

{{< /tabs >}}
