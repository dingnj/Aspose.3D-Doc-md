---
title: Installation
type: docs
weight: 40
url: /zh/net/installation/
description: 本文介绍如何使用 NuGet 和程序包管理器控制台安装 Aspose.3D，从 .NET - C# 3D 文件格式操作和转换 API。
---
本文介绍如何使用 NuGet 和程序包管理器控制台安装 Aspose.3D，从 .NET - C# 3D 文件格式操作和转换 API。

##  **正在安装 Aspose.3D for .NET 到 NuGet**
NuGet 是面向 .NET 平台的免费开源包管理系统，旨在简化在开发期间将第三方库合并到 .NET 应用程序中的过程。它是一个Visual Studio扩展，可以轻松地在使用 .NET 框架的Visual Studio项目中添加、删除和更新库和工具。通过创建 NuGet 包并将其存储在 NuGet 存储库中，可以轻松地与其他开发人员共享库或工具。安装包时，NuGet 会将文件复制到解决方案并自动进行必要的更改，例如添加引用和更改app.config或web.config文件。如果您决定删除库，NuGet 将删除文件并反转它对项目所做的任何更改，这样就不会留下混乱。
###  **正在引用 Aspose.3D for .NET**
利用这一出色的功能，我们将 [Aspose.3D for .NET](https://www.nuget.org/packages/Aspose.3D) 库捆绑到 NuGet 包中，并将其上传到 NuGet 存储库中。使用此选项，您可以使用 Aspose.3D for .NET 而无需在系统上安装此组件。NuGet 在Visual Studio 2010及更高版本、Visual Web Developer 2010和 Windows Phone Developer Tools 7.1中运行。在我们的测试中，我们使用Visual Studio 2015旗舰版对其进行了测试。

要开始:

1. 在Visual Studio中打开您的解决方案或项目。
1. 将 NuGet 包管理器添加为Visual Studio扩展:
1.选择**工具**菜单后面跟着**扩展经理**.
1.选择**在线画廊**获取在线可用软件包的完整列表。
1.选择**NuGet 包管理器**.
1.点击**下载**.
1.安装软件包管理器后，重新启动Visual Studio以使更改生效。
安装 NuGet 包管理器后，您可以从**管理 NuGet 个包**窗口，或通过在**包管理器控制台**专用Visual Studio窗口。如果选择**工具**接着是**图书馆包管理器**.
###  **使用包管理器控制台安装包**
要使用包管理器控制台引用该组件:

1. 在Visual Studio中打开 .NET 应用程序。
1. 在**工具**菜单，选择**图书馆包管理器**然后**包管理器控制台**.
1. 键入命令 “Install-Package Aspose.3D” 以安装最新的完整版本，或键入命令 “install-Package Aspose.3D -预发行版” 以安装包括热修复程序的最新版本。
1. 按**输入**.
###  **使用包管理器控制台更新包**
如果已通过 NuGet 引用了该组件，请按照以下步骤将引用更新为最新版本:

1. 在Visual Studio中打开 .NET 应用程序。
1. 从**工具**菜单，选择**图书馆包管理器**,接着是**包管理器控制台**要打开包管理器控制台。
1. 键入命令 “Update-Package Aspose.3D” 以引用最新的完整版本，或键入命令 “Update-Package Aspose.3D -预发行版” 以安装包括热修复程序的最新版本。
1. 按**输入**.
###  **使用包管理器GUI安装包**
请按照以下步骤使用包管理器GUI引用组件:

1. 在Visual Studio中打开 .NET 应用程序。
1. 从**工具**菜单，选择**图书馆包管理器**和**管理 NuGet 个包**从**解决方案**选项。
您还可以从解决方案资源管理器中获得类似的选项:
1.右键单击项目名称。
1.选择**管理 NuGet 个包**.
1. 选择**在线**从左侧菜单。
1. 类型**Aspose.3D**进入搜索框以查找 Aspose.3D for .NET。
1. 点击**安装/更新**位于最新版本的 Aspose.3D for .NET 旁边。
