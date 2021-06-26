---
title: 将内容更新到最新 Unity 版本
description: 了解如何将内容更新到最新版本的 Unity。
ms.date: 06/4/2021
ms.topic: article
keywords: kits， worlds， unity， 更新， 着色器， 上传程序， 故障排除
ms.openlocfilehash: f8a805c4b3350f2c97c43d3d48c35733ec7e9710
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/25/2021
ms.locfileid: "112961198"
---
# <a name="updating-content-to-the-latest-unity-version"></a><span data-ttu-id="ca7d8-104">将内容更新到最新 Unity 版本</span><span class="sxs-lookup"><span data-stu-id="ca7d8-104">Updating Content to the Latest Unity Version</span></span>

## <a name="moving-to-unity-202039"></a><span data-ttu-id="ca7d8-105">移动到 Unity 2020.3.9</span><span class="sxs-lookup"><span data-stu-id="ca7d8-105">Moving to Unity 2020.3.9</span></span>

<span data-ttu-id="ca7d8-106">从今天开始，AltspaceVR 已升级到最新版本的 Unity (2020.3.9) 。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-106">Starting today, AltspaceVR has upgraded to a recent version of Unity (2020.3.9).</span></span> <span data-ttu-id="ca7d8-107">除了一些性能改进之外，此更新还证明我们即将推出的功能，我们可以将其纳入其中。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-107">In addition to some performance improvements, this update future-proofs us for forthcoming features that we're excited to incorporate.</span></span> <span data-ttu-id="ca7d8-108">此更改应与所有现有内容兼容。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-108">This change should be compatible with all existing content.</span></span> <span data-ttu-id="ca7d8-109">如果不是，请随意联系支持人员：altvr.com/support</span><span class="sxs-lookup"><span data-stu-id="ca7d8-109">If it isn't, feel free to contact support: altvr.com/support</span></span>

