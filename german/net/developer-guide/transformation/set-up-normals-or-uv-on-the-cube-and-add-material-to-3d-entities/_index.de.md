---
title: Richten Sie Normalen oder UV auf dem Würfel ein und fügen Sie Material zu 3D Entitäten hinzu
type: docs
weight: 20
url: /de/net/set-up-normals-or-uv-on-the-cube-and-add-material-to-3d-entities/
description: So erstellen Sie Normalen oder UV-Daten in einem Netz in Aspose.3D.
---
{{% alert color="primary" %}}

Aspose.3D for .NET bietet Normalen und UV auf die geometrischen Formen zu verwalten. Ein Netz speichert die Schlüssel eigenschaften für jeden Scheitel punkt, sind seine Position im Raum und seine Normalität, ein Vektor senkrecht zur ursprünglichen Oberfläche. Das Normale ist wichtig für die Schattierung zählt. Die Normalen sollten Einheits vektoren sein. Die meisten Netz formate unterstützen auch eine Form von UV-Koordinaten, bei denen es sich um eine separate 2D-Darstellung des "entfalteten" Netzes handelt, um zu zeigen, welcher Teil einer zwei dimensionalen Textur karte auf verschiedene Polygone des Netzes angewendet werden soll.

{{% /alert %}} {{% alert color="primary" %}}

Das `Mesh`-Klassen objekt wird im Code verwendet. Wir können [Erstellen Sie ein Mesh-Klassen objekt, wie es dort erzählt wird](/3d/de/net/create-3d-mesh-and-scene/) und dann den Knoten um [Erstellen einer 3D-Szene](/3d/de/net/create-3d-mesh-and-scene/) auf die Mesh-Geometrie zeigen.

{{% /alert %}}
##  **Normale Vektoren erstellen**
Um ein gutes visuelles Aussehen der Beleuchtung zu haben, müssen wir Normale Informationen für jeden Scheitel punkt angeben, um bessere Details zu haben, können wir auch normale und diffuse Karte verwenden (sicher, dass Sie Schatten/spekulare Karte verwenden können), um pro Pixel normal/Farbe auszuführen. Eine Pro-Vertex-Information wie Normal-oder Scheitel punkt farbe wird durch Vertex Element erreicht. In Aspose.3D können wir zusätzliche Informationen an Kontroll punkte/Polygon vertex/Polygon/Kante abbilden, ein Beispiel, um Normalen für Scheitel punkt zu definieren:

{{< gist "aspose-3d-gists" "9563193e834f0087b554c83130fcf7c7" "Examples-CSharp-Geometry-and-Hierarchy-SetupNormalsOnCube-SetupNormalsOnCube.cs" >}}

Die 8 normalen Vektoren werden direkt 8 Kontroll punkten zugeordnet. Im nächsten Beispiel werden wir ein etwas komplexeres Szenario demonstrieren.
##  **Erstellen von UV-Koordinaten**
Hier haben wir nur 4 UV-Koordinaten definiert, sie jedoch mithilfe von Indizes auf 24 Polygon scheitel punkte (6 Fläche * 4 Scheitel punkt pro Polygon) angewendet.
Die Aspose.3D bietet 5 Mapping-Modi:

- `ControlPoint` -jede Daten wird dem Kontroll punkt der Geometrie zugeordnet.
- `PolygonVertex` -Die Daten werden dem Scheitel punkt des Polygons zugeordnet.
- `Polygon` -die Daten werden dem Polygon zugeordnet.
- `Edge` -die Daten werden dem Rand zugeordnet.
- `AllSame` -eine Daten, die der gesamten Geometrie zugeordnet sind.



{{< gist "aspose-3d-gists" "9563193e834f0087b554c83130fcf7c7" "Examples-CSharp-Geometry-and-Hierarchy-SetupUVOnCube-SetupUVOnCube.cs" >}}
##  **Materialien zu 3D Objekten hinzufügen**
Aspose.3D for .NET ermöglicht es Entwicklern, Shading-Algorithmus für genaue Schattierung und Highlights zu verwenden. Der Phong verfügt über mehrere Karten eingaben, mit denen wir den Effekt auf den Knoten maskieren können. Physically Based Rendering (PBR) berücksicht igt einige physikalische Eigenschaften von Objekten. Ein solcher Ansatz bietet das Erscheinung sbild von Materialien wie in der realen Welt.
###  **Phong Material mit Textur für Würfel**
Wenn die UV-Koordinaten einsatz bereit sind, können wir eine Textur auf die Oberfläche des Netzes anwenden, indem wir Material verwenden. Nur die Scheitel punkt farbe kann die Details der Oberfläche nicht beschreiben, dafür werden Materialien verwendet. Hier ist ein Beispiel zum Anhängen eines Phong-Materials an den Würfel knoten:

{{< gist "aspose-3d-gists" "9563193e834f0087b554c83130fcf7c7" "Examples-CSharp-Geometry-and-Hierarchy-MaterialToCube-AddMaterialToCube.cs" >}}

Wir haben die diffuse Textur abbildung und eine spiegele Farbe mit einem Glanz parameter angegeben.
###  **Wenden Sie physikalisch basiertes Rendering-Material (PBR) auf eine Box an**
PBR spielt eine Schlüssel rolle für die Game Engine-Grafik mit seiner effizienten und realistischen Darstellung von Wechsel wirkungen zwischen Licht und Oberfläche durch Dämpfung der Helligkeit und Streuung von reflektiertem Licht. Entwickler können Aspose.3D API verwenden, um PBR-Material auf 3D-Objekte in einer Szene anzuwenden. In diesem Code beispiel wird ver anschaulicht, wie ein Box-Objekt erstellt und anschließend das PBR-Material angewendet wird.

**.NET, C#**

{{< highlight "java" >}}

 // initialize a scene

Scene scene = new Scene();

// initialize PBR material object

PbrMaterial mat = new PbrMaterial();

// an almost metal material

mat.MetallicFactor = 0.9;

// material surface is very rough

mat.RoughnessFactor = 0.9;

// create a box to which the material will be applied

var boxNode = scene.RootNode.CreateChildNode("box", new Box());

boxNode.Material = mat;

// save 3d scene into STL format

scene.Save(@"C:\3D\PBR_Material_Box_Out.stl", FileFormat.STLASCII);

{{< /highlight >}}
