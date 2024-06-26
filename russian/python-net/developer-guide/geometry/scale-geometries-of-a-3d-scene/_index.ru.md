---
title: Масштабная геометрия сцены 3D
type: docs
weight: 70
url: /ru/python-net/scale-geometries-of-a-3d-scene/
description: Разработчики могут масштабировать только геометрию узла 3D или всех узлов сцены 3D. Чтобы достичь этого, разработчики могут вызывать несколько членов Scale экземпляра класса PolygonModifier.
---
##  **Масштабная геометрия одного узла 3D или всех узлов сцены 3D**
Разработчики могут масштабировать только геометрию узла 3D или всех узлов сцены 3D. Чтобы достичь этого, разработчики могут вызывать несколько членов Scale экземпляра класса `PolygonModifier`. Это пример кода для масштабирования всех узлов или одного узла:



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