<span data-ttu-id="ca7d8-110">虽然这一到 2020.3.9 的迁移没有影响用户生成的内容，但几周后，我们将更改 AltspaceVR 的立体声渲染模式，要求用户更新[其内容。]( https://docs.unity3d.com/Manual/SinglePassStereoRendering.html)</span><span class="sxs-lookup"><span data-stu-id="ca7d8-110">Though this move to 2020.3.9 hasn't affected user-generated content, in a few weeks we're making a change to AltspaceVR's [stereo rendering mode that will require users to update their content]( https://docs.unity3d.com/Manual/SinglePassStereoRendering.html).</span></span> <span data-ttu-id="ca7d8-111">这种升级到 [单一](https://docs.unity3d.com/Manual/SinglePassInstancing.html) 传递实例化将显著改善世界的性能。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-111">This upgrade to [Single Pass Instancing](https://docs.unity3d.com/Manual/SinglePassInstancing.html) will allow for significant performance improvements in your worlds.</span></span> <span data-ttu-id="ca7d8-112">请记住，此新内部版本将不再支持与 2019.4 及更旧版本的内容向后兼容。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-112">Keep in mind that this new build will no longer support backwards-compatibility with content from 2019.4 and older.</span></span> <span data-ttu-id="ca7d8-113">必须尽快更新所有创建者拥有的内容，以避免中断性变更。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-113">It's urgent that all creator-owned content is updated as soon as possible to avoid breaking changes.</span></span> <span data-ttu-id="ca7d8-114">按照以下指南更新内容，并确保在 Unity 2020.3.9 上顺利转换为单一传递实例化。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-114">Follow the guide below to update your content and ensure a smooth transition to Single Pass Instancing on Unity 2020.3.9.</span></span>

> [!NOTE]
> <span data-ttu-id="ca7d8-115">如果你经常使用其他人拥有的内容并且已与用户共享，请联系世界/工具包所有者，并确保他们计划更新其内容。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-115">If you are regularly using content that is owned by someone else and has been shared with you, contact the world/kit owner and make sure they are planning to update their content.</span></span>

> <span data-ttu-id="ca7d8-116">如果你是内容创建者，并且有疑问或需要帮助，请联系我们的支持团队寻求帮助：altvr.com/support</span><span class="sxs-lookup"><span data-stu-id="ca7d8-116">If you are a content creator and you have questions or require assistance, please contact our support team for help: altvr.com/support</span></span>

## <a name="testing-your-spi-content"></a><span data-ttu-id="ca7d8-117">测试 SPI 内容</span><span class="sxs-lookup"><span data-stu-id="ca7d8-117">Testing your SPI content</span></span>

<span data-ttu-id="ca7d8-118">使用以下 AltspaceVR 预览版在 VR 中测试新更新的内容。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-118">Use the following preview versions of AltspaceVR to test your newly updated content in VR.</span></span> <span data-ttu-id="ca7d8-119">预览版仅用于测试目的，不应用于平台的常规使用。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-119">The preview versions are for testing purposes only, and shouldn't be used for a general use of the platform.</span></span>

* [<span data-ttu-id="ca7d8-120">适用于 Windows Mixed Reality 的 AltspaceVR SPI 预览版</span><span class="sxs-lookup"><span data-stu-id="ca7d8-120">AltspaceVR SPI Preview for Windows Mixed Reality</span></span>](https://aka.ms/AvrSpiMr)
* [<span data-ttu-id="ca7d8-121">适用于 SteamVR 的 AltspaceVR SPI 预览版</span><span class="sxs-lookup"><span data-stu-id="ca7d8-121">AltspaceVR SPI Preview for SteamVR</span></span>](https://aka.ms/AvrSpiSteam)
* [<span data-ttu-id="ca7d8-122">适用于 Oculus Rift 的 AltspaceVR SPI 预览版</span><span class="sxs-lookup"><span data-stu-id="ca7d8-122">AltspaceVR SPI Preview for Oculus Rift</span></span>](https://aka.ms/AvrSpiRift)

> <span data-ttu-id="ca7d8-123">注意：仅提供 PC VR 预览版。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-123">Note: Only PC VR previews have been provided.</span></span> <span data-ttu-id="ca7d8-124">单通道实例呈现在 Android 上不可用，在 Mac 等非 VR 平台上也不需要。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-124">Single pass instanced rendering is not available on Android, and is not needed on non-VR platforms like Mac.</span></span> <span data-ttu-id="ca7d8-125">因此，可以使用常规发布版本来测试这些设备。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-125">Thus, you can use the general release version to test these devices.</span></span>


## <a name="storecompatibilitycheck"></a><span data-ttu-id="ca7d8-126">存储兼容性检查</span><span class="sxs-lookup"><span data-stu-id="ca7d8-126">Store Compatibility Check</span></span>

<span data-ttu-id="ca7d8-127">升级到 Unity 2020.3.9 还将影响头戴显示设备和存储生成兼容性。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-127">The upgrade to Unity 2020.3.9 will also affect headset and store-build compatibility.</span></span> <span data-ttu-id="ca7d8-128">现在，需要从与头戴显示设备兼容的应用商店下载 AltspaceVR。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-128">It's now a requirement that you download AltspaceVR from the store that is compatible with your headset.</span></span> <span data-ttu-id="ca7d8-129">例如：对于 WinMR 或 Oculus 头戴显示设备，请分别从 Windows 应用商店或 Oculus Store 下载 AltspaceVR。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-129">As an example: For a WinMR or Oculus headset, download AltspaceVR from the Windows Store or Oculus Store, respectively.</span></span> <span data-ttu-id="ca7d8-130">Windows Mixed Reality应从 Windows 应用商店下载 AltspaceVR，从 Steam 下载 SteamVR 用户，从 Oculus Store 下载 Oculus Rift 用户。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-130">Windows Mixed Reality users should download AltspaceVR from the Windows Store, SteamVR users from Steam, and Oculus Rift users from the Oculus Store.</span></span>

## <a name="altspacevr-uploader-v090-upgrade-guide"></a><span data-ttu-id="ca7d8-131">AltspaceVR Uploader v0.9.0 升级指南</span><span class="sxs-lookup"><span data-stu-id="ca7d8-131">AltspaceVR Uploader v0.9.0 Upgrade Guide</span></span> 

<span data-ttu-id="ca7d8-132">上传程序 0.9 的打包方式与以前版本的上传程序不同。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-132">Uploader 0.9 is packaged differently than previous versions of the Uploader.</span></span> <span data-ttu-id="ca7d8-133">在此打包更改的同时，新的上传程序需要新版本的 Unity。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-133">Simultaneous with this packaging change, the new Uploader requires a new version of Unity.</span></span> <span data-ttu-id="ca7d8-134">本指南旨在使此升级过程更顺畅、更安全，适用于所有参与方。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-134">This guide is intended to make this upgrade process smoother and safer for all who are involved.</span></span>

1. <span data-ttu-id="ca7d8-135">**备份项目** - 创建整个项目目录的副本，并放在安全位置。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-135">**BACK UP YOUR PROJECT** - Create a copy of your entire project directory, and put it somewhere safe.</span></span> <span data-ttu-id="ca7d8-136">此升级是破坏性升级，因此在完成升级后，无法为 Unity 2019.4 创建或上传捆绑包。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-136">This upgrade is a destructive upgrade, so you won't be able to create or upload bundles for Unity 2019.4 after you complete it.</span></span> <span data-ttu-id="ca7d8-137">如果在此升级过程中遇到任何问题，则需要项目干净副本进行回退。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-137">If you come across any problems during this upgrade, you'll NEED a clean copy of your project to fall back on.</span></span> <span data-ttu-id="ca7d8-138">在 AltspaceVR 正式升级到 Unity 2020.3.9 之前，还需要更新任何实时工具包或模板。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-138">You'll also need it to update any live kits or templates before AltspaceVR officially upgrades to Unity 2020.3.9.</span></span>

2. <span data-ttu-id="ca7d8-139">**REMOVE OLD UPLOADER** - 关闭 Unity 后，删除以下文件/文件夹，它是相应的 .meta 文件：</span><span class="sxs-lookup"><span data-stu-id="ca7d8-139">**REMOVE OLD UPLOADER** - With Unity closed, delete the following files/folders, and it's corresponding .meta files:</span></span>

    ```console
    * Assets/Altspace

    * Assets/Plugins

    * Assets/Prefabs/test-folder, Readme.txt

    * Assets/Resources/bg.jpeg, bg2.jpeg, logo.png, UserPreferences.asset

    * Assets/DFloor_v004.fbx

    * Library (This is a Unity system folder, not an Uploader folder. Delete it anyway, and let it be rebuilt during the upgrade.)
    ```

3. <span data-ttu-id="ca7d8-140">**下载引擎版本** - 打开 Unity 中心，安装 Unity 2020.3.9 [ (或单击此处](https://unity3d.com/ru/unity/whats-new/2020.3.9) 直接安装) 。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-140">**DOWNLOAD ENGINE VERSION** - Open the Unity Hub, and install Unity 2020.3.9 (or [click here](https://unity3d.com/ru/unity/whats-new/2020.3.9) to install directly).</span></span>

4. <span data-ttu-id="ca7d8-141">**升级项目** - 在 Unity 2020.3.9 中打开已清理的项目，并允许 Unity 升级项目。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-141">**UPGRADE PROJECT** - Open your cleaned project in Unity 2020.3.9, and allow Unity to upgrade your project.</span></span>

5. <span data-ttu-id="ca7d8-142"> (PC) 下载 **混合** 现实功能工具 - 按照说明下载混合现实功能工具，[](/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool)该工具用于管理上传程序包的安装。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-142">(PC Only) **DOWNLOAD MIXED REALITY FEATURE TOOL** - Follow the instructions to download the [Mixed Reality Feature Tool](/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool), which you'll use to manage the installation of the Uploader package.</span></span>

6. <span data-ttu-id="ca7d8-143">**安装上传程序** - 使用 MR 功能工具选择 Unity 项目，并添加 AltspaceVR 上传程序功能 (AltspaceVR 标题) 。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-143">**INSTALL THE UPLOADER** - Use the MR Feature Tool to select your Unity project, and add the AltspaceVR Uploader feature (under the AltspaceVR heading).</span></span> <span data-ttu-id="ca7d8-144">按照工具中的说明操作。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-144">Follow the instructions in the tool.</span></span>

<span data-ttu-id="ca7d8-145">在 macOS 上，从注册表手动下载最新版本[](https://dev.azure.com/aipmr/MixedReality-Unity-Packages/_packaging?_a=package&feed=Unity-packages&package=com.microsoft.altspacevr_uploader&protocolType=Npm&version=0.9.0&view=versions)，然后从 Unity 编辑器的包管理器 (Windows > 程序包管理器 > + > tarball) 中安装它。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-145">On macOS, manually download the latest version from the [registry](https://dev.azure.com/aipmr/MixedReality-Unity-Packages/_packaging?_a=package&feed=Unity-packages&package=com.microsoft.altspacevr_uploader&protocolType=Npm&version=0.9.0&view=versions), and install it from within the Unity Editor's package manager (Windows > Package Manager > + > Add package from tarball).</span></span>

<span data-ttu-id="ca7d8-146">包完成导入后，"AltspaceVR"菜单项中应会提供熟悉的"上传程序"窗口。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-146">Once the package finishes importing, the familiar Uploader window should be available in the AltspaceVR menu item.</span></span>

## <a name="troubleshooting-tips"></a><span data-ttu-id="ca7d8-147">故障排查提示</span><span class="sxs-lookup"><span data-stu-id="ca7d8-147">Troubleshooting Tips</span></span>

1. <span data-ttu-id="ca7d8-148">如果在 WinMR 头戴显示设备上遇到控制器或输入问题，请确保它位于头部，以正确连接状态传感器。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-148">If you're having controller or input issues on your WinMR headset, ensure it's positioned on your head to properly engage the presence sensor.</span></span> <span data-ttu-id="ca7d8-149">这是一个已知问题，Microsoft 正在积极解决此问题。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-149">This is a known issue and Microsoft is actively working to resolve it.</span></span>

2. <span data-ttu-id="ca7d8-150">检查头戴显示设备和存储生成兼容性。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-150">Check your headset and store-build compatibility.</span></span> <span data-ttu-id="ca7d8-151">例如，如果使用 WinMR 头戴显示设备，请确保 AltspaceVR 生成是通过 Windows 应用商店获取的。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-151">If you're using a WinMR headset, for example, make sure that your AltspaceVR build was acquired through the Windows Store.</span></span>

3. <span data-ttu-id="ca7d8-152">如果在测试期间发现内容仅在 VR 模式下以一只眼睛显示，则使用的自定义着色器很可能不支持 SPI 呈现。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-152">If during testing you discover that your content only appears in one eye in VR mode, it is likely that the custom shaders you use do not support SPI rendering.</span></span> <span data-ttu-id="ca7d8-153">需要选择其他着色器，或按照 Unity 的 [SPI](https://docs.unity3d.com/Manual/SinglePassInstancing.html) 升级指南手动编辑着色器并添加支持。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-153">You’ll need to choose a different shader, or follow [Unity’s SPI upgrade guide](https://docs.unity3d.com/Manual/SinglePassInstancing.html) to manually edit the shader and add support.</span></span>

4. <span data-ttu-id="ca7d8-154">对于 WinMR 上的用户，请记住，在 AltspaceVR 中访问 VR 模式之前，必须：</span><span class="sxs-lookup"><span data-stu-id="ca7d8-154">For those on WinMR, please remember that before you can access VR mode in AltspaceVR, you must:</span></span> 
    1. <span data-ttu-id="ca7d8-155">从客户端下载并安装 openXR Windows Mixed Reality安装Microsoft Store。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-155">Download and install OpenXR for Windows Mixed Reality from the Microsoft Store.</span></span>
        1. <span data-ttu-id="ca7d8-156">打开 混合现实门户 应用</span><span class="sxs-lookup"><span data-stu-id="ca7d8-156">Open the Mixed Reality Portal app</span></span>
        2. <span data-ttu-id="ca7d8-157">在应用的左下角选择"查看更多"</span><span class="sxs-lookup"><span data-stu-id="ca7d8-157">On the lower-left corner of the app select "See More"</span></span>
        3. <span data-ttu-id="ca7d8-158">在出现的菜单中，选择"设置 OpenXR"。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-158">In the menu that appears select Set Up OpenXR.</span></span> <span data-ttu-id="ca7d8-159">这样做将导致 Windows 应用商店从安装运行时的位置启动。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-159">Doing this will cause the Windows Store to launch from where you can install the runtime.</span></span> <span data-ttu-id="ca7d8-160">如果未显示此菜单项，则电脑上可能已安装 OpenXR。</span><span class="sxs-lookup"><span data-stu-id="ca7d8-160">If this menu item does not appear, OpenXR may already be installed on your PC.</span></span>