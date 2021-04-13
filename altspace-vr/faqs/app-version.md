---
title: 查找 AltspaceVR 应用版本
description: 了解如何使用 AltspaceVR 应用、设置和客户端日志查找当前正在运行的 AltspaceVR 的版本。
ms.date: 02/10/2021
ms.topic: article
keywords: 应用版本
ms.openlocfilehash: 5d503d3b89cd213696dd53616c5c7e3013aeef01
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212002"
---
# <a name="finding-the-altspacevr-app-version"></a>查找 AltspaceVR 应用版本

在对问题进行故障排除的过程中，可能会询问你当前正在运行的 AltspaceVR 应用程序的版本。

## <a name="in-altspacevr"></a>在 AltspaceVR 中

若要在 AltspaceVR 中查找应用版本，请导航到 " **设置" 菜单** ，然后在左侧导航栏中选择 " **关于** "。 此处报告了 "应用版本"，如下面的屏幕截图中所示。

!["设置" 菜单打开，并打开 "关于面板"](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a>在 Windows 系统设置中

如果通过 Microsoft Store 安装了 AltspaceVR，则还可以在 Windows 系统设置中查找应用版本。  如果无法成功登录到客户端，则此方案适用于报告应用程序版本。

若要在 Windows 系统设置中查找应用版本，请打开 " **开始" 菜单**，在 " **应用 & 功能**" 中输入，然后选择结果。 在应用列表中导航到 **AltspaceVR** 。 左键单击 "AltspaceVR"，然后从出现的菜单中选择 " **高级选项** "。

![突出显示了 "高级" 选项的 "应用和功能" 菜单](images/app-version-img-02.png)

在 "**规范**" 标头下的 "**高级选项**" 中，**应用版本** 应列在 "**版本**" 标签的右侧。

![已突出显示应用版本的高级选项打开](images/app-version-img-03.png)

## <a name="in-client-logs"></a>在客户端日志中

在应用程序启动过程中，AltspaceVR 将客户端日志文件中的应用版本报告为 "Altspace 版本"。 如果无法成功登录到客户端，则这是获取应用程序版本的一个不错的选择，但它确实会在失败之前尝试启动。

## <a name="windows"></a>Windows

在 Windows 上，可以通过 Windows 资源管理器找到客户端日志文件，网址为：

```
%userprofile%\appdata\locallow\altspacevr\altspacevr\Player.log
%userprofile%\appdata\locallow\altspacevr\altspacevr\Player-prev.log
```

每次启动 AltspaceVR 时，都会覆盖此文件。 "唱机" 代表最新的会话，"Player-prev" 表示上一个会话。

## <a name="via-powershell"></a>通过 PowerShell

高级用户可以通过 PowerShell 搜索此字符串的客户端日志，如下所示：

输入：

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

输出：

[2.047] AltspaceVR 版本： 3.2.23. e66c2