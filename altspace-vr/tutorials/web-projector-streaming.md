---
title: 使用 Web 投影仪流式传输浏览器
description: 了解如何使用 web 投影仪从指定的浏览器将内容流式传输到 AltspaceVR 体验。
ms.date: 03/11/2021
ms.topic: article
keywords: web 投影仪，流，浏览器
ms.openlocfilehash: 2c5cb6ef917b7e799b8da3f1a769d77258866992
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2021
ms.locfileid: "112922994"
---
# <a name="using-the-web-projector-to-stream-a-browser"></a>使用 Web 投影仪流式传输浏览器

AltspaceVR Web 投影仪是一种强大的媒体共享解决方案，可让你将指定的浏览器选项卡从桌上型电脑直接流式传输到 AltspaceVR。 它可用于共享幻灯片、视频和照片，几乎可用于共享浏览器中打开的任何其他内容。 * Web 投影仪需要下载浏览器扩展，当前可通过世界编辑器独占使用。 下面是该功能以及如何使用它的完整概述：

## <a name="requirements"></a>要求

1. 必须使用 PC 或 Mac 流式传输浏览器。
2. Microsoft Edge 浏览器当前支持所需的浏览器扩展。  (我们正在努力展开此列表。 ) 
3. 虽然你可以从 Mac 计算机进行流式处理，但 Web 投影仪还没有在 AltspaceVR Mac 客户端中提供。
4. 如果已将所有设置正确 (使用同一帐户登录到浏览器扩展/AltspaceVR，并在 AltspaceVR 中使用 Web 投影仪进行连接/广播) 并且仍显示为绿色屏幕，WebProjector 需打开 TCP 端口443，UDP 端口范围20000-20400。

> [!NOTE]
> 此功能主要用于流式传输所选的浏览器选项卡。 如果尝试改为流式传输桌面应用程序，Web 投影仪会流式传输所有计算机音频 (包括 AltspaceVR) ，这可能会导致回显/反馈。 你需要静音 AltspaceVR 以防止此情况发生。 或者，还可以使用单独的设备在从电脑进行流式处理时运行 AltspaceVR。

## <a name="getting-started"></a>入门

1. 若要开始，需要下载并安装浏览器扩展，可在 [此处](https://account.altvr.com/web_projector)找到。
2. 接下来， [在 Edge 浏览器中旁加载扩展](https://docs.microsoft.com/microsoft-edge/extensions-chromium/getting-started/extension-sideloading)。
    * 下载完成后，请进入浏览器的 " **扩展** " 部分。 " **设置** " 下 (找到) 
    * 解压缩 .zip 文件。
    * 开启 **开发人员模式** 并选择 "**加载解包**"
    * 选择刚刚解压缩的文件夹。 这是 Web 投影仪扩展。
    * 添加扩展后，可以在 " **详细信息** " 中设置设置。

## <a name="setting-up-a-shareable-browser"></a>设置可共享的浏览器

下载并安装了你的扩展后，你就可以使用它了！

1. 在 Edge 浏览器中打开一个选项卡，然后导航到想要共享的媒体。
2. 设置窗口以便共享。  (注意：整个浏览器窗口将在世界上投影) 
3. 找到新安装的扩展 (，它在浏览器) 中显示为 URL 栏附近的 AltspaceVR 图标。 选择 AltspaceVR。 系统将提示你登录到帐户。  ( * 注意：请务必登录到用于设置 Web 投影仪的同一帐户。 ) 
4. 登录后，应会看到 "扩展" 屏幕提供了 " **开始流式传输** " 选项。 请选择它。

## <a name="projecting-your-browser-in-world"></a>在世界上投影浏览器

1. 将浏览器设置为用于投影，并通过扩展开始流式传输后，打开 AltspaceVR。
2. 在选择的环境中设置 Web 投影仪，方法是打开您的世界编辑器 > 基础知识 > Web 投影仪
3. 放置后，可以使用您的世界编辑器控件调整 Web 投影仪的大小。  (它还将在屏幕上包含说明。 ) 
4. 选择 " **连接** " 按钮开始流式传输你的 Edge 浏览器。
5. 请记得单击 " **广播** " 开始与所有来宾共享空间。
6. 不要忘记 **停止流式处理。** 你的会话最终会超时，但在此之前，它将继续实时投影你的浏览器。 完成后，最好立即结束会话。

![AltspaceVR world 中的浏览器预测](images/web-project-img-01.png)

**视频流提示：** 如果视频 stutters，停止流式传输，将视频质量调整到480p 或360p，然后重新启动流和广播。 较高的分辨率可能会占用 CPU 和上传带宽。

> [!NOTE]
> 此时，Web 投影仪顶部的其他控件按钮还不会处于活动状态。 它们将保持灰色和 unclickable。 这并不是一个 bug，它是目前) 的设计 (。

> [!IMPORTANT]
> 免责声明：注意： Web 投影仪的使用情况（如 AltspaceVR 中的所有其他功能）受我们 [的服务条款](../community/terms-of-service.md) 和我们的 [社区标准](../community/community-standards.md)的约束。 因此，不能使用 Web 投影仪来流式传输违反任一协议的内容。 这样做会导致 AltspaceVR 执行审核操作。 不保证能够访问 Web 投影仪的开放 Beta 版，只能将其授予临时试用版。 Beta 的长度和您的参与时间的长度由 AltspaceVR 团队决定。 不需要使用 Web 投影仪的试用版，并且参与 beta 的工作完全是自愿的。 鼓励开发人员提供有关 Web 投影仪的反馈，以帮助在开发过程中形成功能的功能和可用性。 Web 投影仪的测试版本可能具有有限的功能，可能会导致意外的错误。 请提前感谢你的参与。
