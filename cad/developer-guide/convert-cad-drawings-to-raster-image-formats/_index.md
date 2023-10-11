---
title: "Convert CAD Drawings to Raster Image Formats"
type: docs
url: /convert-cad-drawings-to-raster-image-formats/
weight: 50
---

# **Introduction**
Raster images such as JPEG, PNG, TIFF, BMP are some of the widely used file formats and as we are aware that in order to view CAD files, we need specific software to view and edit such files. But in order to share and view the files without any dependency over any specific application, one of the viable solutions is to render the DWG into raster image formats and share across multiple platforms. Aspose.CAD Cloud provides the capabilities to perform this transformation in the cloud. 

This article explains how to convert CAD drawing/image to raster image format. You can convert CAD Drawings to BMP, PNG, JPG, JPEG, JPEG2000, TIF, TIFF, PSD, GIF and WMF formats. Aspose.CAD provides the following two APIs to perform the said task:

1. [GET /cad/{name}/saveAs](https://apireference.aspose.cloud/cad/#!/SaveAs/GetDrawingSaveAs)
1. [POST /cad/saveAs](https://apireference.aspose.cloud/cad/#!/SaveAs/PostDrawingSaveAs)
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

curl -v "https://api.aspose.cloud/v3.0/cad/910609.dxf/saveAs/jpg" \
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

**Option 2: Export existing images to another format. Image is passed as a request body**

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

curl -v "https://api.aspose.cloud/v3.0/cad/saveAs/jpeg" \
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
**Option 1: Export existing drawing to another format**

{{< tabs tabTotal="3" tabID="7" tabName1="C#" tabName2="Java" tabName3="PHP" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "c8bd6d4c37d5c3f13814621654f144a2" "Examples-.NET-GetImageSaveAs.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "85ffc13011e9427913b8983e97592189" "Examples-CAD-Java-Render-CAD-to-Image.java" >}}

{{< /tab >}}

{{< tab tabNum="3" >}}

{{< gist "aspose-cloud" "771038f7ed5885cfde27c52a9fa2de33" "Examples-CAD-PHP-Render-CAD-to-Image.php" >}}

{{< /tab >}}

{{< /tabs >}}

**Option 2: Export existing images to another format. Image is passed as a request body**

{{< tabs tabTotal="2" tabID="8" tabName1="C#" tabName2="PHP" >}}

{{< tab tabNum="1" >}}

{{< gist "aspose-cloud" "c8bd6d4c37d5c3f13814621654f144a2" "Examples-.NET-PostImageSaveAs.cs" >}}

{{< /tab >}}

{{< tab tabNum="2" >}}

{{< gist "aspose-cloud" "771038f7ed5885cfde27c52a9fa2de33" "Examples-CAD-PHP-Render-CAD-to-Image-Result-in-Response.php" >}}

{{< /tab >}}

{{< /tabs >}}
