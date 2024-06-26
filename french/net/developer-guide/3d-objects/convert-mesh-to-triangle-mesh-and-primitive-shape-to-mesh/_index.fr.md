---
title: Convertir la maille en maille triangulaire et la forme primitive en maille
type: docs
weight: 30
url: /fr/net/convert-mesh-to-triangle-mesh-and-primitive-shape-to-mesh/
description: Aspose.3D for .NET API permet aux développeurs de convertir n'importe quel objet maillage en maillage triangulaire avec une disposition mémoire personnalisée du sommet. La disposition de mémoire personnalisée du sommet est définie à l'aide de la classe Struct ou dynamiquement par VertexDeclaration dans les exemples de code.
---
##  **Convertir un maillage en maillage Triangle avec la disposition de mémoire personnalisée du Vertex**
[Aspose.3D for .NET](https://products.aspose.com/3d/net/) API permet aux développeurs de convertir n'importe quel objet maillage en maillage triangulaire avec une disposition de mémoire personnalisée du sommet. La disposition de mémoire personnalisée du sommet est définie à l'aide de la classe Struct ou dynamiquement par [`VertexDeclaration`](https://reference.aspose.com/3d/net/aspose.threed.utilities/vertexdeclaration/) dans les exemples de code.

{{% alert color="primary" %}}

Cette rubrique d'aide crée des maillages à partir de la boîte et de la sphère pour garder le code complet et court. Les développeurs peuvent construire un maillage manuellement comme rapporté dans cette rubrique d'aide: [Créer un maillage de cube 3D](/3d/fr/net/create-3d-mesh-and-scene/).

{{% /alert %}}

Ces exemples montrent comment:

- [Convertir une sphère en maille triangle avec une disposition de mémoire personnalisée du sommet (défini dans le Struct)](/3d/fr/net/convert-mesh-to-triangle-mesh-and-primitive-shape-to-mesh/).
- [Convertir une boîte en Triangle Mesh avec une disposition de mémoire personnalisée du sommet (définie par la classe VertexDeclaration)](/3d/fr/net/convert-mesh-to-triangle-mesh-and-primitive-shape-to-mesh/).
###  **Convertir Maille**
Les développeurs peuvent convertir le maillage en maillage triangulaire car toute structure complexe (surface) peut être représentée comme un tas de triangles. Le triangle est la géométrie la plus atomique. Ainsi, il est utilisé comme base pour presque tout.
###  **Les sommets d'accès d'un maillage Triangle**
Les développeurs peuvent accéder aux indices, aux sommets réels, aux sommets avant la fusion et au total des octets de sommets en mémoire.

L'exemple ci-dessous convertit une sphère en maillage triangle avec une disposition de mémoire personnalisée.

{{< gist "aspose-3d-gists" "9563193e834f0087b554c83130fcf7c7" "Examples-CSharp-Working-with-Objects-ConvertSphereMeshtoTriangleMeshCustomMemoryLayout-ConvertSphereMeshtoTriangleMeshCustomMemoryLayout.cs" >}}




Ci-dessous, l'exemple convertit une boîte en maillage triangle avec une disposition de mémoire personnalisée.

{{< gist "aspose-3d-gists" "9563193e834f0087b554c83130fcf7c7" "Examples-CSharp-Working-with-Objects-ConvertBoxMeshtoTriangleMeshCustomMemoryLayout-ConvertBoxMeshtoTriangleMeshCustomMemoryLayout.cs" >}}
##  **Convertir le Primitif en Maille**
En utilisant Aspose.3D for .NET, les développeurs peuvent convertir n'importe quel objet primitif en un maillage. Les primitives comprennent plusieurs des objets les plus basiques et les plus utilisés comme la boîte, la sphère, le plan, le cylindre et le tore.

{{% alert color="primary" %}}

Toute classe qui implémente une interface `IMeshConvertible` peut être convertie en maillage lors de l'exportation vers n'importe quel format de fichier 3D.

{{% /alert %}}
###  **Convertir une sphère en maillage**
Une sphère est un objet géométrique parfaitement rond dans un espace tridimensionnel qui apparaît partout, des balles de sport aux planètes dans l'espace. Utilisons la Sphère primitive pour créer un maillage.
L'exemple de code ci-dessous convertit une sphère en maillage.

{{< gist "aspose-3d-gists" "9563193e834f0087b554c83130fcf7c7" "Examples-CSharp-Working-with-Objects-ConvertSpherePrimitivetoMesh-ConvertSpherePrimitivetoMesh.cs" >}}
###  **Convertir une boîte en maillage**
Une boîte décrit une variété de conteneurs et de récipients pour une utilisation permanente comme stockage, ou pour une utilisation temporaire, souvent pour le transport du contenu. Utilisons la boîte primitive pour créer un maillage. L'exemple de code ci-dessous convertit une boîte en maillage.

{{< gist "aspose-3d-gists" "9563193e834f0087b554c83130fcf7c7" "Examples-CSharp-Working-with-Objects-ConvertBoxPrimitivetoMesh-ConvertBoxPrimitivetoMesh.cs" >}}
###  **Convertir un avion en maillage**
Un plan s'étend à l'infini sans épaisseur. Un exemple de plan est un plan de coordonnées. Utilisons la primitive `Plane` pour créer un maillage. L'exemple de code ci-dessous convertit un `Plane` en `Mesh`.

{{< gist "aspose-3d-gists" "9563193e834f0087b554c83130fcf7c7" "Examples-CSharp-Working-with-Objects-ConvertPlanePrimitivetoMesh-ConvertPlanePrimitivetoMesh.cs" >}}
###  **Convertir un cylindre en maille**
Un cylindre est l'une des formes géométriques curvilignes les plus élémentaires, la surface formée par les points à une distance fixe d'une ligne droite donnée, l'axe du cylindre. Il peut être utilisé dans de nombreux endroits, par exemple comme pilier devant une maison ou comme arbre de transmission de voiture. Permet d'utiliser le cylindre primitif pour créer un maillage. L'exemple de code ci-dessous convertit un cylindre en maillage.

{{< gist "aspose-3d-gists" "9563193e834f0087b554c83130fcf7c7" "Examples-CSharp-Working-with-Objects-ConvertCylinderPrimitivetoMesh-ConvertCylinderPrimitivetoMesh.cs" >}}
###  **Convertir un Torus en Maille**
Un tore est une surface de révolution générée en faisant tourner un cercle dans un espace tridimensionnel autour d'un axe coplanaire avec le cercle. Si l'axe de révolution ne touche pas le cercle, la surface a une forme d'anneau et s'appelle un tore de révolution. Utilisons le Torus primitif pour créer un maillage. L'exemple de code ci-dessous convertit un Torus en maillage.

{{< gist "aspose-3d-gists" "9563193e834f0087b554c83130fcf7c7" "Examples-CSharp-Working-with-Objects-ConvertTorusPrimitivetoMesh-ConvertTorusPrimitivetoMesh.cs" >}}
