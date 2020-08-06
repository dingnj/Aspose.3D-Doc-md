---
title : "Public API Changes in Aspose.3D 17.01" 
description : "" 
weight : 20076 
toc : false
type: docs
url: /net/developerguide/knowledgebase/migratingfromearliervs/changesin17x/public+api+changes+in+aspose.3d+17.01/
---

# Aspose.3D for .NET : Public API Changes in Aspose.3D 17.01


{{< panel title="Contents Summary" style="primary" >}}
*   [Adds PLY Format Entry in the Aspose.ThreeD.FileFormat Class](#adds-ply-format-entry-in-the-aspose.threed.fileformat-class)
*   [Importing PLY Files](#importing-ply-files)
*   [Adds Aspose.ThreeD.GlobalTransform Class](#adds-aspose.threed.globaltransform-class)
*   [Adds a GlobalTransform property to Aspose.ThreeD.Node Class](#adds-a-globaltransform-property-to-aspose.threed.node-class)
*   [Adds Polygons property to Aspose.ThreeD.Entities.Mesh Class](#adds-polygons-property-to-aspose.threed.entities.mesh-class)
*   [Load 3D File and Write Meshes in Custom Binary Format](#load-3d-file-and-write-meshes-in-custom-binary-format)
*   [Removes CreateStream member from Aspose.ThreeD.Formats.IOConfig Class](#removes-createstream-member-from-aspose.threed.formats.ioconfig-class)
{{< /panel >}}
This document describes changes to the Aspose.3D API from version 16.12.0 to 17.1.0, that may be of interest to module/application developers. It includes not only new and updated public methods, but also a description of any changes in the behavior behind the scenes in Aspose.3D.

### Adds PLY Format Entry in the Aspose.ThreeD.FileFormat Class

We have added a PLY format entry for loading purposes.

### Importing PLY Files

Using the recent version (17.01) or higher, developers can import PLY files. The PLY format entry is added for loading purposes.

**C#**

{{< code lang="c#" >}}
// an entry of PLY file in the FileFormat class
public static readonly Aspose.ThreeD.FileFormat PLY;
// initialize Scene class object
Scene scene = new Scene();
// initialize an object
PlyLoadOptions loadPLYOpts = new PlyLoadOptions();
// Flip the coordinate system.
loadPLYOpts.FlipCoordinateSystem = true;
// load 3D Ply model
scene.Open( "3DPlyModel.ply", loadPLYOpts);
{{< /code >}}

### Adds Aspose.ThreeD.GlobalTransform Class

The GlobalTransform class provides exactly the same interface like Transform but all its properties are read-only. It is useful for the global transform purposes.

### Adds a GlobalTransform property to Aspose.ThreeD.Node Class

It allows to access the node's global transform. This is useful to transform the scene into the user's custom file format.

### Adds Polygons property to Aspose.ThreeD.Entities.Mesh Class

It allows to get all polygons inside the mesh, each polygon is an array of polygon vertex index. Before this property, we have to use foreach syntax to enumerate each polygon which is inefficient.

### Load 3D File and Write Meshes in Custom Binary Format

**C#**

string = @"c:\\temp\\input.stl", output = @"c:\\temp\\output";// load a 3D fileScene scene = new Scene(input);/\*\* 3D format demonstration is simple\* \* struct File {\*   MeshBlock blocks\[\];\* };\*\* struct Vertex {\*   float x;\*   float y;\*   float z;\* };\* \* struct Triangle {\*   int a;\*   int b;\*   int c;\* };\* \* struct MeshBlock {\*   int numControlPoints;\*   int numTriangles;\*   Vertex vertices\[numControlPoints\];\*   Triangle faces\[numTriangles\];\* };\*/// open file for writing in binary modeusing (var writer = new BinaryWriter(new FileStream(output, FileMode.Create, FileAccess.Write))){    // visit each descent nodes    scene.RootNode.Accept(delegate (Node node)    {        foreach (Entity entity in node.Entities)        {            // only convert meshes, lights/camera and other stuff will be ignored            if (!(entity is IMeshConvertible))                continue;            Mesh m = ((IMeshConvertible)entity).ToMesh();            var controlPoints = m.ControlPoints;            // triangulate the mesh, so triFaces will only store triangle indices            int\[\]\[\] triFaces = PolygonModifier.Triangulate(controlPoints, m.Polygons);            // gets the global transform matrix            Matrix4 transform = node.GlobalTransform.TransformMatrix;            // write number of control points and triangle indices            writer.Write(controlPoints.Count);            writer.Write(triFaces.Length);            // write control points            for (int i = 0; i < controlPoints.Count; i++)            {                // calculate the control points in world space and save them to file                var cp = transform \* controlPoints\[i\];                writer.Write((float)cp.x);                writer.Write((float)cp.y);                writer.Write((float)cp.z);            }            // write triangle indices            for (int i = 0; i < triFaces.Length; i++)            {                writer.Write(triFaces\[i\]\[0\]);                writer.Write(triFaces\[i\]\[1\]);                writer.Write(triFaces\[i\]\[2\]);            }        }        return true;    });}

### Removes CreateStream member from Aspose.ThreeD.Formats.IOConfig Class

This was marked as obsolete in version 16.11.0, the new interface FileSystem was introduced in version 16.11.0 which provides more extensibility.

  
