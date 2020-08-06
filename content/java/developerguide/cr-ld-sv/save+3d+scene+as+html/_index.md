---
title : "Save 3D Scene as HTML" 
description : "" 
weight : 12020 
toc : false
type: docs
url: /java/developerguide/cr-ld-sv/save+3d+scene+as+html/
---

# Aspose.3D for Java : Save 3D Scene as HTML


{{< panel title="Contents Summary" style="primary" >}}
*   1 [Save 3D Scene as HTML](#save-3d-scene-as-html)
{{< /panel >}}
 

 

This feature is supported by version 19.9 or greater.

# Save 3D Scene as HTML

Aspose.3D for Java provides **HTMLSaveOptions** class to save a save 3D scene as HTML. When you export the scene into HTML5 file, API will export three files, an **HTML** file, an Aspose3DWeb file(\*.**a3dw**), and a rendered **JavaScript** file. In order to export a3dw file only, you can specify Aspose3DWeb as the export type, and reuse the JavaScript file within your own HTML page. The following code snippet shows how to save a 3D scene as HTML. 

Due to the browser's security limits, the exported HTML file cannot be opened directly, you need to open it through a web server, if you have python3 installed, you can start the webserver in the command line in the exported directory

python3 -m http.server

Then open it [http://localhost:8000/test.html](http://localhost:8000/test.html). The web renderer uses WebGL2, you can use [https://get.webgl.org/webgl2/](https://get.webgl.org/webgl2/) to check if your browser supports it or not.
