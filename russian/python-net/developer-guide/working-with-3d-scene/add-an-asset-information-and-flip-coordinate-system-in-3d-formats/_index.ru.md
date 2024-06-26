---
title: Добавление информации об активах и перевернуть систему координат в форматах 3D
type: docs
weight: 10
url: /ru/python-net/add-an-asset-information-and-flip-coordinate-system-in-3d-formats/
description: Метаданные-это структурированная информация, которая описывает, объясняет, находит или упрощает извлечение, использование или управление информационным ресурсом. Aspose.3D for Python via .NET API позволяет разработчикам определять метаданные для сцены.
---
##  **Добавить информацию об активе в сцену 3D**
Метаданные-это структурированная информация, которая описывает, объясняет, находит или упрощает извлечение, использование или управление информационным ресурсом. Aspose.3D for Python via .NET API позволяет разработчикам определять метаданные для сцены.
###  **Определите метаданные для сцены**
3D показывает производство огромного количества метаданных и информации о изображениях. Метаданные-это актив и часть шоу.

1. Инициализируйте сцену 3D, используя класс `Scene`.
1. Установите имя приложения/инструмента.
1. Установите имя поставщика приложения/инструмента.
1. Установите единицу измерения.
1. Установите масштабный коэффициент единицы измерения.
1. Сохраните сцену 3D в поддерживаемом формате файла.

В этом примере мы предполагаем, что сцена создана инструментом CAD под названием «Египет», и она разработана «Manualdesk»:

{{< gist "aspose-3d-gists" "cfde9f76113134443c76608c1d19453a" "AssetInformation-InformationToScene-AddAssetInformationToScene.py" >}}
##  **Перевернуть систему координат в форматах 3D**
Aspose.3D for Python via .NET API позволяет пользователям переворачивать систему координат в форматах OBJ, 3DS, STL и U3D.

{{% alert color="primary" %}} 

Чтобы импортировать файл 3ds и сохранить его в формате OBJ, в коде используется класс [`Scene`](https://reference.aspose.com/3d/net/aspose.threed/scene).

{{% /alert %}} 

В этом примере мы перевернули систему координат при импорте 3ds файла и сохранили его в формате OBJ без материалов.
