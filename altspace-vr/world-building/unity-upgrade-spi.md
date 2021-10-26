---
title: Unity 2020.3、Single-Pass实例化以及你
description: 准备 SPI 升级
ms.date: 06/4/2021
ms.topic: article
keywords: kits， worlds， unity， 更新， 着色器， 上传程序， 故障排除
ms.openlocfilehash: bbc5cb38689551dd551bb681874577d968512ebf
ms.sourcegitcommit: 8c58f9f9ad1a3f9534141dee2c78e32792d0db7a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/25/2021
ms.locfileid: "130302372"
---
# <a name="unity-20203-single-pass-instancing-and-you"></a>Unity 2020.3、Single-Pass实例化以及你

## <a name="moving-to-unity-202039"></a>移动到 Unity 2020.3.9

从今天开始，AltspaceVR 已升级到最新版本的 Unity (2020.3.9) 。 除了一些性能改进之外，此更新还证明我们即将推出的功能能够纳入其中。 此更改应与所有现有内容兼容。 如果不是，请与支持人员联系：altvr.com/support

虽然这一到 2020.3.9 的迁移没有影响用户生成的内容，但几周后，我们将更改 AltspaceVR 的立体声渲染模式，要求用户更新[其内容。]( https://docs.unity3d.com/Manual/SinglePassStereoRendering.html) 这种升级到 [单一传递实例](https://docs.unity3d.com/Manual/SinglePassInstancing.html) 化后，将显著改善世界的性能。 请记住，此新内部版本将不再支持与 2019.4 及更旧版本的内容向后兼容。 必须尽快更新所有创建者拥有的内容，以避免中断性变更。 按照以下指南更新内容，并确保在 Unity 2020.3.9 上顺利转换为单一传递实例化。

> [!NOTE]
> 如果你定期使用其他人拥有的内容并且已与用户共享，请联系世界/工具包所有者，并确保他们计划更新其内容。

> 如果你是内容创建者，并且有疑问或需要帮助，请联系我们的支持团队寻求帮助：altvr.com/support

## <a name="testing-your-spi-content"></a>测试 SPI 内容

使用以下 AltspaceVR 预览版在 VR 中测试新更新的内容。 预览版仅用于测试目的，不应用于平台的常规使用。

* [适用于 Windows Mixed Reality 的 AltspaceVR SPI 预览版](https://aka.ms/AvrSpiMr)
* [适用于 SteamVR 的 AltspaceVR SPI 预览版](https://aka.ms/AvrSpiSteam)
* [适用于 Oculus Rift 的 AltspaceVR SPI 预览版](https://aka.ms/AvrSpiRift)

> 注意：仅提供 PC VR 预览版。 单通道实例呈现在 Android 上不可用，在 Mac 等非 VR 平台上也不需要。 因此，可以使用常规发布版本来测试这些设备。


## <a name="storecompatibilitycheck"></a>存储兼容性检查

升级到 Unity 2020.3.9 还将影响头戴显示设备和存储生成兼容性。 现在，需要从与头戴显示设备兼容的应用商店下载 AltspaceVR。 例如：对于 WinMR 或 Oculus 头戴显示设备，请分别从 Windows Store 或 Oculus Store 下载 AltspaceVR。 Windows Mixed Reality用户应从 Oculus Store Windows下载 AltspaceVR、Steam 中的 SteamVR 用户以及 Oculus Store 中的 Oculus Rift 用户。

## <a name="altspacevr-uploader-v090-upgrade-guide"></a>AltspaceVR Uploader v0.9.0 升级指南 

上传程序 0.9 的打包方式与以前版本的上传程序不同。 在此打包更改的同时，新的上传程序需要新版本的 Unity。 本指南旨在使此升级过程更顺畅、更安全，适用于所有参与方。

1. **备份项目** - 创建整个项目目录的副本，并放在安全位置。 此升级是破坏性升级，因此在完成升级后，无法为 Unity 2019.4 创建或上传捆绑包。 如果在此升级过程中遇到任何问题，则需要项目干净副本进行回退。 在 AltspaceVR 正式升级到 Unity 2020.3.9 之前，还需要更新任何实时工具包或模板。

2. **REMOVE OLD UPLOADER** - 关闭 Unity 后，删除以下文件/文件夹，它是相应的 .meta 文件：

    ```console
    * Assets/Altspace

    * Assets/Plugins

    * Assets/Prefabs/test-folder, Readme.txt

    * Assets/Resources/bg.jpeg, bg2.jpeg, logo.png, UserPreferences.asset

    * Assets/DFloor_v004.fbx

    * Library (This is a Unity system folder, not an Uploader folder. Delete it anyway, and let it be rebuilt during the upgrade.)
    ```

3. **下载引擎版本** - 打开 Unity 中心，安装 Unity 2020.3.9 [ (或单击此处](https://unity3d.com/ru/unity/whats-new/2020.3.9) 直接安装) 。

4. **升级项目** - 在 Unity 2020.3.9 中打开已清理的项目，并允许 Unity 升级项目。

5.  (PC) 下载 **混合** 现实功能工具 - 按照说明下载混合现实功能工具，该工具 [](/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool)用于管理上传程序包的安装。

6. **安装上传程序** - 使用 MR 功能工具选择 Unity 项目，并添加 AltspaceVR 上传程序功能 (AltspaceVR 标题下) 。 按照工具中的说明操作。

在 macOS 上，从注册表手动下载最新版本[](https://dev.azure.com/aipmr/MixedReality-Unity-Packages/_packaging?_a=package&feed=Unity-packages&package=com.microsoft.altspacevr_uploader&protocolType=Npm&version=0.9.0&view=versions)，然后从 Unity 编辑器的包管理器 (Windows > 程序包管理器 > + > 从 tarball) 添加包。

包完成导入后，"AltspaceVR"菜单项中应会提供熟悉的"上传程序"窗口。

## <a name="troubleshooting-tips"></a>疑难解答指南

1. 如果在 WinMR 头戴显示设备上遇到控制器或输入问题，请确保它位于头部，以正确连接状态传感器。 这是一个已知问题，Microsoft 正在积极解决此问题。

2. 检查头戴显示设备和存储生成兼容性。 例如，如果使用 WinMR 头戴显示设备，请确保 AltspaceVR 生成是通过 Windows Store 获取的。

3. 如果在测试期间发现内容在 VR 模式下只出现在一只眼睛中，则使用的自定义着色器很可能不支持 SPI 呈现。 需要选择其他着色器，或按照 Unity 的 [SPI](https://docs.unity3d.com/Manual/SinglePassInstancing.html) 升级指南手动编辑着色器并添加支持。

4. 对于 WinMR 上的用户，请记住，在 AltspaceVR 中访问 VR 模式之前，必须： 
    1. 从客户端下载并安装 OpenXR Windows Mixed Reality安装Microsoft Store。
        1. 打开 混合现实门户 应用
        2. 在应用的左下角选择"查看更多"
        3. 在出现的菜单中，选择"设置 OpenXR"。 这样做将导致 Windows Store 从安装运行时的位置启动。 如果未显示此菜单项，则电脑上可能已安装 OpenXR。