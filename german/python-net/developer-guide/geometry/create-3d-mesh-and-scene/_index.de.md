---
title: 3D Mesh und Szene erstellen
type: docs
weight: 10
url: /de/python-net/create-3d-mesh-and-scene/
description: Ein Netz wird durch eine Reihe von Kontroll punkten und die vielen n-seitigen Polygone nach Bedarf definiert. Dieser Artikel erklärt, wie man ein Mesh definiert.
---
##  **Erstellen Sie ein 3D Cube Mesh**
A [`Mesh`](https://reference.aspose.com/3d/net/aspose.threed.entities/mesh) wird durch eine Reihe von Kontroll punkten und die vielen n-seitigen Polygone nach Bedarf definiert. Dieser Artikel erklärt, wie man ein Mesh definiert.

Um eine Mesh-Oberfläche zu erstellen, müssen wir Kontroll punkte und Polygone wie folgt definieren:

- [Definieren Sie die Kontroll punkte](/3d/de/python-net/create-3d-mesh-and-scene/)
- [Erstellen Sie Polygone mit der PolygonBuilder-Klasse](/3d/de/python-net/create-3d-mesh-and-scene/)
- [Polygone erstellen](/3d/de/python-net/create-3d-mesh-and-scene/)

Hier ist ein Beispiel zum Anhängen eines Phong-Materials an den Würfel knoten:
###  **Definieren Sie die Kontroll punkte**
Ein Netz besteht aus einer Reihe von Kontroll punkten im Raum und Polygonen, um die Netz oberfläche zu beschreiben. Um ein Netz zu erstellen, müssen wir die Kontroll punkte definieren:

{{% alert color="primary" %}}

Die Kontroll punkte aller Geometrien in Aspose.3D verwenden eine homogene Koordinate, also `Vector4` statt `Vector3` im Beispiel code.

{{% /alert %}}

**Beispiel:**

{{< gist "aspose-3d-gists" "cfde9f76113134443c76608c1d19453a" "Geometry-and-Hierarchy-Common-DefineControlPoints.py" >}}


###  **Polygone erstellen**
Die Kontroll punkte sind nicht render ierbar. Um den Würfel sichtbar zu machen, müssen wir Polygone auf jeder Seite definieren:

{{< gist "aspose-3d-gists" "cfde9f76113134443c76608c1d19453a" "Geometry-and-Hierarchy-Common-CreateMeshUsingCreatePolygons.py" >}}


###  **Erstellen Sie Polygone mit der PolygonBuilder-Klasse**
Wir können Polygon auch durch Eckpunkte mit der `PolygonBuilder`-Klasse definieren:

{{< gist "aspose-3d-gists" "cfde9f76113134443c76608c1d19453a" "Geometry-and-Hierarchy-Common-CreateMeshUsingPolygonBuilder.py" >}}

Jetzt ist es fertig, um das Netz sichtbar zu machen, müssen wir einen Knoten dafür vorbereiten.
##  **Wie man ein Netz trianguliert**
Triangulate Mesh ist für die Spiele industrie nützlich, da das Dreiecksnetz das einzige unterstützte Primitiv ist, das die GPU-Hardware unterstützt (nicht dreieckige Daten werden auf Treiber ebene trianguliert, was beim Echtzeit-Rendering ineffizient ist).

{{% alert color="primary" %}}

In dieser Version haben wir die Polygone nur trianguliert, da dies für den Export von 3ds-Dateien erforderlich ist. Normalen/Uvs und andere Scheitel punkt elemente gehen während dieses Verfahrens verloren. Wir können dies in Zukunft implemen tieren.

{{% /alert %}}

In diesem Beispiel triangulieren wir ein Mesh, indem wir eine FBX-Datei importieren und im FBX-Format speichern.

{{< gist "aspose-3d-gists" "cfde9f76113134443c76608c1d19453a" "Geometry-and-Hierarchy-TriangulateMesh-TriangulateMesh.py" >}}
##  **Erstellen Sie eine 3D Cube-Szene**
Dieses Thema zeigt, wie Mesh-Geometrie zur 3D-Szene hinzugefügt wird. Der Beispielcode platziert einen Cube und speichert 3D Szene in den unterstützten Dateiformaten.
###  **Erstellen Sie einen Würfel knoten**
Ein Knoten ist unsichtbar, aber die an den Knoten angehängte Geometrie kann gerendert werden.

{{% alert color="primary" %}}

Das Mesh-Klassen objekt wird im Code verwendet. Wir können [Erstellen Sie ein `Mesh`-Klassen objekt, wie es dort erzählt wird](https://docs.aspose.com/3d/python-net/create-3d-mesh-and-scene/#create-a-3d-cube-mesh).

{{% /alert %}}

**Beispiel**

{{< gist "aspose-3d-gists" "cfde9f76113134443c76608c1d19453a" "Geometry-and-Hierarchy-CubeScene-CreateCubeScene.py" >}}

{{% alert color="primary" %}}

HINWEIS: Die an den Stamm knoten angehängten Entitäten werden normaler weise in CAD/CAM-Softwares ignoriert. Daher müssen wir einen neuen Knoten erstellen, um die Geometrie zu rendern.

{{% /alert %}}
