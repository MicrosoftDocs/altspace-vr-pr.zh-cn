---
title: 有关 AltspaceVR 应用的常见问题
description: AltspaceVR 应用的故障排除和支持。
ms.date: 8/16/2021
author: qianw211
ms.author: v-qianwen
ms.topic: article
keywords: vr，AltspaceVR，故障排除，支持
ms.openlocfilehash: a0df1e100ef8511fe3c9129548529577964c2336
ms.sourcegitcommit: 5c452a9092297c0bfbc8efabebf395e7ee31853f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2021
ms.locfileid: "129311840"
---
# <a name="frequently-asked-questions-about-the-altspacevr-app"></a>有关 AltspaceVR 应用的常见问题

## <a name="finding-the-altspacevr-app-version"></a>查找 AltspaceVR 应用版本

在对问题进行故障排除的过程中，可能会询问你当前正在运行的 AltspaceVR 应用程序的版本。

### <a name="in-altspacevr"></a>在 AltspaceVR 中

若要在 AltspaceVR 中查找应用版本，请导航到 " **设置" 菜单** ，然后在左侧导航栏中选择 " **关于** "。 此处报告了 "应用版本"，如下面的屏幕截图中所示。

![打开设置菜单，并打开 "关于面板"](images/app-version-img-01.png)

### <a name="in-windows-system-settings"></a>在 Windows 系统设置

如果通过 Microsoft Store 安装了 AltspaceVR，则还可以在 Windows 系统设置中另外查找应用版本。  如果无法成功登录到客户端，则此方案适用于报告应用程序版本。

若要在 Windows 系统设置 "中查找应用版本，请打开"**开始 "菜单**，键入 **Apps & 功能**"，然后选择结果。 在应用列表中导航到 **AltspaceVR** 。 左键单击 "AltspaceVR"，然后从出现的菜单中选择 " **高级选项** "。

![突出显示了 "高级" 选项的 "应用和功能" 菜单](images/app-version-img-02.png)

在 "**规范**" 标头下的 "**高级选项**" 中，**应用版本** 应列在 "**版本**" 标签的右侧。

![已突出显示应用版本的高级选项打开](images/app-version-img-03.png)

### <a name="app-version-in-client-logs"></a>客户端日志中的应用版本

在应用程序启动过程中，AltspaceVR 将客户端日志文件中的应用版本报告为 "Altspace 版本"。 如果无法成功登录到客户端，则这是获取应用程序版本的一个不错的选择，但它确实会在失败之前尝试启动。

### <a name="windows"></a>Windows

