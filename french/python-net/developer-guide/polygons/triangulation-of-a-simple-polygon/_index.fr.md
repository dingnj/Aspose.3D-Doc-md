---
title: Triangulation d'un polygone simple
type: docs
weight: 30
url: /fr/python-net/triangulation-of-a-simple-polygon/
description: En utilisant Aspose.3D for Python via .NET API, les développeurs peuvent trianguler un polygone simple. Tout polygone peut être divisé en triangles. Toutes les opérations et les calculs pour les triangles peuvent être appliqués par morceaux au polygone.
---
{{% alert color="primary" %}}

En utilisant [Aspose.3D for Python via .NET](https://products.aspose.com/3d/python-net/) API, les développeurs peuvent trianguler un polygone simple. Tout polygone peut être divisé en triangles. Toutes les opérations et les calculs pour les triangles peuvent être appliqués par morceaux au polygone.

{{% /alert %}}
##  **Triangulation d'un polygone**
Les développeurs peuvent choisir des sommets dans une zone de polygone, puis former des triangles en appelant la méthode Triangulate de la classe [`PolygonModifier`](https://reference.aspose.com/3d/net/aspose.threed.entities/polygonmodifier), chacune des formes V{1}, V{i-1}, V{i} avec l'index i allant de 3 à n. Les classes `Vertex` et `PolygonCanvas` dans le fichier `Triangulate/PolygonCanvas.py` sous l'application de démonstration (nom: Triangulate) montre la façon de trianguler un polygone en utilisant Aspose.3D API.

{{% alert color="primary" %}}

Nous avons préparé un projet démo. Veuillez vous référer à [Cette URL](https://github.com/aspose-3d/Aspose.3D-for-.NET/tree/master/Demos).

{{% /alert %}}
###  **Échantillon de programmation pour la triangulation**
Cet exemple de code sélectionne les sommets d'une zone de polygone, puis applique un algorithme pour créer des triangles. Vous pouvez télécharger le projet de travail complet de cet exemple à partir de [Ici](https://github.com/aspose-3d/Aspose.3D-for-.NET/).

{{< gist "aspose-3d-gists" "cfde9f76113134443c76608c1d19453a" "TriangulationSimplePolygon-Triangulate-PolygonCanvas-TriangulationofaSimplePolygon.py" >}}
