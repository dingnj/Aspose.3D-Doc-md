---
title: Geometrien einer 3D-Szene skalieren
type: docs
weight: 70
url: /de/python-net/scale-geometries-of-a-3d-scene/
description: Entwickler können nur Geometrien eines 3D-Knotens oder aller Knoten der 3D-Szene skalieren. Um dies zu erreichen, können Entwickler mehrere Scale-Mitglieder der PolygonModifier-Klassen instanz aufrufen.
---
##  **Skalieren Sie Geometrien eines einzelnen 3D-Knotens oder aller Knoten der 3D-Szene**
Entwickler können nur Geometrien eines 3D-Knotens oder aller Knoten der 3D-Szene skalieren. Um dies zu erreichen, können Entwickler mehrere Scale-Mitglieder der `PolygonModifier`-Klassen instanz aufrufen. Dies ist das Code beispiel, um alle Knoten oder einzelnen Knoten zu skalieren:



**Python**

```py

from aspose.threed.utilities import Vector3
from aspose.threed.entities import PolygonModifier, Box
from aspose.threed import Scene

# scale the model in huge-scene.obj by 0.01 and save it to another file:

scene = Scene.from_file("huge-scene.obj")

# create a Box instance

box = scene.root_node.create_child_node("box", Box())

# scale geometries of a single node

PolygonModifier.scale(box, Vector3(0.01));

# scale geometries of all nodes

PolygonModifier.scale(scene, Vector3(0.01));

scene.save("scaled-scene.obj", FileFormat.WAVEFRONT_OBJ)

```
