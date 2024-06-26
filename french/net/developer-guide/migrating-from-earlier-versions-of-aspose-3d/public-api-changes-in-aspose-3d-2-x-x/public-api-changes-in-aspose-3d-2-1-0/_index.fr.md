---
title: Public API Changements dans Aspose.3D 2.1.0
type: docs
weight: 10
url: /fr/net/public-api-changes-in-aspose-3d-2-1-0/
---
**Résumé du contenu**

- [Ajoute l'exportation des fichiers Collada](#PublicAPIChangesinAspose.3D2.1.0-AddsExportofColladaFiles)
- [Ajoute des options de chargement et de sauvegarde pour les formats de fichier 3D](#PublicAPIChangesinAspose.3D2.1.0-AddsLoadandSaveOptionsfor3DFileFormats) 
-[Ajoute Aspose.ThreeD.Formats.ColladaSaveOptions classe](#PublicAPIChangesinAspose.3D2.1.0-AddsAspose.ThreeD.Formats.ColladaSaveOptionsclass)
-[Ajoute Aspose.ThreeD.Formats.Discreet3DSLoadOptions Classe](#PublicAPIChangesinAspose.3D2.1.0-AddsAspose.ThreeD.Formats.Discreet3DSLoadOptionsClass)
-[Ajoute la classe Aspose.ThreeD.Formats. Discreet3DSsaveOptions](#PublicAPIChangesinAspose.3D2.1.0-AddsAspose.ThreeD.Formats.Discreet3DSSaveOptionsClass)
-[Ajoute Aspose.ThreeD.Formats.FBXSaveOptions Class](#PublicAPIChangesinAspose.3D2.1.0-AddsAspose.ThreeD.Formats.FBXSaveOptionsClass)
-[Ajoute la classe Aspose.ThreeD.Formats.ObjLoadOptions](#PublicAPIChangesinAspose.3D2.1.0-AddsAspose.ThreeD.Formats.ObjLoadOptionsClass)
-[Ajoute la classe Aspose.ThreeD.Formats.ObjSaveOptions](#PublicAPIChangesinAspose.3D2.1.0-AddsAspose.ThreeD.Formats.ObjSaveOptionsClass)
-[Ajoute Aspose.ThreeD.Formats.STLLoadOptions Classe](#PublicAPIChangesinAspose.3D2.1.0-AddsAspose.ThreeD.Formats.STLLoadOptionsClass)
-[Ajoute Aspose.ThreeD.Formats.STLSaveOptions Class](#PublicAPIChangesinAspose.3D2.1.0-AddsAspose.ThreeD.Formats.STLSaveOptionsClass)
-[Ajoute la classe Aspose.ThreeD.Formats.U3DLoadOptions](#PublicAPIChangesinAspose.3D2.1.0-AddsAspose.ThreeD.Formats.U3DLoadOptionsClass)
-[Ajoute Aspose.ThreeD.Formats. U3DSAeOptions Class](#PublicAPIChangesinAspose.3D2.1.0-AddsAspose.ThreeD.Formats.U3DSaveOptionsClass)
- [Ajoute des méthodes à Aspose.ThreeD.Scene Class](#PublicAPIChangesinAspose.3D2.1.0-AddsMethodstoAspose.ThreeD.SceneClass)
- [Suppression de la propriété FillDummyIndexArray de la classe Aspose.ThreeD.Formats.FBXConfig](#PublicAPIChangesinAspose.3D2.1.0-RemovalofFillDummyIndexArrayPropertyfromAspose.ThreeD.Formats.FBXConfigClass)
- [Détecter le type d'un fichier 3D](#PublicAPIChangesinAspose.3D2.1.0-DetecttheTypeofa3DFile) 
-[Ajoute les méthodes Detect, CreateLoadOptions et CreateSaveOptions dans la classe Aspose.ThreeD.FileFormat](#PublicAPIChangesinAspose.3D2.1.0-AddsDetect,CreateLoadOptionsandCreateSaveOptionsMethodsintheAspose.ThreeD.FileFormatClass)
- [Ajoute la propriété exclue aux classes Aspose.ThreeD.Entity et Aspose.ThreeD.Node](#PublicAPIChangesinAspose.3D2.1.0-AddsExcludedPropertytoAspose.ThreeD.EntityandAspose.ThreeD.NodeClasses)
- [Ajoute Aspose.ThreeD.Render.RenderState Class et Aspose.ThreeD.Render.BlendFactor/CompareFunction/CullFaceMode/FrontFace/PolygonMode/StencilAction/StencilState Enums](#PublicAPIChangesinAspose.3D2.1.0-AddsAspose.ThreeD.Render.RenderStateClassandAspose.ThreeD.Render.BlendFactor/CompareFunction/CullFaceMode/FrontFace/PolygonMode/StencilAction/StencilStateEnums)
- [Ajoute des API Shader](#PublicAPIChangesinAspose.3D2.1.0-AddsShaderAPIs) 
-[Ajoute une classe abstraite Aspose.ThreeD.Render.ShaderSource et une sous-classe Aspose.ThreeD.Render. GSLSource](#PublicAPIChangesinAspose.3D2.1.0-AddsanabstractclassAspose.ThreeD.Render.ShaderSourceandsubclassAspose.ThreeD.Render.GLSLSource)
-[Ajoute Aspose.ThreeD.Render.ShaderException Class](#PublicAPIChangesinAspose.3D2.1.0-AddsAspose.ThreeD.Render.ShaderExceptionClass)
-[Ajoute la classe Aspose.ThreeD.Render.ShaderProgram](#PublicAPIChangesinAspose.3D2.1.0-AddsAspose.ThreeD.Render.ShaderProgramClass)
-[Ajouter Aspose.ThreeD.Render.ShaderVariable Class](#PublicAPIChangesinAspose.3D2.1.0-AddAspose.ThreeD.Render.ShaderVariableClass)
-[Ajoute une classe Enum Aspose.ThreeD.Render.VariableSemantic](#PublicAPIChangesinAspose.3D2.1.0-AddsanEnumClassAspose.ThreeD.Render.VariableSemantic)
- [Ajoute des API tampons](#PublicAPIChangesinAspose.3D2.1.0-AddsBufferAPIs) 
-[Ajoute une interface Aspose.ThreeD.Render.IBuffer](#PublicAPIChangesinAspose.3D2.1.0-AddsanInterfaceAspose.ThreeD.Render.IBuffer)
-[Ajoute des interfaces Aspose.ThreeD.Render.IIndexBuffer/IVertexBuffer](#PublicAPIChangesinAspose.3D2.1.0-AddsInterfacesAspose.ThreeD.Render.IIndexBuffer/IVertexBuffer)
-[Ajoute un Enum Aspose.ThreeD.Render.IndexDataType](#PublicAPIChangesinAspose.3D2.1.0-AddsanEnumAspose.ThreeD.Render.IndexDataType)
- [Ajoute des API de Render](#PublicAPIChangesinAspose.3D2.1.0-AddsRenderAPIs) 
-[Ajoute une interface Aspose.ThreeD.Render.IRenderable](#PublicAPIChangesinAspose.3D2.1.0-AddsanInterfaceAspose.ThreeD.Render.IRenderable)
-[Ajout d'un Enum Aspose.ThreeD.Render.DrawOperation](#PublicAPIChangesinAspose.3D2.1.0-AddedanEnumAspose.ThreeD.Render.DrawOperation)
-[Ajoute un Enum Aspose.ThreeD.Render.RenderQueueGroupId](#PublicAPIChangesinAspose.3D2.1.0-AddsanEnumAspose.ThreeD.Render.RenderQueueGroupId)
-[Ajoute Aspose.ThreeD.Render.RenderResource Class](#PublicAPIChangesinAspose.3D2.1.0-AddsAspose.ThreeD.Render.RenderResourceClass)
-[Ajoute la classe Aspose.ThreeD.Render.RenderableResource](#PublicAPIChangesinAspose.3D2.1.0-AddsAspose.ThreeD.Render.RenderableResourceClass)
-[Ajoute la classe Aspose.ThreeD.Entities.ManualEntity](#PublicAPIChangesinAspose.3D2.1.0-AddsAspose.ThreeD.Entities.ManualEntityClass)
- [Ajoute plusieurs méthodes de triangulation dans la classe Aspose.ThreeD.Entities.PolygonModifier](#PublicAPIChangesinAspose.3D2.1.0-AddsMultipleTriangulateMethodsintheAspose.ThreeD.Entities.PolygonModifierClass)
- [Ajoute les méthodes CreateVertexBuffer, CreateIndexBuffer, CreateTextureUnit, CreateRenderState et CreateShaderProgram dans la classe Aspose.ThreeD.Render.RenderFactory](#PublicAPIChangesinAspose.3D2.1.0-AddsCreateVertexBuffer,CreateIndexBuffer,CreateTextureUnit,CreateRenderStateandCreateShaderProgramMethodsintheAspose.ThreeD.Render.RenderFactoryClass)
- [Ajoute les méthodes BindRenderState, DrawIndexed, Draw et SubmitRenderTask dans la classe Aspose.ThreeD.Render.Renderer](#PublicAPIChangesinAspose.3D2.1.0-AddsBindRenderState,DrawIndexed,DrawandSubmitRenderTaskMethodsintheAspose.ThreeD.Render.RendererClass)
- [Ajoute les propriétés RenderStage et Shader dans la classe Aspose.ThreeD.Render.Renderer](#PublicAPIChangesinAspose.3D2.1.0-AddsRenderStageandShaderPropertiesintheAspose.ThreeD.Render.RendererClass)

{{% alert color="primary" %}} 

Ce document décrit les modifications apportées à Aspose.3D API de la version 2.0.0 à 2.1.0, qui peuvent intéresser les développeurs de modules/applications. Il inclut non seulement des méthodes publiques nouvelles et mises à jour, mais aussi une description de tout changement de comportement dans les coulisses de Aspose.3D.

{{% /alert %}} 
###  **Ajoute l'exportation des fichiers Collada**
En utilisant cette version récente (2.1.0), les développeurs peuvent exporter des fichiers Collada 3D. Dans la version précédente (2.0.0), nous avons déjà ajouté sa fonctionnalité d'importation, car les développeurs peuvent également convertir un fichier Collada vers d'autres formats de fichier 3D pris en charge.
###  **Ajoute des options de chargement et de sauvegarde pour les formats de fichier 3D**
Nous avons ajouté des options de charge et de sauvegarde pour chaque format de fichier. Ils sont refactorisés à partir des sous-classes IOConfig originales.
####  **Ajoute Aspose.ThreeD.Formats.ColladaSaveOptions classe**
Il définit les paramètres de sauvegarde d'un fichier Collada 3D.

**C#**

{{< highlight "csharp" >}}

 ColladaSaveOptions opts = new ColladaSaveOptions();

// generates indented XML document

opts.Indented = true;

// the style of node transformation

opts.TransformStyle = ColladaTransformStyle.Matrix;

// configure the look up paths to allow importer to find external dependencies.

opts.LookupPaths = new List<string>(new string[] { @"c:\temp\" });

{{< /highlight >}}
####  **Ajoute Aspose.ThreeD.Formats.Discreet3DSLoadOptions Classe**
Il définit les paramètres de chargement d'un fichier 3DS discret.

**C#**

{{< highlight "csharp" >}}

 Discreet3DSLoadOptions loadOpts = new Discreet3DSLoadOptions();

// sets weather to use the transformation defined in the first frame of animation track.

loadOpts.ApplyAnimationTransform = true;

// flip the coordinate system

loadOpts.FlipCoordinateSystem = true;

// prefer to use gamma-corrected color if a 3ds file provides both original color and gamma-corrected color.

loadOpts.GammaCorrectedColor = true;

// configure the look up paths to allow importer to find external dependencies.

loadOpts.LookupPaths = new List<string>(new string[] { @"c:\temp\" });

{{< /highlight >}}
####  **Ajoute la classe Aspose.ThreeD.Formats. Discreet3DSsaveOptions**
Il définit les paramètres de sauvegarde d'un fichier discret 3DS.

**C#**

{{< highlight "csharp" >}}

 // initialize an object

Discreet3DSSaveOptions saveOpts = new Discreet3DSSaveOptions();

// the start base for generating new name for duplicated names.

saveOpts.DuplicatedNameCounterBase = 2;

// the format of the duplicated counter.

saveOpts.DuplicatedNameCounterFormat = "NameFormat";

// the separator between object's name and the duplicated counter.

saveOpts.DuplicatedNameSeparator = "Separator";

// allows to export cameras

saveOpts.ExportCamera = true;

// allows to export light

saveOpts.ExportLight = true;

// flip the coordinate system

saveOpts.FlipCoordinateSystem = true;

// prefer to use gamma-corrected color if a 3ds file provides both original color and gamma-corrected color.

saveOpts.GammaCorrectedColor = true;

// use high-precise color which each color channel will use 32bit float.

saveOpts.HighPreciseColor = true;

// configure the look up paths to allow importer to find external dependencies.

saveOpts.LookupPaths = new List<string>(new string[] { @"c:\temp\" });

// set the master scale

saveOpts.MasterScale = 1;

{{< /highlight >}}
####  **Ajoute Aspose.ThreeD.Formats.FBXSaveOptions Class**
Il définit les paramètres sur l'enregistrement d'un fichier FBX.

**C#**

{{< highlight "csharp" >}}

 // initialize an object

FBXSaveOptions saveOpts = new FBXSaveOptions(FileFormat.FBX7500ASCII);

// generates the legacy material properties.

saveOpts.ExportLegacyMaterialProperties = true;

// fold repeated curve data using FBX's animation reference count

saveOpts.FoldRepeatedCurveData = true;

// always generates material mapping information for geometries if the attached node contains materials.

saveOpts.GenerateVertexElementMaterial = true;

// configure the look up paths to allow importer to find external dependencies.

saveOpts.LookupPaths = new List< string > (new string[] { @"c:\temp\" });

// generates a video object for texture.

saveOpts.VideoForTexture = true;

{{< /highlight >}}
####  **Ajoute la classe Aspose.ThreeD.Formats.ObjLoadOptions**
Il définit les paramètres sur le chargement d'un fichier Obj.

**C#**

{{< highlight "csharp" >}}

 // initialize an object

ObjLoadOptions loadObjOpts = new ObjLoadOptions();

// import materials from external material library file

loadObjOpts.EnableMaterials = true;

// flip the coordinate system.

loadObjOpts.FlipCoordinateSystem = true;

// configure the look up paths to allow importer to find external dependencies.

loadObjOpts.LookupPaths = new List<string>(new string[] { @"c:\temp\" });

{{< /highlight >}}
####  **Ajoute la classe Aspose.ThreeD.Formats.ObjSaveOptions**
Il définit les paramètres sur la sauvegarde d'un fichier Obj.

**C#**

{{< highlight "csharp" >}}

 // initialize an object

ObjSaveOptions saveObjOpts = new ObjSaveOptions();

// import materials from external material library file

saveObjOpts.EnableMaterials = true;

// flip the coordinate system.

saveObjOpts.FlipCoordinateSystem = true;

// configure the look up paths to allow importer to find external dependencies.

saveObjOpts.LookupPaths = new List<string>(new string[] { @"c:\temp\" });

// serialize W component in model's vertex position

saveObjOpts.SerializeW = true;

// generate comments for each section

saveObjOpts.Verbose = true;

{{< /highlight >}}
####  **Ajoute Aspose.ThreeD.Formats.STLLoadOptions Classe**
Il définit les paramètres de chargement d'un fichier STL.

**C#**

{{< highlight "csharp" >}}

 // initialize an object

STLLoadOptions loadSTLOpts = new STLLoadOptions();

// flip the coordinate system.

loadSTLOpts.FlipCoordinateSystem = true;

// configure the look up paths to allow importer to find external dependencies.

loadSTLOpts.LookupPaths = new List<string>(new string[] { @"c:\temp\" });

{{< /highlight >}}
####  **Ajoute Aspose.ThreeD.Formats.STLSaveOptions Class**
Il définit les paramètres sur l'enregistrement d'un fichier STL.

**C#**

{{< highlight "csharp" >}}

 // initialize an object

STLSaveOptions saveSTLOpts = new STLSaveOptions();

// flip the coordinate system.

saveSTLOpts.FlipCoordinateSystem = true;

// configure the look up paths to allow importer to find external dependencies.

saveSTLOpts.LookupPaths = new List<string>(new string[] { @"c:\temp\" });

{{< /highlight >}}
####  **Ajoute la classe Aspose.ThreeD.Formats.U3DLoadOptions**
Il définit les paramètres de chargement d'un fichier U3D.

**C#**

{{< highlight "csharp" >}}

 // initialize an object

U3DLoadOptions loadU3DOpts = new U3DLoadOptions();

// flip the coordinate system.

loadU3DOpts.FlipCoordinateSystem = true;

// configure the look up paths to allow importer to find external dependencies.

loadU3DOpts.LookupPaths = new List<string>(new string[] { @"c:\temp\" });

{{< /highlight >}}
####  **Ajoute Aspose.ThreeD.Formats. U3DSAeOptions Class**
Il définit les paramètres de sauvegarde d'un fichier U3D.

**C#**

{{< highlight "csharp" >}}

 // initialize an object

U3DSaveOptions saveU3DOptions = new U3DSaveOptions();

// export normal data.

saveU3DOptions.ExportNormals = true;

// export the texture coordinates.

saveU3DOptions.ExportTextureCoordinates = true;

// export the vertex diffuse color.

saveU3DOptions.ExportVertexDiffuse = true;

// export vertex specular color

saveU3DOptions.ExportVertexSpecular = true;

// flip the coordinate system.

saveU3DOptions.FlipCoordinateSystem = true;

// configure the look up paths to allow importer to find external dependencies.

saveU3DOptions.LookupPaths = new List<string>(new string[] { @"c:\temp\" });

// compress the mesh data

saveU3DOptions.MeshCompression = true;

{{< /highlight >}}
###  **Ajoute des méthodes à Aspose.ThreeD.Scene Class**
Nous avons surchargé les méthodes Open et Save dans la classe Scene. Les développeurs peuvent transmettre un objet de flux ou un nom de fichier direct pour importer/exporter un fichier 3D en utilisant les différentes options de chargement/sauvegarde.

**C#**

{{< highlight "csharp" >}}

 public void Open(System.IO.Stream stream, Aspose.ThreeD.Formats.LoadOptions options);

public void Open(string fileName, Aspose.ThreeD.Formats.LoadOptions options);

public void Save(System.IO.Stream stream, Aspose.ThreeD.Formats.SaveOptions options);

public void Save(string fileName, Aspose.ThreeD.Formats.SaveOptions options);

{{< /highlight >}}
###  **Suppression de la propriété FillDummyIndexArray de la classe Aspose.ThreeD.Formats.FBXConfig**
Cette propriété n'était pas utilisée.

**C#**

{{< highlight "csharp" >}}

 System.Nullable<Boolean> FillDummyIndexArray{ get;set;}

{{< /highlight >}}
###  **Détecter le type d'un fichier 3D**
La méthode Detect de la classe Aspose.ThreeD.FileFormat peut reconnaître le type de tout fichier 3D pris en charge.

**C#**

{{< highlight "csharp" >}}

 FileFormat inputFormat = FileFormat.Detect(@"C:\ThreeD\test06\colors.fbx");

Console.WriteLine("File Format: " + inputFormat.ToString());

{{< /highlight >}}
####  **Ajoute les méthodes Detect, CreateLoadOptions et CreateSaveOptions dans la classe Aspose.ThreeD.FileFormat**
Après la reconnaissance d'un type de fichier 3D, les développeurs peuvent créer des objets LoadOptions et SaveOptions pour les tâches de manipulation ultérieures.

**C#**

{{< highlight "csharp" >}}

 // allows to detect file format from file stream or filename

static Aspose.ThreeD.FileFormat Detect(System.IO.Stream stream, string fileName)

// allows to detect file format from filename

static Aspose.ThreeD.FileFormat Detect(string fileName)

// create default load options for this file format

Aspose.ThreeD.Formats.LoadOptions CreateLoadOptions()

// create default save options for this file format

Aspose.ThreeD.Formats.SaveOptions CreateSaveOptions()

{{< /highlight >}}
###  **Ajoute la propriété exclue aux classes Aspose.ThreeD.Entity et Aspose.ThreeD.Node**
Il permet de supprimer une entité lors de l'exportation.

**C#**

{{< highlight "csharp" >}}

 bool Excluded{ get;set;}

{{< /highlight >}}
###  **Ajoute Aspose.ThreeD.Render.RenderState Class et Aspose.ThreeD.Render.BlendFactor/CompareFunction/CullFaceMode/FrontFace/PolygonMode/StencilAction/StencilState Enums**
Les états de rendu fournissent des paramètres au GPU pour rastériser les triangles en pixels.

{{% alert color="primary" %}} 

Encapsulation des états de rendu matériel, des informations détaillées peuvent être trouvées dans la documentation de [OpenGL 4.0](https://www.opengl.org/sdk/docs/man/html/glEnable.xhtml), [DirectX 11](https://msdn.microsoft.com/en-us/library/windows/desktop/hh404489\(v=vs.85\).aspx), [DirectX 9](https://msdn.microsoft.com/en-us/library/windows/desktop/bb147327\(v=vs.85\).aspx) et [Vulkan](https://www.khronos.org/registry/vulkan/specs/1.0/xhtml/vkspec.html#VkPipelineRasterizationStateCreateInfo)

{{% /alert %}} 
###  **Ajoute des API Shader**
Les API Shader définissent comment transformer les triangles de l'espace mondial en espace d'écran et calculer la couleur finale du pixel du côté GPU.
####  **Ajoute une classe abstraite Aspose.ThreeD.Render.ShaderSource et une sous-classe Aspose.ThreeD.Render. GSLSource**
Le GLSLSource indique au moteur de rendu, le code source est pour le langage d'ombrage OpenGL, il peut être compilé en Aspose.ThreeD.Render.ShaderProgram.
####  **Ajoute Aspose.ThreeD.Render.ShaderException Class**
Les exceptions liées à Shader, principalement utilisées dans l'étape de compilation et de liaison du langage shader.
####  **Ajoute la classe Aspose.ThreeD.Render.ShaderProgram**
C'est le programme de shader compilé.
####  **Ajouter Aspose.ThreeD.Render.ShaderVariable Class**
Il définit les variables utilisées dans shader.
####  **Ajoute une classe Enum Aspose.ThreeD.Render.VariableSemantic**
Il est utilisé pour identifier la sémantique de la variable shader, Aspose. Le rendu 3D préparera automatiquement les valeurs des variables de shader en fonction de la sémantique.
###  **Ajoute des API tampons**
Les tampons fournissent la définition et les données des triangles.
####  **Ajoute une interface Aspose.ThreeD.Render.IBuffer**
C'est l'interface de base pour IIndexBuffer et IVertexBuffer.
####  **Ajoute des interfaces Aspose.ThreeD.Render.IIndexBuffer/IVertexBuffer**
Ils présentent des tampons matériels pour stocker les indices de géométrie.
####  **Ajoute un Enum Aspose.ThreeD.Render.IndexDataType**
Le type de données des indices de géométrie.
###  **Ajoute des API de Render**
####  **Ajoute une interface Aspose.ThreeD.Render.IRenderable**
Un objet qui prend en charge le rendu doit implémenter cette interface.
####  **Ajout d'un Enum Aspose.ThreeD.Render.DrawOperation**
Le type primitif à dessiner.
####  **Ajoute un Enum Aspose.ThreeD.Render.RenderQueueGroupId**
Aspose.3D API utilise la file d'attente de rendu pour gérer le flux de travail de rendu, ceci est utilisé pour soumettre l'opération de rendu à la file d'attente de rendu spécifiée.
####  **Ajoute Aspose.ThreeD.Render.RenderResource Class**
Base class for bridging the Aspose.3D's model API to hardware resources, this is used by Aspose.3D internally, but exposed to unleash the full power of Aspose.3D rendering.
####  **Ajoute la classe Aspose.ThreeD.Render.RenderableResource**
Une sous-classe de RenderResource, mais concentrez-vous sur le rendu.
####  **Ajoute la classe Aspose.ThreeD.Entities.ManualEntity**
L'utilisateur doit utiliser cette classe pour implémenter sa propre entité qui prend en charge le rendu, cette classe encapsule les détails des opérations de rendu et de la gestion des ressources.
###  **Ajoute plusieurs méthodes de triangulation dans la classe Aspose.ThreeD.Entities.PolygonModifier**
Plus de surcharges pour simplifier l'utilisation de la fonction d'origine.

**C#**

{{< highlight "csharp" >}}

 public static int[][] Triangulate(IList<[Aspose.ThreeD.Utilities.Vector4> controlPoints, IList<int[]> polygons);

public static int[][] Triangulate(IList<[Aspose.ThreeD.Utilities.Vector4> controlPoints, Int32[] polygon);

public static int[][] Triangulate(IList<Aspose.ThreeD.Utilities.Vector4> controlPoints);

{{< /highlight >}}
###  **Ajoute les méthodes CreateVertexBuffer, CreateIndexBuffer, CreateTextureUnit, CreateRenderState et CreateShaderProgram dans la classe Aspose.ThreeD.Render.RenderFactory**
**C#**

{{< highlight "csharp" >}}

 public Aspose.ThreeD.Render.IVertexBuffer CreateVertexBuffer(Aspose.ThreeD.Utilities.VertexDeclaration declaration)

public Aspose.ThreeD.Render.IIndexBuffer CreateIndexBuffer()

public Aspose.ThreeD.Render.ITextureUnit CreateTextureUnit()

public Aspose.ThreeD.Render.RenderState CreateRenderState()

public Aspose.ThreeD.Render.ShaderProgram CreateShaderProgram(Aspose.ThreeD.Render.ShaderSource shaderSource, IList<Aspose.ThreeD.Utilities.VertexField> inputFields)

public Aspose.ThreeD.Render.ShaderProgram CreateShaderProgram(Aspose.ThreeD.Render.ShaderSource shaderSource, Aspose.ThreeD.Utilities.VertexDeclaration vertexDeclaration)

{{< /highlight >}}
###  **Ajoute les méthodes BindRenderState, DrawIndexed, Draw et SubmitRenderTask dans la classe Aspose.ThreeD.Render.Renderer**
**C#**

{{< highlight "csharp" >}}

 public void BindRenderState(Aspose.ThreeD.Render.RenderState renderState)

public void DrawIndexed(Aspose.ThreeD.Render.DrawOperation drawOperation, Aspose.ThreeD.Render.IVertexBuffer vertexBuffer, Aspose.ThreeD.Render.IIndexBuffer indexBuffer, Int32 count)

public void Draw(Aspose.ThreeD.Render.DrawOperation drawOperation, Aspose.ThreeD.Render.IVertexBuffer vertexBuffer, Int32 first, Int32 count)

public void Draw(Aspose.ThreeD.Render.DrawOperation drawOperation, Aspose.ThreeD.Render.IVertexBuffer vertexBuffer)

public void DrawIndexed(Aspose.ThreeD.Render.DrawOperation drawOperation, Aspose.ThreeD.Render.IVertexBuffer vertexBuffer, Aspose.ThreeD.Render.IIndexBuffer indexBuffer)

public void SubmitRenderTask(Aspose.ThreeD.Render.RenderQueueGroupId groupId, Int32 priority, Aspose.ThreeD.Render.IRenderable renderableTask)

{{< /highlight >}}
###  **Ajoute les propriétés RenderStage et Shader dans la classe Aspose.ThreeD.Render.Renderer**
**C#**

{{< highlight "csharp" >}}

 public RenderStage RenderStage { get; }

public Aspose.ThreeD.Render.ShaderProgram Shader{ get;set;}

{{< /highlight >}}
