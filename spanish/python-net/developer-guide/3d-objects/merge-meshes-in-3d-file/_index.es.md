---
title: Combinar mallas en el archivo 3D
type: docs
weight: 90
url: /es/python-net/merge-meshes-in-3d-file/
description: Los desarrolladores pueden combinar varias mallas en una sola malla válida. Podrían convertir todas las mallas de una escena 3D, un nodo o un conjunto de nodos en una sola malla. Para lograr esto, hay tres miembros de MergeMesh en la clase Aspose.ThreeD.Entities.PolygonModifier.
---
##  **Combinar mallas en una sola malla válida**
Los desarrolladores pueden combinar varias mallas en una sola malla válida. Podrían convertir todas las mallas de una escena 3D, un nodo o un conjunto de nodos en una sola malla. Para lograr esto, hay varios miembros `merge_mesh` en la clase `aspose.threed.entities.PolygonModifier`.

El ejemplo de código a continuación combina todas las mallas de una escena en una única malla válida.

**Python**

```py

import aspose.threed as a3d
# load a 3D scene

scene = a3d.Scene.from_file("LAD-TOP.rvm")

# merge all meshes

mesh = a3d.PolygonModifier.merge_mesh(scene)

# encode this mesh into the PLY format

a3d.FileFormat.PLY.encode_mesh(mesh, "LAD-TOP.ply")

```
