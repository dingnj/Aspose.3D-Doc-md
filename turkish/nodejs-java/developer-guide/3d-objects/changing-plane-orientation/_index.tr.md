---
title: Hanging Plane entation rientation asılı
type: docs
weight: 70
url: /tr/nodejs-java/changing-plane-orientation/
description: Aspose.3D for Node.js via Java bir sahnenin değişen yönünü sağlar. Yönelimi değiştirmek için, düzlem sınıfında getup () ve kurulum () yöntemleri tanıtılır.
---
{{% alert color="primary" %}} 

Bu özellik 23.12 veya daha büyük bir sürümle desteklenir.

{{% /alert %}} 

#  **Hanging Plane entation rientation asılı**
Aspose.3D for Node.js via Java allows changing orientation of a scene. In order to change the orientation, `getUp()` and `setUp()` methods are introduced in `Plane` Class. Following code snippet shows how to change the plane's orientation:

{{< highlight "java" >}}

var aspose = aspose || {};

aspose.threed = require("aspose.threed");

// Initialize Scene
var scene = new aspose.threed.Scene();

// Initialize Plane
var plane=new aspose.threed.Plane();

// Set Vector
plane.setUp(new aspose.threed.Vector3(1, 1, 3));
scene.getRootNode().createChildNode(plane);

//This will generate a plane that has customized orientation
scene.save("ChangePlaneOrientation.obj");

{{< /highlight >}}
