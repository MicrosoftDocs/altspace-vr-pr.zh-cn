---
title: 使用 Web 投影仪流式传输浏览器
description: 了解如何使用 Web 投影仪将指定浏览器的内容流式传输到 AltspaceVR 体验中。
ms.date: 03/11/2021
ms.topic: article
keywords: Web 投影仪、流、浏览器
ms.openlocfilehash: 8f25de68ba633e10b9192b85c883de4ba48fd7987ec5d301ebac8443982a1a55
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127295"
---
# <a name="using-the-web-projector-to-stream-a-browser"></a>使用 Web 投影仪流式传输浏览器

AltspaceVR Web 投影仪是一种可靠的媒体共享解决方案，可用于将指定的浏览器选项卡从桌面电脑直接流式传输到 AltspaceVR。 它可用于共享幻灯片、视频、照片，以及可从浏览器打开的几乎任何其他内容。* Web 投影仪需要下载浏览器扩展，当前仅通过世界编辑器提供。 下面是该功能及其使用方法的完整概述：

## <a name="requirements"></a>要求

1. 必须使用电脑或 Mac 流式传输浏览器。
2. Edge 浏览器当前支持必要的浏览器扩展。  (我们正在努力展开此列表。) 
3. 虽然可从 Mac 计算机进行流式传输，但 Web 投影仪在 AltspaceVR Mac 客户端中尚不可用。
4. 如果已正确设置所有内容 (使用相同的帐户登录到浏览器扩展/AltspaceVR，使用 AltspaceVR) 中的 Web 投影仪进行连接/广播，并且仍看到绿色屏幕，则 WebProjector 需要打开 TCP 端口 443，UDP 端口范围为 20000-20400。

> [!NOTE]
> 此功能主要用于流式传输你选择的浏览器选项卡。 如果尝试改为流式传输桌面应用程序，Web 投影仪将流式传输所有计算机音频 (包括 AltspaceVR) 可能会导致回显/反馈。 需要将 AltspaceVR 静音，以防止发生这种情况。 或者，在从电脑流式传输时，也可使用单独的设备运行 AltspaceVR。

## <a name="getting-started"></a>入门

1. 首先，需要下载并安装浏览器扩展，可在此处 [找到该扩展](https://account.altvr.com/web_projector)。
2. 接下来， [在 Edge 浏览器 旁加载扩展](https://docs.microsoft.com/microsoft-edge/extensions-chromium/getting-started/extension-sideloading)。
    * 下载完成后，转到 **浏览器的"扩展** "部分。  (**找到设置)**
    * 解压缩.zip文件。
    * 打开开发人员 **模式并选择** " **加载已解压缩"**
    * 选择刚解压缩的文件夹。 这是 Web 投影仪扩展。
    * 添加扩展后，可以 **转到"详细信息** "来设置设置。

## <a name="setting-up-a-shareable-browser"></a>设置可共享浏览器

下载并安装扩展后，即可使用它了！

1. 在 Edge 浏览器中打开一个选项卡，并导航到要共享媒体。
2. 设置窗口，以便可以共享。  (注意：整个浏览器窗口将按全球) 
3. 找到新安装的扩展 (浏览器浏览器中 URL 栏附近显示为 AltspaceVR) 。 选择 AltspaceVR。 系统会提示你登录帐户。  (*注意：登录到用于设置 Web 投影仪的同一帐户) 
4. 登录后，应会看到扩展屏幕提供"开始 **流式处理"** 选项。 选择该文件夹。

## <a name="projecting-your-browser-in-world"></a>将浏览器预测到世界

1. 为浏览器设置投影并开始通过扩展流式传输后，打开 AltspaceVR。
2. 通过打开"Web 投影仪"中的"世界编辑器"，在>设置> Web 投影仪
3. 放置后，可以使用"世界编辑器"控件调整 Web 投影仪的大小。  (还包括 screen.) 上的说明
4. 选择 **"连接"** 按钮开始流式处理 Edge 浏览器。
5. 请记得单击 **"** 广播"，开始与空间内的所有来宾共享。
6. 不要忘记停止 **流式处理。** 会话最终会退出，但在此之前，它将继续实时对浏览器进行项目设计。 完成操作后，最好尽快结束会话。

![AltspaceVR world 中预计的浏览器](images/web-project-img-01.png)

**视频流式处理提示：** 如果视频放大器，请停止流式传输，将视频质量调整为 480p 或 360p，然后重启流和广播。 更高的分辨率可能会增加 CPU 和上传带宽。

> [!NOTE]
> 目前，Web 投影仪顶部的其他控制按钮尚未上架。 它们将保持灰色且不可单击。 这不是一个 bug，目前 (设计) 。

> [!IMPORTANT]
> 免责声明：注意：与 AltspaceVR 中的所有其他功能一样，Web 投影仪的使用受服务条款[](../community/terms-of-service.md)和标准Community[限制](../community/community-standards.md)。 因此，Web 投影仪不得用于流式传输违反任一协议的内容。 这样做将导致 AltspaceVR 采取审核操作。 不保证访问 Web 投影仪 Open Beta 版，只能授予临时试用版。 beta 版本的长度和参与时长由 AltspaceVR 团队决定。 不需要使用 Web 投影仪的 beta 版本，并且参与 beta 版完全自愿性。 建议参与者提供有关 Web 投影仪的反馈，以帮助在开发继续时塑造功能的功能和可用性。 Web 投影仪的 beta 版本的功能可能有限，并且可能会受到意外 bug 影响。 请提前感谢你的参与。
