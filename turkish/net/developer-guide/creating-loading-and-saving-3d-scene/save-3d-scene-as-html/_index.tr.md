---
title: Save 3D Scene as HTML in C#
linktitle: Save 3D Scene as HTML
type: docs
weight: 90
url: /tr/net/save-3d-scene-as-html/
---
##  **Overview**

This article explains how you can convert 3D files to HTML after [loading them into Scene object](https://docs.aspose.com/3d/net/create-and-read-an-existing-3d-scene/) using C# and covers wide range of topics (considering [supported file formats](https://docs.aspose.com/3d/net/supported-file-formats/)) e.g.

- Convert 3DS to HTML using C#
- Convert FBX to HTML in C#
- Convert STL to HTML in C#
- Convert U3D to HTML in C#
- Convert OBJ to HTML in C#


{{% alert color="primary" %}} 

This özelliği 19.9 veya daha büyük sürümle desteklenir.

{{% /alert %}} 
##  **Save 3D Scene as HTML**
Aspose.3D for .NET provides `Html5SaveOptions` class to save a save 3D scene as HTML. When you export the scene into HTML5 file, API will export three files, an `HTML` file, an Aspose3DWeb file(*.*a3dw**), and a rendered `JavaScript` file. In order to export a3dw file only, you can specify Aspose3DWeb as the export type, and reuse the JavaScript file within your own HTML page. The following C# code snippet shows how to save a 3D scene as HTML. 



{{< gist "aspose-3d-gists" "9563193e834f0087b554c83130fcf7c7" "Examples-CSharp-Loading-and-Saving-SaveOptions-HtmlSaveOption.cs" >}}

{{% alert color="primary" %}} 

Due to the browser's security limits, the exported HTML file cannot be opened directly, you need to open it through a web server, if you have python3 installed, you can start the web server in the command line in the exported directory

{{% /alert %}} 

{{< highlight "java" >}}

 python3 -m http.server

{{< /highlight >}}

Then aç<http://localhost:8000/test.html>. The web renderer WebGL2 kullanır, kullanabilirsiniz<https://get.webgl.org/webgl2/>Tarayıcınızın destekleyip desteklemediğini kontrol etmek için.


