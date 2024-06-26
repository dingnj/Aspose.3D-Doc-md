---
title: Lägga till omvandling i noden
type: docs
weight: 30
url: /sv/net/adding-transformation-to-the-node/
description: TSR (översättning/skalning/rotation) används oftast i 3D scenario, vi tillhandahöll en klass Transform för att komma åt dessa i Aspose. 3D.
---
{{% alert color="primary" %}}

Aspose.3D for .NET erbjuder att rotera objekt i 3D mellanslag. Det finns tre sätt att definiera objekts rotation i 3D utrymme, Euler vinklar, Quaternion och Custom Matrix, Alla stöds av klassen [`Transform`](https://reference.aspose.com/3d/net/aspose.threed/transform).

{{% /alert %}}

TSR (översättning/skalning/rotation) används oftast i 3D scenario, vi tillhandahöll en klass `Transform` för att komma åt dessa i Aspose. 3D. Affina transformationer omfattar:

- Översättning
- Skalning
- Rotationer
- Skjut avbildning
- Tryck på kartläggning

{{% alert color="primary" %}}

The [`Mesh`](https://reference.aspose.com/3d/net/aspose.threed.entities/mesh) class object is being used in the code. We can [create a Mesh class object as narrated there](/3d/net/create-3d-mesh-and-scene/).

{{% /alert %}}
##  **Rotera med kvittering**
{{< gist "aspose-3d-gists" "9563193e834f0087b554c83130fcf7c7" "Examples-CSharp-Geometry-and-Hierarchy-TransformationToNodeByQuaternion-AddTransformationToNodeByQuaternion.cs" >}}
##  **Rotera med Euler vinklar**
{{< gist "aspose-3d-gists" "9563193e834f0087b554c83130fcf7c7" "Examples-CSharp-Geometry-and-Hierarchy-TransformationToNodeByEulerAngles-AddTransformationToNodeByEulerAngles.cs" >}}
##  **Egen omvandlingsmatris**
Vi kan också använda Matrix direkt:

{{< gist "aspose-3d-gists" "9563193e834f0087b554c83130fcf7c7" "Examples-CSharp-Geometry-and-Hierarchy-TransformationToNodeByTransformationMatrix-AddTransformationToNodeByTransformationMatrix.cs" >}}
