---
title: Erstellen Sie rechteckige Torus in 3D Szene
type: docs
weight: 50
url: /de/net/create-rectangular-torus-in-3d-scene/
description: Mit Aspose.3D for .NET API können Entwickler 3D-Objekte erstellen und dann 3D-Szene in jedem unterstützten 3D-Format speichern.
---
{{% alert color="primary" %}} 

Mit [Aspose.3D for .NET](https://products.aspose.com/3d/net/) API können Entwickler 3D-Objekte erstellen und dann 3D-Szene in jedem unterstützten 3D-Format speichern.

{{% /alert %}} 
##  **Rechteckiger Torus**
Wir haben eine `RectangularTorus`-Klasse hinzugefügt, mit der Entwickler einen param etrisierten rechteckigen Torus in die Szene einbauen können. Dies kann in ein Ordnungsnetz/Dreiecks netz umgewandelt werden, während die Szene in verschiedene unterstützte Dateiformate gespeichert wird.

**C#**

{{< highlight "java" >}}

 RectangularTorus rt = new RectangularTorus();

rt.InnerRadius = 17;

rt.OuterRadius = 22;

rt.Height = 30;

rt.Arc = Math.PI * 0.5;

Scene scene = new Scene();

scene.RootNode.CreateChildNode(rt);

scene.Save("rtorus.obj", FileFormat.WavefrontOBJ);

{{< /highlight >}}

Der erzeugte rechteckige Torus sieht wie folgt aus:

! [Todo: image_alt_text](create-rectangular-torus-in-3d-scene_1.png)
