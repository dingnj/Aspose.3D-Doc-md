---
title: Save 3D Scene as HTML
type: docs
weight: 70
url: /tr/java/save-3d-scene-as-html/
description: Aspose.3D for Java ** htmlsaveoptions ** 3D sahneyi HTML olarak kaydetmek için sınıf sağlar.
---
{{% alert color="primary" %}} 

This özelliği 19.9 veya daha büyük sürümle desteklenir.

{{% /alert %}} 
#  **Save 3D Scene as HTML**
Aspose.3D for Java provides `HtmlSaveOptions` class to save a save 3D scene as HTML. When you export the scene into HTML5 file, API will export three files, an `HTML` file, an Aspose3DWeb file(*.*a3dw**), and a rendered `JavaScript` file. In order to export a3dw file only, you can specify Aspose3DWeb as the export type, and reuse the JavaScript file within your own HTML page. The following code snippet shows how to save a 3D scene as HTML. 



{{< gist "aspose-3d-gists" "50e7f479a64956c0bf78841c0799ba76" "src-java-examples-loadsave-SaveOptions-html5SaveOption.java" >}}

{{% alert color="primary" %}} 

Due to the browser's security limits, the exported HTML file cannot be opened directly, you need to open it through a web server, if you have python3 installed, you can start the web-server in the command line in the exported directory

{{% /alert %}} 

{{< highlight "java" >}}

 python3 -m http.server

{{< /highlight >}}

Then aç<http://localhost:8000/test.html>. The web renderer WebGL2 kullanır, kullanabilirsiniz<https://get.webgl.org/webgl2/>Tarayıcınızın destekleyip desteklemediğini kontrol etmek için.


