---
title: 无法启动 AltspaceVR
description: 了解如何识别、报告并修复与启动 AltspaceVR 环境相关的任何问题。
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
# <a name="i-cant-launch-altspacevr"></a>无法启动 AltspaceVR

AltspaceVR 可能无法启动的原因有多种。 尝试执行以下步骤，确保应用程序已使用必要的第三方软件正确安装。

## <a name="if-youre-trying-to-launch-altspacevr-for-the-first-time"></a>如果尝试首次启动 AltspaceVR：

1. 验证设备是否受支持并满足 [最低指定要求](../getting-started/system-requirements.md)。
2. 确保已安装最新的[Oculus 软件](https://www.oculus.com/setup)，并且"常规设置>">"设置为"打开"。 如果在 2D 模式下启动，则无需安装 Oculus。
3. 请确保具有正常工作的 Internet 连接。 如果尝试从网络防火墙内启动 Altspace，请打开 UDP 端口 5055 和 5056 以及 TCP 端口 80 和 443。 如果位于企业或教育防火墙的网络中，可能需要联系网络管理员或 IT 部门。
4. 另请参阅：
    * [安装 AltspaceVR for Oculus Quest](../getting-started/oculus-installation.md)
    * [安装 AltspaceVR for Windows Mixed Reality](../getting-started/wmr-installation.md)

## <a name="if-altspacevr-reports-that-the-current-version-is-out-of-date"></a>如果 AltspaceVR 报告当前版本已过期：

* 不再支持你使用的应用程序版本。 如果通过店面下载了 AltspaceVR，则更新可能最近在商店能够更新客户端之前启动。
* 若要强制更新，可以通过各种店面执行更新：
    * **Microsoft Store：Microsoft Store**[支持 - 获取应用中应用和游戏的更新Microsoft Store](https://support.microsoft.com/account-billing/get-updates-for-apps-and-games-in-microsoft-store-a1fe19c0-532d-ec47-7035-d1c5a1dd464f)
    * **Oculus：** 打开 Oculus 库，导航到左侧导航栏中的"更新"。
    * **流：**[流支持 - &安装问题](https://support.steampowered.com/kb_article.php?ref=2274-IFLV-5334)

## <a name="if-the-program-was-working-but-ceased-to-launch-after-update"></a>如果程序正常工作，但需要更新后启动：

* 对软件执行"干净重新安装"。 这要求卸载或删除应用程序的现有版本。 从系统完全删除后，通过 Steam、Oculus 或 Microsoft Store。
* 如果在启动 AltspaceVR 时出现问题，请通过支持票证 [告知我们](https://help.altvr.com/hc/requests/new)。 包括 [会话中](uploading-client-logs.md) 的日志文件。

## <a name="if-altspacevr-fails-to-launch-after-customizing-your-home-space"></a>如果在自定义主空间后 AltspaceVR 无法启动：

* 导航到 [主页空间的网站](https://account.altvr.com/users/sign_in)。
* 验证你的世界模板是否仍然存在。 如果模板已与用户共享，则所有者可能已删除该模板，这可能会导致主空间无法加载。
    * 如果模板已删除，只需从左侧"世界工具"面板中"编辑"世界，将现有模板替换为另一个模板，然后使用"更新"保存更改。
* 从左侧"世界工具"面板中选择"对象"，删除可能无法加载的任何对象。 有问题的对象可能包括：
    * 来自已删除的工具包的对象，或从工具包中删除的对象，这些对象仍存在于你的世界。
    * 实验性 GLTF。
* 解决上述项后，尝试重新进入 AltspaceVR。

有关网络管理员或 IT 部门（包括 Azure IP 范围和服务标记）的更高级支持，请参阅下载 [详细信息](https://www.microsoft.com/en-us/download/details.aspx?id=56519)。