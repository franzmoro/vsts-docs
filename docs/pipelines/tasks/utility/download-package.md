---
title: Download Package task
description: Download a package from a Package Management feed in Azure Artifacts or TFS.
ms.topic: reference
ms.prod: devops
ms.technology: devops-cicd
ms.assetid: 8d6e8f7e-267d-442d-8c92-1f586864c62f
ms.manager: jillfra
ms.custom: seodec18
ms.author: phwilson
author: chasewilson
ms.date: 12/07/2018
monikerRange: 'azure-devops'
---

# Download Package task

**Azure Pipelines**

Use this task in a build or release pipeline to download a package from a package management feed in Azure Artifacts or TFS.
Requires the Package Management extension.

> [!NOTE]
> This task currently only supports downloading NuGet packages.

::: moniker range="> tfs-2018"

## YAML snippet

[!INCLUDE [temp](../_shared/yaml/DownloadPackageV0.md)]

::: moniker-end

## Arguments

<table><thead><tr><th>Argument</th><th>Description</th></tr></thead>
<tr><td>Feed</td><td>(Required) Select the package source</td></tr>
<tr><td>Package</td><td>(Required) Select the package to download, only NuGet packages are supported currently</td></tr>
<tr><td>Version</td><td>(Required) Version of the package</td></tr>
<tr><td>Destination directory</td><td>(Required) Path on the agent machine where the package will be downloaded</td></tr>


<tr>
<th style="text-align: center" colspan="2"><a href="~/pipelines/process/tasks.md#controloptions" data-raw-source="[Control options](../../process/tasks.md#controloptions)">Control options</a></th>
</tr>

</table>

## Open source

This task is open source [on GitHub](https://github.com/Microsoft/azure-pipelines-tasks). Feedback and contributions are welcome.
