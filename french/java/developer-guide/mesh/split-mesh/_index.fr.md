---
title: Maille fendue
type: docs
weight: 10
url: /fr/java/split-mesh/
description: Aspose.3D for Java API a le support pour diviser tous les maillages d'une scène en plusieurs sous-maillages par matériau. La méthode SplitMesh ne divise pas un maillage de la scène, si un seul matériau lui a été attribué. Cela peut être réalisé en utilisant Aspose.3D for Java API.
---
##  **Fractionnez tous les mailles de la scène par matériau**
Aspose.3D for Java API a le support pour diviser tous les maillages d'une scène en plusieurs sous-maillages par matériau. La méthode SplitMesh ne divise pas un maillage de la scène, si un seul matériau lui a été attribué. Cela peut être réalisé en utilisant Aspose.3D for Java API.

{{% alert color="primary" %}} 

`SplitMeshPolicy` enum spécifie la politique de données utilisée dans l'algorithme de division de maillage, il prend en charge deux politiques, partage de données entre sous-maillages ou chaque sous-maillage a ses propres données (uniquement des données utilisées).

{{% /alert %}} 

L'échantillon de code ci-dessous divise toutes les mailles d'une scène par matériau. Chaque sous-maillage partage les mêmes données directes et ne diffère que dans les indices.

{{< gist "aspose-3d-gists" "50e7f479a64956c0bf78841c0799ba76" "aspose-3d-src-examples-mesh-SplitAllMeshesofScenebyMaterial.java" >}}
##  **Diviser un maillage en spécifiant le matériau**
Aspose.3D for Java API a le support pour diviser un maillage en spécifiant manuellement le matériau. L'option de maillage fractionné crée des objets séparés et chaque sous maillage utilisera un seul matériau.
###  **Maille fendue de la boîte**
Cette rubrique d'aide crée un maillage de la boîte pour garder le code complet et court. Les développeurs peuvent construire un maillage manuellement comme rapporté dans cette rubrique d'aide: [Créer un maillage de cube 3D](https://docs.dynabic.com/display/3djava/Create+3D+Mesh+and+Scene). En outre, une boîte est composée de 6 plans et chaque plan deviendra un sous-maillage. L'exemple de code ci-dessous divise un maillage primitif en spécifiant manuellement le matériau.

{{< gist "aspose-3d-gists" "50e7f479a64956c0bf78841c0799ba76" "aspose-3d-src-examples-mesh-SplitMeshbyMaterial.java" >}}
