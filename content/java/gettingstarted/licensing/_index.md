---
title : "Licensing" 
description : "" 
weight : 8008 
toc : false
type: docs
url: /java/gettingstarted/licensing/
---

# Aspose.3D for Java : Licensing


{{< panel title="Contents Summary" style="primary" >}}
*   1 [Evaluate Aspose.3D](#evaluate-aspose.3d)
*   2 [Applying a License](#applying-a-license)
    *   2.1 [Apply License using File or Stream Object](#apply-license-using-file-or-stream-object)
    *   2.2 [Including the License File as an Embedded Resource](#including-the-license-file-as-an-embedded-resource)
    *   2.3 [Validate the License](#validate-the-license)
*   3 [Apply Metered License](#apply-metered-license)
*   4 [When to Apply a License](#when-to-apply-a-license)
*   5 [You can Change the License File Name](#you-can-change-the-license-file-name)
*   6 [Exception Cannot find license filename](#exception-cannot-find-license-filename)
*   7 [Using Multiple APIs from Aspose](#using-multiple-apis-from-aspose)
{{< /panel >}}
 

 

## Evaluate Aspose.3D

You can easily download/install Aspose.3D for Java from [Aspose Repository](http://repository.aspose.com/repo/com/aspose/aspose-3d/) for evaluation. The evaluation download is the same as the purchased download. The evaluation version simply becomes licensed when you add a few lines of code to apply the license.

The evaluation version provides all the features except the following:

*   Users can only open / import maximum 50 3D documents to a Scene.
*   Users can only save maximum 50 3D documents to a Scene.
*   Users will also see an evaluation watermark in the rendered images and all other output files.
*   Each node can have no more than 5 child nodes.
    
*   Each node can have no more than 2 attached entities.
    
*   Each geometry can have no more than 2 attached vertex elements.
    
*   Each node can have no more than 1 material.
    

If you want to test 'Aspose.3D for Java' without the evaluation version limitations, you can also request a 30-day Temporary License. Please refer to [How to get a Temporary License?](https://purchase.aspose.com/temporary-license)

## Applying a License

The license is a plain text XML file that contains details such as the product name, number of developers it is licensed to, subscription expiry date and so on. The file is digitally signed, so do not modify the file; even the inadvertent addition of an extra line break into the file will invalidate it. You need to set a license before performing any operations with documents. Make sure you do this before creating a Scene object.

Licenses can be applied from various locations:

*   Explicit path
*   The folder that contains the Aspose.3D' JAR file.
*   An embedded resource in the JAR that called Aspose.3D JAR.

Use the License.setLicense method to license the APIs. Often the easiest way to set a license is to put the license file in the same folder as Aspose.3D' JAR and specify just the file name without path.

### Apply License using File or Stream Object

In this example Aspose.3D will attempt to find the license file in the folder that contain the JARs of your application.

Initializes a license from a stream.

### Including the License File as an Embedded Resource

You can simply copy the LIC file in the **resources** folder of your project. Rebuilding the project should embed the .lic file into application’s .jar file. After that you can apply license by using the code like below:

### Validate the License

It is possible to validate if the license has been set properly or not. The License class has the isLicensed field that will return true if license has been properly set.

## Apply Metered License

Aspose.3D allows developers to apply metered key. It is a new licensing mechanism. The new licensing mechanism will be used along with existing licensing method. Those customers who want to be billed based on the usage of the API features can use the metered licensing. For more details, please refer to [Metered Licensing FAQ](https://purchase.aspose.com/faqs/licensing/metered) section.

A new class **Metered** has been introduced to apply metered key. Following is the sample code demonstrating how to set metered public and private key.

## When to Apply a License

Follow these simple rules:

*   The license only needs to be set once per application domain.
*   You need to set the license before using any other Aspose.3D classes.
*   Calling License.SetLicense multiple times is not harmful, but simply wastes processor time.

If you are developing a class library, you can call License.SetLicense from a static constructor of your class that uses Aspose.3D. The static constructor will execute before an instance of your class is created making sure Aspose.3D license is properly set.

## You can Change the License File Name

The license file name does not have to be 'Aspose.3D.LIC'. You can rename it to anything you like and use that name when calling License.SetLicense.

## Exception Cannot find license filename

When you purchase and download a license, Aspose website names the license file 'Aspose.3D.LIC'. You download the license file using your browser. Some browsers recognize the license file as XML and append an .xml extension to it so the full name of the file on your computer becomes 'Aspose.3D.lic.XML'.

When Microsoft Windows, for example, is configured to hide extensions of known file types (unfortunately this is default in most Windows installations), the license file will appear to you as 'Aspose.3D.LIC ' in Windows Explorer. You are likely to think this is the real file name and call License.SetLicense passing it 'Aspose.3D.LIC ', but there is no such file, hence the exception.

In order to solve the problem, rename the file to remove the invisible .xml extension. We also recommend you disable the "hide extensions" option in Microsoft Windows.

## Using Multiple APIs from Aspose

If you use multiple Aspose APIs in your application, for example Aspose.3D and Aspose.Cells, here are a few useful tips.

*   Set the License for each Aspose API separately. Even if you have a single license file for all APIs, for example 'Aspose.Total.lic', you still need to call License.SetLicense separately for each Aspose API you are using in your application.
*   Use Fully Qualified License Class Name. Each Aspose API has a License class in its namespace. For example, Aspose.3D has com.aspose.3d.License and Aspose.Cells has com.aspose.cells.License class. Using the fully qualified class name allows you to avoid any confusion about which license is applied to which product.
