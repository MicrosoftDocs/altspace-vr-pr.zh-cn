---
title: 将内容更新到最新 Unity 版本
description: 了解如何将内容更新到最新版本的 Unity。
ms.date: 06/4/2021
ms.topic: article
keywords: 工具包，世界，unity，更新，着色器，上载器，故障排除
ms.openlocfilehash: a10e64b4dc19e256dcae9d61620de0140db60ccc0bf2a10dc864313f139bbd10
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "119126755"
---
# <a name="updating-content-to-the-latest-unity-version"></a>将内容更新到最新 Unity 版本

## <a name="moving-to-unity-202039"></a>移动到 Unity 2020.3。9

到目前为止，AltspaceVR 已升级到 Unity (2020.3.9) 的最新版本。 除了一些性能改进外，此更新还会将我们的后续功能更新为我们非常乐意引入的功能。 此更改应该与所有现有内容兼容。 如果不是这样，请随意联系支持人员： altvr.com/support

尽管这会转向2020.3.9 不会影响用户生成的内容，但在几周内，我们将更改 AltspaceVR 的 [立体声渲染模式，这将要求用户更新其内容]( https://docs.unity3d.com/Manual/SinglePassStereoRendering.html)。 此升级到 [单个 Pass 实例](https://docs.unity3d.com/Manual/SinglePassInstancing.html) 化将允许在你的世界中获得显著的性能改进。 请记住，这一新版本将不再支持2019.4 及更低版本中的内容的向后兼容性。 很有可能会尽快更新所有创建者拥有的内容，以避免重大更改。 请按照下面的指南进行操作，以更新你的内容，并确保顺利过渡到 Unity 2020.3.9 上的单个 Pass 实例。

> [!NOTE]
> 如果你经常使用其他人拥有的内容，并且已与你共享，请联系世界/套件所有者，并确保他们计划更新其内容。

> 如果你是内容创建者，但你有疑问或需要帮助，请与我们的支持团队联系以获取帮助： altvr.com/support

## <a name="testing-your-spi-content"></a>测试 SPI 内容

使用以下预览版本的 AltspaceVR 来测试 VR 中新更新的内容。 预览版仅用于测试目的，不应将其用于平台一般用途。

* [Windows Mixed Reality 的 AltspaceVR SPI 预览版](https://aka.ms/AvrSpiMr)
* [SteamVR 的 AltspaceVR SPI 预览版](https://aka.ms/AvrSpiSteam)
* [适用于 Oculus Rift 的 AltspaceVR SPI 预览版](https://aka.ms/AvrSpiRift)

> 注意：仅提供了 PC VR 预览。 单个传递实例呈现在 Android 上不可用，并且在 Mac 等非 VR 平台上不需要。 因此，你可以使用通用版本来测试这些设备。


## <a name="storecompatibilitycheck"></a>存储兼容性检查

升级到 Unity 2020.3.9 还会影响耳机和存储生成兼容性。 现在需要从与耳机兼容的商店下载 AltspaceVR。 例如：对于 WinMR 或 Oculus 耳机，请分别从 Windows 存储或 Oculus 存储下载 AltspaceVR。 Windows Mixed Reality 用户应该从 Windows 存储下载 AltspaceVR，从流中 SteamVR 用户，并从 Oculus 应用商店下载 Oculus Rift 用户。

## <a name="altspacevr-uploader-v090-upgrade-guide"></a>AltspaceVR 上传0.9.0 升级指南 

上载0.9 的打包方式不同于以前版本的上载者。 随着此打包的更改，新的上载者需要新版本的 Unity。 本指南旨在使此升级过程更顺利、更安全。

1. **备份项目** -创建整个项目目录的副本，并将其放在一个安全的位置。 此升级是一种破坏性升级，因此在完成后，你将无法为 Unity 2019.4 创建或上传捆绑包。 如果在此升级过程中遇到任何问题，则需要一个干净的项目副本才能回退。 在 AltspaceVR 正式升级到 Unity 2020.3.9 之前，还需要它更新任何实时工具包或模板。

2. **删除旧的上载** 程序-已关闭 Unity，删除以下文件/文件夹，这是对应的元文件：

    ```console
    * Assets/Altspace

    * Assets/Plugins

    * Assets/Prefabs/test-folder, Readme.txt

    * Assets/Resources/bg.jpeg, bg2.jpeg, logo.png, UserPreferences.asset

    * Assets/DFloor_v004.fbx

    * Library (This is a Unity system folder, not an Uploader folder. Delete it anyway, and let it be rebuilt during the upgrade.)
    ```

3. **下载引擎版本** -打开 unity 中心，安装 unity 2020.3.9 (或 [单击此处](https://unity3d.com/ru/unity/whats-new/2020.3.9) 直接安装) 。

4. **升级项目** -在 Unity 2020.3.9 中打开已清理的项目，并允许 Unity 升级项目。

5.  (PC 仅) **下载混合现实功能工具** -按照说明下载将用于管理上载程序包安装的 [Mixed reality 功能工具](/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool)。

6. **安装上载** 程序-使用 MR 功能工具选择 Unity 项目，并将 AltspaceVR 上载程序功能 (添加到 AltspaceVR 标题) 。 按照工具中的说明进行操作。

在 macOS 上，手动从[注册表](https://dev.azure.com/aipmr/MixedReality-Unity-Packages/_packaging?_a=package&feed=Unity-packages&package=com.microsoft.altspacevr_uploader&protocolType=Npm&version=0.9.0&view=versions)下载最新版本，并从 Unity 编辑器的包管理器中安装它 (Windows > 程序包管理器 > + > 从 tarball) 添加包。

包导入完成后，将在 "AltspaceVR" 菜单项中提供熟悉的上载窗口。

## <a name="troubleshooting-tips"></a>疑难解答指南

1. 如果你的 WinMR 耳机上出现控制器或输入问题，请确保将其定位在你的打印头上，以正确地与状态传感器交流。 这是一个已知问题，Microsoft 正在努力解决该问题。

2. 检查头戴显示设备和存储版本的兼容性。 例如，如果你使用的是 WinMR 耳机，请确保 AltspaceVR 生成是通过 Windows 存储获取的。

3. 如果在测试过程中发现内容仅在 "VR" 模式下出现，则可能使用的自定义着色器不支持 SPI 渲染。 需要选择其他着色器，或遵循 [Unity 的 SPI 升级指南](https://docs.unity3d.com/Manual/SinglePassInstancing.html) ，手动编辑着色器并添加支持。

4. 对于 WinMR 上的用户，请记住，在 AltspaceVR 中访问 VR 模式之前，必须执行以下操作： 
    1. 从 Microsoft Store 下载并安装用于 Windows Mixed Reality 的 OpenXR。
        1. 打开混合现实门户应用
        2. 在应用左下角选择 "查看更多"
        3. 在出现的菜单中，选择 "设置 OpenXR"。 这样做将导致 Windows 存储启动，从中可以安装运行时。 如果此菜单项未出现，则可能已在您的 PC 上安装 OpenXR。