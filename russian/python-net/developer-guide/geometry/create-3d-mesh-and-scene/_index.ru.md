﻿---
title: Создать 3D Сетка и Сцена
type: docs
weight: 10
url: /ru/python-net/create-3d-mesh-and-scene/
description: Сетка определяется набором контрольных точек и множеством n-сторонних многоугольников по мере необходимости. В этой статье объясняется, как определить сетку.
---
## **Создайте сетку куба 3D**
[`Mesh`](https://reference.aspose.com/3d/net/aspose.threed.entities/mesh) определяется набором контрольных точек и множеством n-сторонних многоугольников по мере необходимости. В этой статье объясняется, как определить сетку.

Чтобы создать поверхность сетки, нам нужно определить контрольные точки и полигоны следующим образом:

- [Определите контрольные точки](/3d/ru/python-net/create-3d-mesh-and-scene/)
- [Создание полигонов с классом PolygonBuilder](/3d/ru/python-net/create-3d-mesh-and-scene/)
- [Создание полигонов](/3d/ru/python-net/create-3d-mesh-and-scene/)

Вот пример для прикрепления материала Фонга к узлу куба:
### **Определите контрольные точки**
Сетка состоит из набора контрольных точек в пространстве и полигонов для описания поверхности сетки, чтобы создать сетку, нам нужно определить контрольные точки:

{{% alert color="primary" %}}

Контрольные точки всех геометрий в Aspose.3D используют однородную координату, поэтому в примере кода она `Vector4` вместо `Vector3`.

{{% /alert %}}

**Пример:**

{{< gist "aspose-3d-gists" "cfde9f76113134443c76608c1d19453a" "Geometry-and-Hierarchy-Common-DefineControlPoints.py" >}}


### **Создание полигонов**
Контрольные точки не отображаются, чтобы сделать куб видимым, нам нужно определить полигоны в каждой стороне:

{{< gist "aspose-3d-gists" "cfde9f76113134443c76608c1d19453a" "Geometry-and-Hierarchy-Common-CreateMeshUsingCreatePolygons.py" >}}


### **Создание полигонов с классом PolygonBuilder**
Мы также можем определить многоугольник по вершинам с классом `PolygonBuilder`:

{{< gist "aspose-3d-gists" "cfde9f76113134443c76608c1d19453a" "Geometry-and-Hierarchy-Common-CreateMeshUsingPolygonBuilder.py" >}}

Теперь он закончен, чтобы сделать сетку видимой, нам нужно подготовить узел для нее.
## **Как триангулировать сетку**
Треугольная сетка полезна для игровой индустрии, потому что треугольная-единственный поддерживаемый примитив, который поддерживает оборудование GPU (нетреугольные данные триангулированы на уровне драйвера, что неэффективно при рендеринге в реальном времени)

{{% alert color="primary" %}}

В этой версии мы только триангулировали полигоны, так как это требуется для экспорта файлов 3ds, нормали/uvs и другие элементы вершины теряются во время этой процедуры, мы можем реализовать это в будущем.

{{% /alert %}}

В этом примере мы триангулируем Mesh, импортировав файл FBX и сохранив его в формате FBX.

{{< gist "aspose-3d-gists" "cfde9f76113134443c76608c1d19453a" "Geometry-and-Hierarchy-TriangulateMesh-TriangulateMesh.py" >}}
## **Создайте сцену куба 3D**
Эта тема демонстрирует, как добавить геометрию сетки к сцене 3D. Пример кода помещает куб и сохраняет сцену 3D в поддерживаемых форматах файлов.
### **Создать узел куба**
Узел невидим, но можно визуализировать геометрию, прикрепленную к узлу.

{{% alert color="primary" %}}

Объект класса Mesh используется в коде. Мы можем[Создать объект класса `Mesh`, как там рассказано](https://docs.aspose.com/3d/python-net/create-3d-mesh-and-scene/#create-a-3d-cube-mesh).

{{% /alert %}}

**Пример**

{{< gist "aspose-3d-gists" "cfde9f76113134443c76608c1d19453a" "Geometry-and-Hierarchy-CubeScene-CreateCubeScene.py" >}}

{{% alert color="primary" %}}

ПРИМЕЧАНИЕ: сущности, прикрепленные к корневому узлу, обычно игнорируются в программных приложениях CAD/CAM, поэтому нам нужно создать новый узел для визуализации геометрии.

{{% /alert %}}