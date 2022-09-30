﻿---
title: Aspose.3D for Java 21.3 Note di rilascio
type: docs
weight: 10
url: /it/java/aspose-3d-for-java-21-3-release-notes/
---
{{% alert color="primary" %}}

Questa pagina contiene le informazioni sulle note di rilascio per lo Aspose.3D for Java 21.3.

{{% /alert %}}
## **Miglioramenti e modifiche**

|**Chiave**|**Riassunto**|**Categoria**|
|:- |:- |:- |
|THREEDNET-847 |Aggiungi supporto per la nuvola di punti in glb|Nuova funzionalità|
|THREEDNET-830 |Fornire mesh di basso livello API per il renderer web.|Miglioramento|
|THREEDNET-838 |Esporta la topografia 2.5D con il colore in un file|Miglioramento|
|THREEDNET-849 |Aggiungi supporto byte[4] nell'esportazione glTF|Miglioramento|
|THREEDNET-832 |Implementare aggeggi per la luce nel renderer web|Miglioramento|
|THREEDNET-833 |Implementare gizmo per fotocamera nel renderer web|Miglioramento|
|THREEDNET-842 |Aggiungi fattore di supporto per analisi UV nel FBX|Miglioramento|
|THREEDNET-852 |Architettura del renderer dell'entità refactor per il renderer web|Attività|
|THREEDNET-836 |Aggiornare i nomi delle classi delle opzioni di salvataggio/caricamento.|Attività|
|THREEDNET-858 |Alcuni file obj non sono stati completamente renderizzati in renderer web.|Correzione di bug|
|THREEDNET-859 |I file X con struttura di animazione non standard non possono essere importati.|Correzione di bug|
|THREEDNET-861 |Impossibile importare file X con dati definiti FVF|Correzione di bug|
|THREEDNET-860 |Impossibile importare file X con più materiali collegati su una singola mesh|Correzione di bug|
|THREEDNET-839 |FBX con il file ConstraintParent non sono supportati.|Correzione di bug|
|THREEDNET-841 |Alcuni vecchi file FBX contengono sezione Forma sotto modello non sono supportati.|Correzione di bug|
|THREEDNET-840 |ASCII FBX Il file con FileId non è riuscito a importare.|Correzione di bug|
|THREEDNET-844 |API sta lanciando un'eccezione durante l'impostazione di una licenza valida nel Core .NET|Correzione di bug|
|THREEDNET-843 |API non sta impostando un'eccezione valida per il lancio di licenze nel progetto Core .NET|Correzione di bug|
|THREEDNET-848 |Alcune nuvole di punti non possono essere esportate in drc|Correzione di bug|
|THREEDNET-854 |Aspose.3D si è bloccato all'importazione di alcuni file collada con definizioni di materiale errate.|Correzione di bug|


## API modifiche ##


Questa versione è principalmente una versione bug-fix, risolto un sacco di bug, e migliorato un sacco di compatibilità per FBX, Collada, DirectX X file.


Solo alcune modifiche minori API.

### Aggiunto nuovo tipo di dati in classe `com.aspose.threed.VertexFieldDataType`:

{{< highlight "java" >}}

    /**
     * Type of byte[4], can be used to represent color with less memory consumption.
     */
    public static final int BYTE_VECTOR4;

{{< /highlight >}}

VertexElementVertexColor in com.aspose.threed.Geometry sarà codificato come un numero intero di 4 byte con il tipo VertexFieldDataType.BYTE _ VECTOR4.

Questo può ridurre molto il file generato finale in glTF/glb che utilizzava il colore dei vertici, molto utile per la codifica di nuvole di punti.

E da questa versione, il com.aspose.threed.PointCloud è supportato in glTF/glb open and save.



### Membri aggiunti alla classe `com.aspose.threed.BoundingBox`


{{< highlight "java" >}}

    /**
     * The size of the bounding box
     */
    public Vector3 getSize();
  
    /**
     * The center of the bounding box.
     */
    public Vector3 getCenter();

{{< /highlight >}}

Ora è più facile ottenere le dimensioni e il centro del riquadro di delimitazione, queste proprietà hanno senso solo quando BoundingBox è finito.
