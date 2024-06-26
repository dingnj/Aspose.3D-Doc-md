---
title: Работа с XPath-подобными объектными запросов
type: docs
weight: 120
url: /ru/net/work-with-xpath-like-object-queries/
description: Используя Aspose.3D for .NET, вы можете выбрать один или несколько объектов в текущем узле, используя синтаксис запроса XPath-Like. Синтаксис запроса был вдохновлен XPath, поэтому большинство концепций и синтаксиса похожи, синтаксис запроса совместим с URL, поэтому он будет использоваться в нашей облачной версии в будущем.
---
{{% alert color="primary" %}} 

Эта функция поддерживается версией 19,3 или выше.

{{% /alert %}} 
##  **Работа с XPath-подобными объектными запросов**
Используя Aspose.3D for .NET, вы можете выбрать один или несколько объектов в текущем узле, используя синтаксис запроса XPath-Like. Синтаксис запроса был вдохновлен XPath, поэтому большинство концепций и синтаксиса похожи, синтаксис запроса совместим с URL, поэтому он будет использоваться в нашей облачной версии в будущем. Как правило, синтаксис состоит из**Условие имени префикса** / **Имя Состояние** /.

|**Префикс =**|**Описание =**|
| :- | :- |
| // |Глобальный селектор, любой потомок рассматривается как корневой узел для выполнения выбора|
|/|Корневой селектор, только один предок используется для поиска|
|Другие|Предположим, что это имя, и выберите объект по имени в глобальном режиме селектора|
Имя-это строка, которая соответствует имени объекта, или подстановочный знак `*` используется для сопоставления любого имени. Условие является выражением, определяющим, следует ли выбирать объект, поддерживаются логические операторы (не) и/или операторы сравнения `>/</>=/<=/=/!=`. Для доступа к свойству в выражении условия используется префикс '@', например, `@Name` будет читать свойство Name. Синтаксис ярлыка для тестируемого типа поддерживается `<Mesh>`, это эквивалентно `[@Type = 'Mesh']`, идентификаторы без кавычки будут рассматриваться как строка.
###  **Выберите все узлы, используя глобальный селектор синтаксиса**
{{< highlight "java" >}}

 //<Node>

{{< /highlight >}}

Это короткий синтаксис:

{{< highlight "java" >}}

 //*[<Node>]

{{< /highlight >}}

Или

{{< highlight "java" >}}

 //*[@Type = Node]

{{< /highlight >}}
###  **Выберите узел второго уровня с видимым родителем**
{{< highlight "java" >}}

 //<Node>[@Visible]/<Node>

{{< /highlight >}}

Ниже приводится пример кода для запроса одного или нескольких объектов:

{{< gist "aspose-3d-gists" "9563193e834f0087b554c83130fcf7c7" "Examples-CSharp-Working-with-Objects-XPathLikeObjectQueries-XPathLikeObjectQueries.cs" >}}
