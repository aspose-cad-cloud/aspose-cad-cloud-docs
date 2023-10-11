---
title: "Change Scale of an Image"
type: docs
url: /change-scale-of-an-image/
weight: 20
---

# **Introduction**
This article explains how to change scale or resize an image. You can change either request using GET or POST methods by using the below APIs:

- [GET /cad/{name}/resize](https://apireference.aspose.cloud/cad/#!/Resize/GetChangeImageScale)
- [POST /cad/resize](https://apireference.aspose.cloud/cad/#!/Resize/PostChangeImageScale)
## **Resource URI**
[Swagger UI](https://apireference.aspose.cloud/cad/) lets you call Aspose.CAD REST APIs directly from the browser. The description of the APIs and their parameters are also given there.
## **cURL Example**
**Option 1: Change scale of an existing image**

**Input Document:** [910609.dxf](https://github.com/aspose-cad-cloud/aspose-cad-cloud-dotnet/blob/master/TestData/910609.dxf)



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



// cURL example to change scale of an existing image

curl -v "https://api.aspose.cloud/v3.0/cad/910609.dxf/resize?outputFormat=pdf&newWidth=200&newHeight=150" \
-X GET \
-H "Content-Type: application/json" \
-H "Accept: multipart/form-data" \
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

**Option 2: Change scale of an image from body**

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



// cURL example to change scale of an image from body

curl -v "https://api.aspose.cloud/v3.0/cad/resize?format=pdf&newWidth=200&newHeight=150" \
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
**Option 1: Change scale of an existing image**

{{< tabs tabTotal="5" tabID="7" tabName1="C#" tabName2="PHP" tabName3="Ruby" tabName4="Python" tabName5="Node.js" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "c8bd6d4c37d5c3f13814621654f144a2" "Examples-.NET-GetImageResize.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "771038f7ed5885cfde27c52a9fa2de33" "Examples-CAD-PHP-Scale-CAD-Result-In-Storage.php" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "4622acaf999d638b0735551bd1aa2709" "Examples-CAD-PHP-Scale-CAD-Save-to-Storage.rb" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "6c0182692bf71c98fc3266e1d77490c3" "Scale-CAD-Save-to-Storage.py" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "49dc674a9de19e007289548bd69e1486" "change-image-scale.js" >}}

{{< /tab >}}

{{< /tabs >}}

**Option 2: Change the scale of an image from the body**

{{< tabs tabTotal="5" tabID="8" tabName1="C#" tabName2="PHP" tabName3="Ruby" tabName4="Python" tabName5="Node.js" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "c8bd6d4c37d5c3f13814621654f144a2" "Examples-.NET-PostImageResize.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "771038f7ed5885cfde27c52a9fa2de33" "Examples-CAD-PHP-Scale-CAD-Result-In-Response.php" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "4622acaf999d638b0735551bd1aa2709" "Examples-CAD-PHP-Scale-CAD-Save-to-Response.rb" >}}

{{< /tab >}}

{{< tab tabNum="4" >}}

{{< gist "aspose-cloud" "6c0182692bf71c98fc3266e1d77490c3" "Scale-CAD-Save-to-Response.py" >}}

{{< /tab >}}

{{< tab tabNum="5" >}}

{{< gist "aspose-cloud" "49dc674a9de19e007289548bd69e1486" "change-image-scale-with-body.js" >}}

{{< /tab >}}

{{< /tabs >}}