在 Windows 上，可以通过 Windows 资源管理器在以下位置找到客户端日志文件：

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
```

每次启动 AltspaceVR 时，都会覆盖此文件。 "唱机" 代表最新的会话，"Player-prev" 表示上一个会话。

### <a name="via-powershell"></a>通过 PowerShell

高级用户可以通过 PowerShell 搜索此字符串的客户端日志，如下所示：

输入：

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

输出：

[2.047] AltspaceVR 版本： 3.2.23. e66c2

## <a name="how-do-i-upload-my-client-logs"></a>如何实现上传我的客户端日志？

当你使用 AltspaceVR 时，AltspaceVR 客户端应用程序会保留诊断数据和事件的日志。 在对问题进行故障排除的过程中，可能会要求你 "上载日志"，以便我们的团队可以查看它们。 这是 AltspaceVR 的一项功能，它允许你将我们的团队发送到你的本地日志内容，以帮助我们解决你的问题。

### <a name="in-altspacevr"></a>在 AltspaceVR 中

若要在 AltspaceVR 中上载客户端日志，请导航到 " **设置" 菜单** ，然后在左侧导航栏中选择 " **支持** "。 此处提供了几个用于上载日志的选项，如以下屏幕截图中所示。

![打开 "支持面板" 设置菜单并突出显示 "日志" 字段](images/help-altvr-uploadlogs.png)

### <a name="fields"></a>字段

**"出现了什么问题？"**
描述发生的情况-例如，如果发现一个 bug，请描述你预期会发生什么情况，这与) 实际发生的情况相反。 当你按 "上传" 时，此信息将与日志一起发送。

**"Upload 日志"** 此按钮将从当前会话上传日志。 如果在同一会话中发现问题，请使用此选项 (例如，如果你尚未关闭 AltspaceVR 客户端) 并且要报告它。

**"Upload 上个日志"** 此按钮将从上一个会话上传日志。

**"Upload 上一次崩溃日志"** 此按钮将从遇到的最新崩溃上传更多的日志内容。

### <a name="in-client-logs"></a>在客户端日志中

您还可以从您的计算机中检索日志文件。 有关如何检索这些日志的说明，请参阅 [此处](#app-version-in-client-logs)。


找到这些文件后，请在单击 "提交" 之前， [打开支持票证](https://help.altvr.com/hc/en-us/requests/new) 并在票证请求上上传日志。

## <a name="what-do-i-do-if-i-cant-launch-altspacevr"></a>如果无法启动 AltspaceVR，该怎么办？

AltspaceVR 可能无法启动的原因有多种。 尝试执行以下步骤，以确保应用程序正确安装了必要的第三方软件。

### <a name="if-youre-trying-to-launch-altspacevr-for-the-first-time"></a>如果是第一次尝试启动 AltspaceVR：

1. 验证你的设备是否受支持并满足 [指定的最低要求](../getting-started/system-requirements.md)。
2. 请确保已安装最新的[Oculus 软件](https://www.oculus.com/setup)，并且设置 > 常规 > 未知设备设置为 ON。 如果在2D 模式下启动，则无需安装 Oculus。
3. 请确保你具有有效的 internet 连接。 如果尝试从网络防火墙内启动 Altspace，请打开 UDP 端口5055和5056，以及 TCP 端口80和443。 如果你在公司或教育防火墙的网络内，你可能需要联系网络管理员或 IT 部门。
4. 另请参阅：
    * [为 Oculus 寻找安装 AltspaceVR](../getting-started/oculus-installation.md)
    * [为 Windows Mixed Reality 安装 AltspaceVR](../getting-started/wmr-installation.md)

### <a name="if-altspacevr-reports-that-the-current-version-is-out-of-date"></a>如果 AltspaceVR 报告当前版本已过期：

* 你使用的应用程序版本不再受支持。 如果已通过店面下载 AltspaceVR，则可能会在你的应用商店更新你的客户端之前最近启动了更新。
* 如果要强制更新，可以通过各种商店实现此目的：
    * **Microsoft Store：** [Microsoft Store 支持-获取 Microsoft Store 中的应用和游戏更新](https://support.microsoft.com/account-billing/get-updates-for-apps-and-games-in-microsoft-store-a1fe19c0-532d-ec47-7035-d1c5a1dd464f)
    * **Oculus：** 打开 Oculus 库，然后导航到左侧导航栏中的 "更新"。
    * **流：** [流支持-更新 & 安装问题](https://support.steampowered.com/kb_article.php?ref=2274-IFLV-5334)

### <a name="if-the-program-was-working-but-ceased-to-launch-after-update"></a>如果程序正在运行，但在更新后没有启动，请执行以下操作：

* 执行软件的 "干净重新安装"。 这需要你卸载或删除应用程序的现有版本。 完全从系统中删除后，通过流、Oculus 或 Microsoft Store 安装 Altspace。
* 如果你在启动 AltspaceVR 时遇到问题，请通过 [支持票证](https://help.altvr.com/hc/requests/new)告诉我们。 包含会话中的 [日志文件](altspacevr-app-faq.md#how-do-i-upload-my-client-logs) 。

### <a name="if-altspacevr-fails-to-launch-after-customizing-your-home-space"></a>如果在自定义 home space 后 AltspaceVR 无法启动：

* 导航到 [家庭共享空间的网站](https://account.altvr.com/users/sign_in)。
* 验证你的世界模板是否仍然存在。 如果已与你共享模板，则可能已被所有者删除，这将导致你的主空间无法加载。
    * 如果已删除模板，只需从左侧的 "世界工具" 面板中的 "编辑"，将现有模板替换为其他模板，将 "更新" 替换为保存更改。
* 从左侧的 "世界工具" 面板中选择 "对象"，删除可能加载失败的任何对象。 有问题的对象可能包括：
    * 来自已删除工具包或从包中删除的对象的对象仍然存在于你的世界中。
    * 实验性 GLTFs。
* 解决上述项后，请尝试重新输入 AltspaceVR。

有关网络管理员或 IT 部门的更高级支持，包括 Azure IP 范围和服务标记，请参阅我们的 [下载详细信息](https://www.microsoft.com/en-us/download/details.aspx?id=56519)。

## <a name="support"></a>支持

AltspaceVR 团队的问题或反馈？ 

> [!div class="nextstepaction"]
> [单击此处发送支持请求](https://help.altvr.com/hc/requests/new)