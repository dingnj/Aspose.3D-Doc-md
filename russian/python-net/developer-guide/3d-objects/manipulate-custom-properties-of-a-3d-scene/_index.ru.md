---
title: Манипулирование пользовательскими свойствами сцены 3D
type: docs
weight: 80
url: /ru/python-net/manipulate-custom-properties-of-a-3d-scene/
description: Разработчики могут добавлять, извлекать и удалять пользовательские свойства объектов 3D. Члены RemoveProperty, GetProperty, SetProperty объектов 3D представляют собой набор коротких методов для манипулирования настраивающимися свойствами объекта.
---
##  **Добавление, извлечение и удаление пользовательских свойств объекта 3D**
Разработчики могут добавлять, извлекать и удалять пользовательские свойства объектов 3D. `remove_property`, `get_property`, `set_property` члены 3D объектов представляют собой набор коротких методов для манипулирования настраивающимися свойствами объекта. Это пример кода для установки, извлечения и удаления пользовательского свойства:

**Python**

```py

# initialize a scene 

from aspose.threed import Scene
from aspose.threed.entities import Box
from aspose.threed.formats import GLTFSaveOptions, FileFormat

scene = Scene()

# create a Box instance

box = scene.root_node.create_child_node("box", Box())

# add custom property

box.set_property("property-name", "property-value");

box.set_property("property-name2", "property-value2");

# get a custom property by name

property = box.get_property("property-name");

# remove the custom property by name or property instance

box.remove_property("property-name");

box.remove_property(property);

# save 3D scene

opt = GLTFSaveOptions(FileFormat.GLTF2)
opt.save_extras = True

scene.save("test-2.gltf", opt)

```

{{% alert color="primary" %}} 

Чтобы сохранить пользовательские свойства в моделях GLTF, вам необходимо установить `save_extras` на `True`. Значение свойства `save_extras` по умолчанию-`False`.

{{% /alert %}}
