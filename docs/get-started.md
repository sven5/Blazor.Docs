---
title: Get started with Blazor
author: danroth27
description: Learn how to get started with the Blazor framework.
manager: wpickett
ms.author: riande
ms.custom: mvc
ms.date: 04/16/2018
ms.prod: asp.net-core
ms.technology: aspnet
ms.topic: article
uid: client-side/blazor/get-started
---
# Get started with Blazor

[!INCLUDE[](~/includes/blazor-preview-notice.md)]

## Setup

1. Install the [.NET Core 2.1 SDK (2.1.302)](https://go.microsoft.com/fwlink/?linkid=873092).
1. Install [Visual Studio 2017](https://go.microsoft.com/fwlink/?linkid=873093) (15.7 or later) with the *ASP.NET and web development* workload selected.
1. Install the latest [Blazor Language Services extension](https://go.microsoft.com/fwlink/?linkid=870389) from the Visual Studio Marketplace.

To create your first project from Visual Studio:

1. Select **File** > **New Project** > **Web** > **ASP.NET Core Web Application**.
1. Make sure **.NET Core** and **ASP.NET Core 2.1** (or later) are selected at the top.
1. Choose the Blazor template and select **OK**.

   ![New Blazor app dialog](https://msdnshared.blob.core.windows.net/media/2018/07/new-blazor-app-dialog-0.5.0.png)
   
1. Press **Ctrl-F5** to run the app *without the debugger*. Running with the debugger (**F5**) isn't supported at this time.

You can also install and use the Blazor templates from the command-line:

```console
dotnet new -i Microsoft.AspNetCore.Blazor.Templates
dotnet new blazor -o BlazorApp1
cd BlazorApp1
dotnet run
```

Congrats! You just ran your first Blazor app!

![Blazor app home page](https://msdnshared.blob.core.windows.net/media/2018/04/blazor-bootstrap-4.png)

> [!IMPORTANT]
> The default *global.json* file included in the Blazor project templates may cause the project to fail to load or run if you don't have version 2.1.3xx of the .NET Core SDK installed. The *global.json* file pins the project to 2.1.3xx; so if you don't have that specific version range installed, the project fails to load or run even if you have a newer SDK installed. The workaround is to remove the *global.json* file from the project or install version [2.1.302 of the .NET Core SDK](https://github.com/dotnet/core/blob/master/release-notes/2.1/2.1.2.md).

## Help & feedback

Your feedback is especially important to us during this experimental phase for Blazor. If you run into issues or have questions while trying out Blazor, please let us know!

* [File issues on GitHub](https://github.com/aspnet/blazor/issues) for any problems you run into or to make suggestions for improvements.
* Chat with us and the Blazor community on [Gitter](https://gitter.im/aspnet/blazor) if you get stuck or to share how Blazor is working for you.

After you've tried out Blazor, please let us know what you think by taking our in-product survey. Just click the survey link shown on the app home page when running one of the Blazor project templates:

![Blazor survey](https://msdnshared.blob.core.windows.net/media/2018/05/blazor-survey-new.png)

## What's next?

<xref:client-side/blazor/tutorials/first-app>
