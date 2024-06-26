---
title: Fügen Sie Knoten hierarchie hinzu und teilen Sie geometrische Daten von Mesh unter mehreren Knoten der 3D-Szene
type: docs
weight: 40
url: /de/python-net/add-node-hierarchy-and-share-geometric-data-of-mesh-among-multiple-nodes-of-3d-scene/
description: Aspose.3D for Python via .NET bietet an, eine Knoten hierarchie zu erstellen. Der Knoten ist der grundlegende Baustein einer Szene. Eine Knoten hierarchie definiert die logische Struktur einer Szene und liefert sichtbare Inhalte, indem Geometrien, Lichter und Kameras an Knoten angebracht werden.
---
##  **Knoten hierarchie in 3D Szenen dokument hinzufügen**
Aspose.3D for Python via .NET bietet an, eine Knoten hierarchie zu erstellen. Der Knoten ist der grundlegende Baustein einer Szene. Eine Knoten hierarchie definiert die logische Struktur einer Szene und liefert sichtbare Inhalte, indem Geometrien, Lichter und Kameras an Knoten angebracht werden.
###  **Szenen-Grafik-Beispiel**
Eine Beispiel-Szenen hierarchie sieht so aus:

! [Todo: image_alt_text](add-node-hierarchy-and-share-geometric-data-of-mesh-among-multiple-nodes-of-3d-scene_1.png)

In Aspose.3D kann jede `Node`-Instanz mehrere unter geordnete Knoten haben. In diesem Beispiel haben wir einen Knoten mit zwei Würfel knoten erstellt. Wenn wir den Stamm knoten drehen, sind auch alle unter geordneten Knoten betroffen:

{{< gist "aspose-3d-gists" "cfde9f76113134443c76608c1d19453a" "Geometry-and-Hierarchy-NodeHierarchy-AddNodeHierarchy.py" >}}
##  **Teilen Sie die Geometrie daten von Mesh zwischen mehreren Knoten**
Um den Speicher bedarf zu verringern, kann eine einzelne Instanz der [`Mesh`](https://reference.aspose.com/3d/net/aspose.threed.entities/mesh)-Klasse an verschiedene Instanzen der [`Node`](https://reference.aspose.com/3d/net/aspose.threed/node)-Klasse gebunden werden. Stellen Sie sich vor, dass Sie ein System benötigen, in dem alle 3D Würfel nicht zu unterscheiden schienen, aber Sie benötigten zahlreiche viele davon. Sie können Speicher platz sparen, indem Sie ein Mesh-Objekt erstellen, wenn das System gestartet wird. An diesem Punkt erstellen Sie jedes Mal, wenn Sie eine andere Form benötigen, ein anderes Knoten objekt und zeigen diesen Knoten auf das eine Mesh. Dies wird als Instancing bezeichnet. Aspose.3D for Python via .NET APIs erlauben Instancing.
###  **Instancing Beispiel**
In den RTS-Spielen (Echtzeit strategie) wie können wir immer mehrere NPCs (Non-Player Character) mit demselben 3D-Modell sehen, möglicher weise in verschiedenen Farben. Die Rendering-Engine teilt normaler weise dieselben Mesh-Geometrie-Daten über verschiedene NPCs hinweg wird Instancing genannt.

{{% alert color="primary" %}}

Das `Mesh`-Klassen objekt wird im Code verwendet. Wir können [Erstellen Sie ein `Mesh`-Klassen objekt, wie es dort erzählt wird](/3d/de/python-net/create-3d-mesh-and-scene/).

{{% /alert %}}

Demonstration des Beispiel codes:

{{< gist "aspose-3d-gists" "cfde9f76113134443c76608c1d19453a" "Geometry-and-Hierarchy-MeshGeometryData-ShareMeshGeometryData.py" >}}

In diesem Beispiel haben wir 3 Würfel knoten erstellt, die dasselbe Netz haben. Jeder von ihnen hat unterschied liches Material mit unterschied lichen Farben.
