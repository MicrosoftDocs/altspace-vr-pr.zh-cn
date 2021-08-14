---
title: 查找 AltspaceVR 应用版本
description: 了解如何使用 AltspaceVR 应用、设置和客户端日志查找当前正在运行的 AltspaceVR 版本。
ms.date: 02/10/2021
ms.topic: article
keywords: 应用版本
ms.openlocfilehash: fbf67a8302a67ddb916772420949cf0509a0d4a60c472711975c651862438b93
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "119128234"
---
# <a name="finding-the-altspacevr-app-version"></a>查找 AltspaceVR 应用版本

在排查问题时，可能会询问你当前运行的 AltspaceVR 应用的版本。

## <a name="in-altspacevr"></a>在 AltspaceVR 中

若要在 AltspaceVR 中查找应用版本，请导航到设置 **菜单，然后选择****左侧导航栏中** 的"关于"。 此处报告"应用版本"，如以下屏幕截图所示。

![设置打开"关于面板"的菜单](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a>在 Windows System 设置

如果通过 Microsoft Store 安装了 AltspaceVR，则还可以在 Windows 设置中查找应用版本。  如果无法成功登录到客户端，则报告应用版本时，此方案非常合适。

若要在系统设置Windows中查找应用版本，请打开"开始"菜单，键入"应用 **&功能**"，然后选择结果。 导航到 **应用列表中的 AltspaceVR。** 左键单击 AltspaceVR，然后 **从出现的** 菜单中选择"高级选项"。

!["应用和功能"菜单打开，突出显示了高级选项](images/app-version-img-02.png)

在 **"高级选项"** 的"**规范"** 标头下，"版本"标签右侧应列出 **"应用版本**"。 

![打开高级选项，并突出显示应用版本](images/app-version-img-03.png)

## <a name="in-client-logs"></a>在客户端日志中

AltspaceVR 在应用程序启动期间将客户端日志文件中的应用版本报告为"Altspace 版本"。 如果无法成功登录到客户端，但尝试在失败之前启动，则这是获取应用版本的一个不错的选择。

## <a name="windows"></a>Windows

在Windows，可以通过以下位置的 Windows 资源管理器找到客户端日志文件：

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
```

每次启动 AltspaceVR 时，此文件将被覆盖。 "Player.log"表示最新会话，"Player-prev.log"表示上一个会话。

## <a name="via-powershell"></a>通过 PowerShell

高级用户可以通过 PowerShell 在客户端日志中搜索此字符串，如下所示：

输入：

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

输出：

[2.047] AltspaceVR 版本：3.2.23.e66c2