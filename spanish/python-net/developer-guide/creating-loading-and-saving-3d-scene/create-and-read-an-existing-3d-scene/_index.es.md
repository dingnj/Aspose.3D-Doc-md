---
title: Crear y leer una escena 3D existente
type: docs
weight: 10
url: /es/python-net/create-and-read-an-existing-3d-scene/
description: Aspose.3D API admite la creación de las nuevas escenas 3D desde cero y luego guardadas en cualquier formato de archivo compatible. Los desarrolladores también pueden cargar una escena 3D existente para la modificación, la adición o el procesamiento.
---
##  **Crear una escena 3D vacía y guardar en los formatos de archivo 3D compatibles**
Aspose.3D API admite la creación de las nuevas escenas 3D desde cero y luego guardadas en cualquier formato de archivo compatible. Los desarrolladores también pueden cargar una escena 3D existente para la modificación, la adición o el procesamiento.
###  **Creación de un documento de escena 3D**
Siga estos pasos para crear un documento de escena 3D utilizando las API Aspose.3D:

1. Cree una instancia de la clase [`Scene`](https://reference.aspose.com/3d/net/aspose.threed/scene) que represente un documento de escena 3D.
1. Genere un documento 3D Scene llamando al método [`Save`](https://reference.aspose.com/3d/net/aspose.threed/scene/methods/save) del objeto de clase Scene.
####  **Creación de un documento de escena 3D: ejemplos de programación**


{{< gist "aspose-3d-gists" "cfde9f76113134443c76608c1d19453a" "Loading-and-Saving-CreateEmpty3DDocument.py" >}}
##  **Leyendo una escena de 3D**
Con Aspose.3D API, los desarrolladores pueden cargar todos los documentos 3D compatibles. Los constructores disponibles del**Escena**La clase permite hacerlo y aceptan una cadena de ruta de archivo válida. Los formatos de archivo legibles admitidos son los siguientes:

1. FBX 7,7 (ASCII, binario)
1. FBX 7,6 (ASCII, binario)
1. FBX 7,5 (ASCII, binario)
1. FBX 7,4 (ASCII, binario)
1. FBX 7,3 (ASCII, binario)
1. FBX 7,2 (ASCII, binario)
1. STL (ASCII, binario)
1. WavefrontOBJ
1. Discreet3DS
1. Universal3D
1. Collada
1. glTF
1. DXF
1. PLY (ASCII, binario)
1. X (ASCII... Binary)
1. XYZ
1. Draco
1. 3MF
1. RVM (Texto, binario)
1. ASE
1. USDZ
1. USD

Los constructores de la clase `Scene` detectan internamente el formato de documento 3D.
###  **Lectura de una escena 3D: Muestras de programación**
{{< gist "aspose-3d-gists" "cfde9f76113134443c76608c1d19453a" "Loading-and-Saving-ReadExistingScene.py" >}}
