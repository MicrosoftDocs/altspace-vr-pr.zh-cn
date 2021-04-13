---
title: 引入世界建筑工具包
description: 了解如何使用全球构建工具包，通过 Unity 场景模板来设置和上传 AltspaceVR。
ms.date: 03/11/2021
ms.topic: article
keywords: 工具包
ms.openlocfilehash: cf4660f46d93ca5c5f23de3f567ff04b12519617
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "107211729"
---
# <a name="introducing-the-world-building-toolkit"></a><span data-ttu-id="9c56f-104">引入世界建筑工具包</span><span class="sxs-lookup"><span data-stu-id="9c56f-104">Introducing the World Building Toolkit</span></span>

> [!NOTE]
> <span data-ttu-id="9c56f-105">世界建筑工具包是一个由我们的出色朋友（ [Anthony Madden](https://twitter.com/chigamesstudio)）运行的社区项目，支持我们。</span><span class="sxs-lookup"><span data-stu-id="9c56f-105">The World Building Toolkit is a community project run by our awesome friend, [Anthony Madden](https://twitter.com/chigamesstudio), with support from us.</span></span> <span data-ttu-id="9c56f-106">如果你感兴趣，请加入 [官方 AltspaceVR Discord](https://discordapp.com/invite/altspacevr) ，并访问 #world 构建渠道。</span><span class="sxs-lookup"><span data-stu-id="9c56f-106">If you're interested, please join the [Official AltspaceVR Discord](https://discordapp.com/invite/altspacevr) and visit the #world-building channel.</span></span> <span data-ttu-id="9c56f-107">目前有一个 Mac 试用版试用版， [更多详细信息](https://altvr.com/altspacevr-mac)</span><span class="sxs-lookup"><span data-stu-id="9c56f-107">We currently have a Mac Trial Beta right now, [more details](https://altvr.com/altspacevr-mac)</span></span>

<span data-ttu-id="9c56f-108">使用上载程序，你可以使用 Unity 场景作为你的世界的模板。</span><span class="sxs-lookup"><span data-stu-id="9c56f-108">The Uploader allows you to use a Unity scene as a Template for your Worlds.</span></span> <span data-ttu-id="9c56f-109">你可以从 Minecraft 为万圣节或你最喜欢的创建 haunted。</span><span class="sxs-lookup"><span data-stu-id="9c56f-109">You can bring in a haunted house for Halloween or your favorite creation from Minecraft.</span></span> <span data-ttu-id="9c56f-110">如果可以将其导入到 Unity 中，则可能会以这种方式将其导入 Altspace。</span><span class="sxs-lookup"><span data-stu-id="9c56f-110">If you can import it into Unity, you can probably get it into Altspace this way.</span></span> <span data-ttu-id="9c56f-111">下面是几个 [示例](https://account.altvr.com/worlds/1046572460192825569)。</span><span class="sxs-lookup"><span data-stu-id="9c56f-111">Here are a few [example Worlds](https://account.altvr.com/worlds/1046572460192825569).</span></span>

![示例世界](images/unity-uploader-img-01.png)

## <a name="setup"></a><span data-ttu-id="9c56f-113">设置</span><span class="sxs-lookup"><span data-stu-id="9c56f-113">Setup</span></span>

1. <span data-ttu-id="9c56f-114">加入 [官方 AltspaceVR Discord](https://discordapp.com/invite/altspacevr) 并访问 #world 构建渠道-朋友不让朋友单独构建。</span><span class="sxs-lookup"><span data-stu-id="9c56f-114">Join the [Official AltspaceVR Discord](https://discordapp.com/invite/altspacevr) and visit the #world-building channel - Friends don't let friends build Worlds alone.</span></span>
2. <span data-ttu-id="9c56f-115">阅读我们的 [世界构建入门指南](world-building-getting-started.md) 以了解基础知识</span><span class="sxs-lookup"><span data-stu-id="9c56f-115">Read our [World-Building Getting Started Guide](world-building-getting-started.md) for the basics</span></span>
3. <span data-ttu-id="9c56f-116">[安装 Unity 中心](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) 并安装 **unity 2019.4.2 f1**。</span><span class="sxs-lookup"><span data-stu-id="9c56f-116">[Install Unity Hub](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) and install **Unity 2019.4.2f1**.</span></span> <span data-ttu-id="9c56f-117">除非完全匹配此版本，否则上载不起作用。</span><span class="sxs-lookup"><span data-stu-id="9c56f-117">The Uploader won't work unless you match this version exactly.</span></span> <span data-ttu-id="9c56f-118">如果你没有帐户并选择 " **个人** "，你将需要一个免费的 Unity 帐户，因为这样做有乐趣！</span><span class="sxs-lookup"><span data-stu-id="9c56f-118">You'll need a free Unity account if you don't have one and choose **Personal** since you're doing this for fun!</span></span> <span data-ttu-id="9c56f-119">在安装过程中，请确保选中 " **Android 生成** " 选项并禁用自动更新。</span><span class="sxs-lookup"><span data-stu-id="9c56f-119">During the install, make sure you check the **Android Builds** option and disable auto-update.</span></span>
4. [<span data-ttu-id="9c56f-120">下载最新 Unity 上载者</span><span class="sxs-lookup"><span data-stu-id="9c56f-120">Download the latest Unity Uploader</span></span>](https://aka.ms/AsvrCommunityUploader)
5. <span data-ttu-id="9c56f-121">在我们的网站上[创建模板](https://account.altvr.com/space_templates/new)。</span><span class="sxs-lookup"><span data-stu-id="9c56f-121">[Create a Template](https://account.altvr.com/space_templates/new) on our website.</span></span> <span data-ttu-id="9c56f-122">将其命名为 **模板 Hello World**。</span><span class="sxs-lookup"><span data-stu-id="9c56f-122">Name it **Hello World Template**.</span></span>
6. <span data-ttu-id="9c56f-123">[创建一个世界](https://account.altvr.com/worlds/my) ，并将其命名为 **Hello World**。</span><span class="sxs-lookup"><span data-stu-id="9c56f-123">[Create a World](https://account.altvr.com/worlds/my) and name it **Hello World**.</span></span> <span data-ttu-id="9c56f-124">选择 " **Hello World 模板** " 作为模板。</span><span class="sxs-lookup"><span data-stu-id="9c56f-124">Select **Hello World Template** as the Template.</span></span>

![已创建世界屏幕](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a><span data-ttu-id="9c56f-126">上传场景</span><span class="sxs-lookup"><span data-stu-id="9c56f-126">Upload your scene</span></span>

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-a-Template/player]

1. <span data-ttu-id="9c56f-127">打开 Unity 中心并创建新的 Unity 2019.4.2 f1 项目。</span><span class="sxs-lookup"><span data-stu-id="9c56f-127">Open Unity Hub and create a new Unity 2019.4.2f1 project.</span></span>
2. <span data-ttu-id="9c56f-128">打开项目后，通过双击下载的文件（ (它是 Unity 包) 导入上载程序。</span><span class="sxs-lookup"><span data-stu-id="9c56f-128">With your project open, import the Uploader by double-clicking the file you downloaded (it's a Unity package).</span></span> <span data-ttu-id="9c56f-129">现在应会看到一个名为 " **AltspaceVR**" 的新选项卡。</span><span class="sxs-lookup"><span data-stu-id="9c56f-129">You should now see a new tab called **AltspaceVR**.</span></span> <span data-ttu-id="9c56f-130">需要为每个要与 Altspace 一起使用的 Unity 项目导入包</span><span class="sxs-lookup"><span data-stu-id="9c56f-130">You'll need to import the package for every Unity project you want to use with Altspace</span></span>
3. <span data-ttu-id="9c56f-131">打开 **菜单 > AltspaceVR > 生成设置**</span><span class="sxs-lookup"><span data-stu-id="9c56f-131">Open **Menu > AltspaceVR > Build Settings**</span></span>
4. <span data-ttu-id="9c56f-132">用你的 Altspace 帐户凭据登录</span><span class="sxs-lookup"><span data-stu-id="9c56f-132">Sign in with your Altspace account credentials</span></span>
5. <span data-ttu-id="9c56f-133">选择 " **加载模板** "，然后选择 " **Hello World 模板**</span><span class="sxs-lookup"><span data-stu-id="9c56f-133">Select **Load Templates** and then select **Hello World Template**</span></span>
6. <span data-ttu-id="9c56f-134">将多维数据集添加到场景并保存。</span><span class="sxs-lookup"><span data-stu-id="9c56f-134">Add a cube to your scene and save.</span></span>
7. <span data-ttu-id="9c56f-135">检查 **Windows 版本是否适用** **？**</span><span class="sxs-lookup"><span data-stu-id="9c56f-135">Check **Build for Windows?** and uncheck **Build for Android?**</span></span>
8. <span data-ttu-id="9c56f-136">选择“上传”。</span><span class="sxs-lookup"><span data-stu-id="9c56f-136">Select **Upload**.</span></span> <span data-ttu-id="9c56f-137">大约一分钟后，应该会看到 " **上载** 完成"。</span><span class="sxs-lookup"><span data-stu-id="9c56f-137">In about a minute, you should see **Upload** complete.</span></span>
9. <span data-ttu-id="9c56f-138">通过从菜单 > 中启动 Altspace 和进入来加入 **Hello World** **> 我的世界**</span><span class="sxs-lookup"><span data-stu-id="9c56f-138">Join **Hello World** by launching Altspace and entering from **Menu > Worlds > My Worlds**</span></span>
10. <span data-ttu-id="9c56f-139">从菜单重置世界 **> 设置 > 适中 > 重置空间**</span><span class="sxs-lookup"><span data-stu-id="9c56f-139">Reset the World from **Menu > Settings > Moderate > Reset Space**</span></span>
11. <span data-ttu-id="9c56f-140">应会看到多维数据集。</span><span class="sxs-lookup"><span data-stu-id="9c56f-140">You should see the cube.</span></span> <span data-ttu-id="9c56f-141">如以上视频所示，如以上视频所示，你可以在很少10秒内看到更改。</span><span class="sxs-lookup"><span data-stu-id="9c56f-141">If you do it fast like in the video above, you can see changes within as little as 10 seconds.</span></span>

## <a name="whats-supported"></a><span data-ttu-id="9c56f-142">支持的操作</span><span class="sxs-lookup"><span data-stu-id="9c56f-142">What's supported</span></span>

* <span data-ttu-id="9c56f-143">是：模型、冲突、动画、粒子效果、音频、skyboxes 等</span><span class="sxs-lookup"><span data-stu-id="9c56f-143">Yes: models, collision, animations, particle effects, audio, skyboxes, and so on</span></span>
* <span data-ttu-id="9c56f-144">No：脚本。</span><span class="sxs-lookup"><span data-stu-id="9c56f-144">No: scripts.</span></span> <span data-ttu-id="9c56f-145">出于安全考虑，包含脚本的上载将被拒绝</span><span class="sxs-lookup"><span data-stu-id="9c56f-145">For security purposes, uploads containing scripts will be rejected</span></span>
* <span data-ttu-id="9c56f-146">可能：动态全局照明等别致的内容</span><span class="sxs-lookup"><span data-stu-id="9c56f-146">Maybe: fancy stuff like dynamic global illumination</span></span>
* <span data-ttu-id="9c56f-147">分别或一起为不同平台上传场景</span><span class="sxs-lookup"><span data-stu-id="9c56f-147">Upload scenes for different platforms separately or together</span></span>
* <span data-ttu-id="9c56f-148">请参阅 [特色世界](https://account.altvr.com/worlds/featured)，其中许多都是使用上载器生成的</span><span class="sxs-lookup"><span data-stu-id="9c56f-148">See [Featured Worlds](https://account.altvr.com/worlds/featured), many were built using the Uploader</span></span>

## <a name="tips"></a><span data-ttu-id="9c56f-149">提示</span><span class="sxs-lookup"><span data-stu-id="9c56f-149">Tips</span></span>

* <span data-ttu-id="9c56f-150">加入 [官方 AltspaceVR Discord](https://discordapp.com/invite/altspacevr)。</span><span class="sxs-lookup"><span data-stu-id="9c56f-150">Join the [Official AltspaceVR Discord](https://discordapp.com/invite/altspacevr).</span></span>
* <span data-ttu-id="9c56f-151">在左侧的 "模板" 页上，我们会显示平台的最新上载。</span><span class="sxs-lookup"><span data-stu-id="9c56f-151">On the Template page on the left side, we show you the latest uploads by platform.</span></span> <span data-ttu-id="9c56f-152">如果成功，则会看到 **1-2 分钟前**。Screen_Shot_2019-01-11 _at_1.21.04_AM.png</span><span class="sxs-lookup"><span data-stu-id="9c56f-152">If it was successful, you'd see **1-2 mins ago**.Screen_Shot_2019-01-11 _at_1.21.04_AM.png</span></span>

![突出显示了上传的模板面板打开](images/unity-uploader-img-03.png)

* <span data-ttu-id="9c56f-154">你可以在中进行更新。</span><span class="sxs-lookup"><span data-stu-id="9c56f-154">You can be in-World when you update.</span></span> <span data-ttu-id="9c56f-155">**上传完毕** 后，可以重置世界来查看所做的更改。</span><span class="sxs-lookup"><span data-stu-id="9c56f-155">The moment the Uploader says **Upload Complete** you can reset the World to see the changes.</span></span>
* <span data-ttu-id="9c56f-156">使用简单场景构建仅适用于 PC 的时间应不到1分钟才能看到 Altspace 的变化</span><span class="sxs-lookup"><span data-stu-id="9c56f-156">Building for PC-only with a simple scene should take less than 1 minute to see a change in Altspace</span></span>
* <span data-ttu-id="9c56f-157">将世界设置为 "专用"，以避免干扰。</span><span class="sxs-lookup"><span data-stu-id="9c56f-157">Set your World to be Private and Unlisted to avoid distractions.</span></span>
* <span data-ttu-id="9c56f-158">将多维数据集放在源位置，以便可以看到用户在默认情况下将生成的位置。</span><span class="sxs-lookup"><span data-stu-id="9c56f-158">Place a cube at the origin so you can see where people will spawn by default.</span></span> <span data-ttu-id="9c56f-159">上载时隐藏多维数据集。</span><span class="sxs-lookup"><span data-stu-id="9c56f-159">Hide the cube when uploading.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="9c56f-160">疑难解答</span><span class="sxs-lookup"><span data-stu-id="9c56f-160">Troubleshooting</span></span>

<span data-ttu-id="9c56f-161">**我会落下来或无法传送任何东西** 需要向要传送到对象的对象添加冲突。</span><span class="sxs-lookup"><span data-stu-id="9c56f-161">**I'm falling or can't teleport onto anything** You need to add collision to objects to teleport onto them.</span></span>

<span data-ttu-id="9c56f-162">**无更改**</span><span class="sxs-lookup"><span data-stu-id="9c56f-162">**Nothing changed**</span></span>
    * <span data-ttu-id="9c56f-163">是否在 Unity 中保存了场景？</span><span class="sxs-lookup"><span data-stu-id="9c56f-163">Did you save the scene in Unity?</span></span>
    * <span data-ttu-id="9c56f-164">选择了要测试的平台吗？</span><span class="sxs-lookup"><span data-stu-id="9c56f-164">Did you choose the platform you're testing on?</span></span>
    * <span data-ttu-id="9c56f-165">你是否在正确的领域？</span><span class="sxs-lookup"><span data-stu-id="9c56f-165">Are you in the right World?</span></span> <span data-ttu-id="9c56f-166">是否在上载者和世界窗体中选择了正确的模板？</span><span class="sxs-lookup"><span data-stu-id="9c56f-166">Did you choose the right Template in the Uploader AND in the World form?</span></span>
    * <span data-ttu-id="9c56f-167">是否检查了模板页统计信息？</span><span class="sxs-lookup"><span data-stu-id="9c56f-167">Did you check the Template page stats?</span></span>

<span data-ttu-id="9c56f-168">**上传失败或超时**</span><span class="sxs-lookup"><span data-stu-id="9c56f-168">**Upload fails or times out**</span></span>
    * <span data-ttu-id="9c56f-169">最常见的上传错误是具有错误的 Unity 版本。</span><span class="sxs-lookup"><span data-stu-id="9c56f-169">Most common upload error is having the wrong Unity version.</span></span> <span data-ttu-id="9c56f-170">它必须与所需的版本完全匹配。</span><span class="sxs-lookup"><span data-stu-id="9c56f-170">It must match the required version exactly.</span></span>
    * <span data-ttu-id="9c56f-171">上传可能太大。</span><span class="sxs-lookup"><span data-stu-id="9c56f-171">Your upload might be too large.</span></span> <span data-ttu-id="9c56f-172">尝试将 PC 场景保持 < 100 MB。</span><span class="sxs-lookup"><span data-stu-id="9c56f-172">Try to keep PC scenes < 100 MB.</span></span> <span data-ttu-id="9c56f-173">从小开始，然后生成。</span><span class="sxs-lookup"><span data-stu-id="9c56f-173">Start small and build up.</span></span> <span data-ttu-id="9c56f-174">优化、优化、优化。</span><span class="sxs-lookup"><span data-stu-id="9c56f-174">Optimize, optimize, optimize.</span></span>
    * <span data-ttu-id="9c56f-175">尝试使用简单的多维数据集的新项目。</span><span class="sxs-lookup"><span data-stu-id="9c56f-175">Try with a fresh project with a simple cube.</span></span>
    * <span data-ttu-id="9c56f-176">请不要在生成过程中强制退出-它会损坏场景。</span><span class="sxs-lookup"><span data-stu-id="9c56f-176">Don't force quit during a build--it can corrupt your scene.</span></span> <span data-ttu-id="9c56f-177">尝试 reuploading。</span><span class="sxs-lookup"><span data-stu-id="9c56f-177">Try reuploading.</span></span>

<span data-ttu-id="9c56f-178">**这是缓慢的过程**</span><span class="sxs-lookup"><span data-stu-id="9c56f-178">**It's a slow process**</span></span>
    * <span data-ttu-id="9c56f-179">建议仅在循环访问时，为 PC 构建。</span><span class="sxs-lookup"><span data-stu-id="9c56f-179">We recommend building for PC only while iterating and for Android later.</span></span>
    * <span data-ttu-id="9c56f-180">尝试删除未使用的文件。</span><span class="sxs-lookup"><span data-stu-id="9c56f-180">Try removing unused files.</span></span> <span data-ttu-id="9c56f-181">出于任何原因，Unity 有时会过度。</span><span class="sxs-lookup"><span data-stu-id="9c56f-181">For whatever reason Unity gets overzealous sometimes.</span></span>

<span data-ttu-id="9c56f-182">**我无法用我的 Altspace 凭据登录**</span><span class="sxs-lookup"><span data-stu-id="9c56f-182">**I can't sign in with my Altspace credentials**</span></span>
    * <span data-ttu-id="9c56f-183">电子邮件区分大小写。</span><span class="sxs-lookup"><span data-stu-id="9c56f-183">Emails are case-sensitive.</span></span>
    * <span data-ttu-id="9c56f-184">尝试新的项目。</span><span class="sxs-lookup"><span data-stu-id="9c56f-184">Try with a new project.</span></span>
    * <span data-ttu-id="9c56f-185">确保 Altspace 帐户处于良好地位。</span><span class="sxs-lookup"><span data-stu-id="9c56f-185">Make sure your Altspace account is in good standing.</span></span>

## <a name="see-also"></a><span data-ttu-id="9c56f-186">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9c56f-186">See also</span></span>

* [<span data-ttu-id="9c56f-187">Unity 学习</span><span class="sxs-lookup"><span data-stu-id="9c56f-187">Unity Learn</span></span>](https://unity3d.com/learn)
* [<span data-ttu-id="9c56f-188">Unity 论坛</span><span class="sxs-lookup"><span data-stu-id="9c56f-188">Unity Forums</span></span>](https://forum.unity.com)
