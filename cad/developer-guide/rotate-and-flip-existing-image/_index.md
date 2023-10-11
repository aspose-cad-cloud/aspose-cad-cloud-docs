---
title: "Rotate and Flip Existing Image"
type: docs
url: /rotate-and-flip-existing-image/
weight: 30
---

# **Introduction**
This article explains how to rotate and flip the existing image. Rotate and Flip **method** parameter values could be one of the following:

- Rotate180FlipNone, Rotate180FlipX, Rotate180FlipXY, Rotate180FlipY,
- Rotate270FlipNone, Rotate270FlipX, Rotate270FlipXY, Rotate270FlipY,
- Rotate90FlipNone, Rotate90FlipX, Rotate90FlipXY, Rotate90FlipY,
- RotateNoneFlipNone, RotateNoneFlipX, RotateNoneFlipXY, RotateNoneFlipY

With the following APIs you can rotate and flip existing image:

- [GET /cad/{name}/rotateflip](https://apireference.aspose.cloud/cad/#!/RotateFlip/GetImageRotateFlip)
- [POST /cad/rotateflip](https://apireference.aspose.cloud/cad/#!/RotateFlip/PostImageRotateFlip)
## **Resource URI**
[Swagger UI](https://apireference.aspose.cloud/cad/) lets you call Aspose.CAD REST APIs directly from the browser. The description of the APIs and their parameters are also given there.
## **cURL Example**
**Option 1: Rotate and flip an existing image**

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



// cURL example to rotate and flip existing image

curl -v "https://api.aspose.cloud/v3.0/cad/910609.dxf/rotateflip?outputFormat=pdf&rotateFlipType=Rotate180FlipNone" \
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

**Option 2: Rotate and flip existing image and get it from response**

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



// cURL example to rotate and flip existing image and get it from response

curl -v "https://api.aspose.cloud/v3.0/cad/rotateflip?outputFormat=pdf&rotateFlipType=Rotate180FlipNone" \
-X POST \
-H "Content-Type: multipart/form-data" \
-H "Accept: application/json" \
-H "Authorization: Bearer <jwt token>" \
-d @path/to/data.dxf https://aspose.com/file

```

{{< /tab >}}

{{< tab tabNum="2" >}}

```java

PDF Document 

```

{{< /tab >}}

{{< /tabs >}}
# **SDKs**
Using an SDK (API client) is the quickest way for a developer to speed up the development. An SDK takes care of a lot of low-level details of making requests and handling responses and lets you focus on writing code specific to your particular project. Checkout our [GitHub repository](https://github.com/aspose-cad-cloud) for a complete list of Aspose.CAD SDKs along with working examples, to get you started in no time. Please check [Available SDKs](/cad/available-sdks/) article to learn how to add an SDK to your project.
## **SDK Examples**
**Option 1: Rotate and flip existing image**

{{< tabs tabTotal="5" tabID="7" tabName1="C#" tabName2="PHP" tabName3="Ruby" tabName4="Python" tabName5="Node.js" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "c8bd6d4c37d5c3f13814621654f144a2" "Examples-.NET-GetImageRotateFlip.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "771038f7ed5885cfde27c52a9fa2de33" "Examples-CAD-PHP-Scale-CAD-Result-In-Storage.php" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "4622acaf999d638b0735551bd1aa2709" "Examples-CAD-PHP-Rotate-CAD-Save-to-Storage.rb" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "6c0182692bf71c98fc3266e1d77490c3" "Flip-Rotate-CAD.py" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "49dc674a9de19e007289548bd69e1486" "rotate-flip.js" >}}

{{< /tab >}}

{{< /tabs >}}

**Option 2: Rotate and flip an existing image and get it from the response**

{{< tabs tabTotal="5" tabID="8" tabName1="C#" tabName2="PHP" tabName3="Ruby" tabName4="Python" tabName5="Node.js" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "c8bd6d4c37d5c3f13814621654f144a2" "Examples-.NET-PostImageRotateFlip.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "771038f7ed5885cfde27c52a9fa2de33" "Examples-CAD-PHP-Scale-CAD-Result-In-Response.php" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "4622acaf999d638b0735551bd1aa2709" "Examples-CAD-PHP-Flip-Rotate-CAD.rb" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "6c0182692bf71c98fc3266e1d77490c3" "Post-Flip-Rotate-CAD.py" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "49dc674a9de19e007289548bd69e1486" "rotate-flip-with-stream.js" >}}

{{< /tab >}}

{{< /tabs >}}
