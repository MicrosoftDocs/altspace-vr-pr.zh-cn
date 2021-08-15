---
title: 我无法启动 AltspaceVR
description: 了解如何识别、报告和修复与启动 AltspaceVR 环境有关的任何问题。
ms.date: 02/10/2021
ms.topic: article
keywords: 常见问题
ms.openlocfilehash: 50edddef669aca14640fd6e910c12c15864cf46a099e54bceed40494e9817de4
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127923"
---
# <a name="i-cant-launch-altspacevr"></a>我无法启动 AltspaceVR

AltspaceVR 可能无法启动的原因有多种。 尝试执行以下步骤，以确保应用程序正确安装了必要的第三方软件。

## <a name="if-youre-trying-to-launch-altspacevr-for-the-first-time"></a>如果是第一次尝试启动 AltspaceVR：

1. 验证你的设备是否受支持并满足 [指定的最低要求](../getting-started/system-requirements.md)。
2. 请确保已安装最新的[Oculus 软件](https://www.oculus.com/setup)，并且设置 > 常规 > 未知设备设置为 ON。 如果在2D 模式下启动，则无需安装 Oculus。
3. 请确保你具有有效的 internet 连接。 如果尝试从网络防火墙内启动 Altspace，请打开 UDP 端口5055和5056，以及 TCP 端口80和443。 如果你在公司或教育防火墙的网络内，你可能需要联系网络管理员或 IT 部门。
4. 另请参阅：
    * [为 Oculus 寻找安装 AltspaceVR](../getting-started/oculus-installation.md)
    * [为 Windows Mixed Reality 安装 AltspaceVR](../getting-started/wmr-installation.md)

## <a name="if-altspacevr-reports-that-the-current-version-is-out-of-date"></a>如果 AltspaceVR 报告当前版本已过期：

* 你使用的应用程序版本不再受支持。 如果已通过店面下载 AltspaceVR，则可能会在你的应用商店更新你的客户端之前最近启动了更新。
* 如果要强制更新，可以通过各种商店实现此目的：
    * **Microsoft Store：** [Microsoft Store 支持-获取 Microsoft Store 中的应用和游戏更新](https://support.microsoft.com/account-billing/get-updates-for-apps-and-games-in-microsoft-store-a1fe19c0-532d-ec47-7035-d1c5a1dd464f)
    * **Oculus：** 打开 Oculus 库，然后导航到左侧导航栏中的 "更新"。
    * **流：** [流支持-更新 & 安装问题](https://support.steampowered.com/kb_article.php?ref=2274-IFLV-5334)

## <a name="if-the-program-was-working-but-ceased-to-launch-after-update"></a>如果程序正在运行，但在更新后没有启动，请执行以下操作：

* 执行软件的 "干净重新安装"。 这需要你卸载或删除应用程序的现有版本。 完全从系统中删除后，通过流、Oculus 或 Microsoft Store 安装 Altspace。
* 如果你在启动 AltspaceVR 时遇到问题，请通过 [支持票证](https://help.altvr.com/hc/requests/new)告诉我们。 包含会话中的 [日志文件](uploading-client-logs.md) 。

## <a name="if-altspacevr-fails-to-launch-after-customizing-your-home-space"></a>如果在自定义 home space 后 AltspaceVR 无法启动：

* 导航到 [家庭共享空间的网站](https://account.altvr.com/users/sign_in)。
* 验证你的世界模板是否仍然存在。 如果已与你共享模板，则可能已被所有者删除，这将导致你的主空间无法加载。
    * 如果已删除模板，只需从左侧的 "世界工具" 面板中的 "编辑"，将现有模板替换为其他模板，将 "更新" 替换为保存更改。
* 从左侧的 "世界工具" 面板中选择 "对象"，删除可能加载失败的任何对象。 有问题的对象可能包括：
    * 来自已删除工具包或从包中删除的对象的对象仍然存在于你的世界中。
    * 实验性 GLTFs。
* 解决上述项后，请尝试重新输入 AltspaceVR。

有关网络管理员或 IT 部门的更高级支持，包括 Azure IP 范围和服务标记，请参阅我们的 [下载详细信息](https://www.microsoft.com/en-us/download/details.aspx?id=56519)。